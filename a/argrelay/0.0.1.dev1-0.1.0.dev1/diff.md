# Comparing `tmp/argrelay-0.0.1.dev1.tar.gz` & `tmp/argrelay-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argrelay-0.0.1.dev1.tar", last modified: Sun Jul  2 08:11:20 2023, max compression
+gzip compressed data, was "argrelay-0.1.0.dev1.tar", last modified: Sat Jul 29 17:41:41 2023, max compression
```

## Comparing `argrelay-0.0.1.dev1.tar` & `argrelay-0.1.0.dev1.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.618641 argrelay-0.0.1.dev1/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2022-12-27 20:38:16.000000 argrelay-0.0.1.dev1/LICENSE
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1002 2023-07-02 08:11:20.618641 argrelay-0.0.1.dev1/PKG-INFO
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.591641 argrelay-0.0.1.dev1/docs/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.594641 argrelay-0.0.1.dev1/docs/dev_notes/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      538 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/dev_notes/argrelay_env_var_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5522 2023-07-02 06:13:07.000000 argrelay-0.0.1.dev1/docs/dev_notes/bootstrap_procedure.1.project_creation.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2508 2023-07-02 06:13:07.000000 argrelay-0.0.1.dev1/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1716 2023-07-02 06:13:07.000000 argrelay-0.0.1.dev1/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2506 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/dev_notes/code_style.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/dev_notes/completion_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5991 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/dev_notes/completion_perf_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4799 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/dev_notes/how_search_works.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1289 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/dev_notes/mongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        6 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/dev_notes/plugin_development.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        6 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/dev_notes/plugin_interaction.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7764 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/dev_notes/query_perf_10_x_more_data_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7125 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/dev_notes/query_perf_cache_vs_no_cache.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4264 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/dev_notes/query_perf_mongomock_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8339 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/dev_notes/query_perf_pymongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/dev_notes/release_procedure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      729 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/dev_notes/screencast_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/dev_notes/scripts_summary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      357 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/docs/dev_notes/semver_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1964 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/docs/dev_notes/term_dictionary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      904 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/docs/dev_notes/testing_guidelines.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10377 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/dev_notes/top_todos.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      758 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/docs/dev_notes/ui_tests_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1637 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/docs/dev_notes/version_format.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.596641 argrelay-0.0.1.dev1/docs/feature_stories/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1922 2023-07-02 07:19:34.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_01_89_09_24.tree_path_selecting_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      983 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      990 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1256 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1685 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      545 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2826 2023-07-02 07:19:34.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_29_54_67_86.dir_structure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1239 2023-07-02 07:19:34.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_31_70_49_15.search_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      392 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1184 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1465 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_41_40_39_44.suggest_from_tree_path.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1251 2023-07-02 07:19:34.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_42_76_93_51.very_first_or_zero_arg_mapping_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2023-07-02 07:19:34.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_46_96_59_05.init_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1478 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_55_57_45_04.demo_logic.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      564 2023-07-02 07:19:34.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_58_61_77_69.dev_shell.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      372 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1439 2023-07-02 07:19:34.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_62_25_92_06.assigned_context.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1316 2023-07-02 07:19:34.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_71_87_33_52.help_hint.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1485 2023-07-02 07:19:34.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_72_40_53_00.fill_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2072 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2023-07-02 06:13:07.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      473 2023-07-02 07:19:34.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_88_66_66_73.intercept_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1385 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2023-07-02 07:19:34.000000 argrelay-0.0.1.dev1/docs/feature_stories/FS_94_30_49_28.help_doc.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      376 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/docs/feature_stories/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.596641 argrelay-0.0.1.dev1/docs/known_issues/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1032 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/docs/known_issues/KI_51_67_38_37.impossible_arg_combinations.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      962 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/known_issues/KI_80_82_13_35.option_list_on_describe_with_prefix.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      325 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/docs/known_issues/KI_99_81_19_25.no_space_in_options.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/known_issues/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      668 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/docs/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.597641 argrelay-0.0.1.dev1/docs/test_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      694 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/test_data/TD_38_03_48_51.large_data_set.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      386 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9497 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/docs/test_data/TD_63_37_05_36.demo_services_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/test_data/TD_70_69_38_46.no_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      398 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/docs/test_data/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.0.1.dev1/pyproject.toml
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15811 2023-06-24 18:15:13.000000 argrelay-0.0.1.dev1/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2023-07-02 08:11:20.618641 argrelay-0.0.1.dev1/setup.cfg
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3849 2023-07-02 06:13:07.000000 argrelay-0.0.1.dev1/setup.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.589641 argrelay-0.0.1.dev1/src/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.597641 argrelay-0.0.1.dev1/src/argrelay/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.598641 argrelay-0.0.1.dev1/src/argrelay/client_command_local/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1679 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/client_command_local/AbstractLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      876 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/client_command_local/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.598641 argrelay-0.0.1.dev1/src/argrelay/client_command_remote/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2290 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3711 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      845 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/client_command_remote/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.599641 argrelay-0.0.1.dev1/src/argrelay/custom_integ/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      282 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/DemoInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      823 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/DemoInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1555 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/DemoInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      807 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/GitRepoArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2733 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/GitRepoDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8951 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/GitRepoLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      639 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      713 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/ServiceArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8041 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/ServiceDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      188 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/ServiceEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    59593 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/ServiceLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      835 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      208 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ/value_constants.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.600641 argrelay-0.0.1.dev1/src/argrelay/custom_integ_res/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6779 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ_res/argrelay_rc.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    20152 2023-07-02 06:13:07.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ_res/bootstrap_dev_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     1150 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ_res/dev_shell.bash
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1875 2023-06-24 18:15:13.000000 argrelay-0.0.1.dev1/src/argrelay/custom_integ_res/init_shell_env.bash
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.601641 argrelay-0.0.1.dev1/src/argrelay/enum_desc/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1158 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/ArgSource.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2701 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/CompType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      568 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/GlobalArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/InterpStep.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      191 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/PluginType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      151 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/ReservedArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      164 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/ReservedEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1163 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/RunMode.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      105 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/SpecialChar.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      106 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/SpecialFunc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      685 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/TermColor.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/TokenType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/enum_desc/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.601641 argrelay-0.0.1.dev1/src/argrelay/handler_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1699 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/handler_request/AbstractServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1242 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      943 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2949 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/handler_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.601641 argrelay-0.0.1.dev1/src/argrelay/handler_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      177 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/handler_response/AbstractClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      716 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      446 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      990 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/handler_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.602641 argrelay-0.0.1.dev1/src/argrelay/misc_helper/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1347 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/misc_helper/AbstractPlugin.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1711 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/misc_helper/ElapsedTime.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      903 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/misc_helper/TypeDesc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1357 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/misc_helper/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.602641 argrelay-0.0.1.dev1/src/argrelay/mongo_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      181 2023-01-16 12:38:17.000000 argrelay-0.0.1.dev1/src/argrelay/mongo_data/MongoClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2389 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/mongo_data/MongoClientWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      413 2023-01-16 12:38:17.000000 argrelay-0.0.1.dev1/src/argrelay/mongo_data/MongoConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      312 2023-01-16 12:38:17.000000 argrelay-0.0.1.dev1/src/argrelay/mongo_data/MongoServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1729 2023-01-16 12:38:17.000000 argrelay-0.0.1.dev1/src/argrelay/mongo_data/MongoServerWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.0.1.dev1/src/argrelay/mongo_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.603641 argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4136 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/AbstractDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1670 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/ErrorDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      807 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5330 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/HelpDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2732 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/InterceptDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1157 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/InvocationInput.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1077 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/NoopDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.604641 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1500 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/AbstractInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      351 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/AbstractInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1034 2023-05-22 13:40:22.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/FirstArgInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1948 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/FirstArgInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      940 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12638 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/FuncArgsInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2524 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/FuncArgsInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      856 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/NoopInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      666 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/NoopInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5770 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/TreePathInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      911 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/TreePathInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1953 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/TreePathInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.604641 argrelay-0.0.1.dev1/src/argrelay/plugin_loader/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_loader/AbstractLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1587 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_loader/HelpLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1675 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_loader/InterceptLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_loader/NoopLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/plugin_loader/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.605641 argrelay-0.0.1.dev1/src/argrelay/relay_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1037 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/relay_client/AbstractClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      460 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/relay_client/AbstractClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1150 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/relay_client/AbstractClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1290 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/relay_client/LocalClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2239 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/relay_client/LocalClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/relay_client/RemoteClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1564 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/relay_client/RemoteClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.0.1.dev1/src/argrelay/relay_client/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2194 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/relay_client/__main__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.606641 argrelay-0.0.1.dev1/src/argrelay/relay_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4692 2023-05-07 10:56:22.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/CustomFlaskApp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      112 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/GuiBannerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1400 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/HelpHintCache.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5767 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/LocalServer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      193 2023-04-02 14:56:48.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/QueryCacheConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5941 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/QueryEngine.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      525 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/QueryResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/__main__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.606641 argrelay-0.0.1.dev1/src/argrelay/relay_server/gui_static/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    27871 2023-05-09 14:35:50.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/gui_static/argrelay_client.js
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4505 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/gui_static/argrelay_style.css
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/gui_static/external_link.svg
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.606641 argrelay-0.0.1.dev1/src/argrelay/relay_server/gui_templates/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5567 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/gui_templates/argrelay_main.html
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5438 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/route_api.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      921 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/relay_server/route_gui.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.607641 argrelay-0.0.1.dev1/src/argrelay/runtime_context/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5467 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_context/EnvelopeContainer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      253 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_context/InitControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2848 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_context/InputContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10107 2023-05-22 14:50:28.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_context/InterpContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5871 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_context/ParsedContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      421 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_context/RequestContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2179 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_context/SearchControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_context/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.608641 argrelay-0.0.1.dev1/src/argrelay/runtime_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       33 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_data/ArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      165 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_data/AssignedValue.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      220 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_data/ClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      140 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_data/ConnectionConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      242 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_data/PluginEntry.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2092 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_data/ServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      604 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_data/StaticData.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/runtime_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.608641 argrelay-0.0.1.dev1/src/argrelay/sample_conf/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/sample_conf/argrelay.client.json
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10432 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/sample_conf/argrelay.server.yaml
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.608641 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1347 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_client/ClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1056 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_client/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.609641 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      850 2023-06-19 19:41:32.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1066 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1621 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/MongoConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1196 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4010 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/ServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1570 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/StaticDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.610641 argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3942 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1088 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/FuncArgsInterpConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1104 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1035 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/InitControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2047 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/SearchControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.610641 argrelay-0.0.1.dev1/src/argrelay/schema_config_plugin/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2598 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_plugin/PluginEntrySchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/schema_config_plugin/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.610641 argrelay-0.0.1.dev1/src/argrelay/schema_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3255 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/schema_request/RequestContextSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/schema_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.611641 argrelay-0.0.1.dev1/src/argrelay/schema_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      706 2023-05-07 13:37:37.000000 argrelay-0.0.1.dev1/src/argrelay/schema_response/ArgValuesSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1742 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_response/AssignedValueSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3026 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_response/EnvelopeContainerSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      856 2023-03-06 12:58:57.000000 argrelay-0.0.1.dev1/src/argrelay/schema_response/FilteredDict.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1170 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/schema_response/InterpResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2126 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/schema_response/InterpResultSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3250 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/schema_response/InvocationInputSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.0.1.dev1/src/argrelay/schema_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.611641 argrelay-0.0.1.dev1/src/argrelay/server_spec/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1543 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/server_spec/DescribeLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1292 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/server_spec/ProposeArgValuesSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1350 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/server_spec/RelayLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.0.1.dev1/src/argrelay/server_spec/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      773 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/server_spec/const_int.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3031 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/server_spec/server_data_schema.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.612641 argrelay-0.0.1.dev1/src/argrelay/test_helper/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    19612 2023-05-20 15:47:09.000000 argrelay-0.0.1.dev1/src/argrelay/test_helper/EnvMockBuilder.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4046 2023-05-14 15:40:58.000000 argrelay-0.0.1.dev1/src/argrelay/test_helper/InOutTestCase.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      718 2023-05-06 16:07:54.000000 argrelay-0.0.1.dev1/src/argrelay/test_helper/OpenFileMock.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1892 2023-05-14 15:38:13.000000 argrelay-0.0.1.dev1/src/argrelay/test_helper/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-02 08:11:20.597641 argrelay-0.0.1.dev1/src/argrelay.egg-info/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1002 2023-07-02 08:11:20.000000 argrelay-0.0.1.dev1/src/argrelay.egg-info/PKG-INFO
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    27780 2023-07-02 08:11:20.000000 argrelay-0.0.1.dev1/src/argrelay.egg-info/SOURCES.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2023-07-02 08:11:20.000000 argrelay-0.0.1.dev1/src/argrelay.egg-info/dependency_links.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      148 2023-07-02 08:11:20.000000 argrelay-0.0.1.dev1/src/argrelay.egg-info/requires.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2023-07-02 08:11:20.000000 argrelay-0.0.1.dev1/src/argrelay.egg-info/top_level.txt
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.791926 argrelay-0.1.0.dev1/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2022-12-27 20:38:16.000000 argrelay-0.1.0.dev1/LICENSE
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1002 2023-07-29 17:41:41.791926 argrelay-0.1.0.dev1/PKG-INFO
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.767926 argrelay-0.1.0.dev1/docs/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.769926 argrelay-0.1.0.dev1/docs/dev_notes/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      538 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/dev_notes/argrelay_env_var_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5522 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/dev_notes/bootstrap_procedure.1.project_creation.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2508 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1716 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2506 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/code_style.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/dev_notes/completion_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5991 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/completion_perf_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4799 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/how_search_works.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1289 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/dev_notes/mongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        6 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/plugin_development.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        6 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/plugin_interaction.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7764 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/query_perf_10_x_more_data_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7125 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/query_perf_cache_vs_no_cache.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4264 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/query_perf_mongomock_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8339 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/query_perf_pymongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/dev_notes/release_procedure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      729 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/dev_notes/screencast_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/dev_notes/scripts_summary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      357 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/semver_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1964 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/term_dictionary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      904 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/testing_guidelines.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10550 2023-07-29 17:16:08.000000 argrelay-0.1.0.dev1/docs/dev_notes/top_todos.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      758 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/ui_tests_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1637 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/dev_notes/version_format.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.771926 argrelay-0.1.0.dev1/docs/feature_stories/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1922 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_01_89_09_24.tree_path_selecting_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      983 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      990 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1256 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1685 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      545 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3030 2023-07-29 07:57:51.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_29_54_67_86.dir_structure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1239 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_31_70_49_15.search_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      392 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1184 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1465 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_41_40_39_44.suggest_from_tree_path.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1251 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_42_76_93_51.very_first_or_zero_arg_mapping_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_46_96_59_05.init_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1478 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_55_57_45_04.demo_logic.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      564 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_58_61_77_69.dev_shell.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      372 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1454 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_62_25_92_06.assigned_context.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1316 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_71_87_33_52.help_hint.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1485 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_72_40_53_00.fill_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2072 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      473 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_88_66_66_73.intercept_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1385 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/docs/feature_stories/FS_94_30_49_28.help_doc.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      376 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/feature_stories/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.771926 argrelay-0.1.0.dev1/docs/known_issues/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1032 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/docs/known_issues/KI_51_67_38_37.impossible_arg_combinations.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      962 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/known_issues/KI_80_82_13_35.option_list_on_describe_with_prefix.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      325 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/docs/known_issues/KI_99_81_19_25.no_space_in_options.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/docs/known_issues/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      668 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.772926 argrelay-0.1.0.dev1/docs/test_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      694 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/docs/test_data/TD_38_03_48_51.large_data_set.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      386 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9497 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/test_data/TD_63_37_05_36.demo_services_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/test_data/TD_70_69_38_46.no_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      398 2023-07-22 05:41:07.000000 argrelay-0.1.0.dev1/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/docs/test_data/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15811 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2023-07-29 17:41:41.791926 argrelay-0.1.0.dev1/setup.cfg
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3849 2023-07-29 17:15:49.000000 argrelay-0.1.0.dev1/setup.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.765926 argrelay-0.1.0.dev1/src/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.772926 argrelay-0.1.0.dev1/src/argrelay/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.773926 argrelay-0.1.0.dev1/src/argrelay/client_command_local/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1642 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/client_command_local/AbstractLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      876 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/client_command_local/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.773926 argrelay-0.1.0.dev1/src/argrelay/client_command_remote/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2252 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3734 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      845 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/client_command_remote/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.774926 argrelay-0.1.0.dev1/src/argrelay/custom_integ/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      282 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/DemoInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      828 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/DemoInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1555 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/DemoInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1272 2023-07-29 16:36:10.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/GitRepoArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      822 2023-07-29 16:20:24.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/GitRepoBasePathConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2841 2023-07-29 15:11:08.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/GitRepoDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10135 2023-07-29 16:38:29.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/GitRepoLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1014 2023-07-29 17:18:28.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      713 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/ServiceArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8041 2023-07-22 04:43:50.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/ServiceDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      188 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/ServiceEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    59593 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/ServiceLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      835 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      209 2023-07-29 15:03:47.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ/value_constants.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.775926 argrelay-0.1.0.dev1/src/argrelay/custom_integ_res/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6779 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ_res/argrelay_rc.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    20152 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ_res/bootstrap_dev_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     1150 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ_res/dev_shell.bash
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1875 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/src/argrelay/custom_integ_res/init_shell_env.bash
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.776926 argrelay-0.1.0.dev1/src/argrelay/enum_desc/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1158 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/ArgSource.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2701 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/CompType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      568 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/GlobalArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/InterpStep.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      191 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/PluginType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      151 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/ReservedArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      164 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/ReservedEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1163 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/RunMode.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      105 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/SpecialChar.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      106 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/SpecialFunc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      685 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/TermColor.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/TokenType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/enum_desc/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.776926 argrelay-0.1.0.dev1/src/argrelay/handler_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1691 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/handler_request/AbstractServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1242 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      943 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2949 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/handler_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.777926 argrelay-0.1.0.dev1/src/argrelay/handler_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      177 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/handler_response/AbstractClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      716 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      446 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      990 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/handler_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.777926 argrelay-0.1.0.dev1/src/argrelay/misc_helper/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1308 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/misc_helper/AbstractPlugin.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1738 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/misc_helper/ElapsedTime.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      950 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/misc_helper/TypeDesc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1360 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/misc_helper/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.777926 argrelay-0.1.0.dev1/src/argrelay/mongo_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      198 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/mongo_data/MongoClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2389 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/mongo_data/MongoClientWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      450 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/mongo_data/MongoConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      349 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/mongo_data/MongoServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1732 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/mongo_data/MongoServerWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.1.0.dev1/src/argrelay/mongo_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.778926 argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4136 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/AbstractDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1670 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/ErrorDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      807 2023-07-22 04:43:50.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5330 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/HelpDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2732 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/InterceptDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1214 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/InvocationInput.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1077 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/NoopDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.779926 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1444 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/AbstractInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      351 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/AbstractInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      646 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/FirstArgInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1948 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/FirstArgInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      940 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12638 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/FuncArgsInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2524 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/FuncArgsInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      833 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/NoopInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      666 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/NoopInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5734 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/TreePathInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      911 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/TreePathInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/TreePathInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.780926 argrelay-0.1.0.dev1/src/argrelay/plugin_loader/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_loader/AbstractLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1587 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_loader/HelpLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1675 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_loader/InterceptLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_loader/NoopLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/plugin_loader/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.780926 argrelay-0.1.0.dev1/src/argrelay/relay_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1028 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_client/AbstractClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      439 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_client/AbstractClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1150 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/relay_client/AbstractClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1290 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/relay_client/LocalClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2204 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_client/LocalClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/relay_client/RemoteClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1546 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_client/RemoteClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.1.0.dev1/src/argrelay/relay_client/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2180 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_client/__main__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.781926 argrelay-0.1.0.dev1/src/argrelay/relay_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4665 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/CustomFlaskApp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      139 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/GuiBannerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1419 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/HelpHintCache.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5700 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/LocalServer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      251 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/QueryCacheConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5872 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/QueryEngine.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      562 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/QueryResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/__main__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.781926 argrelay-0.1.0.dev1/src/argrelay/relay_server/gui_static/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    27871 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/gui_static/argrelay_client.js
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4505 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/gui_static/argrelay_style.css
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/gui_static/external_link.svg
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.781926 argrelay-0.1.0.dev1/src/argrelay/relay_server/gui_templates/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5567 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/gui_templates/argrelay_main.html
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5438 2023-07-22 04:43:50.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/route_api.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      922 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/relay_server/route_gui.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.782926 argrelay-0.1.0.dev1/src/argrelay/runtime_context/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5451 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_context/EnvelopeContainer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_context/InitControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2875 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_context/InputContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10157 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_context/InterpContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5871 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_context/ParsedContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      468 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_context/RequestContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2179 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_context/SearchControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_context/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.783926 argrelay-0.1.0.dev1/src/argrelay/runtime_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_data/AssignedValue.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      247 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_data/ClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_data/ConnectionConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      289 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_data/PluginEntry.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2162 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_data/ServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      604 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_data/StaticData.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/runtime_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.783926 argrelay-0.1.0.dev1/src/argrelay/sample_conf/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2023-07-22 05:44:14.000000 argrelay-0.1.0.dev1/src/argrelay/sample_conf/argrelay.client.json
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10576 2023-07-29 17:37:23.000000 argrelay-0.1.0.dev1/src/argrelay/sample_conf/argrelay.server.yaml
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.783926 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1347 2023-07-22 06:00:32.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_client/ClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1056 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_client/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.784926 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      852 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1066 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1621 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/MongoConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1196 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3999 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/ServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1570 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/StaticDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.784926 argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3942 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1088 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/FuncArgsInterpConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1104 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1035 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/InitControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2047 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/SearchControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.784926 argrelay-0.1.0.dev1/src/argrelay/schema_config_plugin/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2598 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_plugin/PluginEntrySchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/schema_config_plugin/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.784926 argrelay-0.1.0.dev1/src/argrelay/schema_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3257 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/schema_request/RequestContextSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/schema_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.785926 argrelay-0.1.0.dev1/src/argrelay/schema_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      706 2023-05-07 13:37:37.000000 argrelay-0.1.0.dev1/src/argrelay/schema_response/ArgValuesSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1742 2023-03-06 12:58:57.000000 argrelay-0.1.0.dev1/src/argrelay/schema_response/AssignedValueSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3026 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/schema_response/EnvelopeContainerSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      856 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/schema_response/FilteredDict.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1207 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/schema_response/InterpResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2126 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/schema_response/InterpResultSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3250 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/schema_response/InvocationInputSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.1.0.dev1/src/argrelay/schema_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.785926 argrelay-0.1.0.dev1/src/argrelay/server_spec/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1543 2023-07-22 04:43:50.000000 argrelay-0.1.0.dev1/src/argrelay/server_spec/DescribeLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1268 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/server_spec/ProposeArgValuesSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1325 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/server_spec/RelayLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.1.0.dev1/src/argrelay/server_spec/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      772 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/server_spec/const_int.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3031 2023-07-22 04:43:50.000000 argrelay-0.1.0.dev1/src/argrelay/server_spec/server_data_schema.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.785926 argrelay-0.1.0.dev1/src/argrelay/test_helper/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    20113 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/test_helper/EnvMockBuilder.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4046 2023-07-11 13:28:30.000000 argrelay-0.1.0.dev1/src/argrelay/test_helper/InOutTestCase.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      684 2023-07-29 07:51:27.000000 argrelay-0.1.0.dev1/src/argrelay/test_helper/OpenFileMock.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1892 2023-07-08 16:56:00.000000 argrelay-0.1.0.dev1/src/argrelay/test_helper/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-07-29 17:41:41.772926 argrelay-0.1.0.dev1/src/argrelay.egg-info/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1002 2023-07-29 17:41:41.000000 argrelay-0.1.0.dev1/src/argrelay.egg-info/PKG-INFO
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    27763 2023-07-29 17:41:41.000000 argrelay-0.1.0.dev1/src/argrelay.egg-info/SOURCES.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2023-07-29 17:41:41.000000 argrelay-0.1.0.dev1/src/argrelay.egg-info/dependency_links.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      148 2023-07-29 17:41:41.000000 argrelay-0.1.0.dev1/src/argrelay.egg-info/requires.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2023-07-29 17:41:41.000000 argrelay-0.1.0.dev1/src/argrelay.egg-info/top_level.txt
```

### Comparing `argrelay-0.0.1.dev1/LICENSE` & `argrelay-0.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/PKG-INFO` & `argrelay-0.1.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.0.1.dev1
+Version: 0.1.0.dev1
 Summary: Tab-completion & data search server - total recall
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Environment :: Console
```

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/argrelay_env_var_notes.md` & `argrelay-0.1.0.dev1/docs/dev_notes/argrelay_env_var_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/bootstrap_procedure.1.project_creation.md` & `argrelay-0.1.0.dev1/docs/dev_notes/bootstrap_procedure.1.project_creation.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md` & `argrelay-0.1.0.dev1/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md` & `argrelay-0.1.0.dev1/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/code_style.md` & `argrelay-0.1.0.dev1/docs/dev_notes/code_style.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/completion_notes.md` & `argrelay-0.1.0.dev1/docs/dev_notes/completion_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/completion_perf_notes.md` & `argrelay-0.1.0.dev1/docs/dev_notes/completion_perf_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/how_search_works.md` & `argrelay-0.1.0.dev1/docs/dev_notes/how_search_works.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/mongo_notes.md` & `argrelay-0.1.0.dev1/docs/dev_notes/mongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/query_perf_10_x_more_data_notes.md` & `argrelay-0.1.0.dev1/docs/dev_notes/query_perf_10_x_more_data_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/query_perf_cache_vs_no_cache.md` & `argrelay-0.1.0.dev1/docs/dev_notes/query_perf_cache_vs_no_cache.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/query_perf_mongomock_notes.md` & `argrelay-0.1.0.dev1/docs/dev_notes/query_perf_mongomock_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/query_perf_pymongo_notes.md` & `argrelay-0.1.0.dev1/docs/dev_notes/query_perf_pymongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/release_procedure.md` & `argrelay-0.1.0.dev1/docs/dev_notes/release_procedure.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/screencast_notes.md` & `argrelay-0.1.0.dev1/docs/dev_notes/screencast_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/scripts_summary.md` & `argrelay-0.1.0.dev1/docs/dev_notes/scripts_summary.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/term_dictionary.md` & `argrelay-0.1.0.dev1/docs/dev_notes/term_dictionary.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/testing_guidelines.md` & `argrelay-0.1.0.dev1/docs/dev_notes/testing_guidelines.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/top_todos.md` & `argrelay-0.1.0.dev1/docs/dev_notes/top_todos.md`

 * *Files 3% similar despite different names*

