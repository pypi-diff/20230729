# Comparing `tmp/fern_sentra-0.0.5.tar.gz` & `tmp/fern_sentra-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_sentra-0.0.5.tar", max compression
+gzip compressed data, was "fern_sentra-0.0.6.tar", max compression
```

## Comparing `fern_sentra-0.0.5.tar` & `fern_sentra-0.0.6.tar`

### file list

```diff
@@ -1,267 +1,267 @@
--rw-r--r--   0        0        0     2693 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/README.md
--rw-r--r--   0        0        0      390 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    16435 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/__init__.py
--rw-r--r--   0        0        0     5551 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/client.py
--rw-r--r--   0        0        0      519 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/api_error.py
--rw-r--r--   0        0        0      765 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      156 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/environment.py
--rw-r--r--   0        0        0      230 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/errors/__init__.py
--rw-r--r--   0        0        0      246 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/errors/not_found_error.py
--rw-r--r--   0        0        0      313 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-28 17:52:57.514060 fern_sentra-0.0.5/src/sentra/py.typed
--rw-r--r--   0        0        0      618 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/alerts/__init__.py
--rw-r--r--   0        0        0    34335 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/alerts/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/api_keys/__init__.py
--rw-r--r--   0        0        0    14573 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/api_keys/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/audit_log/__init__.py
--rw-r--r--   0        0        0    12862 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/audit_log/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/connectors/__init__.py
--rw-r--r--   0        0        0    23305 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/connectors/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/context_labels/__init__.py
--rw-r--r--   0        0        0     5525 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/context_labels/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/dashboard/__init__.py
--rw-r--r--   0        0        0     3686 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/dashboard/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_access/__init__.py
--rw-r--r--   0        0        0    56254 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_access/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_assets/__init__.py
--rw-r--r--   0        0        0    22663 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_assets/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_classes/__init__.py
--rw-r--r--   0        0        0    25370 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_classes/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_stores/__init__.py
--rw-r--r--   0        0        0    31203 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/data_stores/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/export/__init__.py
--rw-r--r--   0        0        0     9780 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/export/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/integrations/__init__.py
--rw-r--r--   0        0        0    13703 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/integrations/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/policies/__init__.py
--rw-r--r--   0        0        0    30961 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/policies/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/roles/__init__.py
--rw-r--r--   0        0        0     5530 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/roles/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/sensitivity/__init__.py
--rw-r--r--   0        0        0     3804 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/sensitivity/client.py
--rw-r--r--   0        0        0       65 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/users/__init__.py
--rw-r--r--   0        0        0    13468 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/resources/users/client.py
--rw-r--r--   0        0        0    23027 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/__init__.py
--rw-r--r--   0        0        0     1081 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/access_data_store.py
--rw-r--r--   0        0        0     1078 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/access_method_accessible_entities_flowchart.py
--rw-r--r--   0        0        0      897 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/access_permissions.py
--rw-r--r--   0        0        0      957 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/accessible_entities_flowchart_identity_node.py
--rw-r--r--   0        0        0     1009 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/accessible_entities_flowchart_store_node.py
--rw-r--r--   0        0        0     1177 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/account_type.py
--rw-r--r--   0        0        0      881 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_comment_schema.py
--rw-r--r--   0        0        0      847 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_entity_type.py
--rw-r--r--   0        0        0     1483 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_response_schema.py
--rw-r--r--   0        0        0     1901 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_response_schema_content.py
--rw-r--r--   0        0        0      782 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_stats_by_date.py
--rw-r--r--   0        0        0      676 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_status.py
--rw-r--r--   0        0        0     1201 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_status_reason.py
--rw-r--r--   0        0        0     1171 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/alert_type.py
--rw-r--r--   0        0        0      858 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/amazon_security_lake_integration.py
--rw-r--r--   0        0        0      938 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/amazon_security_lake_item.py
--rw-r--r--   0        0        0      952 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/app_schemas_assets_public_access_level.py
--rw-r--r--   0        0        0      952 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/app_schemas_stores_public_access_level.py
--rw-r--r--   0        0        0      960 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/asset_class_user_request.py
--rw-r--r--   0        0        0      886 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/asset_classes_props.py
--rw-r--r--   0        0        0      931 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/asset_type.py
--rw-r--r--   0        0        0      945 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/auth_token_row.py
--rw-r--r--   0        0        0      910 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/auth_token_schema.py
--rw-r--r--   0        0        0     1452 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/aws_connector_args.py
--rw-r--r--   0        0        0      523 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/aws_installation_mode.py
--rw-r--r--   0        0        0      829 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/azure_boards_integration.py
--rw-r--r--   0        0        0      946 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/azure_boards_item.py
--rw-r--r--   0        0        0     1348 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/azure_connector_args.py
--rw-r--r--   0        0        0      807 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/choice_filter_data.py
--rw-r--r--   0        0        0     1394 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/class_and_classifier_config_schema.py
--rw-r--r--   0        0        0     1301 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/class_and_classifier_config_schema_classifier_config.py
--rw-r--r--   0        0        0     1027 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/class_categories.py
--rw-r--r--   0        0        0      494 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/class_source.py
--rw-r--r--   0        0        0      909 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/classification_result_example.py
--rw-r--r--   0        0        0      545 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/compute_connectivity_type.py
--rw-r--r--   0        0        0     1105 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_aws.py
--rw-r--r--   0        0        0      929 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_azure.py
--rw-r--r--   0        0        0      909 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_gcp.py
--rw-r--r--   0        0        0     1511 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_display.py
--rw-r--r--   0        0        0      510 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_display_args.py
--rw-r--r--   0        0        0     1213 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_display_compute_properties.py
--rw-r--r--   0        0        0     1287 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_input.py
--rw-r--r--   0        0        0      508 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_input_args.py
--rw-r--r--   0        0        0     1190 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_input_compute_properties.py
--rw-r--r--   0        0        0     1476 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_schema.py
--rw-r--r--   0        0        0      509 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_schema_args.py
--rw-r--r--   0        0        0     1197 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/connector_schema_compute_properties.py
--rw-r--r--   0        0        0      844 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/context_label_schema.py
--rw-r--r--   0        0        0      218 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/create_api_v_2_connectors_post_request.py
--rw-r--r--   0        0        0      228 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/create_api_v_2_integrations_post_request.py
--rw-r--r--   0        0        0      954 2023-07-28 17:52:57.518060 fern_sentra-0.0.5/src/sentra/types/create_class_request_schema_classifier_schema.py
--rw-r--r--   0        0        0     1010 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/create_dictionary_classifier_request_schema.py
--rw-r--r--   0        0        0     1066 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/create_regex_classifier_request_schema.py
--rw-r--r--   0        0        0      897 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/current_user_data.py
--rw-r--r--   0        0        0      802 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/dashboard_data.py
--rw-r--r--   0        0        0      956 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_at_risk.py
--rw-r--r--   0        0        0      527 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_class_user_operation.py
--rw-r--r--   0        0        0     2714 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_extended.py
--rw-r--r--   0        0        0     1012 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_object.py
--rw-r--r--   0        0        0     1457 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_props.py
--rw-r--r--   0        0        0     2163 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_row.py
--rw-r--r--   0        0        0     1969 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_asset_schema.py
--rw-r--r--   0        0        0     1283 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_class_config_with_user_schema.py
--rw-r--r--   0        0        0     1131 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_class_item.py
--rw-r--r--   0        0        0      848 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_dog_integration.py
--rw-r--r--   0        0        0      972 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_dog_item.py
--rw-r--r--   0        0        0      763 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_dog_region.py
--rw-r--r--   0        0        0     1515 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_hub_fabric.py
--rw-r--r--   0        0        0      813 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_hub_integration.py
--rw-r--r--   0        0        0      999 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_hub_item.py
--rw-r--r--   0        0        0      835 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_access_metadata.py
--rw-r--r--   0        0        0     2481 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_extended.py
--rw-r--r--   0        0        0      999 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_identity.py
--rw-r--r--   0        0        0     2404 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_props.py
--rw-r--r--   0        0        0      878 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_risk_aggregation.py
--rw-r--r--   0        0        0     2110 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/data_store_row.py
--rw-r--r--   0        0        0     1877 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema.py
--rw-r--r--   0        0        0     1901 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_content.py
--rw-r--r--   0        0        0     2025 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_with_comment.py
--rw-r--r--   0        0        0     2022 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_with_comment_content.py
--rw-r--r--   0        0        0     1201 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_iam_group_schema.py
--rw-r--r--   0        0        0     1280 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/detailed_iam_role_schema.py
--rw-r--r--   0        0        0      927 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/dictionary_classifier_response.py
--rw-r--r--   0        0        0      920 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/email_input_item.py
--rw-r--r--   0        0        0      858 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/email_integration.py
--rw-r--r--   0        0        0      860 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/email_integration_input.py
--rw-r--r--   0        0        0      926 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/email_output_item.py
--rw-r--r--   0        0        0     5757 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/event_log_action.py
--rw-r--r--   0        0        0     1687 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/event_log_entity_type.py
--rw-r--r--   0        0        0     1129 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/event_log_row.py
--rw-r--r--   0        0        0     1138 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/gcp_connector_args.py
--rw-r--r--   0        0        0      284 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_alerts_get_response.py
--rw-r--r--   0        0        0      303 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_audit_log_get_response.py
--rw-r--r--   0        0        0      353 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_classes_get_response.py
--rw-r--r--   0        0        0      332 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_connectors_get_response.py
--rw-r--r--   0        0        0      320 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_data_access_identities_get_response.py
--rw-r--r--   0        0        0      298 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_data_assets_get_response.py
--rw-r--r--   0        0        0      302 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_policies_get_response.py
--rw-r--r--   0        0        0      290 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_roles_get_response.py
--rw-r--r--   0        0        0      290 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_api_v_2_users_get_response.py
--rw-r--r--   0        0        0      319 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_all_external_api_v_2_data_stores_get_response.py
--rw-r--r--   0        0        0      282 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_alerts_filter_name_get_response.py
--rw-r--r--   0        0        0      284 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_audit_log_filter_name_get_response.py
--rw-r--r--   0        0        0      283 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_classes_filter_name_get_response.py
--rw-r--r--   0        0        0      286 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_data_access_filter_name_get_response.py
--rw-r--r--   0        0        0      286 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_data_assets_filter_name_get_response.py
--rw-r--r--   0        0        0      286 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_data_stores_filter_name_get_response.py
--rw-r--r--   0        0        0      284 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/get_filter_api_v_2_policies_filter_name_get_response.py
--rw-r--r--   0        0        0      853 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/group_item.py
--rw-r--r--   0        0        0      947 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/grouped_data_table_result.py
--rw-r--r--   0        0        0      843 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/http_validation_error.py
--rw-r--r--   0        0        0      888 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/iam_access_key_schema.py
--rw-r--r--   0        0        0      885 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/iam_group_data_classes.py
--rw-r--r--   0        0        0      951 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/iam_group_schema.py
--rw-r--r--   0        0        0      884 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/iam_role_data_classes.py
--rw-r--r--   0        0        0     1030 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/iam_role_schema.py
--rw-r--r--   0        0        0     1262 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart.py
--rw-r--r--   0        0        0      937 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_direct_access.py
--rw-r--r--   0        0        0      945 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_group.py
--rw-r--r--   0        0        0      943 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_role.py
--rw-r--r--   0        0        0      523 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_origin.py
--rw-r--r--   0        0        0     1623 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/identity_schema.py
--rw-r--r--   0        0        0     1117 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_display.py
--rw-r--r--   0        0        0     1080 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_display_properties.py
--rw-r--r--   0        0        0      981 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_input.py
--rw-r--r--   0        0        0     1126 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_input_properties.py
--rw-r--r--   0        0        0     1110 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_output_schema.py
--rw-r--r--   0        0        0     1085 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_output_schema_properties.py
--rw-r--r--   0        0        0     1085 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_schema.py
--rw-r--r--   0        0        0     1127 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_schema_properties.py
--rw-r--r--   0        0        0     2067 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/integration_type.py
--rw-r--r--   0        0        0      835 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/jira_integration.py
--rw-r--r--   0        0        0      946 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/jira_item.py
--rw-r--r--   0        0        0      764 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/keyword_requirement.py
--rw-r--r--   0        0        0      974 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_alerts_response.py
--rw-r--r--   0        0        0      956 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_assets_response.py
--rw-r--r--   0        0        0      960 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_auth_tokens_response.py
--rw-r--r--   0        0        0      978 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_connector_displays_response.py
--rw-r--r--   0        0        0      980 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_context_label_response.py
--rw-r--r--   0        0        0     1028 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_data_class_config_with_users_response.py
--rw-r--r--   0        0        0      960 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_data_stores_response.py
--rw-r--r--   0        0        0      955 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_event_log_response.py
--rw-r--r--   0        0        0      965 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_identities_response.py
--rw-r--r--   0        0        0      957 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_policies_response.py
--rw-r--r--   0        0        0      948 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_roles_response.py
--rw-r--r--   0        0        0      948 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_all_users_response.py
--rw-r--r--   0        0        0      979 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_similar_assets_pair_response.py
--rw-r--r--   0        0        0      978 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_similar_assets_response.py
--rw-r--r--   0        0        0      980 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_violated_data_assets_response.py
--rw-r--r--   0        0        0      967 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/list_violated_objects_response.py
--rw-r--r--   0        0        0     1133 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/microsoft_365_connector_args.py
--rw-r--r--   0        0        0      843 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/monday_integration.py
--rw-r--r--   0        0        0      973 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/monday_item.py
--rw-r--r--   0        0        0      842 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/new_auth_token_response.py
--rw-r--r--   0        0        0      775 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/object_class.py
--rw-r--r--   0        0        0      830 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/open_alerts_aggregation.py
--rw-r--r--   0        0        0      821 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/pager_duty_integration.py
--rw-r--r--   0        0        0      932 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/pager_duty_item.py
--rw-r--r--   0        0        0     7556 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/permissions.py
--rw-r--r--   0        0        0     1061 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_rule.py
--rw-r--r--   0        0        0     1169 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_rule_entity.py
--rw-r--r--   0        0        0      503 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_rule_type.py
--rw-r--r--   0        0        0     1698 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_schema.py
--rw-r--r--   0        0        0      797 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_severity.py
--rw-r--r--   0        0        0      512 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_status.py
--rw-r--r--   0        0        0      536 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_triggering_type.py
--rw-r--r--   0        0        0      682 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_type.py
--rw-r--r--   0        0        0      874 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/policy_update_response.py
--rw-r--r--   0        0        0      836 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/proprietary_classifier_response.py
--rw-r--r--   0        0        0      835 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/provider_minimal_metadata.py
--rw-r--r--   0        0        0      955 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/provider_schema.py
--rw-r--r--   0        0        0     1604 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/provider_types.py
--rw-r--r--   0        0        0      795 2023-07-28 17:52:57.522060 fern_sentra-0.0.5/src/sentra/types/range_filter_data.py
--rw-r--r--   0        0        0      891 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/regex_classifier_response.py
--rw-r--r--   0        0        0      533 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/resolved_alert_source.py
--rw-r--r--   0        0        0     1897 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/risk_type.py
--rw-r--r--   0        0        0     1173 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/role_identity.py
--rw-r--r--   0        0        0      877 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/role_schema.py
--rw-r--r--   0        0        0     1229 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/runtime_properties.py
--rw-r--r--   0        0        0      911 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/schedule_properties.py
--rw-r--r--   0        0        0      828 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/seemplicity_integration.py
--rw-r--r--   0        0        0      902 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/seemplicity_item.py
--rw-r--r--   0        0        0      859 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/sensitivity_levels.py
--rw-r--r--   0        0        0       83 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/session_type.py
--rw-r--r--   0        0        0     2982 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_asset_schema.py
--rw-r--r--   0        0        0      812 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_assets_alert_content.py
--rw-r--r--   0        0        0     1037 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_assets_pair.py
--rw-r--r--   0        0        0     1065 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_assets_pair_schema.py
--rw-r--r--   0        0        0      789 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_assets_props.py
--rw-r--r--   0        0        0      914 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similar_store.py
--rw-r--r--   0        0        0      523 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/similarity_type.py
--rw-r--r--   0        0        0      846 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/slack_integration.py
--rw-r--r--   0        0        0      848 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/slack_integration_input.py
--rw-r--r--   0        0        0     1096 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/slack_web_hook_input_item.py
--rw-r--r--   0        0        0     1102 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/slack_web_hook_output_item.py
--rw-r--r--   0        0        0     1106 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/snowflake_connector_args.py
--rw-r--r--   0        0        0      811 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/sort.py
--rw-r--r--   0        0        0      463 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/sort_order.py
--rw-r--r--   0        0        0      823 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/teams_integration.py
--rw-r--r--   0        0        0      896 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/teams_output_item.py
--rw-r--r--   0        0        0      775 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/test_connection_result.py
--rw-r--r--   0        0        0      954 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/update_class_request_schema_classifier_schema.py
--rw-r--r--   0        0        0     1010 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/update_dictionary_classifier_request_schema.py
--rw-r--r--   0        0        0     1083 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/update_regex_classifier_request_schema.py
--rw-r--r--   0        0        0      872 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/user_schema.py
--rw-r--r--   0        0        0      506 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/user_status.py
--rw-r--r--   0        0        0      788 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/validation_error.py
--rw-r--r--   0        0        0     2436 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_data_asset.py
--rw-r--r--   0        0        0      747 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_iam_group_alert_content.py
--rw-r--r--   0        0        0      746 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_iam_role_alert_content.py
--rw-r--r--   0        0        0      747 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_identity_alert_content.py
--rw-r--r--   0        0        0      963 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_object.py
--rw-r--r--   0        0        0      786 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/violated_store_alert_content.py
--rw-r--r--   0        0        0      928 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/web_hook_input_item.py
--rw-r--r--   0        0        0      832 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/web_hook_integration.py
--rw-r--r--   0        0        0      834 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/web_hook_integration_input.py
--rw-r--r--   0        0        0      934 2023-07-28 17:52:57.526060 fern_sentra-0.0.5/src/sentra/types/web_hook_output_item.py
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 fern_sentra-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2693 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/README.md
+-rw-r--r--   0        0        0      390 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    16435 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/__init__.py
+-rw-r--r--   0        0        0     5551 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/client.py
+-rw-r--r--   0        0        0      519 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/core/api_error.py
+-rw-r--r--   0        0        0      765 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      156 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/environment.py
+-rw-r--r--   0        0        0      230 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/errors/__init__.py
+-rw-r--r--   0        0        0      246 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/errors/not_found_error.py
+-rw-r--r--   0        0        0      313 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/py.typed
+-rw-r--r--   0        0        0      618 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/alerts/__init__.py
+-rw-r--r--   0        0        0    34335 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/alerts/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/api_keys/__init__.py
+-rw-r--r--   0        0        0    14573 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/api_keys/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/audit_log/__init__.py
+-rw-r--r--   0        0        0    12862 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/audit_log/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/connectors/__init__.py
+-rw-r--r--   0        0        0    23305 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/connectors/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/context_labels/__init__.py
+-rw-r--r--   0        0        0     5525 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/context_labels/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/dashboard/__init__.py
+-rw-r--r--   0        0        0     3686 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/dashboard/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/data_access/__init__.py
+-rw-r--r--   0        0        0    56254 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/data_access/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/data_assets/__init__.py
+-rw-r--r--   0        0        0    22663 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/data_assets/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/data_classes/__init__.py
+-rw-r--r--   0        0        0    25370 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/data_classes/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/data_stores/__init__.py
+-rw-r--r--   0        0        0    31203 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/data_stores/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/export/__init__.py
+-rw-r--r--   0        0        0     9780 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/export/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/integrations/__init__.py
+-rw-r--r--   0        0        0    13703 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/integrations/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/policies/__init__.py
+-rw-r--r--   0        0        0    30961 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/policies/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/roles/__init__.py
+-rw-r--r--   0        0        0     5530 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/roles/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/sensitivity/__init__.py
+-rw-r--r--   0        0        0     3804 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/sensitivity/client.py
+-rw-r--r--   0        0        0       65 2023-07-29 11:11:38.440416 fern_sentra-0.0.6/src/sentra/resources/users/__init__.py
+-rw-r--r--   0        0        0    13468 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/resources/users/client.py
+-rw-r--r--   0        0        0    23027 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/__init__.py
+-rw-r--r--   0        0        0     1081 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/access_data_store.py
+-rw-r--r--   0        0        0     1078 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/access_method_accessible_entities_flowchart.py
+-rw-r--r--   0        0        0      897 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/access_permissions.py
+-rw-r--r--   0        0        0      957 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/accessible_entities_flowchart_identity_node.py
+-rw-r--r--   0        0        0     1009 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/accessible_entities_flowchart_store_node.py
+-rw-r--r--   0        0        0     1177 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/account_type.py
+-rw-r--r--   0        0        0      881 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/alert_comment_schema.py
+-rw-r--r--   0        0        0      847 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/alert_entity_type.py
+-rw-r--r--   0        0        0     1483 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/alert_response_schema.py
+-rw-r--r--   0        0        0     1901 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/alert_response_schema_content.py
+-rw-r--r--   0        0        0      782 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/alert_stats_by_date.py
+-rw-r--r--   0        0        0      676 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/alert_status.py
+-rw-r--r--   0        0        0     1201 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/alert_status_reason.py
+-rw-r--r--   0        0        0     1171 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/alert_type.py
+-rw-r--r--   0        0        0      858 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/amazon_security_lake_integration.py
+-rw-r--r--   0        0        0      938 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/amazon_security_lake_item.py
+-rw-r--r--   0        0        0      952 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/app_schemas_assets_public_access_level.py
+-rw-r--r--   0        0        0      952 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/app_schemas_stores_public_access_level.py
+-rw-r--r--   0        0        0      960 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/asset_class_user_request.py
+-rw-r--r--   0        0        0      886 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/asset_classes_props.py
+-rw-r--r--   0        0        0      931 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/asset_type.py
+-rw-r--r--   0        0        0      945 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/auth_token_row.py
+-rw-r--r--   0        0        0      910 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/auth_token_schema.py
+-rw-r--r--   0        0        0     1452 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/aws_connector_args.py
+-rw-r--r--   0        0        0      523 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/aws_installation_mode.py
+-rw-r--r--   0        0        0      829 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/azure_boards_integration.py
+-rw-r--r--   0        0        0      946 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/azure_boards_item.py
+-rw-r--r--   0        0        0     1348 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/azure_connector_args.py
+-rw-r--r--   0        0        0      807 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/choice_filter_data.py
+-rw-r--r--   0        0        0     1394 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/class_and_classifier_config_schema.py
+-rw-r--r--   0        0        0     1301 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/class_and_classifier_config_schema_classifier_config.py
+-rw-r--r--   0        0        0     1027 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/class_categories.py
+-rw-r--r--   0        0        0      494 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/class_source.py
+-rw-r--r--   0        0        0      909 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/classification_result_example.py
+-rw-r--r--   0        0        0      545 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/compute_connectivity_type.py
+-rw-r--r--   0        0        0     1105 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/compute_connector_properties_aws.py
+-rw-r--r--   0        0        0      929 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/compute_connector_properties_azure.py
+-rw-r--r--   0        0        0      909 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/compute_connector_properties_gcp.py
+-rw-r--r--   0        0        0     1511 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/connector_display.py
+-rw-r--r--   0        0        0      510 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/connector_display_args.py
+-rw-r--r--   0        0        0     1213 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/connector_display_compute_properties.py
+-rw-r--r--   0        0        0     1287 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/connector_input.py
+-rw-r--r--   0        0        0      508 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/connector_input_args.py
+-rw-r--r--   0        0        0     1190 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/connector_input_compute_properties.py
+-rw-r--r--   0        0        0     1476 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/connector_schema.py
+-rw-r--r--   0        0        0      509 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/connector_schema_args.py
+-rw-r--r--   0        0        0     1197 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/connector_schema_compute_properties.py
+-rw-r--r--   0        0        0      844 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/context_label_schema.py
+-rw-r--r--   0        0        0      218 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/create_api_v_2_connectors_post_request.py
+-rw-r--r--   0        0        0      228 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/create_api_v_2_integrations_post_request.py
+-rw-r--r--   0        0        0      954 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/create_class_request_schema_classifier_schema.py
+-rw-r--r--   0        0        0     1010 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/create_dictionary_classifier_request_schema.py
+-rw-r--r--   0        0        0     1066 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/create_regex_classifier_request_schema.py
+-rw-r--r--   0        0        0      897 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/current_user_data.py
+-rw-r--r--   0        0        0      802 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/dashboard_data.py
+-rw-r--r--   0        0        0      956 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_asset_at_risk.py
+-rw-r--r--   0        0        0      527 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_asset_class_user_operation.py
+-rw-r--r--   0        0        0     2714 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_asset_extended.py
+-rw-r--r--   0        0        0     1012 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_asset_object.py
+-rw-r--r--   0        0        0     1457 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_asset_props.py
+-rw-r--r--   0        0        0     2163 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_asset_row.py
+-rw-r--r--   0        0        0     1969 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_asset_schema.py
+-rw-r--r--   0        0        0     1283 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_class_config_with_user_schema.py
+-rw-r--r--   0        0        0     1131 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_class_item.py
+-rw-r--r--   0        0        0      848 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_dog_integration.py
+-rw-r--r--   0        0        0      972 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_dog_item.py
+-rw-r--r--   0        0        0      763 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_dog_region.py
+-rw-r--r--   0        0        0     1515 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_hub_fabric.py
+-rw-r--r--   0        0        0      813 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_hub_integration.py
+-rw-r--r--   0        0        0      999 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_hub_item.py
+-rw-r--r--   0        0        0      835 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_store_access_metadata.py
+-rw-r--r--   0        0        0     2481 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_store_extended.py
+-rw-r--r--   0        0        0      999 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_store_identity.py
+-rw-r--r--   0        0        0     2404 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_store_props.py
+-rw-r--r--   0        0        0      878 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_store_risk_aggregation.py
+-rw-r--r--   0        0        0     2110 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/data_store_row.py
+-rw-r--r--   0        0        0     1877 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/detailed_alert_schema.py
+-rw-r--r--   0        0        0     1901 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/detailed_alert_schema_content.py
+-rw-r--r--   0        0        0     2025 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/detailed_alert_schema_with_comment.py
+-rw-r--r--   0        0        0     2022 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/detailed_alert_schema_with_comment_content.py
+-rw-r--r--   0        0        0     1201 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/detailed_iam_group_schema.py
+-rw-r--r--   0        0        0     1280 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/detailed_iam_role_schema.py
+-rw-r--r--   0        0        0      927 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/dictionary_classifier_response.py
+-rw-r--r--   0        0        0      920 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/email_input_item.py
+-rw-r--r--   0        0        0      858 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/email_integration.py
+-rw-r--r--   0        0        0      860 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/email_integration_input.py
+-rw-r--r--   0        0        0      926 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/email_output_item.py
+-rw-r--r--   0        0        0     5757 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/event_log_action.py
+-rw-r--r--   0        0        0     1687 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/event_log_entity_type.py
+-rw-r--r--   0        0        0     1129 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/event_log_row.py
+-rw-r--r--   0        0        0     1138 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/gcp_connector_args.py
+-rw-r--r--   0        0        0      284 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_all_api_v_2_alerts_get_response.py
+-rw-r--r--   0        0        0      303 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_all_api_v_2_audit_log_get_response.py
+-rw-r--r--   0        0        0      353 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_all_api_v_2_classes_get_response.py
+-rw-r--r--   0        0        0      332 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_all_api_v_2_connectors_get_response.py
+-rw-r--r--   0        0        0      320 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_all_api_v_2_data_access_identities_get_response.py
+-rw-r--r--   0        0        0      298 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_all_api_v_2_data_assets_get_response.py
+-rw-r--r--   0        0        0      302 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_all_api_v_2_policies_get_response.py
+-rw-r--r--   0        0        0      290 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_all_api_v_2_roles_get_response.py
+-rw-r--r--   0        0        0      290 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_all_api_v_2_users_get_response.py
+-rw-r--r--   0        0        0      319 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_all_external_api_v_2_data_stores_get_response.py
+-rw-r--r--   0        0        0      282 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_filter_api_v_2_alerts_filter_name_get_response.py
+-rw-r--r--   0        0        0      284 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_filter_api_v_2_audit_log_filter_name_get_response.py
+-rw-r--r--   0        0        0      283 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_filter_api_v_2_classes_filter_name_get_response.py
+-rw-r--r--   0        0        0      286 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_filter_api_v_2_data_access_filter_name_get_response.py
+-rw-r--r--   0        0        0      286 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_filter_api_v_2_data_assets_filter_name_get_response.py
+-rw-r--r--   0        0        0      286 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_filter_api_v_2_data_stores_filter_name_get_response.py
+-rw-r--r--   0        0        0      284 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/get_filter_api_v_2_policies_filter_name_get_response.py
+-rw-r--r--   0        0        0      853 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/group_item.py
+-rw-r--r--   0        0        0      947 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/grouped_data_table_result.py
+-rw-r--r--   0        0        0      843 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/http_validation_error.py
+-rw-r--r--   0        0        0      888 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/iam_access_key_schema.py
+-rw-r--r--   0        0        0      885 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/iam_group_data_classes.py
+-rw-r--r--   0        0        0      951 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/iam_group_schema.py
+-rw-r--r--   0        0        0      884 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/iam_role_data_classes.py
+-rw-r--r--   0        0        0     1030 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/iam_role_schema.py
+-rw-r--r--   0        0        0     1262 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/identity_accessible_entities_flowchart.py
+-rw-r--r--   0        0        0      937 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/identity_accessible_entities_flowchart_direct_access.py
+-rw-r--r--   0        0        0      945 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/identity_accessible_entities_flowchart_group.py
+-rw-r--r--   0        0        0      943 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/identity_accessible_entities_flowchart_role.py
+-rw-r--r--   0        0        0      523 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/identity_origin.py
+-rw-r--r--   0        0        0     1623 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/identity_schema.py
+-rw-r--r--   0        0        0     1117 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/integration_display.py
+-rw-r--r--   0        0        0     1080 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/integration_display_properties.py
+-rw-r--r--   0        0        0      981 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/integration_input.py
+-rw-r--r--   0        0        0     1126 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/integration_input_properties.py
+-rw-r--r--   0        0        0     1110 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/integration_output_schema.py
+-rw-r--r--   0        0        0     1085 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/integration_output_schema_properties.py
+-rw-r--r--   0        0        0     1085 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/integration_schema.py
+-rw-r--r--   0        0        0     1127 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/integration_schema_properties.py
+-rw-r--r--   0        0        0     2067 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/integration_type.py
+-rw-r--r--   0        0        0      835 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/jira_integration.py
+-rw-r--r--   0        0        0      946 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/jira_item.py
+-rw-r--r--   0        0        0      764 2023-07-29 11:11:38.444416 fern_sentra-0.0.6/src/sentra/types/keyword_requirement.py
+-rw-r--r--   0        0        0      974 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_alerts_response.py
+-rw-r--r--   0        0        0      956 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_all_assets_response.py
+-rw-r--r--   0        0        0      960 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_all_auth_tokens_response.py
+-rw-r--r--   0        0        0      978 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_all_connector_displays_response.py
+-rw-r--r--   0        0        0      980 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_all_context_label_response.py
+-rw-r--r--   0        0        0     1028 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_all_data_class_config_with_users_response.py
+-rw-r--r--   0        0        0      960 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_all_data_stores_response.py
+-rw-r--r--   0        0        0      955 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_all_event_log_response.py
+-rw-r--r--   0        0        0      965 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_all_identities_response.py
+-rw-r--r--   0        0        0      957 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_all_policies_response.py
+-rw-r--r--   0        0        0      948 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_all_roles_response.py
+-rw-r--r--   0        0        0      948 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_all_users_response.py
+-rw-r--r--   0        0        0      979 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_similar_assets_pair_response.py
+-rw-r--r--   0        0        0      978 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_similar_assets_response.py
+-rw-r--r--   0        0        0      980 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_violated_data_assets_response.py
+-rw-r--r--   0        0        0      967 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/list_violated_objects_response.py
+-rw-r--r--   0        0        0     1133 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/microsoft_365_connector_args.py
+-rw-r--r--   0        0        0      843 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/monday_integration.py
+-rw-r--r--   0        0        0      973 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/monday_item.py
+-rw-r--r--   0        0        0      842 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/new_auth_token_response.py
+-rw-r--r--   0        0        0      775 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/object_class.py
+-rw-r--r--   0        0        0      830 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/open_alerts_aggregation.py
+-rw-r--r--   0        0        0      821 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/pager_duty_integration.py
+-rw-r--r--   0        0        0      932 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/pager_duty_item.py
+-rw-r--r--   0        0        0     7556 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/permissions.py
+-rw-r--r--   0        0        0     1061 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/policy_rule.py
+-rw-r--r--   0        0        0     1169 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/policy_rule_entity.py
+-rw-r--r--   0        0        0      503 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/policy_rule_type.py
+-rw-r--r--   0        0        0     1698 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/policy_schema.py
+-rw-r--r--   0        0        0      797 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/policy_severity.py
+-rw-r--r--   0        0        0      512 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/policy_status.py
+-rw-r--r--   0        0        0      536 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/policy_triggering_type.py
+-rw-r--r--   0        0        0      682 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/policy_type.py
+-rw-r--r--   0        0        0      874 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/policy_update_response.py
+-rw-r--r--   0        0        0      836 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/proprietary_classifier_response.py
+-rw-r--r--   0        0        0      835 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/provider_minimal_metadata.py
+-rw-r--r--   0        0        0      955 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/provider_schema.py
+-rw-r--r--   0        0        0     1604 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/provider_types.py
+-rw-r--r--   0        0        0      795 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/range_filter_data.py
+-rw-r--r--   0        0        0      891 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/regex_classifier_response.py
+-rw-r--r--   0        0        0      533 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/resolved_alert_source.py
+-rw-r--r--   0        0        0     1897 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/risk_type.py
+-rw-r--r--   0        0        0     1173 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/role_identity.py
+-rw-r--r--   0        0        0      877 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/role_schema.py
+-rw-r--r--   0        0        0     1229 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/runtime_properties.py
+-rw-r--r--   0        0        0      911 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/schedule_properties.py
+-rw-r--r--   0        0        0      828 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/seemplicity_integration.py
+-rw-r--r--   0        0        0      902 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/seemplicity_item.py
+-rw-r--r--   0        0        0      859 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/sensitivity_levels.py
+-rw-r--r--   0        0        0       83 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/session_type.py
+-rw-r--r--   0        0        0     2982 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/similar_asset_schema.py
+-rw-r--r--   0        0        0      812 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/similar_assets_alert_content.py
+-rw-r--r--   0        0        0     1037 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/similar_assets_pair.py
+-rw-r--r--   0        0        0     1065 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/similar_assets_pair_schema.py
+-rw-r--r--   0        0        0      789 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/similar_assets_props.py
+-rw-r--r--   0        0        0      914 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/similar_store.py
+-rw-r--r--   0        0        0      523 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/similarity_type.py
+-rw-r--r--   0        0        0      846 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/slack_integration.py
+-rw-r--r--   0        0        0      848 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/slack_integration_input.py
+-rw-r--r--   0        0        0     1096 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/slack_web_hook_input_item.py
+-rw-r--r--   0        0        0     1102 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/slack_web_hook_output_item.py
+-rw-r--r--   0        0        0     1106 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/snowflake_connector_args.py
+-rw-r--r--   0        0        0      811 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/sort.py
+-rw-r--r--   0        0        0      463 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/sort_order.py
+-rw-r--r--   0        0        0      823 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/teams_integration.py
+-rw-r--r--   0        0        0      896 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/teams_output_item.py
+-rw-r--r--   0        0        0      775 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/test_connection_result.py
+-rw-r--r--   0        0        0      954 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/update_class_request_schema_classifier_schema.py
+-rw-r--r--   0        0        0     1010 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/update_dictionary_classifier_request_schema.py
+-rw-r--r--   0        0        0     1083 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/update_regex_classifier_request_schema.py
+-rw-r--r--   0        0        0      872 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/user_schema.py
+-rw-r--r--   0        0        0      506 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/user_status.py
+-rw-r--r--   0        0        0      788 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/validation_error.py
+-rw-r--r--   0        0        0     2436 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/violated_data_asset.py
+-rw-r--r--   0        0        0      747 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/violated_iam_group_alert_content.py
+-rw-r--r--   0        0        0      746 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/violated_iam_role_alert_content.py
+-rw-r--r--   0        0        0      747 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/violated_identity_alert_content.py
+-rw-r--r--   0        0        0      963 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/violated_object.py
+-rw-r--r--   0        0        0      786 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/violated_store_alert_content.py
+-rw-r--r--   0        0        0      928 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/web_hook_input_item.py
+-rw-r--r--   0        0        0      832 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/web_hook_integration.py
+-rw-r--r--   0        0        0      834 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/web_hook_integration_input.py
+-rw-r--r--   0        0        0      934 2023-07-29 11:11:38.448416 fern_sentra-0.0.6/src/sentra/types/web_hook_output_item.py
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 fern_sentra-0.0.6/PKG-INFO
```

### Comparing `fern_sentra-0.0.5/README.md` & `fern_sentra-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/__init__.py` & `fern_sentra-0.0.6/src/sentra/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/client.py` & `fern_sentra-0.0.6/src/sentra/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/core/__init__.py` & `fern_sentra-0.0.6/src/sentra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/core/client_wrapper.py` & `fern_sentra-0.0.6/src/sentra/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/core/datetime_utils.py` & `fern_sentra-0.0.6/src/sentra/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/core/jsonable_encoder.py` & `fern_sentra-0.0.6/src/sentra/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/__init__.py` & `fern_sentra-0.0.6/src/sentra/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/alerts/client.py` & `fern_sentra-0.0.6/src/sentra/resources/alerts/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/api_keys/client.py` & `fern_sentra-0.0.6/src/sentra/resources/api_keys/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/audit_log/client.py` & `fern_sentra-0.0.6/src/sentra/resources/audit_log/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/connectors/client.py` & `fern_sentra-0.0.6/src/sentra/resources/connectors/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/context_labels/client.py` & `fern_sentra-0.0.6/src/sentra/resources/context_labels/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/dashboard/client.py` & `fern_sentra-0.0.6/src/sentra/resources/dashboard/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/data_access/client.py` & `fern_sentra-0.0.6/src/sentra/resources/data_access/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/data_assets/client.py` & `fern_sentra-0.0.6/src/sentra/resources/data_assets/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/data_classes/client.py` & `fern_sentra-0.0.6/src/sentra/resources/data_classes/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/data_stores/client.py` & `fern_sentra-0.0.6/src/sentra/resources/data_stores/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/export/client.py` & `fern_sentra-0.0.6/src/sentra/resources/export/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/integrations/client.py` & `fern_sentra-0.0.6/src/sentra/resources/integrations/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/policies/client.py` & `fern_sentra-0.0.6/src/sentra/resources/policies/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/roles/client.py` & `fern_sentra-0.0.6/src/sentra/resources/roles/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/sensitivity/client.py` & `fern_sentra-0.0.6/src/sentra/resources/sensitivity/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/resources/users/client.py` & `fern_sentra-0.0.6/src/sentra/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/__init__.py` & `fern_sentra-0.0.6/src/sentra/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/access_data_store.py` & `fern_sentra-0.0.6/src/sentra/types/access_data_store.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/access_method_accessible_entities_flowchart.py` & `fern_sentra-0.0.6/src/sentra/types/access_method_accessible_entities_flowchart.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/access_permissions.py` & `fern_sentra-0.0.6/src/sentra/types/access_permissions.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/accessible_entities_flowchart_identity_node.py` & `fern_sentra-0.0.6/src/sentra/types/accessible_entities_flowchart_identity_node.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/accessible_entities_flowchart_store_node.py` & `fern_sentra-0.0.6/src/sentra/types/accessible_entities_flowchart_store_node.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/account_type.py` & `fern_sentra-0.0.6/src/sentra/types/account_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/alert_comment_schema.py` & `fern_sentra-0.0.6/src/sentra/types/alert_comment_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/alert_entity_type.py` & `fern_sentra-0.0.6/src/sentra/types/alert_entity_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/alert_response_schema.py` & `fern_sentra-0.0.6/src/sentra/types/alert_response_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/alert_response_schema_content.py` & `fern_sentra-0.0.6/src/sentra/types/alert_response_schema_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/alert_stats_by_date.py` & `fern_sentra-0.0.6/src/sentra/types/alert_stats_by_date.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/alert_status.py` & `fern_sentra-0.0.6/src/sentra/types/alert_status.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/alert_status_reason.py` & `fern_sentra-0.0.6/src/sentra/types/alert_status_reason.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/alert_type.py` & `fern_sentra-0.0.6/src/sentra/types/alert_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/amazon_security_lake_integration.py` & `fern_sentra-0.0.6/src/sentra/types/amazon_security_lake_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/amazon_security_lake_item.py` & `fern_sentra-0.0.6/src/sentra/types/amazon_security_lake_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/app_schemas_assets_public_access_level.py` & `fern_sentra-0.0.6/src/sentra/types/app_schemas_assets_public_access_level.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/app_schemas_stores_public_access_level.py` & `fern_sentra-0.0.6/src/sentra/types/app_schemas_stores_public_access_level.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/asset_class_user_request.py` & `fern_sentra-0.0.6/src/sentra/types/asset_class_user_request.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/asset_classes_props.py` & `fern_sentra-0.0.6/src/sentra/types/asset_classes_props.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/asset_type.py` & `fern_sentra-0.0.6/src/sentra/types/asset_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/auth_token_row.py` & `fern_sentra-0.0.6/src/sentra/types/auth_token_row.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/auth_token_schema.py` & `fern_sentra-0.0.6/src/sentra/types/auth_token_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/aws_connector_args.py` & `fern_sentra-0.0.6/src/sentra/types/aws_connector_args.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/aws_installation_mode.py` & `fern_sentra-0.0.6/src/sentra/types/aws_installation_mode.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/azure_boards_integration.py` & `fern_sentra-0.0.6/src/sentra/types/azure_boards_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/azure_boards_item.py` & `fern_sentra-0.0.6/src/sentra/types/azure_boards_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/azure_connector_args.py` & `fern_sentra-0.0.6/src/sentra/types/azure_connector_args.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/choice_filter_data.py` & `fern_sentra-0.0.6/src/sentra/types/choice_filter_data.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/class_and_classifier_config_schema.py` & `fern_sentra-0.0.6/src/sentra/types/class_and_classifier_config_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/class_and_classifier_config_schema_classifier_config.py` & `fern_sentra-0.0.6/src/sentra/types/class_and_classifier_config_schema_classifier_config.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/class_categories.py` & `fern_sentra-0.0.6/src/sentra/types/class_categories.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/classification_result_example.py` & `fern_sentra-0.0.6/src/sentra/types/classification_result_example.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/compute_connectivity_type.py` & `fern_sentra-0.0.6/src/sentra/types/compute_connectivity_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_aws.py` & `fern_sentra-0.0.6/src/sentra/types/compute_connector_properties_aws.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_azure.py` & `fern_sentra-0.0.6/src/sentra/types/compute_connector_properties_azure.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/compute_connector_properties_gcp.py` & `fern_sentra-0.0.6/src/sentra/types/compute_connector_properties_gcp.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/connector_display.py` & `fern_sentra-0.0.6/src/sentra/types/connector_display.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/connector_display_compute_properties.py` & `fern_sentra-0.0.6/src/sentra/types/connector_display_compute_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/connector_input.py` & `fern_sentra-0.0.6/src/sentra/types/connector_input.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/connector_input_compute_properties.py` & `fern_sentra-0.0.6/src/sentra/types/connector_input_compute_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/connector_schema.py` & `fern_sentra-0.0.6/src/sentra/types/connector_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/connector_schema_compute_properties.py` & `fern_sentra-0.0.6/src/sentra/types/connector_schema_compute_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/context_label_schema.py` & `fern_sentra-0.0.6/src/sentra/types/context_label_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/create_class_request_schema_classifier_schema.py` & `fern_sentra-0.0.6/src/sentra/types/create_class_request_schema_classifier_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/create_dictionary_classifier_request_schema.py` & `fern_sentra-0.0.6/src/sentra/types/create_dictionary_classifier_request_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/create_regex_classifier_request_schema.py` & `fern_sentra-0.0.6/src/sentra/types/create_regex_classifier_request_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/current_user_data.py` & `fern_sentra-0.0.6/src/sentra/types/current_user_data.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/dashboard_data.py` & `fern_sentra-0.0.6/src/sentra/types/dashboard_data.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_asset_at_risk.py` & `fern_sentra-0.0.6/src/sentra/types/data_asset_at_risk.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_asset_class_user_operation.py` & `fern_sentra-0.0.6/src/sentra/types/data_asset_class_user_operation.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_asset_extended.py` & `fern_sentra-0.0.6/src/sentra/types/data_asset_extended.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_asset_object.py` & `fern_sentra-0.0.6/src/sentra/types/data_asset_object.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_asset_props.py` & `fern_sentra-0.0.6/src/sentra/types/data_asset_props.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_asset_row.py` & `fern_sentra-0.0.6/src/sentra/types/data_asset_row.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_asset_schema.py` & `fern_sentra-0.0.6/src/sentra/types/data_asset_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_class_config_with_user_schema.py` & `fern_sentra-0.0.6/src/sentra/types/data_class_config_with_user_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_class_item.py` & `fern_sentra-0.0.6/src/sentra/types/data_class_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_dog_integration.py` & `fern_sentra-0.0.6/src/sentra/types/data_dog_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_dog_item.py` & `fern_sentra-0.0.6/src/sentra/types/data_dog_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_dog_region.py` & `fern_sentra-0.0.6/src/sentra/types/data_dog_region.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_hub_fabric.py` & `fern_sentra-0.0.6/src/sentra/types/data_hub_fabric.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_hub_integration.py` & `fern_sentra-0.0.6/src/sentra/types/data_hub_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_hub_item.py` & `fern_sentra-0.0.6/src/sentra/types/data_hub_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_store_access_metadata.py` & `fern_sentra-0.0.6/src/sentra/types/data_store_access_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_store_extended.py` & `fern_sentra-0.0.6/src/sentra/types/data_store_extended.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_store_identity.py` & `fern_sentra-0.0.6/src/sentra/types/data_store_identity.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_store_props.py` & `fern_sentra-0.0.6/src/sentra/types/data_store_props.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_store_risk_aggregation.py` & `fern_sentra-0.0.6/src/sentra/types/data_store_risk_aggregation.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/data_store_row.py` & `fern_sentra-0.0.6/src/sentra/types/data_store_row.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema.py` & `fern_sentra-0.0.6/src/sentra/types/detailed_alert_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_content.py` & `fern_sentra-0.0.6/src/sentra/types/detailed_alert_schema_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_with_comment.py` & `fern_sentra-0.0.6/src/sentra/types/detailed_alert_schema_with_comment.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/detailed_alert_schema_with_comment_content.py` & `fern_sentra-0.0.6/src/sentra/types/detailed_alert_schema_with_comment_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/detailed_iam_group_schema.py` & `fern_sentra-0.0.6/src/sentra/types/detailed_iam_group_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/detailed_iam_role_schema.py` & `fern_sentra-0.0.6/src/sentra/types/detailed_iam_role_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/dictionary_classifier_response.py` & `fern_sentra-0.0.6/src/sentra/types/dictionary_classifier_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/email_input_item.py` & `fern_sentra-0.0.6/src/sentra/types/email_input_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/email_integration.py` & `fern_sentra-0.0.6/src/sentra/types/email_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/email_integration_input.py` & `fern_sentra-0.0.6/src/sentra/types/email_integration_input.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/email_output_item.py` & `fern_sentra-0.0.6/src/sentra/types/email_output_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/event_log_action.py` & `fern_sentra-0.0.6/src/sentra/types/event_log_action.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/event_log_entity_type.py` & `fern_sentra-0.0.6/src/sentra/types/event_log_entity_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/event_log_row.py` & `fern_sentra-0.0.6/src/sentra/types/event_log_row.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/gcp_connector_args.py` & `fern_sentra-0.0.6/src/sentra/types/gcp_connector_args.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/group_item.py` & `fern_sentra-0.0.6/src/sentra/types/group_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/grouped_data_table_result.py` & `fern_sentra-0.0.6/src/sentra/types/grouped_data_table_result.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/http_validation_error.py` & `fern_sentra-0.0.6/src/sentra/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/iam_access_key_schema.py` & `fern_sentra-0.0.6/src/sentra/types/iam_access_key_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/iam_group_data_classes.py` & `fern_sentra-0.0.6/src/sentra/types/iam_group_data_classes.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/iam_group_schema.py` & `fern_sentra-0.0.6/src/sentra/types/iam_group_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/iam_role_data_classes.py` & `fern_sentra-0.0.6/src/sentra/types/iam_role_data_classes.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/iam_role_schema.py` & `fern_sentra-0.0.6/src/sentra/types/iam_role_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart.py` & `fern_sentra-0.0.6/src/sentra/types/identity_accessible_entities_flowchart.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_direct_access.py` & `fern_sentra-0.0.6/src/sentra/types/identity_accessible_entities_flowchart_direct_access.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_group.py` & `fern_sentra-0.0.6/src/sentra/types/identity_accessible_entities_flowchart_group.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/identity_accessible_entities_flowchart_role.py` & `fern_sentra-0.0.6/src/sentra/types/identity_accessible_entities_flowchart_role.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/identity_origin.py` & `fern_sentra-0.0.6/src/sentra/types/identity_origin.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/identity_schema.py` & `fern_sentra-0.0.6/src/sentra/types/identity_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/integration_display.py` & `fern_sentra-0.0.6/src/sentra/types/integration_display.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/integration_display_properties.py` & `fern_sentra-0.0.6/src/sentra/types/integration_display_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/integration_input.py` & `fern_sentra-0.0.6/src/sentra/types/integration_input.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/integration_input_properties.py` & `fern_sentra-0.0.6/src/sentra/types/integration_input_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/integration_output_schema.py` & `fern_sentra-0.0.6/src/sentra/types/integration_output_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/integration_output_schema_properties.py` & `fern_sentra-0.0.6/src/sentra/types/integration_output_schema_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/integration_schema.py` & `fern_sentra-0.0.6/src/sentra/types/integration_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/integration_schema_properties.py` & `fern_sentra-0.0.6/src/sentra/types/integration_schema_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/integration_type.py` & `fern_sentra-0.0.6/src/sentra/types/integration_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/jira_integration.py` & `fern_sentra-0.0.6/src/sentra/types/jira_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/jira_item.py` & `fern_sentra-0.0.6/src/sentra/types/jira_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/keyword_requirement.py` & `fern_sentra-0.0.6/src/sentra/types/keyword_requirement.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_alerts_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_alerts_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_all_assets_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_all_assets_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_all_auth_tokens_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_all_auth_tokens_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_all_connector_displays_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_all_connector_displays_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_all_context_label_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_all_context_label_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_all_data_class_config_with_users_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_all_data_class_config_with_users_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_all_data_stores_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_all_data_stores_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_all_event_log_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_all_event_log_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_all_identities_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_all_identities_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_all_policies_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_all_policies_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_all_roles_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_all_roles_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_all_users_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_all_users_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_similar_assets_pair_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_similar_assets_pair_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_similar_assets_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_similar_assets_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_violated_data_assets_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_violated_data_assets_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/list_violated_objects_response.py` & `fern_sentra-0.0.6/src/sentra/types/list_violated_objects_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/microsoft_365_connector_args.py` & `fern_sentra-0.0.6/src/sentra/types/microsoft_365_connector_args.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/monday_integration.py` & `fern_sentra-0.0.6/src/sentra/types/monday_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/monday_item.py` & `fern_sentra-0.0.6/src/sentra/types/monday_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/new_auth_token_response.py` & `fern_sentra-0.0.6/src/sentra/types/new_auth_token_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/object_class.py` & `fern_sentra-0.0.6/src/sentra/types/object_class.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/open_alerts_aggregation.py` & `fern_sentra-0.0.6/src/sentra/types/open_alerts_aggregation.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/pager_duty_integration.py` & `fern_sentra-0.0.6/src/sentra/types/pager_duty_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/pager_duty_item.py` & `fern_sentra-0.0.6/src/sentra/types/pager_duty_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/permissions.py` & `fern_sentra-0.0.6/src/sentra/types/permissions.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/policy_rule.py` & `fern_sentra-0.0.6/src/sentra/types/policy_rule.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/policy_rule_entity.py` & `fern_sentra-0.0.6/src/sentra/types/policy_rule_entity.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/policy_schema.py` & `fern_sentra-0.0.6/src/sentra/types/policy_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/policy_severity.py` & `fern_sentra-0.0.6/src/sentra/types/policy_severity.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/policy_status.py` & `fern_sentra-0.0.6/src/sentra/types/policy_status.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/policy_triggering_type.py` & `fern_sentra-0.0.6/src/sentra/types/policy_triggering_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/policy_type.py` & `fern_sentra-0.0.6/src/sentra/types/policy_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/policy_update_response.py` & `fern_sentra-0.0.6/src/sentra/types/policy_update_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/proprietary_classifier_response.py` & `fern_sentra-0.0.6/src/sentra/types/proprietary_classifier_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/provider_minimal_metadata.py` & `fern_sentra-0.0.6/src/sentra/types/provider_minimal_metadata.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/provider_schema.py` & `fern_sentra-0.0.6/src/sentra/types/provider_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/provider_types.py` & `fern_sentra-0.0.6/src/sentra/types/provider_types.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/range_filter_data.py` & `fern_sentra-0.0.6/src/sentra/types/range_filter_data.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/regex_classifier_response.py` & `fern_sentra-0.0.6/src/sentra/types/regex_classifier_response.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/resolved_alert_source.py` & `fern_sentra-0.0.6/src/sentra/types/resolved_alert_source.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/risk_type.py` & `fern_sentra-0.0.6/src/sentra/types/risk_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/role_identity.py` & `fern_sentra-0.0.6/src/sentra/types/role_identity.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/role_schema.py` & `fern_sentra-0.0.6/src/sentra/types/role_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/runtime_properties.py` & `fern_sentra-0.0.6/src/sentra/types/runtime_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/schedule_properties.py` & `fern_sentra-0.0.6/src/sentra/types/schedule_properties.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/seemplicity_integration.py` & `fern_sentra-0.0.6/src/sentra/types/seemplicity_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/seemplicity_item.py` & `fern_sentra-0.0.6/src/sentra/types/seemplicity_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/sensitivity_levels.py` & `fern_sentra-0.0.6/src/sentra/types/sensitivity_levels.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/similar_asset_schema.py` & `fern_sentra-0.0.6/src/sentra/types/similar_asset_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/similar_assets_alert_content.py` & `fern_sentra-0.0.6/src/sentra/types/similar_assets_alert_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/similar_assets_pair.py` & `fern_sentra-0.0.6/src/sentra/types/similar_assets_pair.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/similar_assets_pair_schema.py` & `fern_sentra-0.0.6/src/sentra/types/similar_assets_pair_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/similar_assets_props.py` & `fern_sentra-0.0.6/src/sentra/types/similar_assets_props.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/similar_store.py` & `fern_sentra-0.0.6/src/sentra/types/similar_store.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/similarity_type.py` & `fern_sentra-0.0.6/src/sentra/types/similarity_type.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/slack_integration.py` & `fern_sentra-0.0.6/src/sentra/types/slack_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/slack_integration_input.py` & `fern_sentra-0.0.6/src/sentra/types/slack_integration_input.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/slack_web_hook_input_item.py` & `fern_sentra-0.0.6/src/sentra/types/slack_web_hook_input_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/slack_web_hook_output_item.py` & `fern_sentra-0.0.6/src/sentra/types/slack_web_hook_output_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/snowflake_connector_args.py` & `fern_sentra-0.0.6/src/sentra/types/snowflake_connector_args.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/sort.py` & `fern_sentra-0.0.6/src/sentra/types/sort.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/teams_integration.py` & `fern_sentra-0.0.6/src/sentra/types/teams_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/teams_output_item.py` & `fern_sentra-0.0.6/src/sentra/types/teams_output_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/test_connection_result.py` & `fern_sentra-0.0.6/src/sentra/types/test_connection_result.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/update_class_request_schema_classifier_schema.py` & `fern_sentra-0.0.6/src/sentra/types/update_class_request_schema_classifier_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/update_dictionary_classifier_request_schema.py` & `fern_sentra-0.0.6/src/sentra/types/update_dictionary_classifier_request_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/update_regex_classifier_request_schema.py` & `fern_sentra-0.0.6/src/sentra/types/update_regex_classifier_request_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/user_schema.py` & `fern_sentra-0.0.6/src/sentra/types/user_schema.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/validation_error.py` & `fern_sentra-0.0.6/src/sentra/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/violated_data_asset.py` & `fern_sentra-0.0.6/src/sentra/types/violated_data_asset.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/violated_iam_group_alert_content.py` & `fern_sentra-0.0.6/src/sentra/types/violated_iam_group_alert_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/violated_iam_role_alert_content.py` & `fern_sentra-0.0.6/src/sentra/types/violated_iam_role_alert_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/violated_identity_alert_content.py` & `fern_sentra-0.0.6/src/sentra/types/violated_identity_alert_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/violated_object.py` & `fern_sentra-0.0.6/src/sentra/types/violated_object.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/violated_store_alert_content.py` & `fern_sentra-0.0.6/src/sentra/types/violated_store_alert_content.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/web_hook_input_item.py` & `fern_sentra-0.0.6/src/sentra/types/web_hook_input_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/web_hook_integration.py` & `fern_sentra-0.0.6/src/sentra/types/web_hook_integration.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/web_hook_integration_input.py` & `fern_sentra-0.0.6/src/sentra/types/web_hook_integration_input.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/src/sentra/types/web_hook_output_item.py` & `fern_sentra-0.0.6/src/sentra/types/web_hook_output_item.py`

 * *Files identical despite different names*

### Comparing `fern_sentra-0.0.5/PKG-INFO` & `fern_sentra-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-sentra
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

