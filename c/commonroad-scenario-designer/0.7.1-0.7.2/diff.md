# Comparing `tmp/commonroad_scenario_designer-0.7.1.tar.gz` & `tmp/commonroad_scenario_designer-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonroad_scenario_designer-0.7.1.tar", max compression
+gzip compressed data, was "commonroad_scenario_designer-0.7.2.tar", max compression
```

## Comparing `commonroad_scenario_designer-0.7.1.tar` & `commonroad_scenario_designer-0.7.2.tar`

### file list

```diff
@@ -1,234 +1,234 @@
--rw-r--r--   0        0        0    35148 2023-04-26 01:03:30.014174 commonroad_scenario_designer-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0    11418 2023-06-21 05:40:36.506124 commonroad_scenario_designer-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.462115 commonroad_scenario_designer-0.7.1/crdesigner/__init__.py
--rw-r--r--   0        0        0     8245 2023-06-19 10:49:53.585780 commonroad_scenario_designer-0.7.1/crdesigner/config/config.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/configurations/__init__.py
--rw-r--r--   0        0        0      382 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/configurations/custom_settings.yaml
--rw-r--r--   0        0        0     2566 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/configurations/custom_settings_osm2cr.yaml
--rw-r--r--   0        0        0      382 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/configurations/default_settings.yaml
--rw-r--r--   0        0        0     2564 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/configurations/default_settings_osm2cr.yaml
--rw-r--r--   0        0        0       47 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/configurations/definition.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/__init__.py
--rw-r--r--   0        0        0    17976 2023-06-14 05:25:23.786499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/conversion_lanelet.py
--rw-r--r--   0        0        0    71077 2023-06-14 05:25:23.786499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/conversion_lanelet_network.py
--rw-r--r--   0        0        0    28332 2023-06-14 05:25:23.786499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/geometry.py
--rw-r--r--   0        0        0     1470 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/utils.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/__init__.py
--rw-r--r--   0        0        0    31052 2023-06-19 10:49:53.585780 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/cr2lanelet.py
--rw-r--r--   0        0        0    12890 2023-06-20 13:58:00.286809 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2.py
--rw-r--r--   0        0        0     4645 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2_parser.py
--rw-r--r--   0        0        0    47862 2023-06-19 11:30:56.919488 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2cr.py
--rw-r--r--   0        0        0     6758 2023-06-20 09:11:13.860075 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/map_conversion_interface.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/__init__.py
--rw-r--r--   0        0        0    10196 2023-06-14 05:25:23.786499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/converter.py
--rw-r--r--   0        0        0    37032 2023-06-20 09:11:13.860075 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/network.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/__init__.py
--rw-r--r--   0        0        0     4821 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/border.py
--rw-r--r--   0        0        0     1982 2023-04-26 01:03:30.022174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/crosswalks.py
--rw-r--r--   0        0        0      944 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/geo_reference.py
--rw-r--r--   0        0        0    16247 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane.py
--rw-r--r--   0        0        0    23257 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane_group.py
--rw-r--r--   0        0        0    11695 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/traffic_signals.py
--rw-r--r--   0        0        0     3935 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/utils.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/__init__.py
--rw-r--r--   0        0        0     3985 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/eulerspiral.py
--rw-r--r--   0        0        0    18380 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/geometry.py
--rw-r--r--   0        0        0     5862 2023-04-26 01:03:30.022174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/junction.py
--rw-r--r--   0        0        0     4828 2023-06-20 09:11:13.860075 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/opendrive.py
--rw-r--r--   0        0        0     6096 2023-04-26 01:03:30.022174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road.py
--rw-r--r--   0        0        0      632 2023-04-26 01:03:30.022174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadElevationProfile.py
--rw-r--r--   0        0        0    21954 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLanes.py
--rw-r--r--   0        0        0     5275 2023-04-26 01:03:30.022174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLateralProfile.py
--rw-r--r--   0        0        0     7605 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLink.py
--rw-r--r--   0        0        0     8351 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadObject.py
--rw-r--r--   0        0        0    12550 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadPlanView.py
--rw-r--r--   0        0        0     8212 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadSignal.py
--rw-r--r--   0        0        0     1430 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road_record.py
--rw-r--r--   0        0        0     3922 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadtype.py
--rw-r--r--   0        0        0    28758 2023-06-20 09:20:47.449328 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/parser.py
--rw-r--r--   0        0        0       47 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/.gitignore
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/__init__.py
--rw-r--r--   0        0        0     7546 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/config.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/__init__.py
--rw-r--r--   0        0        0     5613 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/converter.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/__init__.py
--rw-r--r--   0        0        0    19464 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/cleanup.py
--rw-r--r--   0        0        0    10397 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/export.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/__init__.py
--rw-r--r--   0        0        0     4131 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/intersection_merger.py
--rw-r--r--   0        0        0    36721 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/lane_linker.py
--rw-r--r--   0        0        0     2801 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/mapillary.py
--rw-r--r--   0        0        0     4422 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/offsetter.py
--rw-r--r--   0        0        0     2161 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/restrictions.py
--rw-r--r--   0        0        0      501 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/__init__.py
--rw-r--r--   0        0        0    31611 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph.py
--rw-r--r--   0        0        0    18421 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_edge.py
--rw-r--r--   0        0        0     6470 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_functions.py
--rw-r--r--   0        0        0     9630 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_lane.py
--rw-r--r--   0        0        0     4124 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_node.py
--rw-r--r--   0        0        0     1192 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_light.py
--rw-r--r--   0        0        0     1966 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_sign.py
--rw-r--r--   0        0        0     2729 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_sublayered_graph.py
--rw-r--r--   0        0        0    14872 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/segment_clusters.py
--rw-r--r--   0        0        0    11702 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/traffic_sign_parser.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/__init__.py
--rw-r--r--   0        0        0      237 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/__init__.py
--rw-r--r--   0        0        0     6345 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_edge.py
--rw-r--r--   0        0        0    21200 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_format.py
--rw-r--r--   0        0        0      581 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_node.py
--rw-r--r--   0        0        0    12858 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intersection_enhancement.py
--rw-r--r--   0        0        0     2333 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/traffic_light_generator.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/__init__.py
--rw-r--r--   0        0        0     3482 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/downloader.py
--rw-r--r--   0        0        0     7332 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/info_deduction.py
--rw-r--r--   0        0        0    36854 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/osm_parser.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/__init__.py
--rw-r--r--   0        0        0      508 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/custom_types.py
--rw-r--r--   0        0        0     2055 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/geonamesID.py
--rw-r--r--   0        0        0     1286 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/graph_analysis.py
--rw-r--r--   0        0        0      857 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/idgenerator.py
--rw-r--r--   0        0        0     9259 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/plots.py
--rw-r--r--   0        0        0     3554 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/main.py
--rw-r--r--   0        0        0      198 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/.gitignore
--rw-r--r--   0        0        0      288 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/__init__.py
--rw-r--r--   0        0        0     8301 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/config.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/__init__.py
--rw-r--r--   0        0        0   116978 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/converter.py
--rw-r--r--   0        0        0     9601 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/mapping.py
--rw-r--r--   0        0        0     5087 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_light.py
--rw-r--r--   0        0        0     9635 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_sign.py
--rw-r--r--   0        0        0      387 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/errors.py
--rw-r--r--   0        0        0     2769 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/merge.py
--rw-r--r--   0        0        0     2050 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/sumo2cr.py
--rw-r--r--   0        0        0    62888 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/sumolib_net.py
--rw-r--r--   0        0        0     5629 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/DEU.typ.xml
--rw-r--r--   0        0        0      647 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/README.md
--rw-r--r--   0        0        0     4613 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/USA.typ.xml
--rw-r--r--   0        0        0     5629 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/ZAM.typ.xml
--rw-r--r--   0        0        0      796 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/default.sumo.cfg
--rw-r--r--   0        0        0    20378 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/util.py
--rw-r--r--   0        0        0      731 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/start_gui.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/cli/__init__.py
--rw-r--r--   0        0        0     7028 2023-06-19 11:30:56.919488 commonroad_scenario_designer-0.7.1/crdesigner/ui/cli/command_line.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/__init__.py
--rw-r--r--   0        0        0      427 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/gui.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/__init__.py
--rw-r--r--   0        0        0     4670 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/animated_viewer_wrapper.py
--rw-r--r--   0        0        0       44 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/__init__.py
--rw-r--r--   0        0        0    16825 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/animated_viewer.py
--rw-r--r--   0        0        0    44796 2023-06-19 10:49:53.585780 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/dynamic_canvas.py
--rw-r--r--   0        0        0     2154 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/helper.py
--rw-r--r--   0        0        0      346 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/__init__.py
--rw-r--r--   0        0        0     8704 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/draw_params_updater.py
--rw-r--r--   0        0        0      566 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/general_services.py
--rw-r--r--   0        0        0     1511 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/scenario_resizer.py
--rw-r--r--   0        0        0     6239 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/gui_sumo_simulation.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/__init__.py
--rw-r--r--   0        0        0      828 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/crdesigner_console_wrapper.py
--rw-r--r--   0        0        0     6882 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/mwindow.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/__init__.py
--rw-r--r--   0        0        0    11509 2023-06-19 10:49:53.585780 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/aerial_data.py
--rw-r--r--   0        0        0      690 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/config.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/__init__.py
--rw-r--r--   0        0        0      499 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/converter_interface.py
--rw-r--r--   0        0        0     3382 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/opendrive_interface.py
--rw-r--r--   0        0        0     2203 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/osm_interface.py
--rw-r--r--   0        0        0      883 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/errors.py
--rw-r--r--   0        0        0     5193 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/general_services.py
--rw-r--r--   0        0        0     1567 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.py
--rw-r--r--   0        0        0     2702 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.ui
--rw-r--r--   0        0        0     6650 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.py
--rw-r--r--   0        0        0     6134 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.ui
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/__init__.py
--rw-r--r--   0        0        0    23092 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/gui_settings_ui.py
--rw-r--r--   0        0        0    34788 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/osm_settings_ui.py
--rw-r--r--   0        0        0    10566 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog.py
--rw-r--r--   0        0        0     5960 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog_ui.py
--rw-r--r--   0        0        0     5536 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/settings_ui.py
--rw-r--r--   0        0        0      464 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/size_policies.py
--rw-r--r--   0        0        0    41909 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/sumo_settings_ui.py
--rw-r--r--   0        0        0     9993 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_settings.py
--rw-r--r--   0        0        0  1852651 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.py
--rw-r--r--   0        0        0     1136 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.qrc
--rw-r--r--   0        0        0    33556 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/Groupe_6.png
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/__init__.py
--rw-r--r--   0        0        0     8020 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_left.png
--rw-r--r--   0        0        0      645 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_right.png
--rw-r--r--   0        0        0      770 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_lane.png
--rw-r--r--   0        0        0    21597 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_redo.png
--rw-r--r--   0        0        0    21742 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_undo.png
--rw-r--r--   0        0        0    32283 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/close.png
--rw-r--r--   0        0        0    67646 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr.ico
--rw-r--r--   0        0        0    89174 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.ico
--rw-r--r--   0        0        0    26980 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.png
--rw-r--r--   0        0        0    96318 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr2.ico
--rw-r--r--   0        0        0    17853 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/drawing_mode.png
--rw-r--r--   0        0        0    68262 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.ico
--rw-r--r--   0        0        0      646 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.png
--rw-r--r--   0        0        0      207 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/iconmonstr-trash-can-darkmode.png
--rw-r--r--   0        0        0      409 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/iconmonstr-trash-can.svg
--rw-r--r--   0        0        0     1417 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/merge_lanelet.png
--rw-r--r--   0        0        0    26374 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/new_file.png
--rw-r--r--   0        0        0    12185 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.png
--rw-r--r--   0        0        0   140025 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.svg
--rw-r--r--   0        0        0    25413 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/open_file.png
--rw-r--r--   0        0        0     1438 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause.png
--rw-r--r--   0        0        0     3976 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause_darkmode.png
--rw-r--r--   0        0        0     2303 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/play.png
--rw-r--r--   0        0        0   109822 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.png
--rw-r--r--   0        0        0    90702 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.svg
--rw-r--r--   0        0        0   432254 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save.ico
--rw-r--r--   0        0        0    10339 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_file.png
--rw-r--r--   0        0        0     1673 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.png
--rw-r--r--   0        0        0     3382 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.svg
--rw-r--r--   0        0        0      734 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/split_lanelet.png
--rw-r--r--   0        0        0     4596 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/target-darkmode.png
--rw-r--r--   0        0        0     8300 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/target.png
--rw-r--r--   0        0        0    67646 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/tools.ico
--rw-r--r--   0        0        0      956 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/help_actions.py
--rw-r--r--   0        0        0    71248 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/map_creator.py
--rw-r--r--   0        0        0    29430 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/osm_settings.py
--rw-r--r--   0        0        0    29122 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/osm_settings_ui.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/__init__.py
--rw-r--r--   0        0        0     6254 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/config_default.py
--rw-r--r--   0        0        0    22397 2023-06-14 05:25:23.794499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/plots_interactive.py
--rw-r--r--   0        0        0     7409 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/waitingspinnerwidget.py
--rw-r--r--   0        0        0      115 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/settings.json
--rw-r--r--   0        0        0     3965 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/settings.py
--rw-r--r--   0        0        0     8395 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/sumo_settings.py
--rw-r--r--   0        0        0      356 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/transfer.py
--rw-r--r--   0        0        0     2064 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/util.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/__init__.py
--rw-r--r--   0        0        0      940 2023-06-14 05:25:23.794499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/create_converter_toolbox.py
--rw-r--r--   0        0        0    18391 2023-06-14 05:25:23.794499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox.py
--rw-r--r--   0        0        0     7878 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox_ui.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/__init__.py
--rw-r--r--   0        0        0      770 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/create_obstacle_toolbox.py
--rw-r--r--   0        0        0    54836 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox.py
--rw-r--r--   0        0        0    15463 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox_ui.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/__init__.py
--rw-r--r--   0        0        0      926 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/create_road_network_toolbox.py
--rw-r--r--   0        0        0   114598 2023-06-20 09:11:13.860075 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox.py
--rw-r--r--   0        0        0    79596 2023-06-20 09:11:13.860075 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox_ui.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/service_layer/__init__.py
--rw-r--r--   0        0        0      450 2023-06-14 05:25:23.794499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/service_layer/general_services.py
--rw-r--r--   0        0        0    14360 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/toolbox_ui.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/__init__.py
--rw-r--r--   0        0        0     3183 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/menu_bar_wrapper.py
--rw-r--r--   0        0        0      510 2023-04-26 01:03:30.054174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/__init__.py
--rw-r--r--   0        0        0     4665 2023-06-14 05:25:23.794499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/file_actions.py
--rw-r--r--   0        0        0      993 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/general_services.py
--rw-r--r--   0        0        0      451 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/help_actions.py
--rw-r--r--   0        0        0     1391 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/setting_actions.py
--rw-r--r--   0        0        0        0 2023-06-21 06:48:08.478115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/__init__.py
--rw-r--r--   0        0        0    12620 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/toolbar_wrapper.py
--rw-r--r--   0        0        0     1230 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/top_bar_wrapper.py
--rw-r--r--   0        0        0     2211 2023-06-21 05:40:36.510124 commonroad_scenario_designer-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    13271 1970-01-01 00:00:00.000000 commonroad_scenario_designer-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-26 01:03:31.194176 commonroad_scenario_designer-0.7.2/LICENSE.txt
+-rw-r--r--   0        0        0    11248 2023-07-29 13:25:24.554301 commonroad_scenario_designer-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.434302 commonroad_scenario_designer-0.7.2/crdesigner/__init__.py
+-rw-r--r--   0        0        0     8245 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/config/config.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.438302 commonroad_scenario_designer-0.7.2/crdesigner/configurations/__init__.py
+-rw-r--r--   0        0        0      382 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/configurations/custom_settings.yaml
+-rw-r--r--   0        0        0     2566 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/configurations/custom_settings_osm2cr.yaml
+-rw-r--r--   0        0        0      382 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/configurations/default_settings.yaml
+-rw-r--r--   0        0        0     2564 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/configurations/default_settings_osm2cr.yaml
+-rw-r--r--   0        0        0       47 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/configurations/definition.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.438302 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.438302 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/common/__init__.py
+-rw-r--r--   0        0        0    17976 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/common/conversion_lanelet.py
+-rw-r--r--   0        0        0    71122 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/common/conversion_lanelet_network.py
+-rw-r--r--   0        0        0    28332 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/common/geometry.py
+-rw-r--r--   0        0        0     1175 2023-07-27 09:37:35.669542 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/common/utils.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.438302 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/lanelet2/__init__.py
+-rw-r--r--   0        0        0    32751 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/lanelet2/cr2lanelet.py
+-rw-r--r--   0        0        0    12912 2023-07-27 12:30:19.259846 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/lanelet2/lanelet2.py
+-rw-r--r--   0        0        0     4898 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/lanelet2/lanelet2_parser.py
+-rw-r--r--   0        0        0    48239 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/lanelet2/lanelet2cr.py
+-rw-r--r--   0        0        0     6758 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/map_conversion_interface.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.438302 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.438302 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/__init__.py
+-rw-r--r--   0        0        0    10196 2023-06-14 05:25:20.326492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/converter.py
+-rw-r--r--   0        0        0    37032 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/network.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.438302 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/__init__.py
+-rw-r--r--   0        0        0     4821 2023-06-14 05:25:20.326492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/border.py
+-rw-r--r--   0        0        0     1982 2023-04-26 01:03:31.198176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/crosswalks.py
+-rw-r--r--   0        0        0      944 2023-06-14 05:25:20.326492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/geo_reference.py
+-rw-r--r--   0        0        0    16247 2023-06-14 05:25:20.326492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane.py
+-rw-r--r--   0        0        0    23257 2023-06-14 05:25:20.326492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane_group.py
+-rw-r--r--   0        0        0    11730 2023-07-27 11:04:21.204500 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/traffic_signals.py
+-rw-r--r--   0        0        0     3935 2023-06-14 05:25:20.326492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/utils.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.442303 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.442303 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/__init__.py
+-rw-r--r--   0        0        0     3985 2023-06-14 05:25:20.326492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/eulerspiral.py
+-rw-r--r--   0        0        0    18380 2023-06-14 05:25:20.326492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/geometry.py
+-rw-r--r--   0        0        0     5862 2023-04-26 01:03:31.198176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/junction.py
+-rw-r--r--   0        0        0     4828 2023-06-20 09:11:13.888075 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/opendrive.py
+-rw-r--r--   0        0        0     6096 2023-04-26 01:03:31.198176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road.py
+-rw-r--r--   0        0        0      632 2023-04-26 01:03:31.198176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadElevationProfile.py
+-rw-r--r--   0        0        0    21954 2023-06-14 05:25:20.326492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLanes.py
+-rw-r--r--   0        0        0     5275 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLateralProfile.py
+-rw-r--r--   0        0        0     7605 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLink.py
+-rw-r--r--   0        0        0     8351 2023-06-14 05:25:20.326492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadObject.py
+-rw-r--r--   0        0        0    12550 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadPlanView.py
+-rw-r--r--   0        0        0     8212 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadSignal.py
+-rw-r--r--   0        0        0     1430 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road_record.py
+-rw-r--r--   0        0        0     3922 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadtype.py
+-rw-r--r--   0        0        0    28758 2023-06-20 09:20:47.453328 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/parser.py
+-rw-r--r--   0        0        0       47 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/.gitignore
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.442303 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/__init__.py
+-rw-r--r--   0        0        0     7546 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/config.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.442303 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/__init__.py
+-rw-r--r--   0        0        0     5613 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/converter.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.442303 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/__init__.py
+-rw-r--r--   0        0        0    19790 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/cleanup.py
+-rw-r--r--   0        0        0    10397 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/export.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.442303 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/__init__.py
+-rw-r--r--   0        0        0     4131 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/intersection_merger.py
+-rw-r--r--   0        0        0    36721 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/lane_linker.py
+-rw-r--r--   0        0        0     2801 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/mapillary.py
+-rw-r--r--   0        0        0     4422 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/offsetter.py
+-rw-r--r--   0        0        0     2161 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/restrictions.py
+-rw-r--r--   0        0        0      501 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/__init__.py
+-rw-r--r--   0        0        0    31611 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph.py
+-rw-r--r--   0        0        0    18421 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_edge.py
+-rw-r--r--   0        0        0     6470 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_functions.py
+-rw-r--r--   0        0        0     9630 2023-06-14 05:25:20.330492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_lane.py
+-rw-r--r--   0        0        0     4124 2023-06-14 05:25:20.330492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_node.py
+-rw-r--r--   0        0        0     1183 2023-07-27 11:04:21.204500 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_light.py
+-rw-r--r--   0        0        0     1966 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_sign.py
+-rw-r--r--   0        0        0     2729 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_sublayered_graph.py
+-rw-r--r--   0        0        0    14872 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/segment_clusters.py
+-rw-r--r--   0        0        0    11702 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/traffic_sign_parser.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.442303 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-26 01:03:31.202176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/__init__.py
+-rw-r--r--   0        0        0     6345 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_edge.py
+-rw-r--r--   0        0        0    21245 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_format.py
+-rw-r--r--   0        0        0      581 2023-06-14 05:25:20.330492 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_node.py
+-rw-r--r--   0        0        0    12783 2023-07-27 11:04:21.204500 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intersection_enhancement.py
+-rw-r--r--   0        0        0     2407 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/traffic_light_generator.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.442303 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/__init__.py
+-rw-r--r--   0        0        0     3482 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/downloader.py
+-rw-r--r--   0        0        0     7332 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/info_deduction.py
+-rw-r--r--   0        0        0    36854 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/osm_parser.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.442303 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/utility/__init__.py
+-rw-r--r--   0        0        0      508 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/utility/custom_types.py
+-rw-r--r--   0        0        0     2055 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/utility/geonamesID.py
+-rw-r--r--   0        0        0     1286 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/utility/graph_analysis.py
+-rw-r--r--   0        0        0      857 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/utility/idgenerator.py
+-rw-r--r--   0        0        0     9259 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/utility/plots.py
+-rw-r--r--   0        0        0     3554 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/main.py
+-rw-r--r--   0        0        0      198 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/.gitignore
+-rw-r--r--   0        0        0      288 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/__init__.py
+-rw-r--r--   0        0        0     8301 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/config.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.442303 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/cr2sumo/__init__.py
+-rw-r--r--   0        0        0   117001 2023-07-27 11:04:21.204500 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/cr2sumo/converter.py
+-rw-r--r--   0        0        0     9602 2023-07-27 11:04:21.204500 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/cr2sumo/mapping.py
+-rw-r--r--   0        0        0     5166 2023-07-27 11:04:21.204500 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_light.py
+-rw-r--r--   0        0        0     9635 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_sign.py
+-rw-r--r--   0        0        0      387 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/errors.py
+-rw-r--r--   0        0        0     2769 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/merge.py
+-rw-r--r--   0        0        0     2050 2023-06-29 12:45:08.428478 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/sumo2cr.py
+-rw-r--r--   0        0        0    62888 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/sumolib_net.py
+-rw-r--r--   0        0        0     5629 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/templates/DEU.typ.xml
+-rw-r--r--   0        0        0      647 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/templates/README.md
+-rw-r--r--   0        0        0     4613 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/templates/USA.typ.xml
+-rw-r--r--   0        0        0     5629 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/templates/ZAM.typ.xml
+-rw-r--r--   0        0        0      796 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/templates/default.sumo.cfg
+-rw-r--r--   0        0        0    20378 2023-04-26 01:03:31.206176 commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/util.py
+-rw-r--r--   0        0        0      731 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/start_gui.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.446303 commonroad_scenario_designer-0.7.2/crdesigner/ui/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.446303 commonroad_scenario_designer-0.7.2/crdesigner/ui/cli/__init__.py
+-rw-r--r--   0        0        0     7028 2023-07-29 13:25:24.558301 commonroad_scenario_designer-0.7.2/crdesigner/ui/cli/command_line.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.446303 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/__init__.py
+-rw-r--r--   0        0        0      427 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/gui.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.446303 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.446303 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/__init__.py
+-rw-r--r--   0        0        0     4670 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/animated_viewer_wrapper.py
+-rw-r--r--   0        0        0       44 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/__init__.py
+-rw-r--r--   0        0        0    16825 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/animated_viewer.py
+-rw-r--r--   0        0        0    44796 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/dynamic_canvas.py
+-rw-r--r--   0        0        0     2154 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/helper.py
+-rw-r--r--   0        0        0      346 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/__init__.py
+-rw-r--r--   0        0        0     8704 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/draw_params_updater.py
+-rw-r--r--   0        0        0      566 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/general_services.py
+-rw-r--r--   0        0        0     1511 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/scenario_resizer.py
+-rw-r--r--   0        0        0     6239 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/gui_sumo_simulation.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.446303 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/__init__.py
+-rw-r--r--   0        0        0      828 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/crdesigner_console_wrapper.py
+-rw-r--r--   0        0        0     6882 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/mwindow.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.446303 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/__init__.py
+-rw-r--r--   0        0        0    11509 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/aerial_data.py
+-rw-r--r--   0        0        0      690 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/config.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.446303 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/converter_modules/__init__.py
+-rw-r--r--   0        0        0      499 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/converter_modules/converter_interface.py
+-rw-r--r--   0        0        0     3382 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/converter_modules/opendrive_interface.py
+-rw-r--r--   0        0        0     2203 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/converter_modules/osm_interface.py
+-rw-r--r--   0        0        0      883 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/errors.py
+-rw-r--r--   0        0        0     5193 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/general_services.py
+-rw-r--r--   0        0        0     1567 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.py
+-rw-r--r--   0        0        0     2702 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.ui
+-rw-r--r--   0        0        0     6650 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.py
+-rw-r--r--   0        0        0     6134 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.ui
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.446303 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/__init__.py
+-rw-r--r--   0        0        0    23092 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/gui_settings_ui.py
+-rw-r--r--   0        0        0    34788 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/osm_settings_ui.py
+-rw-r--r--   0        0        0    10566 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog.py
+-rw-r--r--   0        0        0     5960 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog_ui.py
+-rw-r--r--   0        0        0     5536 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/settings_ui.py
+-rw-r--r--   0        0        0      464 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/size_policies.py
+-rw-r--r--   0        0        0    41909 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/sumo_settings_ui.py
+-rw-r--r--   0        0        0     9993 2023-07-29 13:25:24.562301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_settings.py
+-rw-r--r--   0        0        0  1852651 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.py
+-rw-r--r--   0        0        0     1136 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.qrc
+-rw-r--r--   0        0        0    33556 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/Groupe_6.png
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.446303 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/__init__.py
+-rw-r--r--   0        0        0     8020 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_left.png
+-rw-r--r--   0        0        0      645 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_right.png
+-rw-r--r--   0        0        0      770 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_lane.png
+-rw-r--r--   0        0        0    21597 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_redo.png
+-rw-r--r--   0        0        0    21742 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_undo.png
+-rw-r--r--   0        0        0    32283 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/close.png
+-rw-r--r--   0        0        0    67646 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr.ico
+-rw-r--r--   0        0        0    89174 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.ico
+-rw-r--r--   0        0        0    26980 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.png
+-rw-r--r--   0        0        0    96318 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr2.ico
+-rw-r--r--   0        0        0    17853 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/drawing_mode.png
+-rw-r--r--   0        0        0    68262 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.ico
+-rw-r--r--   0        0        0      646 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.png
+-rw-r--r--   0        0        0      207 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/iconmonstr-trash-can-darkmode.png
+-rw-r--r--   0        0        0      409 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/iconmonstr-trash-can.svg
+-rw-r--r--   0        0        0     1417 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/merge_lanelet.png
+-rw-r--r--   0        0        0    26374 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/new_file.png
+-rw-r--r--   0        0        0    12185 2023-07-29 13:25:24.574301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.png
+-rw-r--r--   0        0        0   140025 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.svg
+-rw-r--r--   0        0        0    25413 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/open_file.png
+-rw-r--r--   0        0        0     1438 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause.png
+-rw-r--r--   0        0        0     3976 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause_darkmode.png
+-rw-r--r--   0        0        0     2303 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/play.png
+-rw-r--r--   0        0        0   109822 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.png
+-rw-r--r--   0        0        0    90702 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.svg
+-rw-r--r--   0        0        0   432254 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/save.ico
+-rw-r--r--   0        0        0    10339 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_file.png
+-rw-r--r--   0        0        0     1673 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.png
+-rw-r--r--   0        0        0     3382 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.svg
+-rw-r--r--   0        0        0      734 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/split_lanelet.png
+-rw-r--r--   0        0        0     4596 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/target-darkmode.png
+-rw-r--r--   0        0        0     8300 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/target.png
+-rw-r--r--   0        0        0    67646 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/tools.ico
+-rw-r--r--   0        0        0      956 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/help_actions.py
+-rw-r--r--   0        0        0    72753 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/map_creator.py
+-rw-r--r--   0        0        0    29430 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/osm_settings.py
+-rw-r--r--   0        0        0    29122 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/osm_settings_ui.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.450302 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/services/__init__.py
+-rw-r--r--   0        0        0     6254 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/services/config_default.py
+-rw-r--r--   0        0        0    22397 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/services/plots_interactive.py
+-rw-r--r--   0        0        0     7409 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/services/waitingspinnerwidget.py
+-rw-r--r--   0        0        0      115 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/settings.json
+-rw-r--r--   0        0        0     3965 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/settings.py
+-rw-r--r--   0        0        0     8395 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/sumo_settings.py
+-rw-r--r--   0        0        0      356 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/transfer.py
+-rw-r--r--   0        0        0     2064 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/util.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.450302 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.450302 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/__init__.py
+-rw-r--r--   0        0        0      940 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/create_converter_toolbox.py
+-rw-r--r--   0        0        0    18391 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox.py
+-rw-r--r--   0        0        0     7878 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox_ui.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.450302 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/__init__.py
+-rw-r--r--   0        0        0      770 2023-07-29 13:25:24.578301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/create_obstacle_toolbox.py
+-rw-r--r--   0        0        0    54836 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox.py
+-rw-r--r--   0        0        0    15463 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox_ui.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.450302 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/__init__.py
+-rw-r--r--   0        0        0      926 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/create_road_network_toolbox.py
+-rw-r--r--   0        0        0   114922 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox.py
+-rw-r--r--   0        0        0    79617 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox_ui.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.450302 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/service_layer/__init__.py
+-rw-r--r--   0        0        0      450 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/service_layer/general_services.py
+-rw-r--r--   0        0        0    14360 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/toolbox_ui.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.450302 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.450302 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/__init__.py
+-rw-r--r--   0        0        0     3183 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/menu_bar_wrapper.py
+-rw-r--r--   0        0        0      510 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/__init__.py
+-rw-r--r--   0        0        0     4665 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/file_actions.py
+-rw-r--r--   0        0        0      993 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/general_services.py
+-rw-r--r--   0        0        0      451 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/help_actions.py
+-rw-r--r--   0        0        0     1391 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/setting_actions.py
+-rw-r--r--   0        0        0        0 2023-07-29 13:25:25.454302 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/__init__.py
+-rw-r--r--   0        0        0    12620 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/toolbar_wrapper.py
+-rw-r--r--   0        0        0     1230 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/top_bar_wrapper.py
+-rw-r--r--   0        0        0     2211 2023-07-29 13:25:24.582301 commonroad_scenario_designer-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    13101 1970-01-01 00:00:00.000000 commonroad_scenario_designer-0.7.2/PKG-INFO
```

### Comparing `commonroad_scenario_designer-0.7.1/LICENSE.txt` & `commonroad_scenario_designer-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/README.md` & `commonroad_scenario_designer-0.7.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # CommonRoad Scenario Designer
-[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
-[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
-[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)  
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)  
 [![PyPI version fury.io](https://badge.fury.io/py/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)
 [![PyPI download week](https://img.shields.io/pypi/dw/commonroad-scenario-designer.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-scenario-designer/) 
 [![PyPI download month](https://img.shields.io/pypi/dm/commonroad-scenario-designer.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-scenario-designer/)  
 [![PyPI license](https://img.shields.io/pypi/l/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)
 
 This toolbox provides map converters for [OpenStreetMap](https://www.openstreetmap.de/karte.html) (OSM), 
@@ -143,19 +140,19 @@
 
 ## Bug and feature reporting
 This release (v0.7.1) is still a BETA version.  
 In case you detect a bug or you want to suggest a new feature, please report it in our [forum](https://commonroad.in.tum.de/forum/c/scenario-designer/18).   
 If you want to contribute to the toolbox, you can also post it in the [forum](https://commonroad.in.tum.de/forum/c/scenario-designer/18) or contact [Sebastian Maierhofer](sebastian.maierhofer@tum.de).
 
 ## Authors
-
-Responsible: Sebastian Maierhofer, Sebastian Mair
-Contribution (in alphabetic order by last name): Daniel Asch, Hamza Begic, Florian Braunmiller, Tim Dang, 
-Behtarin Ferdousi, Maximilian Fruehauf, Marcus Gabler, Fabian Hoeltke, Aaron Kaefer, David Le, Gustaf Lindgren, 
-Sarra Ben Mohamed, Benjamin Orthen, Luisa Ortner, Louis Pröbstle, Benedikt Reinhard, Maximilian Rieger, Til Stotz, Stefan Urban
+Responsible: Sebastian Maierhofer, Sebastian Mair  
+Contribution (in alphabetic order by last name): Daniel Asch, Hamza Begic, Mohamed Bouhali, Florian Braunmiller, 
+Tim Dang, Behtarin Ferdousi, Maximilian Fruehauf, Marcus Gabler, Fabian Hoeltke, Tom Irion, Aaron Kaefer, Anton Kluge, 
+David Le, Gustaf Lindgren, Sarra Ben Mohamed, Benjamin Orthen, Luisa Ortner, Louis Pröbstle, Benedikt Reinhard, 
+Maximilian Rieger, Til Stotz, Stefan Urban, Max Winklhofer
 
 ## Credits
 We gratefully acknowledge partial financial support by
 - DFG (German Research Fundation) Priority Program SPP 1835 Cooperative Interacting Automobiles
 - BMW Group within the Car@TUM project
 - Central Innovation Programme of the German Federal Government under grant no. ZF4086007BZ8
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/config/config.py` & `commonroad_scenario_designer-0.7.2/crdesigner/config/config.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/configurations/custom_settings_osm2cr.yaml` & `commonroad_scenario_designer-0.7.2/crdesigner/configurations/custom_settings_osm2cr.yaml`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/configurations/default_settings_osm2cr.yaml` & `commonroad_scenario_designer-0.7.2/crdesigner/configurations/default_settings_osm2cr.yaml`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/conversion_lanelet.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/common/conversion_lanelet.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/conversion_lanelet_network.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/common/conversion_lanelet_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import numpy as np
 import shapely
 from shapely.validation import make_valid
 from pyproj import Transformer
 
 from commonroad.scenario.lanelet import LaneletNetwork, StopLine
 from commonroad.scenario.intersection import IntersectionIncomingElement, Intersection
-from commonroad.scenario.traffic_sign import TrafficLightDirection, TrafficLight, TrafficSign
+from commonroad.scenario.traffic_sign import TrafficSign
+from commonroad.scenario.traffic_light import TrafficLight, TrafficLightDirection
 
 from crdesigner.config.config import OpenDRIVEConversionParams
 from crdesigner.map_conversion.common import geometry
 from crdesigner.map_conversion.common.utils import convert_to_new_lanelet_id
 from crdesigner.map_conversion.common.conversion_lanelet import ConversionLanelet
 from crdesigner.map_conversion.common.utils import generate_unique_id
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/geometry.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/common/geometry.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/utils.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/common/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,31 +14,22 @@
         return generate_unique_id.counter
     generate_unique_id.counter += 1
     return generate_unique_id.counter
 
 
 def convert_to_new_lanelet_id(old_lanelet_id: str, ids_assigned: dict) -> int:
     """
-    Convert the old lanelet ids (format 501.1.-1.-1) to newer, simpler ones (100, 101 etc.). Do this by consecutively
-    assigning numbers, starting at 100, to the old_lanelet_id strings. Save the assignments in the dict which is passed
-    to the function as ids_assigned.
+    Convert the old lanelet ids (format 501.1.-1.-1) to newer, simpler ones (100, 101 etc.).
+    Save the assignments in the dict which is passed to the function as ids_assigned.
 
     :param old_lanelet_id: Old id with format '501.1.-1.-1'
-    :type old_lanelet_id: str
     :param ids_assigned: Dict with all previous assignments
-    :type ids_assigned: dict
     :return: The new lanelet id
-    :rtype: int
     """
 
-    starting_lanelet_id = 100
-
     if old_lanelet_id in ids_assigned.keys():
         new_lanelet_id = ids_assigned[old_lanelet_id]
     else:
-        try:
-            new_lanelet_id = generate_unique_id()
-        except ValueError:
-            new_lanelet_id = starting_lanelet_id
+        new_lanelet_id = generate_unique_id()
         ids_assigned[old_lanelet_id] = new_lanelet_id
 
     return new_lanelet_id
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/cr2lanelet.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/lanelet2/cr2lanelet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Optional, Tuple, Union, Dict
 
 import numpy as np
 from pyproj import CRS, Transformer
-from commonroad.scenario.lanelet import Lanelet  # type: ignore
-from commonroad.scenario.traffic_sign import TrafficLight, TrafficSign  # type: ignore
+from commonroad.scenario.lanelet import Lanelet
+from commonroad.scenario.traffic_sign import TrafficSign
+from commonroad.scenario.traffic_light import TrafficLight
 
 from crdesigner.config.config import Lanelet2ConversionParams
 from crdesigner.map_conversion.common.utils import generate_unique_id
 from crdesigner.map_conversion.lanelet2.lanelet2 import OSMLanelet, Node, Way, WayRelation, RegulatoryElement
 
 
 def _convert_subtype_names(subtype: str, subtypes: List[str]) -> [str, bool]:
@@ -114,21 +115,21 @@
         self.last_nodes = {}  # saves last left and right node
         self.left_ways = {}
         self.right_ways = {}
         if self._config.translate:
             if scenario.location is not None and not isinstance(scenario.location.gps_longitude, str) and\
                     abs(scenario.location.gps_longitude) <= 180 and abs(scenario.location.gps_latitude) <= 90:
                 self.origin_utm = self.transformer.transform(scenario.location.gps_latitude,
-                                                              scenario.location.gps_longitude)
+                                                             scenario.location.gps_longitude)
             elif scenario.location is not None and isinstance(scenario.location.gps_longitude, str) and\
                     abs(float(scenario.location.gps_longitude)) <= 180 \
                     and abs(float(scenario.location.gps_latitude)) <= 90:
                 self.origin_utm = \
                     self.transformer.transform(float(scenario.location.gps_latitude),
-                                                float(scenario.location.gps_longitude))
+                                               float(scenario.location.gps_longitude))
             else:
                 self.origin_utm = self.transformer.transform(0, 0)
 
             # convert lanelets
         for lanelet in scenario.lanelet_network.lanelets:
             self._convert_lanelet(lanelet)
 
@@ -155,25 +156,30 @@
         # One regulatory element is created for each lanelet that has a corresponding traffic_light element
         for ll in self.lanelet_network.lanelets:
             traffic_light_reference_list = []
             for lightID in ll.traffic_lights:
                 # find the coordinates of the CR traffic light
                 # and check them with traffic light in L2 format that we have created
 
-                # x,y = self.lanelet_network._traffic_lights[lightID].position
-                x, y = self.lanelet_network.find_traffic_light_by_id(lightID).position
+                # if 'position' returns 2 values, *z will be empty. Else, it will be an array with remaining values
+                x, y, *z = self.lanelet_network.find_traffic_light_by_id(lightID).position
+                if len(z) == 0:
+                    z = 0
+                else:
+                    z = z[0]
 
-                xsign, ysign = self.transformer.transform(self.origin_utm[0] + x, self.origin_utm[1] + y)
+                lat_sign, lon_sign = self.transformer.transform(self.origin_utm[0] + x, self.origin_utm[1] + y)
                 for way in self.osm.ways:
                     if self.osm.find_way_by_id(way).tag_dict.get('type') == "traffic_light":
 
-                        nx = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lon
-                        ny = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lat
+                        n_lon = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lon
+                        n_lat = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lat
+                        n_ele = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).ele
 
-                        if str(xsign) == nx and str(ysign) == ny:
+                        if str(lon_sign) == n_lon and str(lat_sign) == n_lat and str(z) == n_ele:
                             # found the same traffic light, now to reference it
                             traffic_light_reference_list.append(way)
 
             if len(ll.traffic_lights) > 0:
                 # map the end of the lanelet to the ref_line
                 # maybe map the stop line also? Lanelets from examples didn't have stopLines so double check if needed
                 x, y = self._get_shared_last_nodes_from_other_lanelets(ll)
@@ -186,36 +192,41 @@
 
     def _convert_traffic_light(self, light: TrafficLight):
         """
         Add traffic light to the lanelet2 format
         """
         traffic_light_id = self.id_count
         # create a node that represent the sign position
-        x1, y1 = self.transformer.transform(self.origin_utm[0] + light.position[0],
-                                            self.origin_utm[1] + light.position[1])
+        lat1, lon1 = self.transformer.transform(self.origin_utm[0] + light.position[0],
+                                                self.origin_utm[1] + light.position[1])
+
+        # consider z-coordinate
+        z = 0
+        if len(light.position) == 3:
+            z = light.position[2]
 
         id1 = self.id_count
 
         # since 3 nodes are needed to represent the sign in the l2 format (only 1 in the cr format)
         # create another 2 nodes that are close to the first one
 
-        x2, y2 = self.transformer.transform(self.origin_utm[0] + light.position[0] + 0.1,
-                                             self.origin_utm[1] + light.position[1] + 0.1)
-        x3, y3 = self.transformer.transform(self.origin_utm[0] + light.position[0] - 0.1,
-                                             self.origin_utm[1] + light.position[1] - 0.1)
+        lat2, lon2 = self.transformer.transform(self.origin_utm[0] + light.position[0] + 0.1,
+                                                self.origin_utm[1] + light.position[1] + 0.1)
+        lat3, lon3 = self.transformer.transform(self.origin_utm[0] + light.position[0] - 0.1,
+                                                self.origin_utm[1] + light.position[1] - 0.1)
         id2 = self.id_count
         id3 = self.id_count
 
         # creating and adding those nodes to our osm
-        self.osm.add_node(Node(id1, y1, x1, autoware=self._config.autoware))
-        self.osm.add_node(Node(id2, y2, x2, autoware=self._config.autoware))
-        self.osm.add_node(Node(id3, y3, x3, autoware=self._config.autoware))
+        self.osm.add_node(Node(id1, lat1, lon1, z, autoware=self._config.autoware))
+        self.osm.add_node(Node(id2, lat2, lon2, z, autoware=self._config.autoware))
+        self.osm.add_node(Node(id3, lat3, lon3, z, autoware=self._config.autoware))
 
         # get the first light color as subtype
-        traffic_light_subtype = light.cycle[0].state.value
+        traffic_light_subtype = light.traffic_light_cycle.cycle_elements[0].state.value
 
         self.osm.add_way(Way(traffic_light_id, [id1, id2, id3],
                              tag_dict={"subtype": traffic_light_subtype, "type": "traffic_light"}))
 
     def _add_right_of_way_relation(self):
         """
         Add traffic sign relations to the lanelet2 format
@@ -229,27 +240,35 @@
         dict_stop_lines = self._create_stop_line_to_way_dictionary()
 
         # go through signs
         for way in self.osm.ways:
             if self.osm.find_way_by_id(way).tag_dict.get('type') == "traffic_sign":
                 # find the corresponding yield and right of way ways
                 # find x and y coordinates of the sign and match it to signs of the lanelets to find the lanelet
+                # consider z-coordinate as well
 
                 # in lanelet2cr, only node 0 is taken for the position
-                nx = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lon
-                ny = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lat
+                n_lon = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lon
+                n_lat = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lat
+                n_ele = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).ele
 
                 # go through the lanelets to find the lanelet that has the matching traffic_sign in its attribute
                 for ll in self.lanelet_network.lanelets:
                     for traffic_sign_id in ll.traffic_signs:
-                        x, y = self.lanelet_network.find_traffic_sign_by_id(traffic_sign_id).position
-                        x_sign, y_sign = self.transformer.transform(self.origin_utm[0] + x, self.origin_utm[1] + y)
+                        # if 'position' returns 2 values, *z will be empty. Else, it will be an array with remaining
+                        # values
+                        x, y, *z = self.lanelet_network.find_traffic_sign_by_id(traffic_sign_id).position
+                        if len(z) == 0:
+                            z = 0
+                        else:
+                            z = z[0]
+                        lat_sign, lon_sign = self.transformer.transform(self.origin_utm[0] + x, self.origin_utm[1] + y)
                         # have to map the signs based on the position,
                         # as the same 2 signs do not have the same ID in L2 and CR format
-                        if nx == str(x_sign) and ny == str(y_sign):
+                        if n_lon == str(lon_sign) and n_lat == str(lat_sign) and n_ele == str(z):
                             # position matches, found the corresponding lanelet with selected sign
                             # extract the way that corresponds to our lanelet
                             # sign -> lanelet -> way (right+left) -> wayrelation
                             right_way_id = self.right_ways[ll.lanelet_id]
                             left_way_id = self.left_ways[ll.lanelet_id]
                             for way_rel in self.osm.way_relations:
                                 if (self.osm.find_way_rel_by_id(
@@ -275,21 +294,30 @@
             if ll.stop_line:
                 # found a lanelet with a stop line
                 stop_line = ll.stop_line
                 # stop line has 2 points (each point has x and y coordinates)
                 stop_line_start = stop_line.start
                 stop_line_end = stop_line.end
                 # transform the x and y coordinates to the L2 coordinate system
-                x_start, y_start = self.transformer.transform(self.origin_utm[0] + stop_line_start[0],
-                                                              self.origin_utm[1] + stop_line_start[1])
-                x_end, y_end = self.transformer.transform(self.origin_utm[0] + stop_line_end[0],
-                                                          self.origin_utm[1] + stop_line_end[1])
+                lat_start, lon_start = self.transformer.transform(self.origin_utm[0] + stop_line_start[0],
+                                                                  self.origin_utm[1] + stop_line_start[1])
+                lat_end, lon_end = self.transformer.transform(self.origin_utm[0] + stop_line_end[0],
+                                                              self.origin_utm[1] + stop_line_end[1])
+
+                # consider the z-coordinate
+                z_start = 0
+                if len(stop_line_start) == 3:
+                    z_start = stop_line_start[2]
+                z_end = 0
+                if len(stop_line_end) == 3:
+                    z_end = stop_line_end[2]
+
                 # create nodes from the points and add them to the osm
-                node_start = Node(self.id_count, y_start, x_start, autoware=self._config.autoware)
-                node_end = Node(self.id_count, y_end, x_end, autoware=self._config.autoware)
+                node_start = Node(self.id_count, lat_start, lon_start, z_start, autoware=self._config.autoware)
+                node_end = Node(self.id_count, lat_end, lon_end, z_end, autoware=self._config.autoware)
                 self.osm.add_node(node_start)
                 self.osm.add_node(node_end)
                 # create a way from newly created nodes and add it to the osm
                 stop_line_way = Way(self.id_count, [node_start.id_, node_end.id_], tag_dict={"type": "stop_line"})
                 self.osm.add_way(stop_line_way)
                 # map the way with the lanelet
                 dict_stop_lines[ll.lanelet_id] = stop_line_way.id_
@@ -343,27 +371,32 @@
         """
         Convert a traffic sign to way which will be mapped by RightOfWay Regulatory element
         Add the resulting right of way relation to the OSM.
 
         :param sign: Traffic Sign to be converted.
         """
         # create a node that represent the sign position
-        x1, y1 = self.transformer.transform(self.origin_utm[0] + sign.position[0],
-                                             self.origin_utm[1] + sign.position[1])
+        lat_1, lon_1 = self.transformer.transform(self.origin_utm[0] + sign.position[0],
+                                                  self.origin_utm[1] + sign.position[1])
         id1 = self.id_count
 
         # since 2 nodes are needed to represent the sign in the l2 format (only 1 in the cr format)
         # create another node that is close to the first one
-        x2, y2 = self.transformer.transform(self.origin_utm[0] + sign.position[0] + 0.25,
-                                             self.origin_utm[1] + sign.position[1] + 0.25)
+        lat_2, lon_2 = self.transformer.transform(self.origin_utm[0] + sign.position[0] + 0.25,
+                                                  self.origin_utm[1] + sign.position[1] + 0.25)
         id2 = self.id_count
 
+        # check if the sign has z-coordinate (elevation)
+        z = 0
+        if len(sign.position) == 3:  # the sign has a z-coordinate
+            z = sign.position[2]
+
         # creating and adding those nodes to our osm
-        self.osm.add_node(Node(id1, y1, x1, autoware=self._config.autoware))
-        self.osm.add_node(Node(id2, y2, x2, autoware=self._config.autoware))
+        self.osm.add_node(Node(id1, lat_1, lon_1, z, autoware=self._config.autoware))
+        self.osm.add_node(Node(id2, lat_2, lon_2, z, autoware=self._config.autoware))
 
         # matching the type of the traffic sign
         sign_id = sign.traffic_sign_elements[0].traffic_sign_element_id
         val = ""
         for country in self._config.supported_countries:
             for k in country:
                 if k == sign_id:
@@ -506,19 +539,22 @@
 
         :param vertices: List of vertices from a lanelet boundary.
         :return: Ids of nodes which were created.
         """
         nodes = []
         for vertex in vertices:
             lat, lon = self.transformer.transform(self.origin_utm[0] + vertex[0], self.origin_utm[1] + vertex[1])
+            ele = 0  # z-coordinate value
+            if len(vertex) > 2:  # if vertex returns z-coordinate (along with x and y), take it into account
+                ele = vertex[2]
             if self._config.use_local_coordinates:
-                node = Node(self.id_count, lat, lon, autoware=self._config.autoware, local_x=vertex[0],
+                node = Node(self.id_count, lat, lon, ele, autoware=self._config.autoware, local_x=vertex[0],
                             local_y=vertex[1])
             else:
-                node = Node(self.id_count, lat, lon, autoware=self._config.autoware)
+                node = Node(self.id_count, lat, lon, ele, autoware=self._config.autoware)
             nodes.append(node.id_)
             self.osm.add_node(node)
         return nodes
 
     def _get_potential_right_way(self, lanelet) -> Union[None, int]:
         """
         Check if a shared right boundary with another lanelet can be transformed
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/lanelet2/lanelet2.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             local_x.set("k", "local_x")
             local_x.set("v", str(self.local_x))
             local_y = etree.SubElement(node, "tag")
             local_y.set("k", "local_y")
             local_y.set("v", str(self.local_y))
             node.append(local_x)
             node.append(local_y)
-        if self.ele != "0.0" or self.autoware:
+        if (self.ele != "0.0" and self.ele != '0') or self.autoware:
             ele = etree.SubElement(node, "tag")
             ele.set("k", "ele")
             ele.set("v", self.ele)
             node.append(ele)
 
         return node
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2_parser.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/lanelet2/lanelet2_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,20 @@
 
     def parse(self):
         """
         Parses the nodes, way relations, reg_element relations
         """
         osm = OSMLanelet()
         for node in self.xml.xpath("//node[@lat and @lon and @id]"):
-            osm.add_node(Node(node.get("id"), node.get("lat"), node.get("lon")))
+            for tag in node.findall("./tag"):
+                if tag.attrib.get("k") == "ele":
+                    osm.add_node(Node(node.get("id"), node.get("lat"), node.get("lon"), tag.attrib.get("v")))
+                    break
+            else:
+                osm.add_node(Node(node.get("id"), node.get("lat"), node.get("lon")))
 
         for way in self.xml.xpath("//way[@id]"):
             node_ids = [nd.get("ref") for nd in way.xpath("./nd")]
             tag_dict = {tag.get("k"): tag.get("v") for tag in way.xpath("./tag[@k and @v]") if
                         tag.get("k") in ALLOWED_TAGS}
 
             osm.add_way(Way(way.get("id"), node_ids, tag_dict))
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2cr.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/lanelet2/lanelet2cr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from collections import defaultdict
 from typing import List, Optional, Tuple, Dict, Union
 from shapely.geometry import LineString  # type: ignore
 import numpy as np
 from pyproj import Transformer, CRS
 import logging
 
-from commonroad.scenario.lanelet import StopLine, LineMarking, RoadUser, Lanelet, LaneletNetwork  # type: ignore
-from commonroad.scenario.traffic_sign import (TrafficSignElement, TrafficSignIDGermany,  # type: ignore
-                                              TrafficSignIDUsa,  # type: ignore
-                                              TrafficSignIDZamunda, TrafficLightCycleElement,
-                                              TrafficLightState, TrafficLightDirection)  # type: ignore
+from commonroad.scenario.lanelet import StopLine, LineMarking, RoadUser, Lanelet, LaneletNetwork
+from commonroad.scenario.traffic_sign import (TrafficSignElement, TrafficSignIDGermany, TrafficSignIDUsa,
+                                              TrafficSignIDZamunda)
+from commonroad.scenario.traffic_light import (TrafficLightCycleElement, TrafficLightState, TrafficLightDirection,
+                                               TrafficLightCycle)
 from commonroad.scenario.scenario import Scenario, ScenarioID, TrafficSign, Location, TrafficLight, \
     GeoTransformation  # type: ignore
 
 from crdesigner.map_conversion.lanelet2.lanelet2 import OSMLanelet
 from crdesigner.map_conversion.common.utils import generate_unique_id
 from crdesigner.map_conversion.common.conversion_lanelet import ConversionLanelet
 from crdesigner.map_conversion.common.conversion_lanelet_network import \
@@ -248,16 +248,16 @@
         scenario = Scenario(dt=self._cr_config.time_step_size, scenario_id=scenario_id,
                             location=Location(gps_latitude=origin_lat, gps_longitude=origin_lon))
         self.lanelet_network = ConversionLaneletNetwork()
 
         speed_limits = {}
         speed_limit_lanelets = {}  # type: ignore
         for speed_limit_key in osm.speed_limit_signs.keys():
-            light_id = generate_unique_id()
-            speed_limits[speed_limit_key] = light_id
+            sign_id = generate_unique_id()
+            speed_limits[speed_limit_key] = sign_id
             speed_limit_lanelets[speed_limit_key] = []
 
         for way_rel in osm.way_relations.values():
             # add traffic sign id to traffic signs for speed limit
             # create dictionary for mapping of osm id to cr id and keep id constant
             # later add speed limit as traffic sign
             lanelet = self._way_rel_to_lanelet(way_rel, self._config.adjacencies, self._config.left_driving,
@@ -289,19 +289,21 @@
             except NotImplementedError as e:
                 logging.error("Lanelet2CRConverter: " + str(e))
 
         # speed limit sign conversion
         for speed_limit_key in osm.speed_limit_signs.keys():
             speed, traffic_sign_id = osm.speed_limit_signs[speed_limit_key]
             light_id = speed_limits[speed_limit_key]
-            first_occurrence = {self.lanelet_network._old_lanelet_ids[l_id] for l_id in
-                                speed_limit_lanelets[speed_limit_key]}
+            first_occurrence = \
+                {self.lanelet_network._old_lanelet_ids[l_id] for l_id in speed_limit_lanelets[speed_limit_key]}
             position = self.lanelet_network.find_lanelet_by_id(
                     self.lanelet_network._old_lanelet_ids[speed_limit_lanelets[speed_limit_key][0]]).left_vertices[0]
-            speed_limit = TrafficSign(light_id, [TrafficSignElement(traffic_sign_id, [speed])], first_occurrence,
+            speed_limit = TrafficSign(light_id,
+                                      [TrafficSignElement(traffic_sign_id, [speed])],
+                                      first_occurrence,
                                       position, True)
             self.lanelet_network.add_traffic_sign(speed_limit,
                                                   first_occurrence)
 
         # traffic light conversion
         for way in osm.ways:
             if osm.ways[way].tag_dict.get('type') == 'traffic_light':
@@ -328,28 +330,28 @@
         CommonRoad format
 
         :param traffic_light_way: Way that is being used for conversion
         :param new_lanelet_ids: Dictionary that appends new ids to newly created CR objects
         """
         # create a TrafficLight element (CR format) from the traffic light way (L2 format\<)
         # id,cycle,position,offset,direction,active
-        new_id = convert_to_new_lanelet_id(traffic_light_way.id_, new_lanelet_ids)
+        new_id = generate_unique_id()
 
         cycle_list = _append_traffic_light_cycles(traffic_light_way)
 
         # TL in L2 format is represented with 3 nodes, we will take the one in the middle
         node = self.osm.nodes[traffic_light_way.nodes[1]]
-        node_x = node.lon
-        node_y = node.lat
 
         # convert to CR space
-        x, y = self.transformer.transform(node_x, node_x)
+        x, y = self.transformer.transform(node.lon, node.lat)
         x -= self.origin_utm[0]
         y -= self.origin_utm[1]
-        
+
+        position = np.array([x, y, float(node.ele)]) if node.ele != "0.0" else np.array([x, y])
+
         # need to assign lanelet to that trafficLight
         # find the traffic_light_relations corresponding to our traffic_light_way and add them to the list
         traffic_light_relations = []
         for tl_relation in self.osm.traffic_light_relations:
             for ref in self.osm.traffic_light_relations[tl_relation].refers:
                 if ref == traffic_light_way.id_:
                     traffic_light_relations.append(tl_relation)
@@ -360,15 +362,16 @@
             for re in self.osm.way_relations[wr].regulatory_elements:
                 if re in traffic_light_relations:
                     # found the wr, now need to match it with corresponding lanelet
                     # for that the "new_lanelet_ids" dict is used that is sent to this function
                     wr_lanelets.add(new_lanelet_ids[wr])
 
         # create the traffic light
-        traffic_light = TrafficLight(new_id, cycle_list, np.array([x, y]), 1, TrafficLightDirection.STRAIGHT, True)
+        traffic_light = TrafficLight(new_id, position, TrafficLightCycle(cycle_list, 1), active=True,
+                                     direction=TrafficLightDirection.STRAIGHT)
 
         # add the traffic light to our lanelet network
         self.lanelet_network.add_traffic_light(traffic_light, wr_lanelets)
 
     def _right_of_way_to_traffic_sign(self, right_of_way_rel: RegulatoryElement, new_lanelet_ids: Dict[str, int]) -> \
             Tuple[List[TrafficSign], List[TrafficSign], List[int], List[int], List[StopLine]]:
         """
@@ -397,15 +400,15 @@
         """
 
         traffic_sign_ways = [self.osm.find_way_by_id(r) for r in right_of_way_rel.refers]
         # traffic signs will always be "ways"
         # https://github.com/fzi-forschungszentrum-informatik/Lanelet2/blob/master/lanelet2_core/doc
         # /LinestringTagging.md
 
-        priority_signs, yield_signs = self._traffic_sign_ways_to_traffic_signs(traffic_sign_ways, new_lanelet_ids)
+        priority_signs, yield_signs = self._traffic_sign_ways_to_traffic_signs(traffic_sign_ways)
 
         priority_lanelets = []
         for i in right_of_way_rel.right_of_ways:
             # never create new lanelet ids here,
             # if they don't exist yet, they are never created
             if i in new_lanelet_ids.keys():
                 priority_lanelets.append(new_lanelet_ids[i])
@@ -443,21 +446,20 @@
 
             # initialize stop line
             stop_line = StopLine(start=start, end=end, traffic_sign_ref=ref_t_set_id,
                                  line_marking=LineMarking.BROAD_DASHED)
             stop_lines.append(stop_line)
         return yield_signs, priority_signs, yield_lanelets, priority_lanelets, stop_lines
 
-    def _traffic_sign_ways_to_traffic_signs(self, traffic_sign_ways: List, new_lanelet_ids: Dict[str, int]) \
+    def _traffic_sign_ways_to_traffic_signs(self, traffic_sign_ways: List) \
             -> Tuple[List[TrafficSign], List[TrafficSign]]:
         """
         Converts traffic sign ways (L2) into traffic signs (CR)
 
         :param traffic_sign_ways: ways that will be converted into traffic signs
-        :param new_lanelet_ids: dictionary that will map the newly created traffic signs with their new ids
         :return: tuple of lists that match according to the priority of the traffic sign.
         """
 
         priority_signs, yield_signs = [], []
         for traffic_sign_way in traffic_sign_ways:
             # distinguish yield and stop sign
             # also handles right of way and priority road
@@ -502,19 +504,21 @@
             # create the element of the traffic sign
             traffic_sign_element = TrafficSignElement(tsid, [])
 
             # extract position
             x, y = self.transformer.transform(float(traffic_sign_node.lat), float(traffic_sign_node.lon))
             x -= self.origin_utm[0]
             y -= self.origin_utm[1]
-            ref_t_id = convert_to_new_lanelet_id(traffic_sign_way.id_, new_lanelet_ids)
+            ref_t_id = generate_unique_id()
+            position = np.array([x, y, float(traffic_sign_node.ele)]) \
+                if traffic_sign_node.ele != "0.0" else np.array([x, y])
 
             # create the traffic sign
             traffic_sign = TrafficSign(ref_t_id, traffic_sign_elements=[traffic_sign_element], first_occurrence=set(),
-                                       position=np.array([x, y]), virtual=virtual)
+                                       position=position, virtual=virtual)
             # traffic sign names need to be universal(i.e."YIELD" should be the name of both German and USA Yield signs)
 
             # append the sign to either priority or yield signs
             if tsid.name in self._config.priority_signs:
                 priority_signs.append(traffic_sign)
             else:
                 yield_signs.append(traffic_sign)
@@ -818,28 +822,31 @@
                 self.lanelet_network.set_adjacent_left(lanelet, potential_left_adj, False)
 
         if not potential_right_adj:
             potential_right_adj = self._right_way_ids.get(way_rel.right_way)
             if potential_right_adj is not None:
                 self.lanelet_network.set_adjacent_right(lanelet, potential_right_adj, False)
 
-    def _convert_way_to_vertices(self, way) -> np.ndarray:
+    def _convert_way_to_vertices(self, way: Way) -> np.ndarray:
         """
         Convert a Way to a list of points.
 
         :param way: Way to be converted.
         :return: The vertices of the new lanelet border.
         """
-        vertices = np.empty((len(way.nodes), 2))
+        if any([self.osm.find_node_by_id(node_id).ele != "0.0" for node_id in way.nodes]):
+            vertices = np.empty((len(way.nodes), 3))
+        else:
+            vertices = np.empty((len(way.nodes), 2))
         for i, node_id in enumerate(way.nodes):
             nd = self.osm.find_node_by_id(node_id)
             x, y = self.transformer.transform(float(nd.lat), float(nd.lon))
             x -= self.origin_utm[0]
             y -= self.origin_utm[1]
-            vertices[i] = [x, y]
+            vertices[i] = [x, y, float(nd.ele)] if nd.ele != "0.0" else [x, y]
 
         return vertices
 
     def node_distance(self, node_id1: str, node_id2: str) -> float:
         """
         Calculate distance of one node to other node in the projection.
 
@@ -881,22 +888,23 @@
         """
         n = len(longer_way.nodes) - len(shorter_way.nodes)
         # Coordinates of two nodes in the middle to interpolate and add n nodes in between
         mid = int(len(shorter_way.nodes) / 2)
         start_node = self.osm.find_node_by_id(shorter_way.nodes[mid])
         end_node = self.osm.find_node_by_id(shorter_way.nodes[mid - 1])
         # Parse to nodes with numeric values
-        start_node_f = np.array([float(start_node.lat), float(start_node.lon)])
-        end_node_f = np.array([float(end_node.lat), float(end_node.lon)])
+        start_node_f = np.array([float(start_node.lat), float(start_node.lon), float(start_node.ele)])
+        end_node_f = np.array([float(end_node.lat), float(end_node.lon), float(end_node.ele)])
         # Add n nodes, start from last one
         for i in range(n, 0, -1):
             k = self._config.start_node_id_value
             new_id = int(start_node.id_) + k * 100 + i
             while self.osm.find_node_by_id(str(new_id)) is not None:
                 k = k + 1
                 new_id = int(start_node.id_) + k * 100 + i
             # For Getting n additional nodes, we need to split the segment into n+1 smaller segments
             new_lat = round(start_node_f[0] + (end_node_f[0] - start_node_f[0]) * i / (n + 1), 11)
             new_lon = round(start_node_f[1] + (end_node_f[1] - start_node_f[1]) * i / (n + 1), 11)
-            new_node = Node(new_id, new_lat, new_lon)
+            new_ele = round(start_node_f[2] + (end_node_f[2] - start_node_f[2]) * i / (n + 1), 11)
+            new_node = Node(new_id, new_lat, new_lon, new_ele)
             self.osm.add_node(new_node)
             shorter_way.nodes.insert(mid, new_node.id_)
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/map_conversion_interface.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/map_conversion_interface.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/converter.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/converter.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/network.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/network.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/border.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/border.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/crosswalks.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/crosswalks.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/geo_reference.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/geo_reference.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane_group.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane_group.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/traffic_signals.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/traffic_signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from typing import Union, Tuple, List
 
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.road import Road
 from crdesigner.map_conversion.common.utils import generate_unique_id
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadLanes import LaneSection
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadSignal import Signal
 
-from commonroad.scenario.traffic_sign import TrafficSign, TrafficLight, TrafficSignElement, TrafficSignIDZamunda, \
+from commonroad.scenario.traffic_sign import TrafficSign, TrafficSignElement, TrafficSignIDZamunda, \
     TrafficSignIDGermany, TrafficSignIDUsa, TrafficSignIDChina, TrafficSignIDSpain, TrafficSignIDRussia
+from commonroad.scenario.traffic_light import TrafficLight
 from commonroad.scenario.lanelet import StopLine, LineMarking
 
 
 def extract_traffic_element_id(signal_type: str, signal_subtype: str, traffic_sign_enum: enum) \
         -> Union[TrafficSignIDZamunda, TrafficSignIDGermany, TrafficSignIDUsa, TrafficSignIDChina,
                  TrafficSignIDSpain, TrafficSignIDRussia]:
     """Extract the traffic element id from the signal type and subtype string.
@@ -157,15 +158,15 @@
             traffic_signs.append(traffic_sign)
 
         elif signal.dynamic == 'yes':
             # the three listed here are hard to interpret in commonroad.
             # we ignore such signals in order not cause trouble in traffic simulation
             if signal.type != ("1000002" or "1000007" or "1000013"):
 
-                traffic_light = TrafficLight(traffic_light_id=signal.id + 2000, cycle=[], position=position)
+                traffic_light = TrafficLight(traffic_light_id=signal.id + 2000, position=position)
 
                 traffic_lights.append(traffic_light)
             else:
                 continue
 
     return traffic_lights, traffic_signs, stop_lines
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/utils.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_conversion/utils.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/eulerspiral.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/eulerspiral.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/geometry.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/geometry.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/junction.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/junction.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/opendrive.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/opendrive.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadElevationProfile.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadElevationProfile.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLanes.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLanes.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLateralProfile.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLateralProfile.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLink.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLink.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadObject.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadObject.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadPlanView.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadPlanView.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadSignal.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadSignal.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road_record.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road_record.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadtype.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadtype.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/parser.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/opendrive/opendrive_parser/parser.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/config.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/config.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/converter.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/converter.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/cleanup.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/cleanup.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,19 @@
             already_added = False
             for element in net.find_traffic_sign_by_id(lanelet_sign).traffic_sign_elements:
                 if element not in sign_elements:
                     sign_elements.add(element)
                 else:
                     already_added = True
             if not already_added:
-                filtered_signs.add(net.find_traffic_sign_by_id(lanelet_sign))
+                sign = net.find_traffic_sign_by_id(lanelet_sign)
+                #  Adding a default position to the sign
+                if sign.position is None:
+                    sign.position = la.right_vertices[0]
+                filtered_signs.add(sign)
     for sign in filtered_signs:
         scenario.remove_traffic_sign(sign)
 
 
 def remove_non_referenced_signs(scenario: Scenario) -> None:
     """
     Removes non referenced traffic signs from scenario.
@@ -85,14 +89,17 @@
         for lanelet in net.lanelets:
             if sign.traffic_sign_id in lanelet.traffic_signs:
                 referenced = True
                 break
         if referenced:
             continue
         else:
+            #  Adding a default position to the sign
+            if sign.position is None:
+                sign.position = np.ndarray([0, 0])
             filtered_signs.add(sign)
 
     for sign in filtered_signs:
         scenario.remove_traffic_sign(sign)
 
 
 def merge_short_lanes(scenario: Scenario, min_distance=1) -> None:
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/export.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/export.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/intersection_merger.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/intersection_merger.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/lane_linker.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/lane_linker.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/mapillary.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/mapillary.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/offsetter.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/offsetter.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/restrictions.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/restrictions.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_edge.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_edge.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_functions.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_functions.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_lane.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_lane.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_node.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_node.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_light.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_light.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 GraphTrafficLight class
 """
 
 from typing import Dict
 import numpy as np
 
-from commonroad.scenario.traffic_sign import TrafficLight
+from commonroad.scenario.traffic_light import TrafficLight
 from crdesigner.map_conversion.osm2cr.converter_modules.utility import idgenerator
 
 from ._graph_node import GraphNode
 
 
 class GraphTrafficLight:
     def __init__(self, light: Dict,
@@ -32,9 +32,9 @@
                 self.forward = False
 
     def to_traffic_light_cr(self):
         position = None
         if self.node is not None:
             position_point = self.node.get_point()
             position = np.array([position_point.x, position_point.y])
-        traffic_light = TrafficLight(self.id, cycle=[], position=position)
+        traffic_light = TrafficLight(self.id, position=position)
         return traffic_light
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_sign.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_sign.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_sublayered_graph.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_sublayered_graph.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/segment_clusters.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/segment_clusters.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/traffic_sign_parser.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/traffic_sign_parser.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_edge.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_edge.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_format.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 import commonroad
 import numpy as np
 
 from commonroad.scenario.lanelet import LaneletNetwork
 from commonroad.scenario.obstacle import Obstacle
 from commonroad.scenario.scenario import Scenario, ScenarioID
-from commonroad.scenario.traffic_sign import TrafficSign, TrafficLight
+from commonroad.scenario.traffic_sign import TrafficSign
+from commonroad.scenario.traffic_light import TrafficLight
 from commonroad.scenario.intersection import Intersection, IntersectionIncomingElement
 from commonroad.planning.planning_problem import PlanningProblem, PlanningProblemSet
 from commonroad.scenario.state import CustomState, InitialState
 from commonroad.planning.goal import GoalRegion
 from commonroad.common.util import Interval
 from commonroad.geometry.shape import Rectangle, Circle
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_node.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_node.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intersection_enhancement.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intersection_enhancement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""
-This module is used to enhance intersections with traffic lights.
-"""
-
 from crdesigner.map_conversion.osm2cr.converter_modules.utility import idgenerator
 from crdesigner.map_conversion.common import geometry
 from crdesigner.map_conversion.osm2cr.converter_modules.intermediate_operations.traffic_light_generator import \
     TrafficLightGenerator
 
 
 def intersection_enhancement(intermediate_format):
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/traffic_light_generator.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/traffic_light_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from crdesigner.map_conversion.osm2cr import config
-from commonroad.scenario.traffic_sign import TrafficLight, TrafficLightCycleElement, TrafficLightState, \
-    TrafficLightDirection
+from commonroad.scenario.traffic_light import TrafficLight, TrafficLightCycleElement, TrafficLightState, \
+    TrafficLightDirection, TrafficLightCycle
 
 
 class TrafficLightGenerator:
     """
     This class acts as generator for traffic lights, that can be added to multiple types on intersections.
     Traffic light cycles are based on the number of incoming lanes.
 
@@ -19,24 +19,24 @@
         if number_of_incomings > 4:
             self.cycle['red_phase'] += 50
 
         # internal variables
         self.cycle_length = sum(self.cycle.values())
         self.current_time_offset = 0
 
-    def get_cycle(self):
+    def get_cycle(self) -> TrafficLightCycle:
         """
         Cycle that is applied to all traffic lights
         """
         cycle = [(TrafficLightState.RED, self.cycle['red_phase']),
                  (TrafficLightState.RED_YELLOW, self.cycle['red_yellow_phase']),
                  (TrafficLightState.GREEN, self.cycle['green_phase']),
                  (TrafficLightState.YELLOW, self.cycle['yellow_phase'])]
         cycle_element_list = [TrafficLightCycleElement(state[0], state[1]) for state in cycle]
-        return cycle_element_list
+        return TrafficLightCycle(cycle_element_list, time_offset=self.get_time_offset())
 
     def get_time_offset(self):
         """
         Method is used to get cycle offset for the next new traffic light
         """
 
         offset = self.current_time_offset
@@ -52,11 +52,11 @@
         return offset
 
     def generate_traffic_light(self, position, new_id):
         """
         Method to create the new traffic light
         """
 
-        new_traffic_light = TrafficLight(traffic_light_id=new_id, cycle=self.get_cycle(), position=position,
-                                         time_offset=self.get_time_offset(), direction=TrafficLightDirection.ALL,
+        new_traffic_light = TrafficLight(traffic_light_id=new_id, position=position,
+                                         traffic_light_cycle=self.get_cycle(), direction=TrafficLightDirection.ALL,
                                          active=True)
         return new_traffic_light
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/downloader.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/downloader.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/info_deduction.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/info_deduction.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/osm_parser.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/osm_parser.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/geonamesID.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/utility/geonamesID.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/graph_analysis.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/utility/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/idgenerator.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/utility/idgenerator.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/plots.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/converter_modules/utility/plots.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/main.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/osm2cr/main.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/config.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/config.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/converter.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/cr2sumo/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 from commonroad.common.solution import VehicleType as VehicleTypeParam
 from commonroad.common.util import Interval
 from commonroad.prediction.prediction import TrajectoryPrediction
 from commonroad.scenario.trajectory import State
 from commonroad.scenario.lanelet import LaneletNetwork, Lanelet, LineMarking, LaneletType
 from commonroad.scenario.obstacle import ObstacleRole, ObstacleType
 from commonroad.scenario.scenario import Scenario
-from commonroad.scenario.traffic_sign import SupportedTrafficSignCountry, TrafficLight, \
-    TrafficLightCycleElement, TrafficLightDirection, TrafficSign
+from commonroad.scenario.traffic_sign import SupportedTrafficSignCountry, TrafficSign
+from commonroad.scenario.traffic_light import TrafficLight, TrafficLightCycleElement, TrafficLightDirection
 from commonroad.scenario.traffic_sign_interpreter import TrafficSigInterpreter
 
 from sumocr.maps.scenario_wrapper import AbstractScenarioWrapper
 
 from crdesigner.map_conversion.sumo_map.sumolib_net import (TLS, Connection, Crossing, Edge, Junction, Lane,
                                                             Node, NodeType, RightOfWay,
                                                             VehicleType, SpreadType, sumo_net_from_xml, Net, Roundabout)
@@ -162,15 +162,15 @@
             logger.addHandler(c_handler)
 
         return logger
 
     @classmethod
     def from_file(cls, file_path_cr, conf: SumoConfig):
         scenario, _ = CommonRoadFileReader(file_path_cr).open()
-        return cls(scenario.lanelet_network, conf)
+        return cls(scenario, conf)
 
     def _convert_map(self):
         self._find_lanes()
         self._init_nodes()
         self._create_sumo_edges_and_lanes()
         self._init_connections()
         self.new_nodes, self.merged_dictionary, replaced_nodes = self._merge_junctions_intersecting_lanelets()
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/mapping.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/cr2sumo/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 from enum import Enum, IntEnum
 
 from commonroad.scenario.lanelet import LaneletType
 from commonroad.scenario.obstacle import ObstacleType
 from commonroad.scenario.traffic_sign import SupportedTrafficSignCountry
-from commonroad.scenario.traffic_sign import TrafficLightState, TrafficLightDirection
+from commonroad.scenario.traffic_light import TrafficLightState, TrafficLightDirection
 from crdesigner.map_conversion.sumo_map.sumolib_net import EdgeTypes, EdgeType, VehicleType, SignalState, \
     ConnectionDirection
 
 
 class ClusterInstruction(IntEnum):
     """
     Defines which clustering approach is chosen for an intersection
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_light.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_light.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import defaultdict
 from typing import Set, List, Dict, Tuple
 
 import numpy as np
-from commonroad.scenario.traffic_sign import TrafficLight, TrafficLightCycleElement, TrafficLightState
+from commonroad.scenario.traffic_light import TrafficLight, TrafficLightCycleElement, TrafficLightState
 from crdesigner.map_conversion.sumo_map.sumolib_net import TLSProgram, Connection, NodeType, SignalState, Node, Phase
 from crdesigner.map_conversion.sumo_map.util import lines_intersect, compute_max_curvature_from_polyline
 
 from .mapping import traffic_light_states_CR2SUMO
 
 
 class TrafficLightEncoder:
@@ -19,15 +19,15 @@
                                                                                   List[Connection]]:
         # create SUMO Traffic Light Node
         self.index += 1
         program_id = f"tl_program_{self.index}"
         traffic_light_id = str(node.id)
         node.type = NodeType.TRAFFIC_LIGHT
 
-        time_offset = max(tl.time_offset for tl in traffic_lights)
+        time_offset = max(tl.traffic_light_cycle.time_offset for tl in traffic_lights)
         tls_program = TLSProgram(traffic_light_id, time_offset * self.conf.dt, program_id)
 
         # sync and ungroup light states
         light_states = _sync_traffic_light_cycles(traffic_lights)
         # ungroup light states
         light_states = [
             [s for i, s in enumerate(state)
@@ -83,16 +83,16 @@
 
 def _sync_traffic_light_cycles(traffic_lights: List[TrafficLight]) -> List[List[TrafficLightCycleElement]]:
     """
     Synchronizes traffic lights cycles for a list
     :param traffic_lights:
     :return: list of synchronized states
     """
-    time_steps = np.lcm.reduce([sum(cycle.duration for cycle in tl.cycle) for tl in traffic_lights])
-    states = np.array([_cycles_to_states(traffic_light.cycle, time_steps)
+    time_steps = np.lcm.reduce([sum(cycle.duration for cycle in tl.traffic_light_cycle.cycle_elements) for tl in traffic_lights])
+    states = np.array([_cycles_to_states(traffic_light.traffic_light_cycle.cycle_elements, time_steps)
                        for traffic_light in traffic_lights]).T
     res: List[List[TrafficLightCycleElement]] = []
     i = 0
     j = 0
     while i < len(states):
         j = i + 1
         while j < len(states):
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_sign.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_sign.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/merge.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/merge.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/sumo2cr.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/sumo2cr.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/sumolib_net.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/sumolib_net.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/DEU.typ.xml` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/templates/DEU.typ.xml`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/README.md` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/templates/README.md`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/USA.typ.xml` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/templates/USA.typ.xml`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/ZAM.typ.xml` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/templates/ZAM.typ.xml`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/default.sumo.cfg` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/templates/default.sumo.cfg`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/util.py` & `commonroad_scenario_designer-0.7.2/crdesigner/map_conversion/sumo_map/util.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/start_gui.py` & `commonroad_scenario_designer-0.7.2/crdesigner/start_gui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/cli/command_line.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/cli/command_line.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/animated_viewer_wrapper.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/animated_viewer_wrapper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/animated_viewer.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/animated_viewer.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/dynamic_canvas.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/dynamic_canvas.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/helper.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/helper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/draw_params_updater.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/draw_params_updater.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/general_services.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/general_services.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/scenario_resizer.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/scenario_resizer.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/gui_sumo_simulation.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/gui_sumo_simulation.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/crdesigner_console_wrapper.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/crdesigner_console_wrapper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/mwindow.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/mwindow.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/aerial_data.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/aerial_data.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/config.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/config.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/opendrive_interface.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/converter_modules/opendrive_interface.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/osm_interface.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/converter_modules/osm_interface.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/errors.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/errors.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/general_services.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/general_services.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.ui` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.ui`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.ui` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.ui`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/gui_settings_ui.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/gui_settings_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/osm_settings_ui.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/osm_settings_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog_ui.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/settings_ui.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/settings_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/sumo_settings_ui.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_resources/sumo_settings_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_settings.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_settings.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.qrc` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.qrc`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/Groupe_6.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/Groupe_6.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_left.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_left.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_right.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_right.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_lane.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_lane.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_redo.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_redo.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_undo.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_undo.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/close.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/close.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr.ico` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.ico` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr2.ico` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr2.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/drawing_mode.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/drawing_mode.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.ico` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/merge_lanelet.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/merge_lanelet.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/new_file.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/new_file.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.svg` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.svg`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/open_file.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/open_file.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause_darkmode.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause_darkmode.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/play.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/play.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.svg` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.svg`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save.ico` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/save.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_file.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_file.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.svg` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.svg`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/split_lanelet.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/split_lanelet.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/target-darkmode.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/target-darkmode.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/target.png` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/target.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/tools.ico` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/gui_src/tools.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/help_actions.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/help_actions.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/map_creator.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/map_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-import numpy as np
 from scipy.interpolate import interp1d
-from typing import Tuple
+from typing import Tuple, Union, Set, List
+import numpy as np
 
 from commonroad.scenario.intersection import Intersection
 from commonroad.scenario.intersection import IntersectionIncomingElement
 from commonroad.scenario.lanelet import RoadUser, LaneletNetwork, Lanelet, LineMarking, LaneletType, StopLine
 from commonroad.scenario.scenario import Scenario
-from commonroad.scenario.traffic_sign import *
+from commonroad.scenario.traffic_sign import (
+    TrafficSign, TrafficSignElement, TrafficSignIDArgentina, TrafficSignIDBelgium, TrafficSignIDChina,
+    TrafficSignIDCroatia, TrafficSignIDFrance, TrafficSignIDGermany, TrafficSignIDGreece, TrafficSignIDItaly,
+    TrafficSignIDPuertoRico, TrafficSignIDRussia, TrafficSignIDSpain, TrafficSignIDUsa,  TrafficSignIDZamunda)
+from commonroad.scenario.traffic_light import (TrafficLight, TrafficLightCycleElement, TrafficLightState,
+                                               TrafficLightCycle)
+from commonroad.common.util import is_natural_number
 
 
+# TODO: UNCERTAIN (either controller or model)
 class MapCreator:
     """
     Collection of functions to work with lanelets
     """
 
     @staticmethod
     def create_straight(width: float, length: float, num_vertices: int, lanelet_id: int,
@@ -43,15 +50,16 @@
         @param line_marking_left: Line markings on the left for new lanelet.
         @param line_marking_right: Line markings on the right for new lanelet.
         @param stop_line: Stop line of new lanelet.
         @param traffic_signs: Referenced traffic signs by new lanelet.
         @param traffic_lights: Referenced traffic lights by new lanelet.
         @param backwards: Boolean indicating whether lanelet should be rotated by 180°.
         @param stop_line_at_end: Boolean indicating whether stop line positions should correspond with end of lanelet.
-        @param stop_line_at_beginning: Boolean indicating whether stop line positions should correspond with beginning of lanelet.
+        @param stop_line_at_beginning: Boolean indicating whether stop line positions should correspond
+        with beginning of lanelet.
         @return: Newly created lanelet.
         """
         eps = 0.1e-15
         length_div = length / (num_vertices - 1)
         left_vertices = []
         center_vertices = []
         right_vertices = []
@@ -278,15 +286,16 @@
 
         len_suc = np.round(np.linalg.norm(successor.center_vertices[0] - successor.center_vertices[-1]), 2)
         len_pred = np.round(np.linalg.norm(predecessor.center_vertices[0] - predecessor.center_vertices[-1]), 2)
         wid_suc = np.round(np.linalg.norm(successor.left_vertices[0] - successor.right_vertices[0]), 2)
         wid_pred = np.round(np.linalg.norm(predecessor.left_vertices[0] - predecessor.right_vertices[0]), 2)
         same_length_width = len_suc == len_pred and wid_suc == wid_pred
 
-        if MapCreator.lanelet_is_straight(predecessor) and MapCreator.lanelet_is_straight(successor) and not intersection and same_length_width:
+        if (MapCreator.lanelet_is_straight(predecessor) and
+                MapCreator.lanelet_is_straight(successor) and not intersection and same_length_width):
             successor._left_vertices = predecessor.left_vertices
             successor._center_vertices = predecessor.center_vertices
             successor._right_vertices = predecessor.right_vertices
 
         if same_length_width:
             factor = (np.linalg.norm(successor.left_vertices[0, :] - successor.right_vertices[0, :]) / np.linalg.norm(
                     (predecessor.left_vertices[-1, :] - predecessor.right_vertices[-1, :])))
@@ -386,15 +395,16 @@
         if pred_straight and suc_straight and same_length_width:
             trans = predecessor.center_vertices[0] - successor.center_vertices[-1]
             predecessor.translate_rotate(trans, 0)
         else:
             trans = successor.center_vertices[0] - predecessor.center_vertices[-1]
             predecessor.translate_rotate(trans, 0)
 
-        if not suc_straight and (np.round(predecessor.left_vertices[-1], 5) != np.round(successor.left_vertices[0], 5)).any() and same_length_width:
+        if not suc_straight and (np.round(predecessor.left_vertices[-1], 5) !=
+                                 np.round(successor.left_vertices[0], 5)).any() and same_length_width:
             ang *= -2
             predecessor.translate_rotate(np.array([0, 0]), ang)
             trans = successor.center_vertices[0] - predecessor.center_vertices[-1]
             predecessor.translate_rotate(trans, 0)
 
         MapCreator.set_predecessor_successor_relation(predecessor, successor)
 
@@ -648,34 +658,38 @@
                                        TrafficLightCycleElement(TrafficLightState.YELLOW, 30),
                                        TrafficLightCycleElement(TrafficLightState.RED, 100),
                                        TrafficLightCycleElement(TrafficLightState.RED_YELLOW, 30)]
             traffic_light_cycle_two = [TrafficLightCycleElement(TrafficLightState.RED, 100),
                                        TrafficLightCycleElement(TrafficLightState.RED_YELLOW, 30),
                                        TrafficLightCycleElement(TrafficLightState.GREEN, 100),
                                        TrafficLightCycleElement(TrafficLightState.YELLOW, 30)]
-            traffic_light_one = TrafficLight(scenario.generate_object_id(), traffic_light_cycle_one,
-                                             new_lanelets[0].right_vertices[-1] + np.array([-1, -2]))
+            traffic_light_one = TrafficLight(scenario.generate_object_id(),
+                                             new_lanelets[0].right_vertices[-1] + np.array([-1, -2]),
+                                             TrafficLightCycle(traffic_light_cycle_one))
             new_traffic_lights.append(traffic_light_one)
             new_lanelets[0].add_traffic_light_to_lanelet(traffic_light_one.traffic_light_id)
             light_ids[0] = {traffic_light_one.traffic_light_id}
 
-            traffic_light_two = TrafficLight(scenario.generate_object_id(), traffic_light_cycle_one,
-                                             new_lanelets[9].right_vertices[-1] + np.array([1, 2]))
+            traffic_light_two = TrafficLight(scenario.generate_object_id(),
+                                             new_lanelets[9].right_vertices[-1] + np.array([1, 2]),
+                                             TrafficLightCycle(traffic_light_cycle_one))
             new_traffic_lights.append(traffic_light_two)
             new_lanelets[9].add_traffic_light_to_lanelet(traffic_light_two.traffic_light_id)
             light_ids[1] = {traffic_light_two.traffic_light_id}
 
-            traffic_light_three = TrafficLight(scenario.generate_object_id(), traffic_light_cycle_two,
-                                               new_lanelets[15].right_vertices[-1] + np.array([2, -2]))
+            traffic_light_three = TrafficLight(scenario.generate_object_id(),
+                                               new_lanelets[15].right_vertices[-1] + np.array([2, -2]),
+                                               TrafficLightCycle(traffic_light_cycle_two))
             new_traffic_lights.append(traffic_light_three)
             new_lanelets[15].add_traffic_light_to_lanelet(traffic_light_three.traffic_light_id)
             light_ids[2] = {traffic_light_three.traffic_light_id}
 
-            traffic_light_four = TrafficLight(scenario.generate_object_id(), traffic_light_cycle_two,
-                                              new_lanelets[7].right_vertices[-1] + np.array([-2, 2]))
+            traffic_light_four = TrafficLight(scenario.generate_object_id(),
+                                              new_lanelets[7].right_vertices[-1] + np.array([-2, 2]),
+                                              TrafficLightCycle(traffic_light_cycle_two))
             new_traffic_lights.append(traffic_light_four)
             new_lanelets[7].add_traffic_light_to_lanelet(traffic_light_four.traffic_light_id)
             light_ids[3] = {traffic_light_four.traffic_light_id}
 
         if add_traffic_lights or add_traffic_signs:
             for ref, la_idx in enumerate([0, 9, 15, 7]):
                 new_lanelets[la_idx].stop_line = StopLine(new_lanelets[la_idx].right_vertices[-1],
@@ -710,70 +724,76 @@
         new_lanelets = []
         rad = (diameter_crossing + width) / 2
         lanelet_ids = [scenario.generate_object_id() for i in range(0, 12)]
         new_lanelets.append(MapCreator.create_straight(width, incoming_length, 10, lanelet_ids[0],
                                                        {LaneletType.UNKNOWN}, road_user_one_way={RoadUser.VEHICLE},
                                                        line_marking_left=LineMarking.DASHED,
                                                        line_marking_right=LineMarking.SOLID))
-        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[0], lanelet_ids[1], False, width,
+        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[0], lanelet_ids[1],
+                                                               False, width,
                                                                {LaneletType.UNKNOWN},
                                                                road_user_one_way={RoadUser.VEHICLE},
                                                                line_marking_left=LineMarking.DASHED,
                                                                line_marking_right=LineMarking.SOLID))
 
         new_lanelets.append(MapCreator.create_curve(width, rad, np.pi * 0.5, 20, lanelet_ids[2],
                                                     {LaneletType.INTERSECTION}, road_user_one_way={RoadUser.VEHICLE},
                                                     line_marking_left=LineMarking.NO_MARKING,
                                                     line_marking_right=LineMarking.NO_MARKING))
         MapCreator.fit_to_predecessor(new_lanelets[0], new_lanelets[2], True)
-        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[2], lanelet_ids[3], False, width,
+        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[2], lanelet_ids[3],
+                                                               False, width,
                                                                {LaneletType.INTERSECTION},
                                                                road_user_one_way={RoadUser.VEHICLE},
                                                                line_marking_left=LineMarking.NO_MARKING,
                                                                line_marking_right=LineMarking.SOLID))
 
         new_lanelets.append(MapCreator.create_straight(width, incoming_length, 10, lanelet_ids[4],
                                                        {LaneletType.UNKNOWN}, road_user_one_way={RoadUser.VEHICLE},
                                                        line_marking_left=LineMarking.DASHED,
                                                        line_marking_right=LineMarking.SOLID))
         MapCreator.fit_to_predecessor(new_lanelets[2], new_lanelets[4], True)
-        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[4], lanelet_ids[5], False, width,
+        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[4], lanelet_ids[5],
+                                                               False, width,
                                                                {LaneletType.UNKNOWN},
                                                                road_user_one_way={RoadUser.VEHICLE},
                                                                line_marking_left=LineMarking.DASHED,
                                                                line_marking_right=LineMarking.SOLID))
 
         new_lanelets.append(MapCreator.create_straight(width, diameter_crossing, 10, lanelet_ids[6],
                                                        {LaneletType.INTERSECTION}, road_user_one_way={RoadUser.VEHICLE},
                                                        line_marking_left=LineMarking.DASHED,
                                                        line_marking_right=LineMarking.NO_MARKING))
         MapCreator.fit_to_predecessor(new_lanelets[5], new_lanelets[6], True)
-        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[6], lanelet_ids[7], False, width,
+        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[6], lanelet_ids[7],
+                                                               False, width,
                                                                {LaneletType.INTERSECTION},
                                                                road_user_one_way={RoadUser.VEHICLE},
                                                                line_marking_left=LineMarking.DASHED,
                                                                line_marking_right=LineMarking.SOLID))
 
         new_lanelets.append(MapCreator.create_straight(width, incoming_length, 10, lanelet_ids[8],
                                                        {LaneletType.UNKNOWN}, road_user_one_way={RoadUser.VEHICLE},
                                                        line_marking_left=LineMarking.DASHED,
                                                        line_marking_right=LineMarking.SOLID))
         MapCreator.fit_to_predecessor(new_lanelets[6], new_lanelets[8], True)
-        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[8], lanelet_ids[9], False, width,
+        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[8], lanelet_ids[9],
+                                                               False, width,
                                                                {LaneletType.UNKNOWN},
                                                                road_user_one_way={RoadUser.VEHICLE},
                                                                line_marking_left=LineMarking.DASHED,
                                                                line_marking_right=LineMarking.SOLID))
 
         new_lanelets.append(MapCreator.create_curve(width, rad, np.pi * 0.5, 20, lanelet_ids[10],
                                                     {LaneletType.INTERSECTION}, road_user_one_way={RoadUser.VEHICLE},
                                                     line_marking_left=LineMarking.NO_MARKING,
                                                     line_marking_right=LineMarking.NO_MARKING))
         MapCreator.fit_to_predecessor(new_lanelets[9], new_lanelets[10], True)
-        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[10], lanelet_ids[11], False, width,
+        new_lanelets.append(MapCreator.create_adjacent_lanelet(True, new_lanelets[10], lanelet_ids[11]
+                                                               , False, width,
                                                                {LaneletType.INTERSECTION},
                                                                road_user_one_way={RoadUser.VEHICLE},
                                                                line_marking_left=LineMarking.NO_MARKING,
                                                                line_marking_right=LineMarking.SOLID))
 
         # missing dependencies
         MapCreator.set_predecessor_successor_relation(new_lanelets[0], new_lanelets[11])
@@ -836,28 +856,31 @@
                                        TrafficLightCycleElement(TrafficLightState.YELLOW, 30),
                                        TrafficLightCycleElement(TrafficLightState.RED, 100),
                                        TrafficLightCycleElement(TrafficLightState.RED_YELLOW, 30)]
             traffic_light_cycle_two = [TrafficLightCycleElement(TrafficLightState.RED, 100),
                                        TrafficLightCycleElement(TrafficLightState.RED_YELLOW, 30),
                                        TrafficLightCycleElement(TrafficLightState.GREEN, 100),
                                        TrafficLightCycleElement(TrafficLightState.YELLOW, 30)]
-            traffic_light_one = TrafficLight(scenario.generate_object_id(), traffic_light_cycle_one,
-                                             new_lanelets[5].right_vertices[-1] + np.array([-2, 2]))
+            traffic_light_one = TrafficLight(scenario.generate_object_id(),
+                                             new_lanelets[5].right_vertices[-1] + np.array([-2, 2]),
+                                             TrafficLightCycle(traffic_light_cycle_one))
             new_traffic_lights.append(traffic_light_one)
             new_lanelets[5].add_traffic_light_to_lanelet(traffic_light_one.traffic_light_id)
             light_ids[0] = {traffic_light_one.traffic_light_id}
 
-            traffic_light_two = TrafficLight(scenario.generate_object_id(), traffic_light_cycle_one,
-                                             new_lanelets[9].right_vertices[-1] + np.array([2, -2]))
+            traffic_light_two = TrafficLight(scenario.generate_object_id(),
+                                             new_lanelets[9].right_vertices[-1] + np.array([2, -2]),
+                                             TrafficLightCycle(traffic_light_cycle_one))
             new_traffic_lights.append(traffic_light_two)
             new_lanelets[9].add_traffic_light_to_lanelet(traffic_light_two.traffic_light_id)
             light_ids[1] = {traffic_light_two.traffic_light_id}
 
-            traffic_light_three = TrafficLight(scenario.generate_object_id(), traffic_light_cycle_two,
-                                               new_lanelets[0].right_vertices[-1] + np.array([-1, -2]))
+            traffic_light_three = TrafficLight(scenario.generate_object_id(),
+                                               new_lanelets[0].right_vertices[-1] + np.array([-1, -2]),
+                                               TrafficLightCycle(traffic_light_cycle_two))
             new_traffic_lights.append(traffic_light_three)
             new_lanelets[0].add_traffic_light_to_lanelet(traffic_light_three.traffic_light_id)
             light_ids[2] = {traffic_light_three.traffic_light_id}
 
         if add_traffic_lights or add_traffic_signs:
             for ref, la_idx in enumerate([5, 9, 0]):
                 new_lanelets[la_idx].stop_line = StopLine(new_lanelets[la_idx].right_vertices[-1],
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/osm_settings.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/osm_settings.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/osm_settings_ui.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/osm_settings_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/config_default.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/services/config_default.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/plots_interactive.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/services/plots_interactive.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/waitingspinnerwidget.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/services/waitingspinnerwidget.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/settings.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/settings.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/sumo_settings.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/sumo_settings.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/util.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/service_layer/util.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/create_converter_toolbox.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/create_converter_toolbox.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox_ui.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/create_obstacle_toolbox.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/create_obstacle_toolbox.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox_ui.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/create_road_network_toolbox.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/create_road_network_toolbox.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from PyQt5.QtCore import *
 import math
 
 from commonroad.scenario.lanelet import LineMarking, LaneletType, RoadUser, StopLine, Lanelet
 from commonroad.scenario.intersection import IntersectionIncomingElement, Intersection
 from commonroad.scenario.scenario import Scenario
 from commonroad.scenario.traffic_sign import *
+from commonroad.scenario.traffic_light import TrafficLightDirection, TrafficLightCycle, TrafficLight, TrafficLightCycleElement, TrafficLightState
 
 from crdesigner.ui.gui.mwindow.service_layer.services.waitingspinnerwidget import QtWaitingSpinner
 from crdesigner.ui.gui.mwindow.toolboxes.toolbox_ui import CheckableComboBox
 from crdesigner.ui.gui.mwindow.service_layer.map_creator import MapCreator
 from crdesigner.ui.gui.mwindow.toolboxes.road_network_toolbox.road_network_toolbox_ui import RoadNetworkToolboxUI
 # from crdesigner.ui.gui.mwindow import AnimatedViewerWrapper
 from crdesigner.ui.gui.mwindow.animated_viewer_wrapper.gui_sumo_simulation import SUMO_AVAILABLE
@@ -1448,16 +1449,19 @@
                 traffic_light_cycle.append(TrafficLightCycleElement(TrafficLightState.YELLOW, time_yellow))
             elif elem == "in" and time_inactive > 0:
                 traffic_light_cycle.append(TrafficLightCycleElement(TrafficLightState.INACTIVE, time_inactive))
 
         if traffic_light_id is None:
             traffic_light_id = self.current_scenario.generate_object_id()
 
-        new_traffic_light = TrafficLight(traffic_light_id, traffic_light_cycle, np.array([x_position, y_position]),
-                                         time_offset, traffic_light_direction, traffic_light_active)
+        new_traffic_light = TrafficLight(traffic_light_id, np.array([x_position, y_position]),
+                                         TrafficLightCycle(traffic_light_cycle, time_offset=time_offset,
+                                                           active=traffic_light_active),
+                                         direction=traffic_light_direction, active=traffic_light_active)
+
 
         self.current_scenario.add_objects(new_traffic_light, referenced_lanelets)
         self.set_default_road_network_list_information()
         self.callback(self.current_scenario)
 
     def remove_traffic_light(self):
         """
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox_ui.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from PyQt5.QtWidgets import *
 import math
 
 from crdesigner.ui.gui.mwindow.service_layer.services.waitingspinnerwidget import QtWaitingSpinner
 from crdesigner.ui.gui.mwindow.toolboxes.toolbox_ui import Toolbox, CheckableComboBox, CollapsibleArrowBox, CollapsibleCheckBox, PositionButton
 
 from commonroad.scenario.lanelet import LaneletType, RoadUser, LineMarking
-from commonroad.scenario.traffic_sign import *
+from commonroad.scenario.traffic_light import TrafficLightDirection
 
 
 class RoadNetworkToolboxUI(Toolbox):
     """a dialog to which collapsible sections can be added;
     reimplement define_sections() to define sections and
     add them as (title, widget) tuples to self.sections
         """
```

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/toolbox_ui.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/toolboxes/toolbox_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/menu_bar_wrapper.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/menu_bar_wrapper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/file_actions.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/file_actions.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/general_services.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/general_services.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/setting_actions.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/setting_actions.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/toolbar_wrapper.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/toolbar_wrapper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/top_bar_wrapper.py` & `commonroad_scenario_designer-0.7.2/crdesigner/ui/gui/mwindow/top_bar_wrapper/top_bar_wrapper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.1/pyproject.toml` & `commonroad_scenario_designer-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "commonroad-scenario-designer"
-version = "0.7.1"
+version = "0.7.2"
 description = "Toolbox for Map Conversion and Scenario Creation for Autonomous Vehicles"
 authors = ["Cyber-Physical Systems Group, Technical University of Munich <commonroad@lists.lrz.de>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 keywords= ["autonomous", "automated", "vehicles", "driving", "motion", "planning", "simulation", "map", "scenario"]
 classifiers = [
     "Programming Language :: Python :: 3.8",
@@ -22,24 +22,24 @@
 [tool.poetry.urls]
 Documentation = "https://commonroad-scenario-designer.readthedocs.io/en/latest/"
 Forum = "https://commonroad.in.tum.de/forum/c/scenario-designer/"
 Source = "https://gitlab.lrz.de/tum-cps/commonroad-scenario-designer"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-commonroad-io = "2023.1"
+commonroad-io = "2023.2"
 pyqt5 = ">=5.15.9"
 matplotlib = ">=3.6.0"
 numpy = "^1.24.2"
 lxml = "^4.9.2"
 pyproj = "^3.4.1"
 utm = "^0.7.0"
 shapely = ">=2.0.1"
 ordered-set = "^4.1.0"
-sumocr = "2023.1"
+sumocr = "2023.2"
 iso3166 = "^2.1.1"
 networkx = "^3.0"
 omegaconf = "^2.3.0"
 pyyaml = "6.0"
 pygeodesy = "^23.3.23"
 mercantile = "^1.2.1"
 urllib3 = "^2.0.3"
```

### Comparing `commonroad_scenario_designer-0.7.1/PKG-INFO` & `commonroad_scenario_designer-0.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonroad-scenario-designer
-Version: 0.7.1
+Version: 0.7.2
 Summary: Toolbox for Map Conversion and Scenario Creation for Autonomous Vehicles
 Home-page: https://commonroad.in.tum.de
 License: GPL-3.0-or-later
 Keywords: autonomous,automated,vehicles,driving,motion,planning,simulation,map,scenario
 Author: Cyber-Physical Systems Group, Technical University of Munich
 Author-email: commonroad@lists.lrz.de
 Requires-Python: >=3.8,<4.0
@@ -13,40 +13,37 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: commonroad-io (==2023.1)
+Requires-Dist: commonroad-io (==2023.2)
 Requires-Dist: iso3166 (>=2.1.1,<3.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: matplotlib (>=3.6.0)
 Requires-Dist: mercantile (>=1.2.1,<2.0.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
 Requires-Dist: pygeodesy (>=23.3.23,<24.0.0)
 Requires-Dist: pyproj (>=3.4.1,<4.0.0)
 Requires-Dist: pyqt5 (>=5.15.9)
 Requires-Dist: pyyaml (==6.0)
 Requires-Dist: shapely (>=2.0.1)
-Requires-Dist: sumocr (==2023.1)
+Requires-Dist: sumocr (==2023.2)
 Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Requires-Dist: utm (>=0.7.0,<0.8.0)
 Project-URL: Documentation, https://commonroad-scenario-designer.readthedocs.io/en/latest/
 Project-URL: Forum, https://commonroad.in.tum.de/forum/c/scenario-designer/
 Project-URL: Source, https://gitlab.lrz.de/tum-cps/commonroad-scenario-designer
 Description-Content-Type: text/markdown
 
 # CommonRoad Scenario Designer
-[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
-[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
-[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)  
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)  
 [![PyPI version fury.io](https://badge.fury.io/py/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)
 [![PyPI download week](https://img.shields.io/pypi/dw/commonroad-scenario-designer.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-scenario-designer/) 
 [![PyPI download month](https://img.shields.io/pypi/dm/commonroad-scenario-designer.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-scenario-designer/)  
 [![PyPI license](https://img.shields.io/pypi/l/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)
 
 This toolbox provides map converters for [OpenStreetMap](https://www.openstreetmap.de/karte.html) (OSM), 
@@ -184,19 +181,19 @@
 
 ## Bug and feature reporting
 This release (v0.7.1) is still a BETA version.  
 In case you detect a bug or you want to suggest a new feature, please report it in our [forum](https://commonroad.in.tum.de/forum/c/scenario-designer/18).   
 If you want to contribute to the toolbox, you can also post it in the [forum](https://commonroad.in.tum.de/forum/c/scenario-designer/18) or contact [Sebastian Maierhofer](sebastian.maierhofer@tum.de).
 
 ## Authors
-
-Responsible: Sebastian Maierhofer, Sebastian Mair
-Contribution (in alphabetic order by last name): Daniel Asch, Hamza Begic, Florian Braunmiller, Tim Dang, 
-Behtarin Ferdousi, Maximilian Fruehauf, Marcus Gabler, Fabian Hoeltke, Aaron Kaefer, David Le, Gustaf Lindgren, 
-Sarra Ben Mohamed, Benjamin Orthen, Luisa Ortner, Louis Pröbstle, Benedikt Reinhard, Maximilian Rieger, Til Stotz, Stefan Urban
+Responsible: Sebastian Maierhofer, Sebastian Mair  
+Contribution (in alphabetic order by last name): Daniel Asch, Hamza Begic, Mohamed Bouhali, Florian Braunmiller, 
+Tim Dang, Behtarin Ferdousi, Maximilian Fruehauf, Marcus Gabler, Fabian Hoeltke, Tom Irion, Aaron Kaefer, Anton Kluge, 
+David Le, Gustaf Lindgren, Sarra Ben Mohamed, Benjamin Orthen, Luisa Ortner, Louis Pröbstle, Benedikt Reinhard, 
+Maximilian Rieger, Til Stotz, Stefan Urban, Max Winklhofer
 
 ## Credits
 We gratefully acknowledge partial financial support by
 - DFG (German Research Fundation) Priority Program SPP 1835 Cooperative Interacting Automobiles
 - BMW Group within the Car@TUM project
 - Central Innovation Programme of the German Federal Government under grant no. ZF4086007BZ8
```