```diff
@@ -158,26 +158,26 @@
 
 *   Add consciously written semver doc.
 
 Ease integration into external project:
 
 *   Enable debug in all bootstrap scripts.
 
-*   How to deal with `@/exe/dev_shell.bash` symlink in custom project?
-    This symlink (unlike inside `argrelay` itself) is not pointing into existing file within the repo,
-    instead, it points into `argrelay` package which still has to be installed.
-
 *   There is constant need to distinguish:
     *   project_dir - the path to special dir (where venv is configured via relative path, artifacts generated, config files, etc.)
     *   package_dir - the path to useful artifacts (where known after venv is sourced)
 
 *   Split `argrelay.server.yaml` into: `argrelay.common.yaml` and `argrelay.server.yaml`.
+    Or at least make it less confusing (because client-side still uses `argrelay.server.yaml`).
+    Maybe instead of "common", it should be called `argrelay.plugins.yaml` which is exactly the part seen and
+    reused by both server and client?
 
 *   Make it possible to override location of `@/conf/` via env var
     (to allow experimental development co-exists).
+    See `FS_16_07_78_84.conf_dir_priority.md` - is it done?
 
 *   Make yaml config composable (to reduce chances of merging):
     allow loading external config which should plug itself into existing config.
     Maybe it should be possible to provide just configured plugins and they
 
 *   Extend EnvMock to help testing on external project side.
     Basically, the main one is a mock to ensure some function is called (although, that's easily done without EnvMock).
@@ -198,14 +198,15 @@
     https://stackoverflow.com/a/11991854/441652
 
 Docs:
 
 *   Split "arg" group of concepts (`arg_value`, `arg_type`) and "prop" group of concepts (`prop_value`, `prop_type`):
     *   `command_line` args are mapped to `data_envelope` props and almost identical
     *   BUT: they are not naturally/intuitively inter-change-able as `data_envelope` properties are hardly `command_line` arguments.
+    *   Maybe write doc on bounded contexts? Add dictionaries (ubiquitous language) per bash, client, server, data backend?
 
 Extra:
 
 *   Add version arg type to the test data.
 
 *   Make describe output take into account current prefix (incomplete and not yet consumed) arg
     which matches several options (which are suggested on Tab, but describe should reduce output from all to just
```

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/ui_tests_notes.md` & `argrelay-0.1.0.dev1/docs/dev_notes/ui_tests_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/dev_notes/version_format.md` & `argrelay-0.1.0.dev1/docs/dev_notes/version_format.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_01_89_09_24.tree_path_selecting_interp.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_01_89_09_24.tree_path_selecting_interp.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_06_99_43_60.list_arg_value.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_06_99_43_60.list_arg_value.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_29_54_67_86.dir_structure.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_29_54_67_86.dir_structure.md`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,19 @@
 It is not supposed to be version controlled by this repo.
 
 In practice, to keep config under version control, `@/conf/` can be a symlink which
 points to different version controlled dir (see sub-dirs under `@/dst/`) depending on the target deployment environment.
 
 To avoid being detected as modified when target deployment environment changes, this `@/conf/` symlink is not committed.
 
+This path is the default (lowest priority) - see [`FS_16_07_78_84.conf_dir_priority.md`][FS_16_07_78_84.conf_dir_priority.md].
+
 # `@/dst/`
 
 This dir contains sub-dirs with config files for multiple target environments.
 
 For example:
 *   Dir `@/dst/` may contain sub-dirs: `@/dst/target_env_a` and `@/dst/target_env_b`.
 *   When the project is deployed to environment `target_env_a`, `@/conf/` should be a symlink to `@/dst/target_env_a`.
 *   When the project is deployed to environment `target_env_b`, `@/conf/` should be a symlink to `@/dst/target_env_b`.
+
+[FS_16_07_78_84.conf_dir_priority.md]: FS_16_07_78_84.conf_dir_priority.md
```

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_31_70_49_15.search_control.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_31_70_49_15.search_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_41_40_39_44.suggest_from_tree_path.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_41_40_39_44.suggest_from_tree_path.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_42_76_93_51.very_first_or_zero_arg_mapping_interp.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_42_76_93_51.very_first_or_zero_arg_mapping_interp.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_55_57_45_04.demo_logic.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_55_57_45_04.demo_logic.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_58_61_77_69.dev_shell.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_58_61_77_69.dev_shell.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_62_25_92_06.assigned_context.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_62_25_92_06.assigned_context.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ---
 feature_story: FS_62_25_92_06
-feature_title: assigned_context
+feature_title: manipulating `assigned_context`
 feature_status: TODO
 ---
 
 TODO: Merge `assigned_context` and `args_context`? Because plural `args_` is easily singular `arg_`.
 TODO: Figure out how to deal with over-specified context.
       How to solve problem when context extra arg type = arg value entry hides `data_envelope`-s
       (which do not contain such entry) from search results?
```

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_71_87_33_52.help_hint.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_71_87_33_52.help_hint.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_72_40_53_00.fill_control.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_72_40_53_00.fill_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md` & `argrelay-0.1.0.dev1/docs/feature_stories/FS_90_48_11_45.force_assignment_from_entire_type_value_space.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/known_issues/KI_51_67_38_37.impossible_arg_combinations.md` & `argrelay-0.1.0.dev1/docs/known_issues/KI_51_67_38_37.impossible_arg_combinations.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/known_issues/KI_80_82_13_35.option_list_on_describe_with_prefix.md` & `argrelay-0.1.0.dev1/docs/known_issues/KI_80_82_13_35.option_list_on_describe_with_prefix.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/readme.md` & `argrelay-0.1.0.dev1/docs/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md` & `argrelay-0.1.0.dev1/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/test_data/TD_63_37_05_36.demo_services_data.md` & `argrelay-0.1.0.dev1/docs/test_data/TD_63_37_05_36.demo_services_data.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/docs/test_data/TD_70_69_38_46.no_data.md` & `argrelay-0.1.0.dev1/docs/test_data/TD_70_69_38_46.no_data.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/readme.md` & `argrelay-0.1.0.dev1/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/setup.py` & `argrelay-0.1.0.dev1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # All paths start with `top_dir_path`:
     return file_paths
 
 
 setuptools.setup(
     name = "argrelay",
     # See `docs/dev_notes/version_format.md`:
-    version = "0.0.1.dev1",
+    version = "0.1.0.dev1",
     author = "uvsmtid",
     author_email = "uvsmtid@gmail.com",
     description = "Tab-completion & data search server - total recall",
     long_description = """
 See: https://github.com/argrelay/argrelay
     """,
     long_description_content_type = "text/markdown",
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/client_command_local/AbstractLocalClientCommand.py` & `argrelay-0.1.0.dev1/src/argrelay/client_command_local/AbstractLocalClientCommand.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,33 +5,30 @@
 from argrelay.relay_server.LocalServer import LocalServer
 from argrelay.runtime_context.InputContext import InputContext
 from argrelay.runtime_context.InterpContext import InterpContext
 from argrelay.runtime_data.ServerConfig import ServerConfig
 
 
 class AbstractLocalClientCommand(AbstractClientCommand):
-    server_config: ServerConfig
-    local_server: LocalServer
-    request_handler: AbstractServerRequestHandler
-    response_dict: dict
-    interp_ctx: InterpContext
 
     def __init__(
         self,
         server_config: ServerConfig,
         local_server: LocalServer,
         request_handler: AbstractServerRequestHandler,
         response_handler: AbstractClientResponseHandler,
     ):
         super().__init__(
             response_handler,
         )
-        self.server_config = server_config
-        self.local_server = local_server
-        self.request_handler = request_handler
+        self.server_config: ServerConfig = server_config
+        self.local_server: LocalServer = local_server
+        self.request_handler: AbstractServerRequestHandler = request_handler
+        self.response_dict: dict
+        self.interp_ctx: InterpContext
 
     def execute_command(self, input_ctx: InputContext):
         self.response_dict = self.request_handler.handle_request(input_ctx)
         ElapsedTime.measure("before_sending_response")
         self.response_handler.handle_response(self.response_dict)
         ElapsedTime.measure("after_handle_response")
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py` & `argrelay-0.1.0.dev1/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py` & `argrelay-0.1.0.dev1/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py` & `argrelay-0.1.0.dev1/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py` & `argrelay-0.1.0.dev1/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,34 +10,30 @@
 from argrelay.runtime_context.InputContext import InputContext
 from argrelay.runtime_data.ConnectionConfig import ConnectionConfig
 from argrelay.schema_request.RequestContextSchema import request_context_desc
 from argrelay.server_spec.const_int import BASE_URL_FORMAT
 
 
 class AbstractRemoteClientCommand(AbstractClientCommand):
-    server_path: str
-    connection_config: ConnectionConfig
-    response_schema: Schema
-    request_schema: Schema
 
     def __init__(
         self,
-        server_path,
-        connection_config,
+        server_path: str,
+        connection_config: ConnectionConfig,
         response_handler: AbstractClientResponseHandler,
-        response_schema,
-        request_schema = request_context_desc.dict_schema,
+        response_schema: Schema,
+        request_schema: Schema = request_context_desc.dict_schema,
     ):
         super().__init__(
             response_handler,
         )
-        self.server_path = server_path
-        self.connection_config = connection_config
-        self.response_schema = response_schema
-        self.request_schema = request_schema
+        self.server_path: str = server_path
+        self.connection_config: ConnectionConfig = connection_config
+        self.response_schema: Schema = response_schema
+        self.request_schema: Schema = request_schema
 
     def execute_command(self, input_ctx: InputContext):
         server_url = BASE_URL_FORMAT.format(**asdict(self.connection_config)) + f"{self.server_path}"
         headers_dict = {
             "Content-Type": "application/json",
         }
         request_json = self.request_schema.dumps(input_ctx)
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py` & `argrelay-0.1.0.dev1/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py` & `argrelay-0.1.0.dev1/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     def __init__(
         self,
         connection_config: ConnectionConfig,
     ):
         super().__init__(
             ProposeArgValuesClientResponseHandler(),
         )
-        self.connection_config = connection_config
-        self.server_path = PROPOSE_ARG_VALUES_PATH
+        self.connection_config: ConnectionConfig = connection_config
+        self.server_path: str = PROPOSE_ARG_VALUES_PATH
 
     def execute_command(self, input_ctx: InputContext):
 
         s = socket.socket(
             socket.AF_INET,
             socket.SOCK_STREAM,
         )
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py` & `argrelay-0.1.0.dev1/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ/DemoInterpFactory.py` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ/DemoInterpFactory.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from argrelay.runtime_context.InterpContext import InterpContext
 
 
 class DemoInterpFactory(AbstractInterpFactory):
 
     def __init__(
         self,
-        plugin_instance_id,
+        plugin_instance_id: str,
         config_dict: dict,
     ):
         super().__init__(
             plugin_instance_id,
             config_dict,
         )
         demo_interp_factory_config_desc.validate_dict(config_dict)
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ/DemoInterpFactoryConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ/DemoInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ/GitRepoDelegator.py` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ/GitRepoDelegator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import subprocess
 
-from argrelay.custom_integ.value_constants import desc_repo_func_, desc_commit_func_
+from argrelay.custom_integ.value_constants import goto_repo_func_, desc_commit_func_
+from argrelay.misc_helper import eprint
 from argrelay.plugin_delegator.AbstractDelegator import AbstractDelegator, get_data_envelopes
 from argrelay.plugin_delegator.InvocationInput import InvocationInput
 from argrelay.relay_server.LocalServer import LocalServer
 from argrelay.runtime_context.InterpContext import InterpContext, function_envelope_ipos_
 from argrelay.schema_config_interp.DataEnvelopeSchema import envelope_payload_, envelope_id_, instance_data_
 from argrelay.schema_config_interp.FunctionEnvelopeInstanceDataSchema import delegator_plugin_instance_id_
 
@@ -42,23 +43,24 @@
             data_envelopes = get_data_envelopes(interp_ctx),
             custom_plugin_data = {},
         )
         return invocation_input
 
     @staticmethod
     def invoke_action(invocation_input: InvocationInput):
-        if invocation_input.data_envelopes[function_envelope_ipos_][envelope_id_] == desc_repo_func_:
+        if invocation_input.data_envelopes[function_envelope_ipos_][envelope_id_] == goto_repo_func_:
             repo_envelope = invocation_input.data_envelopes[repo_envelope_ipos_]
             abs_repo_path = repo_envelope[envelope_payload_]["abs_repo_path"]
+            eprint(f"INFO: starting subshell in: {abs_repo_path}")
             # List Git repo dir:
             subproc = subprocess.run(
                 [
-                    "ls",
-                    "-lrt",
-                    abs_repo_path,
+                    "bash",
+                    "-l",
                 ],
+                cwd = abs_repo_path
             )
             ret_code = subproc.returncode
             if ret_code != 0:
                 raise RuntimeError
         if invocation_input.data_envelopes[function_envelope_ipos_][envelope_id_] == desc_commit_func_:
             raise RuntimeError("not implemented")
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ/GitRepoLoader.py` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ/GitRepoLoader.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 
 import os
 import subprocess
 
 from git import Repo
 
 from argrelay.custom_integ.GitRepoArgType import GitRepoArgType
+from argrelay.custom_integ.GitRepoBasePathConfigSchema import base_path_, repo_aliases_
 from argrelay.custom_integ.GitRepoDelegator import GitRepoDelegator
 from argrelay.custom_integ.GitRepoEnvelopeClass import GitRepoEnvelopeClass
-from argrelay.custom_integ.GitRepoLoaderConfigSchema import base_path_, git_repo_loader_config_desc, is_plugin_enabled_
-from argrelay.custom_integ.value_constants import desc_repo_func_, desc_commit_func_
+from argrelay.custom_integ.GitRepoLoaderConfigSchema import (
+    git_repo_loader_config_desc,
+    is_plugin_enabled_,
+    load_repo_commits_, base_paths_,
+)
+from argrelay.custom_integ.value_constants import goto_repo_func_, desc_commit_func_
 from argrelay.enum_desc.GlobalArgType import GlobalArgType
 from argrelay.enum_desc.ReservedArgType import ReservedArgType
 from argrelay.enum_desc.ReservedEnvelopeClass import ReservedEnvelopeClass
 from argrelay.misc_helper import eprint
 from argrelay.plugin_loader.AbstractLoader import AbstractLoader
 from argrelay.runtime_data.StaticData import StaticData
 from argrelay.schema_config_interp.DataEnvelopeSchema import (
@@ -47,15 +52,26 @@
         """
 
         if not self.config_dict:
             return static_data
         if not self.config_dict[is_plugin_enabled_]:
             return static_data
 
-        base_path = os.path.normpath(os.path.expanduser(self.config_dict[base_path_]))
+        for base_path_config in self.config_dict[base_paths_]:
+            static_data = self.load_git_objects(static_data, base_path_config)
+
+        static_data = self.load_git_funcs(static_data)
+
+        return static_data
+
+    def load_git_objects(self, static_data: StaticData, base_path_config: dict) -> StaticData:
+
+        data_envelopes = static_data.data_envelopes
+
+        base_path = os.path.normpath(os.path.expanduser(base_path_config[base_path_]))
         # Map Git abs path to Git rel path:
         git_repo_paths = {}
         # Collect Git root paths under `base_path` from config:
         for root_path, ignored_dirs, ignored_files in os.walk(base_path, followlinks = True):
             root_path = os.path.normpath(root_path)
 
             # Skip if sub-path of known Git (do not support Git repo under Git repo):
@@ -93,16 +109,14 @@
                 continue
 
         # Init type keys (if they do not exist):
         for type_name in [enum_item.name for enum_item in GitRepoArgType]:
             if type_name not in static_data.known_arg_types:
                 static_data.known_arg_types.append(type_name)
 
-        data_envelopes = static_data.data_envelopes
-
         eprint("Git repos found:")
         for abs_git_path in git_repo_paths.keys():
             print(f"{abs_git_path}: {git_repo_paths[abs_git_path]}")
 
         for abs_git_path in git_repo_paths.keys():
             rel_git_path = git_repo_paths[abs_git_path]
             print(f"Git repo to load: {rel_git_path}")
@@ -111,14 +125,18 @@
             # base_path_ = "/path/to/base/dir/"
             # abs_git_path = "/path/to/base/dir/rel/path/to/git/repo.git/"
             # then:
             # rel_git_path = "rel/path/to/git/repo.git/"
             # path_comp_list = [ "rel", "path", "to", "git", "repo" ]
             rel_git_path = git_repo_paths[abs_git_path]
 
+            repo_alias = "UNKNOWN_ALIAS"
+            if rel_git_path in base_path_config[repo_aliases_]:
+                repo_alias = base_path_config[repo_aliases_][rel_git_path]
+
             path_comp_list = []
             for rel_git_path_comp in rel_git_path.split(os.sep)[:-1]:
                 if rel_git_path_comp not in path_comp_list:
                     path_comp_list.append(rel_git_path_comp)
 
             ############################################################################################################
             # repos
@@ -126,76 +144,90 @@
             repo_envelope = {
                 envelope_id_: rel_git_path,
                 envelope_payload_: {
                     "abs_repo_path": abs_git_path,
                 },
                 ReservedArgType.EnvelopeClass.name: GitRepoEnvelopeClass.ClassGitRepo.name,
                 GlobalArgType.ObjectSelector.name: "repo",
+                GitRepoArgType.GitRepoAlias.name: repo_alias,
                 GitRepoArgType.GitRepoRelPath.name: rel_git_path,
+                GitRepoArgType.GitRepoBaseAbsPath.name: abs_git_path,
                 GitRepoArgType.GitRepoPathComp.name: path_comp_list,
-                # TODO: FS_06_99_43_60: populate list of remotes:
-                GitRepoArgType.GitRepoRemoteUrl.name: [],
-                # TODO: FS_06_99_43_60: populate list of local branches:
-                GitRepoArgType.GitRepoLocalBranch.name: [],
             }
             print(repo_envelope)
             data_envelopes.append(repo_envelope)
 
+            if not self.config_dict[load_repo_commits_]:
+                continue
+
             git_repo = Repo(abs_git_path)
             for git_commit in git_repo.iter_commits():
                 ########################################################################################################
                 # commits
 
                 commit_envelope = {
                     envelope_id_: f"{rel_git_path}:{git_commit.hexsha}",
                     envelope_payload_: {
                     },
                     ReservedArgType.EnvelopeClass.name: GitRepoEnvelopeClass.ClassGitCommit.name,
                     GlobalArgType.ObjectSelector.name: "commit",
+                    GitRepoArgType.GitRepoAlias.name: repo_alias,
                     GitRepoArgType.GitRepoRelPath.name: rel_git_path,
+                    GitRepoArgType.GitRepoBaseAbsPath.name: abs_git_path,
+                    GitRepoArgType.GitRepoPathComp.name: path_comp_list,
                     GitRepoArgType.GitRepoCommitId.name: git_commit.hexsha,
                     GitRepoArgType.GitRepoCommitAuthorName.name: git_commit.author.name,
                     GitRepoArgType.GitRepoCommitAuthorEmail.name: git_commit.author.email,
                     GitRepoArgType.GitRepoCommitMessage.name: git_commit.message,
                 }
                 print(commit_envelope)
                 data_envelopes.append(commit_envelope)
 
+        return static_data
+
+    # noinspection PyMethodMayBeStatic
+    def load_git_funcs(self, static_data: StaticData) -> StaticData:
+
+        data_envelopes = static_data.data_envelopes
+
         ###############################################################################################################
         # functions
 
         repo_search_control = {
             envelope_class_: GitRepoEnvelopeClass.ClassGitRepo.name,
             keys_to_types_list_: [
-                {"part": GitRepoArgType.GitRepoPathComp.name},
+                {"alias": GitRepoArgType.GitRepoAlias.name},
                 {"path": GitRepoArgType.GitRepoRelPath.name},
+                {"base": GitRepoArgType.GitRepoBaseAbsPath.name},
+                {"part": GitRepoArgType.GitRepoPathComp.name},
             ],
         }
 
         commit_search_control = {
             envelope_class_: GitRepoEnvelopeClass.ClassGitCommit.name,
             keys_to_types_list_: [
                 {"path": GitRepoArgType.GitRepoRelPath.name},
+                {"base": GitRepoArgType.GitRepoBaseAbsPath.name},
                 {"email": GitRepoArgType.GitRepoCommitAuthorEmail.name},
                 {"hex": GitRepoArgType.GitRepoCommitId.name},
             ],
         }
 
         given_function_envelope = {
-            envelope_id_: desc_repo_func_,
+            envelope_id_: goto_repo_func_,
             instance_data_: {
                 delegator_plugin_instance_id_: GitRepoDelegator.__name__,
                 search_control_list_: [
                     repo_search_control,
                 ],
             },
             ReservedArgType.EnvelopeClass.name: ReservedEnvelopeClass.ClassFunction.name,
             ReservedArgType.HelpHint.name: "Describe Git repository",
             GlobalArgType.FunctionCategory.name: "external",
-            GlobalArgType.ActionType.name: "desc",
+            GlobalArgType.ActionType.name: "goto",
             GlobalArgType.ObjectSelector.name: "repo",
         }
         data_envelopes.append(given_function_envelope)
 
         given_function_envelope = {
             envelope_id_: desc_commit_func_,
             instance_data_: {
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ/ServiceArgType.py` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ/ServiceArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ/ServiceDelegator.py` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ/ServiceDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ/ServiceLoader.py` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ/ServiceLoader.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ_res/argrelay_rc.bash` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ_res/argrelay_rc.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ_res/bootstrap_dev_env.bash` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ_res/bootstrap_dev_env.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ_res/dev_shell.bash` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ_res/dev_shell.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/custom_integ_res/init_shell_env.bash` & `argrelay-0.1.0.dev1/src/argrelay/custom_integ_res/init_shell_env.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/enum_desc/ArgSource.py` & `argrelay-0.1.0.dev1/src/argrelay/enum_desc/ArgSource.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/enum_desc/CompType.py` & `argrelay-0.1.0.dev1/src/argrelay/enum_desc/CompType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/enum_desc/GlobalArgType.py` & `argrelay-0.1.0.dev1/src/argrelay/enum_desc/GlobalArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/enum_desc/RunMode.py` & `argrelay-0.1.0.dev1/src/argrelay/enum_desc/RunMode.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/enum_desc/TermColor.py` & `argrelay-0.1.0.dev1/src/argrelay/enum_desc/TermColor.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/enum_desc/TokenType.py` & `argrelay-0.1.0.dev1/src/argrelay/enum_desc/TokenType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/handler_request/AbstractServerRequestHandler.py` & `argrelay-0.1.0.dev1/src/argrelay/handler_request/AbstractServerRequestHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 from argrelay.runtime_context.InputContext import InputContext
 from argrelay.runtime_context.InterpContext import InterpContext
 from argrelay.runtime_context.ParsedContext import ParsedContext
 from argrelay.runtime_context.RequestContext import RequestContext
 
 
 class AbstractServerRequestHandler:
-    local_server: LocalServer
-    interp_ctx: InterpContext
 
     def __init__(
         self,
         local_server: LocalServer,
     ):
-        self.local_server = local_server
+        self.local_server: LocalServer = local_server
+        self.interp_ctx: InterpContext
 
     def handle_request(self, input_ctx: InputContext) -> dict:
         raise NotImplementedError
 
     @staticmethod
     def create_input_ctx(request_ctx: RequestContext, run_mode: RunMode):
         input_ctx = InputContext.from_request_context(
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py` & `argrelay-0.1.0.dev1/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py` & `argrelay-0.1.0.dev1/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py` & `argrelay-0.1.0.dev1/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py` & `argrelay-0.1.0.dev1/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py` & `argrelay-0.1.0.dev1/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/misc_helper/AbstractPlugin.py` & `argrelay-0.1.0.dev1/src/argrelay/misc_helper/AbstractPlugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import importlib
 from typing import Type
 
 
 class AbstractPlugin:
-    plugin_instance_id: str
-    config_dict: dict
 
     def __init__(
         self,
         plugin_instance_id: str,
         config_dict: dict,
     ):
-        self.plugin_instance_id = plugin_instance_id
-        self.config_dict = config_dict
+        self.plugin_instance_id: str = plugin_instance_id
+        self.config_dict: dict = config_dict
 
     def activate_plugin(self):
         """
         One-time plugin activation callback during server startup.
 
         This is a chance to initialize (once) any resources plugin requires.
         """
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/misc_helper/ElapsedTime.py` & `argrelay-0.1.0.dev1/src/argrelay/misc_helper/ElapsedTime.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 import time
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import ClassVar
 
 from argrelay.misc_helper import eprint
 
 
 @dataclass
 class ElapsedTime:
     """
     *   Instance holds a named timestamp.
     *   Class maintains a list of all instances (named timestamps) stored in order of measurements.
 
     At the moment, a static singleton is enough as perf measurements are done with single client.
     """
 
-    name: str
-    ts: int
+    name: str = field()
+    ts: int = field()
 
     all_ts: ClassVar[list[ElapsedTime]] = []
 
     is_debug_enabled: bool = False
     """
     This is normally set based on `RequestContext.is_debug_enabled`.
     """
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/misc_helper/TypeDesc.py` & `argrelay-0.1.0.dev1/src/argrelay/misc_helper/TypeDesc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 import yaml
 from marshmallow import Schema, ValidationError
 
 
 @dataclass(frozen = True)
 class TypeDesc:
     """
     Type descriptor: schema, example, etc.
     """
 
-    dict_schema: Schema
-    ref_name: str
-    dict_example: dict
-    default_file_path: str
+    dict_schema: Schema = field()
+    ref_name: str = field()
+    dict_example: dict = field()
+    default_file_path: str = field()
 
     def from_default_file(self):
         return self.from_yaml_file(self.default_file_path)
 
     def from_yaml_file(self, file_path: str):
         return self.from_input_dict(yaml.safe_load(open(file_path)))
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/misc_helper/__init__.py` & `argrelay-0.1.0.dev1/src/argrelay/misc_helper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 import sys
 from os.path import dirname
 
 # This global variable is overridden by `run_argrelay_client` or `run_argrelay_server`:
 # FS_29_54_67_86 dir_structure: `@/src/argrelay/misc_helper/__init__.py` -> `@/`:
 _argrelay_dir = dirname(dirname(dirname(dirname(os.path.abspath(__file__)))))
 
+
 def set_argrelay_dir(argrelay_dir):
     global _argrelay_dir
     _argrelay_dir = argrelay_dir
 
+
 def get_argrelay_dir():
     return _argrelay_dir
 
+
 # noinspection SpellCheckingInspection
 def eprint(*args, **kwargs):
     print(*args, file = sys.stderr, **kwargs)
 
 
 def ensure_value_is_enum(enum_value, enum_cls):
     """
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/mongo_data/MongoClientWrapper.py` & `argrelay-0.1.0.dev1/src/argrelay/mongo_data/MongoClientWrapper.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/mongo_data/MongoServerWrapper.py` & `argrelay-0.1.0.dev1/src/argrelay/mongo_data/MongoServerWrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 from subprocess import TimeoutExpired, Popen
 
 from argrelay.misc_helper import eprint
 from argrelay.mongo_data.MongoConfig import MongoConfig
 
 
 class MongoServerWrapper:
-    is_mongomock: bool
-    is_started: bool
-    mongo_proc: Popen
 
     def __init__(self):
-        self.is_started = False
+        self.is_mongomock: bool
+        self.is_started: bool = False
+        self.mongo_proc: Popen
 
     def start_mongo_server(self, mongo_config: MongoConfig):
 
         if mongo_config.use_mongomock_only:
             self.is_mongomock = True
             return
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/AbstractDelegator.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/AbstractDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/ErrorDelegator.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/ErrorDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/HelpDelegator.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/HelpDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/InterceptDelegator.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/InterceptDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/InvocationInput.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/InvocationInput.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 from argrelay.runtime_data.PluginEntry import PluginEntry
 
 
 # TODO: Combine InterpResult and InvocationInput - only one need to exits
 @dataclass
 class InvocationInput:
     """
     See :class:`InvocationInputSchema`
     """
 
-    all_tokens: list[str]
+    all_tokens: list[str] = field()
     """
     Copy from `ParsedContext.all_tokens` - command line args.
     """
 
-    consumed_tokens: list[int]
+    consumed_tokens: list[int] = field()
     """
     Copy from `InterpContext.consumed_tokens` -
     indexes into `all_tokens` pointing to tokens consumed during interpretation.
     """
 
-    delegator_plugin_entry: PluginEntry
+    delegator_plugin_entry: PluginEntry = field()
     """
     The `PluginEntry` taken from config on the server side to let client invoke that plugin.
 
     It is assumed that server and client code, if not of the same version, at least, compatible.
     """
 
-    data_envelopes: list[dict]
+    data_envelopes: list[dict] = field()
     """
     Envelopes copied from `InterpContext` at the end of command line interpretation on the server side.
     """
 
-    custom_plugin_data: dict
+    custom_plugin_data: dict = field()
     """
     A placeholder dict for exclusive use by plugin.
 
     Whatever plugin server side needs to tell its plugin peer on the client side.
     """
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_delegator/NoopDelegator.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_delegator/NoopDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_interp/AbstractInterp.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_interp/AbstractInterp.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,29 +7,23 @@
 class AbstractInterp:
     """
     Interpret command line sharing current state via :class:`InterpContext`.
 
     New instance of interpreter is created by (plugin implementing) `AbstractInterpFactory` for each request.
     """
 
-    interp_factory_id: str
-
-    config_dict: dict
-
-    interp_ctx: InterpContext
-
     def __init__(
         self,
         interp_factory_id: str,
         config_dict: dict,
         interp_ctx: InterpContext,
     ):
-        self.interp_factory_id = interp_factory_id
-        self.config_dict = config_dict
-        self.interp_ctx = interp_ctx
+        self.interp_factory_id: str = interp_factory_id
+        self.config_dict: dict = config_dict
+        self.interp_ctx: InterpContext = interp_ctx
         self.base_envelope_ipos: int = interp_ctx.curr_container_ipos
 
     def __repr__(self) -> str:
         return f"fid: {self.interp_factory_id}, {super().__repr__()}"
 
     def consume_key_args(self) -> None:
         pass
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_interp/FirstArgInterp.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_interp/FirstArgInterp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-from argrelay.enum_desc.InterpStep import InterpStep
-from argrelay.plugin_interp.AbstractInterp import AbstractInterp
-from argrelay.plugin_interp.FirstArgInterpFactoryConfigSchema import first_arg_vals_to_next_interp_factory_ids_
 from argrelay.plugin_interp.TreePathInterp import TreePathInterp
-from argrelay.plugin_interp.TreePathInterpFactoryConfigSchema import interp_selector_tree_, \
-    tree_path_interp_factory_config_desc
 from argrelay.runtime_context.InterpContext import InterpContext
 
 
 class FirstArgInterp(TreePathInterp):
     """
     Dispatch command line interpretation to the next interpreter based on the command_id.
 
     `FirstArgInterp` was re-implemented in terms of `TreePathInterp` (FS_01_89_09_24).
 
     Implements FS_42_76_93_51.
     """
 
-    command_name: str
-
     def __init__(
         self,
         interp_factory_id: str,
         config_dict: dict,
         interp_ctx: InterpContext,
     ):
         super().__init__(
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_interp/FirstArgInterpFactory.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_interp/FirstArgInterpFactory.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -27,25 +27,25 @@
         converted_config = convert_FirstArgInterpConfig_to_TreePathInterpFactoryConfig(config_dict)
         tree_path_interp_factory_config_desc.validate_dict(converted_config)
         super().__init__(
             plugin_instance_id,
             converted_config,
         )
 
-
     def create_interp(
         self,
         interp_ctx: InterpContext,
     ) -> FirstArgInterp:
         return FirstArgInterp(
             self.plugin_instance_id,
             self.config_dict,
             interp_ctx,
         )
 
+
 def convert_FirstArgInterpConfig_to_TreePathInterpFactoryConfig(config_dict: dict) -> dict:
     """
     `FirstArgInterp` was re-implemented in terms of `TreePathInterp` (FS_01_89_09_24).
     """
     interp_selector_tree = {}
     for command_id, plugin_instance_id in config_dict[first_arg_vals_to_next_interp_factory_ids_].items():
         interp_selector_tree[command_id] = plugin_instance_id
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_interp/FuncArgsInterp.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_interp/FuncArgsInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_interp/FuncArgsInterpFactory.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_interp/FuncArgsInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_interp/NoopInterp.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_interp/NoopInterp.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,24 +8,22 @@
     Interpreter which does nothing
 
     Actually, it:
     *   stops processing of the command line on itself (as `next_interp` returns `None` by default)
     *   sets `arbitrary_comment` based on config
     """
 
-    arbitrary_comment: str
-
     def __init__(
         self,
         interp_factory_id,
         config_dict: dict,
         interp_ctx: InterpContext,
     ):
         super().__init__(
             interp_factory_id,
             config_dict,
             interp_ctx,
         )
-        self.arbitrary_comment = config_dict["arbitrary_comment"]
+        self.arbitrary_comment: str = config_dict["arbitrary_comment"]
 
     def try_iterate(self) -> InterpStep:
         return InterpStep.NextInterp
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_interp/NoopInterpFactory.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_interp/NoopInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_interp/TreePathInterp.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_interp/TreePathInterp.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,36 +27,32 @@
 
 
 class TreePathInterp(AbstractInterp):
     """
     Implements FS_01_89_09_24.
     """
 
-    interp_selector_tree: dict
-
-    interp_factory_id: str
-
-    # Token with ipos = 0 is the command name eaten by `FirstArgInterp`.
-    base_token_ipos: int = 1
-
     def __init__(
         self,
         interp_factory_id: str,
         config_dict: dict,
         interp_ctx: InterpContext,
     ):
         super().__init__(
             interp_factory_id,
             config_dict,
             interp_ctx,
         )
-        self.interp_selector_tree = config_dict[interp_selector_tree_]
-        self.interp_factory_id = interp_factory_id
+        self.interp_selector_tree: dict = config_dict[interp_selector_tree_]
+        self.interp_factory_id: str = interp_factory_id
         self.node_path = []
 
+        # Token with ipos = 0 is the command name eaten by `FirstArgInterp`:
+        self.base_token_ipos: int = 1
+
     def consume_pos_args(self) -> None:
         """
         Consumes heading args in `unconsumed_tokens` according to the `interp_selector_tree`.
         """
 
         self.node_path = []
         curr_sub_tree = self.interp_selector_tree
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_interp/TreePathInterpFactory.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_interp/TreePathInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_interp/TreePathInterpFactoryConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_interp/TreePathInterpFactoryConfigSchema.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     @validates_schema
     def validate_known(self, input_dict, **kwargs):
         interp_selector_tree = input_dict[interp_selector_tree_]
         if not isinstance(interp_selector_tree, dict):
             raise ValidationError(f"not a dict: {interp_selector_tree}")
         validate_tree_node(interp_selector_tree)
 
+
 tree_path_interp_factory_config_example = {
     interp_selector_tree_: {
         # TODO: This may not be currently configured plugin id:
         "intercept": f"{DemoInterpFactory.__name__}.intercept_func",
         default_leaf_: DemoInterpFactory.__name__,
     },
 }
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_loader/HelpLoader.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_loader/HelpLoader.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/plugin_loader/InterceptLoader.py` & `argrelay-0.1.0.dev1/src/argrelay/plugin_loader/InterceptLoader.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_client/AbstractClient.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_client/AbstractClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 
 
 class AbstractClient:
     """
     An abstract `relay_client` to `relay_server`
     """
 
-    client_config: ClientConfig
-    command_factory: AbstractClientCommandFactory
-
-    def __init__(self, client_config: ClientConfig, command_factory: AbstractClientCommandFactory):
-        self.client_config = client_config
-        self.command_factory = command_factory
+    def __init__(
+        self,
+        client_config: ClientConfig,
+        command_factory: AbstractClientCommandFactory
+    ):
+        self.client_config: ClientConfig = client_config
+        self.command_factory: AbstractClientCommandFactory = command_factory
 
     # noinspection PyMethodMayBeStatic
     def make_request(self, input_ctx: InputContext) -> AbstractClientCommand:
         input_ctx.print_debug()
         command_obj = self.command_factory.create_command(input_ctx)
         command_obj.execute_command(input_ctx)
         ElapsedTime.measure("after_execute_command")
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_client/AbstractClientCommandFactory.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_client/AbstractClientCommandFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_client/LocalClient.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_client/LocalClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_client/LocalClientCommandFactory.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_client/LocalClientCommandFactory.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,24 +8,22 @@
     DESCRIBE_LINE_ARGS_PATH,
     RELAY_LINE_ARGS_PATH,
     PROPOSE_ARG_VALUES_PATH,
 )
 
 
 class LocalClientCommandFactory(AbstractClientCommandFactory):
-    server_config: ServerConfig
-    local_server: LocalServer
 
     def __init__(self):
         self._start_local_server()
 
     def _start_local_server(self):
-        self.server_config = server_config_desc.from_default_file()
+        self.server_config: ServerConfig = server_config_desc.from_default_file()
         ElapsedTime.measure("after_server_config_load")
-        self.local_server = LocalServer(self.server_config)
+        self.local_server: LocalServer = LocalServer(self.server_config)
         self.local_server.start_local_server()
         ElapsedTime.measure("after_local_server_start")
 
     def create_command_by_server_path(self, server_path: str) -> AbstractLocalClientCommand:
         if server_path == DESCRIBE_LINE_ARGS_PATH:
             from argrelay.client_command_local.DescribeLineArgsLocalClientCommand import (
                 DescribeLineArgsLocalClientCommand
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_client/RemoteClient.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_client/RemoteClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_client/RemoteClientCommandFactory.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_client/RemoteClientCommandFactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,20 @@
     DESCRIBE_LINE_ARGS_PATH,
     RELAY_LINE_ARGS_PATH,
     PROPOSE_ARG_VALUES_PATH,
 )
 
 
 class RemoteClientCommandFactory(AbstractClientCommandFactory):
-    client_config: ClientConfig
 
     def __init__(
         self,
         client_config: ClientConfig,
     ):
-        self.client_config = client_config
+        self.client_config: ClientConfig = client_config
 
     # noinspection PyMethodMayBeStatic
     def create_command_by_server_path(self, server_path: str) -> "AbstractRemoteClientCommand":
         if server_path == DESCRIBE_LINE_ARGS_PATH:
             from argrelay.client_command_remote.DescribeLineArgsRemoteClientCommand import (
                 DescribeLineArgsRemoteClientCommand,
             )
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_client/__main__.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_client/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from argrelay.misc_helper.ElapsedTime import ElapsedTime
 
 ElapsedTime.measure("after_program_entry")
 
 
 def main():
     # Initial imports - see `completion_perf_notes.md`.
-    import os
     import sys
     from argrelay.runtime_context.InputContext import InputContext
     ElapsedTime.measure("after_initial_imports")
 
     file_path = get_config_path("argrelay.client.json")
     client_config = load_client_config(file_path)
     ElapsedTime.measure("after_loading_client_config")
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_server/CustomFlaskApp.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_server/CustomFlaskApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 import logging
-import os
 
 import pkg_resources
+from flasgger import Swagger
+from flask import Flask, request, redirect
+
 from argrelay import relay_server
 from argrelay.relay_server.LocalServer import LocalServer
 from argrelay.relay_server.route_api import create_blueprint_api
 from argrelay.relay_server.route_gui import create_blueprint_gui
 from argrelay.schema_config_core_server.ServerConfigSchema import server_config_desc
 from argrelay.server_spec.const_int import API_SPEC_PATH, API_DOCS_PATH, ARGRELAY_GUI_PATH
-from flasgger import Swagger
-from flask import Flask, request, redirect
 
 # Set this here (because `require` function may fail in other contexts):
 server_version = pkg_resources.require("argrelay")[0].version
 server_title = relay_server.__name__
 
 
 class CustomFlaskApp(Flask):
     """
     This is an API-wrapper exposing `LocalServer` over the network.
     """
 
-    local_server: LocalServer
-
     def __init__(
         self,
         import_name: str,
         static_url_path = "/gui_static",
         static_folder = pkg_resources.resource_filename(relay_server.__name__, "gui_static"),
         template_folder = pkg_resources.resource_filename(relay_server.__name__, "gui_templates"),
     ):
         super().__init__(
             import_name = import_name,
             static_folder = static_folder,
             template_folder = template_folder,
             static_url_path = static_url_path,
         )
-        self.local_server = LocalServer(server_config_desc.from_default_file())
+        self.local_server: LocalServer = LocalServer(server_config_desc.from_default_file())
 
     def run_with_config(self):
         # Use custom logging at DEBUG level - see: `log_request` and `log_response:
         self.logger.setLevel(logging.DEBUG)
         # Log only at ERROR level by default logger:
         # https://stackoverflow.com/a/18379764/441652
         logging.getLogger("werkzeug").setLevel(logging.ERROR)
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_server/HelpHintCache.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_server/HelpHintCache.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     Implements FS_94_30_49_28 help hint.
     """
 
     def __init__(
         self,
         query_engine: QueryEngine,
     ):
-        self.query_engine = query_engine
-        self.help_hint_dict = {}
+        self.query_engine: QueryEngine = query_engine
+        self.help_hint_dict: dict = {}
 
     def populate_cache(self):
 
         help_hint_envelopes = self.query_engine.query_data_envelopes({
             f"{ReservedArgType.EnvelopeClass.name}": f"{ReservedEnvelopeClass.ClassHelp.name}",
         })
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_server/LocalServer.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_server/LocalServer.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,26 @@
 class LocalServer:
     """
     This is plain server functionality without API-wrapper to expose over the network (hence, local).
 
     The API-wrapper exposing `LocalServer` over the network is `CustomFlaskApp`.
     """
 
-    server_config: ServerConfig
-    mongo_server: MongoServerWrapper
-    mongo_client: MongoClient
-    query_engine: QueryEngine
-    help_hint_cache: HelpHintCache
-
-    def __init__(self, server_config: ServerConfig):
-        self.server_config = server_config
-        self.mongo_server = MongoServerWrapper()
-        self.mongo_client = MongoClientWrapper.get_mongo_client(self.server_config.mongo_config)
-        self.query_engine = QueryEngine(
+    def __init__(
+        self,
+        server_config: ServerConfig,
+    ):
+        self.server_config: ServerConfig = server_config
+        self.mongo_server: MongoServerWrapper = MongoServerWrapper()
+        self.mongo_client: MongoClient = MongoClientWrapper.get_mongo_client(self.server_config.mongo_config)
+        self.query_engine: QueryEngine = QueryEngine(
             self.server_config.query_cache_config,
             self.get_mongo_database(),
         )
-        self.help_hint_cache = HelpHintCache(
+        self.help_hint_cache: HelpHintCache = HelpHintCache(
             self.query_engine,
         )
 
     def start_local_server(self):
         self._activate_plugins()
         self._start_mongo_server()
         self._load_mongo_data()
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_server/QueryEngine.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_server/QueryEngine.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,34 +13,27 @@
 from argrelay.relay_server.QueryResult import QueryResult
 from argrelay.runtime_context.SearchControl import SearchControl
 from argrelay.runtime_data.AssignedValue import AssignedValue
 from argrelay.schema_config_core_server.StaticDataSchema import data_envelopes_
 
 
 class QueryEngine:
-    mongo_db: Database
-
-    mongo_col: Collection
-
-    query_cache: TTLCache
-
-    enable_query_cache: bool
 
     def __init__(
         self,
         query_cache_config: QueryCacheConfig,
         mongo_db: Database,
     ):
-        self.mongo_db = mongo_db
-        self.mongo_col = self.mongo_db[data_envelopes_]
-        self.query_cache = TTLCache(
+        self.mongo_db: Database = mongo_db
+        self.mongo_col: Collection = self.mongo_db[data_envelopes_]
+        self.query_cache: TTLCache = TTLCache(
             maxsize = query_cache_config.query_cache_max_size_bytes,
             ttl = query_cache_config.query_cache_ttl_sec,
         )
-        self.enable_query_cache = query_cache_config.enable_query_cache
+        self.enable_query_cache: bool = query_cache_config.enable_query_cache
 
     def query_data_envelopes(
         self,
         query_dict: dict,
     ) -> list[dict]:
         """
         This query is used for final invocation for vararg-like multiple `data_envelope`-s (FS_18_64_57_18).
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_server/QueryResult.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_server/QueryResult.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 
 @dataclass
 class QueryResult:
     """
     Results of a query via `QueryEngine.query_prop_values`.
     """
 
-    data_envelope: dict
+    data_envelope: dict = field()
     """
     Last `data_envelope` in search results
 
     Normally, it is only useful when `found_count` = 1
     """
 
-    found_count: int
+    found_count: int = field()
     """
     Total number of `data_envelope`-s found.
     """
 
-    remaining_types_to_values: dict[str, list[str]]
+    remaining_types_to_values: dict[str, list[str]] = field()
     """
     See `EnvelopeContainer.remaining_types_to_values`.
     """
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_server/gui_static/argrelay_client.js` & `argrelay-0.1.0.dev1/src/argrelay/relay_server/gui_static/argrelay_client.js`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_server/gui_static/argrelay_style.css` & `argrelay-0.1.0.dev1/src/argrelay/relay_server/gui_static/argrelay_style.css`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_server/gui_templates/argrelay_main.html` & `argrelay-0.1.0.dev1/src/argrelay/relay_server/gui_templates/argrelay_main.html`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_server/route_api.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_server/route_api.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/relay_server/route_gui.py` & `argrelay-0.1.0.dev1/src/argrelay/relay_server/route_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from flask import Blueprint
+from flask import render_template
+
 from argrelay.relay_server.GuiBannerConfig import GuiBannerConfig
 from argrelay.server_spec.const_int import (
     ARGRELAY_GUI_PATH,
     API_SPEC_PATH,
     API_DOCS_PATH,
 )
-from flask import Blueprint
-from flask import render_template
 
 
 def create_blueprint_gui(
     argrelay_version: str,
     gui_banner_config: GuiBannerConfig,
 ):
     blueprint_gui = Blueprint(
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/runtime_context/EnvelopeContainer.py` & `argrelay-0.1.0.dev1/src/argrelay/runtime_context/EnvelopeContainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
 
     search_control: SearchControl = field(default_factory = lambda: SearchControl())
     """
     A specs how to query `data_envelope` for this `EnvelopeContainer`.
     """
 
-    data_envelope: dict = field(default_factory = lambda: None)
+    data_envelope: dict = field(default = None)
     """
     If the last query finds (unique) single result,
     it contains `data_envelope` based on `search_control` and command line input.
     """
 
     found_count: int = field(default = 0)
     """
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/runtime_context/InputContext.py` & `argrelay-0.1.0.dev1/src/argrelay/runtime_context/InputContext.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 import os
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 from argrelay.enum_desc.CompType import CompType
 from argrelay.enum_desc.RunMode import RunMode
 from argrelay.enum_desc.TermColor import TermColor
 from argrelay.misc_helper import eprint
 from argrelay.runtime_context.RequestContext import RequestContext
 
 
 @dataclass(frozen = True)
 class InputContext(RequestContext):
     """
     Immutable input data
     """
 
-    comp_key: str
-    run_mode: RunMode
+    comp_key: str = field()
+    run_mode: RunMode = field()
 
     @classmethod
     def from_request_context(
         cls,
         request_ctx: RequestContext,
         run_mode: RunMode,
         comp_key: str,
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/runtime_context/InterpContext.py` & `argrelay-0.1.0.dev1/src/argrelay/runtime_context/InterpContext.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 @dataclass
 class InterpContext:
     """
     Mutable state for the process of command line interpretation.
     """
 
-    parsed_ctx: ParsedContext
+    parsed_ctx: ParsedContext = field()
 
     # TODO: Move all dynamic and non-serializable objects into `InterpRuntime` (or something like that).
-    interp_factories: dict[str, "AbstractInterpFactory"]
+    interp_factories: dict[str, "AbstractInterpFactory"] = field()
     """
     Reference to `ServerConfig.action_delegators`.
     """
 
-    action_delegators: dict[str, "AbstractDelegator"]
+    action_delegators: dict[str, "AbstractDelegator"] = field()
     """
     Reference to `ServerConfig.action_delegators`.
     """
 
-    query_engine: QueryEngine
+    query_engine: QueryEngine = field()
 
-    help_hint_cache: HelpHintCache
+    help_hint_cache: HelpHintCache = field()
 
     unconsumed_tokens: list[int] = field(init = False)
     """
     Remaining tokens (their ipos) which are still unconsumed (in ascending order).
     """
 
     consumed_tokens: list[int] = field(init = False, default_factory = lambda: [])
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/runtime_context/ParsedContext.py` & `argrelay-0.1.0.dev1/src/argrelay/runtime_context/ParsedContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/runtime_context/SearchControl.py` & `argrelay-0.1.0.dev1/src/argrelay/runtime_context/SearchControl.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/runtime_data/ServerConfig.py` & `argrelay-0.1.0.dev1/src/argrelay/runtime_data/ServerConfig.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 from argrelay.runtime_data.ConnectionConfig import ConnectionConfig
 from argrelay.runtime_data.PluginEntry import PluginEntry
 from argrelay.runtime_data.StaticData import StaticData
 
 
 @dataclass
 class ServerConfig:
-    connection_config: ConnectionConfig
-    mongo_config: MongoConfig
-    query_cache_config: QueryCacheConfig
-    gui_banner_config: GuiBannerConfig
+    connection_config: ConnectionConfig = field()
+    mongo_config: MongoConfig = field()
+    query_cache_config: QueryCacheConfig = field()
+    gui_banner_config: GuiBannerConfig = field()
 
-    plugin_instance_id_load_list: list[str]
+    plugin_instance_id_load_list: list[str] = field()
     """
     List of `plugin_instance_id`s in order of loading. Each `plugin_instance_id` is a key into `plugin_dict`.
     """
 
-    plugin_dict: dict[str, PluginEntry]
+    plugin_dict: dict[str, PluginEntry] = field()
     """
     Key = `plugin_instance_id`
     """
 
-    static_data: StaticData
+    static_data: StaticData = field()
 
     # TODO: Keep this runtime objects in separate (`ServerRuntime`?) class. Ensure/implement ServerConfig dumping on request (for troubleshooting).
     data_loaders: dict[str, "AbstractLoader"] = field(default_factory = lambda: {})
     """
     Entries in `data_loaders` are not directly loaded from config.
     These are plugin instances created during plugin activation.
     """
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/runtime_data/StaticData.py` & `argrelay-0.1.0.dev1/src/argrelay/runtime_data/StaticData.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/sample_conf/argrelay.server.yaml` & `argrelay-0.1.0.dev1/src/argrelay/sample_conf/argrelay.server.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,19 @@
 
     GitRepoLoader:
         plugin_module_name: argrelay.custom_integ.GitRepoLoader
         plugin_class_name: GitRepoLoader
         plugin_type: LoaderPlugin
         plugin_config:
             is_plugin_enabled: False
-            base_path: "~/repos"
+            load_repo_commits: False
+            base_paths:
+                -   base_path: "~/repos"
+                    repo_aliases:
+                        argrelay.git: ar
 
     NoopDelegator:
         plugin_module_name: argrelay.plugin_delegator.NoopDelegator
         plugin_class_name: NoopDelegator
         plugin_type: DelegatorPlugin
         plugin_config: { }
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_core_client/ClientConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_core_client/ClientConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from argrelay.misc_helper.TypeDesc import TypeDesc
 from argrelay.relay_server.GuiBannerConfig import GuiBannerConfig
 
 header_html_ = "header_html"
 footer_html_ = "footer_html"
 
+
 class GuiBannerConfigSchema(Schema):
     class Meta:
         unknown = RAISE
         strict = True
 
     header_html = fields.String()
     footer_html = fields.String()
@@ -17,14 +18,15 @@
     @post_load
     def make_object(self, input_dict, **kwargs):
         return GuiBannerConfig(
             header_html = input_dict[header_html_],
             footer_html = input_dict[footer_html_],
         )
 
+
 gui_banner_config_desc = TypeDesc(
     dict_schema = GuiBannerConfigSchema(),
     ref_name = GuiBannerConfigSchema.__name__,
     dict_example = {
         header_html_: "",
         footer_html_: "",
     },
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/MongoConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/MongoConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/ServerConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/ServerConfigSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 from marshmallow import Schema, fields, RAISE, post_load, validates_schema, ValidationError
 
 from argrelay.misc_helper import get_config_path
 from argrelay.misc_helper.TypeDesc import TypeDesc
 from argrelay.runtime_data.ServerConfig import ServerConfig
 from argrelay.schema_config_core_client.ConnectionConfigSchema import connection_config_desc
 from argrelay.schema_config_core_server.GuiBannerConfigSchema import gui_banner_config_desc
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_core_server/StaticDataSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_core_server/StaticDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/DataEnvelopeSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/DataEnvelopeSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/FuncArgsInterpConfigSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/FuncArgsInterpConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/InitControlSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/InitControlSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_interp/SearchControlSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_interp/SearchControlSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_config_plugin/PluginEntrySchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_config_plugin/PluginEntrySchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_request/RequestContextSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_request/RequestContextSchema.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         },
     )
     comp_type = fields.Enum(
         CompType,
         required = True,
         metadata = {
             "description": (
-                "Name for a completion type - see " + CompType.__name__ + " enum "
+                "Name for a completion type - see " + CompType.__name__ + " enum " +
                 "(which maps into ASCII char sent by Bash to completion callback to indicate completion type)"
             ),
             "example": _request_context_example[comp_type_],
         },
     )
     is_debug_enabled = fields.Boolean(
         required = True,
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_response/ArgValuesSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_response/ArgValuesSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_response/AssignedValueSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_response/AssignedValueSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_response/EnvelopeContainerSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_response/EnvelopeContainerSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_response/FilteredDict.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_response/FilteredDict.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_response/InterpResultSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_response/InterpResultSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/schema_response/InvocationInputSchema.py` & `argrelay-0.1.0.dev1/src/argrelay/schema_response/InvocationInputSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/server_spec/DescribeLineArgsSpec.py` & `argrelay-0.1.0.dev1/src/argrelay/server_spec/DescribeLineArgsSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/server_spec/ProposeArgValuesSpec.py` & `argrelay-0.1.0.dev1/src/argrelay/server_spec/ProposeArgValuesSpec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from argrelay.schema_request.RequestContextSchema import request_context_desc
 from argrelay.schema_response.ArgValuesSchema import arg_values_desc, arg_values_
-from argrelay.server_spec.server_data_schema import server_op_data_schemas, get_schema_definitions
+from argrelay.server_spec.server_data_schema import get_schema_definitions
 
 spec_data = {
     "summary": "Propose arg values for the given command line and cursor position",
     "consumes": [
         "application/json",
     ],
     "produces": [
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/server_spec/RelayLineArgsSpec.py` & `argrelay-0.1.0.dev1/src/argrelay/server_spec/RelayLineArgsSpec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from argrelay.schema_config_plugin.PluginEntrySchema import plugin_entry_desc
 from argrelay.schema_request.RequestContextSchema import request_context_desc
 from argrelay.schema_response.InvocationInputSchema import invocation_input_desc
-from argrelay.server_spec.server_data_schema import server_op_data_schemas, get_schema_definitions
+from argrelay.server_spec.server_data_schema import get_schema_definitions
 
 spec_data = {
     "summary": "Provide input data to delegate execution of command on client side",
     "consumes": [
         "application/json",
     ],
     "produces": [
@@ -34,8 +34,7 @@
     },
     "definitions": get_schema_definitions([
         request_context_desc.ref_name,
         invocation_input_desc.ref_name,
         plugin_entry_desc.ref_name,
     ]),
 }
-
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/server_spec/const_int.py` & `argrelay-0.1.0.dev1/src/argrelay/server_spec/const_int.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,7 @@
 DEFAULT_IP_ADDRESS = "localhost"
 DEFAULT_PORT_NUMBER = 8787
 
 API_SPEC_PATH = "/argrelay_server_api_spec.json"
 
 # noinspection HttpUrlsUsage
 BASE_URL_FORMAT = "http://{server_host_name}:{server_port_number}"
-
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/server_spec/server_data_schema.py` & `argrelay-0.1.0.dev1/src/argrelay/server_spec/server_data_schema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/test_helper/EnvMockBuilder.py` & `argrelay-0.1.0.dev1/src/argrelay/test_helper/EnvMockBuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import io
 import json
 import os
 import re
 import sys
 from contextlib import ExitStack
 from dataclasses import dataclass, field
+from io import StringIO
 from unittest import mock
 
 import mongomock
 import pkg_resources
 import yaml
 
 import argrelay
@@ -79,59 +80,59 @@
 
     *   Verifying plugin `InvocationInput` - see usage of: `delegator_plugin_invoke_action_func_path`
 
     *   ...
 
     """
 
-    run_mode: RunMode = RunMode.CompletionMode
+    run_mode: RunMode = field(default = RunMode.CompletionMode)
 
-    command_line: str = ""
-    _command_line_is_set: bool = False
+    command_line: str = field(default = "")
+    _command_line_is_set: bool = field(default = False)
 
     command_args: list[str] = field(default_factory = lambda: [])
-    _command_args_are_set: bool = False
+    _command_args_are_set: bool = field(default = False)
 
-    cursor_cpos: int = -1
-    _cursor_cpos_is_set: bool = False
+    cursor_cpos: int = field(default = -1)
+    _cursor_cpos_is_set: bool = field(default = False)
 
-    comp_type: CompType = CompType.PrefixShown
-    comp_key: int = 0
+    comp_type: CompType = field(default = CompType.PrefixShown)
+    comp_key: int = field(default = 0)
 
-    _mock_client_input: bool = True
+    _mock_client_input: bool = field(default = True)
 
-    file_mock: OpenFileMock = OpenFileMock({})
+    file_mock: OpenFileMock = field(default = OpenFileMock({}))
 
     client_config_dict: dict = field(default_factory = lambda: load_custom_integ_client_config_dict())
-    mock_client_config_file_read: bool = True
-    is_client_config_with_local_server: bool = True
+    mock_client_config_file_read: bool = field(default = True)
+    is_client_config_with_local_server: bool = field(default = True)
 
     server_config_dict: dict = field(default_factory = lambda: load_custom_integ_server_config_dict())
-    mock_server_config_file_read: bool = True
-    is_server_config_with_mongo_start: bool = False
-    enable_demo_git_loader: bool = False
+    mock_server_config_file_read: bool = field(default = True)
+    is_server_config_with_mongo_start: bool = field(default = False)
+    enable_demo_git_loader: bool = field(default = False)
 
-    actual_stdout = None
-    capture_stdout: bool = False
+    actual_stdout: StringIO = field(default = None)
+    capture_stdout: bool = field(default = False)
 
-    actual_stderr = None
-    capture_stderr: bool = False
+    actual_stderr: StringIO = field(default = None)
+    capture_stderr: bool = field(default = False)
 
-    mock_mongo_client: bool = True
+    mock_mongo_client: bool = field(default = True)
 
-    assert_on_close: bool = True
+    assert_on_close: bool = field(default = True)
 
-    test_data_ids_to_load = [
+    test_data_ids_to_load: list[str] = field(default_factory = lambda: [
         "TD_70_69_38_46",  # no data
-    ]
+    ])
 
-    delegator_plugin_invoke_action_func_path = None
-    invocation_input: InvocationInput = None
+    delegator_plugin_invoke_action_func_path: str = field(default = None)
+    invocation_input: InvocationInput = field(default = None)
 
-    enable_query_cache: bool = True
+    enable_query_cache: bool = field(default = True)
 
     def set_run_mode(self, run_mode: RunMode):
         self.run_mode = run_mode
         return self
 
     def set_command_line(self, command_line: str):
         """
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/test_helper/InOutTestCase.py` & `argrelay-0.1.0.dev1/src/argrelay/test_helper/InOutTestCase.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay/test_helper/OpenFileMock.py` & `argrelay-0.1.0.dev1/src/argrelay/test_helper/OpenFileMock.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 
 class OpenFileMock:
     """
     Mock file data for specific paths:
     https://stackoverflow.com/a/69681105/441652
     """
     builtin_open = open
-    path_to_data: dict[str, str]
-    path_to_mock: dict
 
     def __init__(self, path_to_data: dict[str, str]):
-        self.path_to_data = path_to_data
-        self.path_to_mock = {}
+        self.path_to_data: dict[str, str] = path_to_data
+        self.path_to_mock: dict = {}
 
     def open(self, *args, **kwargs):
         file_path = args[0]
         if file_path in self.path_to_data:
             self.path_to_mock[file_path] = mock.mock_open(read_data = self.path_to_data[file_path])
             return self.path_to_mock[file_path](*args, **kwargs)
         return self.builtin_open(*args, **kwargs)
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay/test_helper/__init__.py` & `argrelay-0.1.0.dev1/src/argrelay/test_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.0.1.dev1/src/argrelay.egg-info/PKG-INFO` & `argrelay-0.1.0.dev1/src/argrelay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.0.1.dev1
+Version: 0.1.0.dev1
 Summary: Tab-completion & data search server - total recall
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Environment :: Console
```

### Comparing `argrelay-0.0.1.dev1/src/argrelay.egg-info/SOURCES.txt` & `argrelay-0.1.0.dev1/src/argrelay.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 ./src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
 ./src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
 ./src/argrelay/client_command_remote/__init__.py
 ./src/argrelay/custom_integ/DemoInterp.py
 ./src/argrelay/custom_integ/DemoInterpFactory.py
 ./src/argrelay/custom_integ/DemoInterpFactoryConfigSchema.py
 ./src/argrelay/custom_integ/GitRepoArgType.py
+./src/argrelay/custom_integ/GitRepoBasePathConfigSchema.py
 ./src/argrelay/custom_integ/GitRepoDelegator.py
 ./src/argrelay/custom_integ/GitRepoEnvelopeClass.py
 ./src/argrelay/custom_integ/GitRepoLoader.py
 ./src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
 ./src/argrelay/custom_integ/ServiceArgType.py
 ./src/argrelay/custom_integ/ServiceDelegator.py
 ./src/argrelay/custom_integ/ServiceEnvelopeClass.py
@@ -190,15 +191,14 @@
 ./src/argrelay/runtime_context/InitControl.py
 ./src/argrelay/runtime_context/InputContext.py
 ./src/argrelay/runtime_context/InterpContext.py
 ./src/argrelay/runtime_context/ParsedContext.py
 ./src/argrelay/runtime_context/RequestContext.py
 ./src/argrelay/runtime_context/SearchControl.py
 ./src/argrelay/runtime_context/__init__.py
-./src/argrelay/runtime_data/ArgType.py
 ./src/argrelay/runtime_data/AssignedValue.py
 ./src/argrelay/runtime_data/ClientConfig.py
 ./src/argrelay/runtime_data/ConnectionConfig.py
 ./src/argrelay/runtime_data/PluginEntry.py
 ./src/argrelay/runtime_data/ServerConfig.py
 ./src/argrelay/runtime_data/StaticData.py
 ./src/argrelay/runtime_data/__init__.py
@@ -482,15 +482,14 @@
 src/argrelay/runtime_context/InitControl.py
 src/argrelay/runtime_context/InputContext.py
 src/argrelay/runtime_context/InterpContext.py
 src/argrelay/runtime_context/ParsedContext.py
 src/argrelay/runtime_context/RequestContext.py
 src/argrelay/runtime_context/SearchControl.py
 src/argrelay/runtime_context/__init__.py
-src/argrelay/runtime_data/ArgType.py
 src/argrelay/runtime_data/AssignedValue.py
 src/argrelay/runtime_data/ClientConfig.py
 src/argrelay/runtime_data/ConnectionConfig.py
 src/argrelay/runtime_data/PluginEntry.py
 src/argrelay/runtime_data/ServerConfig.py
 src/argrelay/runtime_data/StaticData.py
 src/argrelay/runtime_data/__init__.py
```

