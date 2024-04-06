# Comparing `tmp/hgraph-0.2.6.tar.gz` & `tmp/hgraph-0.2.7.tar.gz`

## Comparing `hgraph-0.2.6.tar` & `hgraph-0.2.7.tar`

### file list

```diff
@@ -1,275 +1,276 @@
--rw-r--r--   0        0        0     7750 2020-02-02 00:00:00.000000 hgraph-0.2.6/CHANGELOG.md
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 hgraph-0.2.6/ROADMAP.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hgraph-0.2.6/.github/dependabot.yml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 hgraph-0.2.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hgraph-0.2.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 hgraph-0.2.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/index.md
--rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/concepts/evaluation_clock_uml.png
--rw-r--r--   0        0        0    15820 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/concepts/evaluation_engine_api.png
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/concepts/forward_propagation_graph.md
--rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/concepts/graph_executor_uml.png
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/concepts/graph_runtime.md
--rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/concepts/graph_uml.png
--rw-r--r--   0        0        0    10793 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/concepts/node_uml.png
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/concepts/run_mode_uml.png
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/concepts/services.md
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/concepts/src_cmpt_snk_diagram.png
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/python/component_signature.md
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/python/hg_types.md
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/python/node_signature.md
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/python/program_anatomy.md
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/python/schema_based_types.md
--rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/python/what_is_1_1.png
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/exception_handling.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/exception_handling.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/feedback.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/feedback.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/generics.md
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/generics.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/graphs_and_nodes.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/graphs_and_nodes.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/hello_world.md
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/hello_world.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/injectable_attributes.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/injectable_attributes.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/life_cycle.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/life_cycle.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/map_reduce_switch.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/map_reduce_switch.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/node_testing.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/node_testing.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/push_source_node.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/push_source_node.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 hgraph-0.2.6/docs/quick_start/quick_start.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/examples/monitoring/__init__.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 hgraph-0.2.6/examples/monitoring/monitoring.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/examples/monitoring/phase_1/__init__.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hgraph-0.2.6/examples/monitoring/phase_1/monitoring_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/examples/web_api/__init__.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 hgraph-0.2.6/examples/web_api/web_api.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/__about__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_builder/__init__.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_builder/_builder.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_builder/_graph_builder.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_builder/_input_builder.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_builder/_node_builder.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_builder/_output_builder.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_builder/_scalar_builder.py
--rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_builder/_ts_builder.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/__init__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_impl_configuration.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/graph_construction.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_builder/__init__.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_builder/_graph_builder.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_builder/_map_builder.py
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_builder/_node_builder.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_builder/_node_impl_builder.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_builder/_reduce_builder.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_builder/_service_impl_builder.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_builder/_switch_builder.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_builder/_try_except_builder.py
--rw-r--r--   0        0        0    13563 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_builder/_ts_builder.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_common.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_data_writer.py
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_evaluation_clock.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_evaluation_engine.py
--rw-r--r--   0        0        0     8030 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_graph.py
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_graph_executor.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_graph_recorder.py
--rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_map_node.py
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py
--rw-r--r--   0        0        0    18927 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_node.py
--rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_reduce_node.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_service_node_impl.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_switch_node.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_runtime/_try_except_node.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/_feature_extension.py
--rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/_input.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/_output.py
--rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/_ref.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/_scalar_value.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/_signal.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/_ts.py
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/_tsb.py
--rw-r--r--   0        0        0    11866 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/_tsd.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/_tsl.py
--rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_impl/_types/_tss.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_constants.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_data_writer.py
--rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_evaluation_clock.py
--rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_evaluation_engine.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_feedback.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_global_state.py
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_graph.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_graph_executor.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_graph_recorder.py
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_graph_runner.py
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_lifecycle.py
--rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_node.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_runtime/_operators.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/__init__.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_error_type.py
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_frame_scalar_type_meta_data.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_ref_meta_data.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_ref_type.py
--rw-r--r--   0        0        0    35935 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_scalar_type_meta_data.py
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_scalar_types.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_scalar_value.py
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_schema_type.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_time_series_meta_data.py
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_time_series_types.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_ts_meta_data.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_ts_signal_meta_data.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_ts_type.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_ts_type_var_meta_data.py
--rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_tsb_meta_data.py
--rw-r--r--   0        0        0    12398 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_tsb_type.py
--rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_tsd_meta_data.py
--rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_tsd_type.py
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_tsl_meta_data.py
--rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_tsl_type.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_tss_meta_data.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_tss_type.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_type_meta_data.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_types/_typing_utils.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/__init__.py
--rw-r--r--   0        0        0    19388 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_decorators.py
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_dispatch.py
--rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_exception_handling.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_graph_builder.py
--rw-r--r--   0        0        0    28010 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_map.py
--rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_reduce.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_source_code_details.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_stub_wiring_node.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_switch.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_context.py
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_errors.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_instance.py
--rw-r--r--   0        0        0    16810 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_signature.py
--rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_port.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_utils.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/__init__.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_req_repl_service_node_service.py
--rw-r--r--   0        0        0    13838 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_service_interface_node_class.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_subscription_service_node_service.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py
--rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/__init__.py
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_analytical.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_compound_scalar_operators.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_conditional.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_const.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_data_source_polars.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_datetime_operators.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_drop_dups.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_format.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_frame_operators.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_graph.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_logical.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_math.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_null_sink.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_numpy.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_operators.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_pass_through.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_print.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_record.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_replay.py
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_service_utils.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_set_operators.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_stream_operators.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_tsb_operators.py
--rw-r--r--   0        0        0    12819 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_tsd_operators.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_tsl_operators.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_tss_operators.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_tuple_operators.py
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/nodes/_window_operators.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/test/__init__.py
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/test/_node_printer.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/test/_node_unit_tester.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 hgraph-0.2.6/src/hgraph/test/testing.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/test_wiring.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_impl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_impl/_builder/__init__.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_impl/_runtime/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_impl/_runtime/test_node_impl.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_runtime/__init__.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_runtime/test_feedback.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_runtime/test_scheduler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_types/__init__.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_types/test_complex_types.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_types/test_operator_rank.py
--rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_types/test_type_meta_data.py
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_types/test_type_meta_resolve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/__init__.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_auto_const.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_auto_resolve.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_decorators.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_dispatch.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_error_handling.py
--rw-r--r--   0        0        0    14626 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_map.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_overloads.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_ref.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_service.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_switch.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_ts_wiring.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_tss.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/__init__.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_analytical.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_conditional.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_const.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_data_source_polars.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_drop_dups.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_format.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_frame.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_logical.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_math.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_numpy.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_operators.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_print.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_push_queue.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_recorder.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_replay.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_stream_operators.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_tsb_operators.py
--rw-r--r--   0        0        0     5531 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_tsd_operators.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_tsl_operators.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_tss_operators.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_window_operators.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_wp_operators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/test/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/test/test_eval_node.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 hgraph-0.2.6/tests/python/unit/hgraph/test/test_node_printer.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 hgraph-0.2.6/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hgraph-0.2.6/LICENSE
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 hgraph-0.2.6/README.md
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 hgraph-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 hgraph-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 hgraph-0.2.7/CHANGELOG.md
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 hgraph-0.2.7/ROADMAP.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hgraph-0.2.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 hgraph-0.2.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hgraph-0.2.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 hgraph-0.2.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/index.md
+-rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/evaluation_clock_uml.png
+-rw-r--r--   0        0        0    15820 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/evaluation_engine_api.png
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/forward_propagation_graph.md
+-rw-r--r--   0        0        0     8774 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/graph_executor_uml.png
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/graph_runtime.md
+-rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/graph_uml.png
+-rw-r--r--   0        0        0    10793 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/node_uml.png
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/run_mode_uml.png
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/services.md
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/concepts/src_cmpt_snk_diagram.png
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/component_signature.md
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/hg_types.md
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/node_signature.md
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/program_anatomy.md
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/schema_based_types.md
+-rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/python/what_is_1_1.png
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/exception_handling.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/exception_handling.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/feedback.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/feedback.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/generics.md
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/generics.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/graphs_and_nodes.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/graphs_and_nodes.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/hello_world.md
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/hello_world.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/injectable_attributes.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/injectable_attributes.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/life_cycle.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/life_cycle.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/map_reduce_switch.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/map_reduce_switch.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/node_testing.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/node_testing.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/push_source_node.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/push_source_node.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 hgraph-0.2.7/docs/quick_start/quick_start.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/monitoring/__init__.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/monitoring/monitoring.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/monitoring/phase_1/__init__.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/monitoring/phase_1/monitoring_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/web_api/__init__.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 hgraph-0.2.7/examples/web_api/web_api.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/__about__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/__init__.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_builder.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_graph_builder.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_input_builder.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_node_builder.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_output_builder.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_scalar_builder.py
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_builder/_ts_builder.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/__init__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_impl_configuration.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/graph_construction.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/__init__.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_graph_builder.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_map_builder.py
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_node_builder.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_node_impl_builder.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_reduce_builder.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_service_impl_builder.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_switch_builder.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_try_except_builder.py
+-rw-r--r--   0        0        0    13563 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_builder/_ts_builder.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_common.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_data_writer.py
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_evaluation_clock.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_evaluation_engine.py
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph_executor.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph_recorder.py
+-rw-r--r--   0        0        0     7503 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_map_node.py
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py
+-rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_node.py
+-rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_reduce_node.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_service_node_impl.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_switch_node.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_runtime/_try_except_node.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_feature_extension.py
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_input.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_output.py
+-rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_ref.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_scalar_value.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_signal.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_ts.py
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_tsb.py
+-rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_tsd.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_tsl.py
+-rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_impl/_types/_tss.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_constants.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_data_writer.py
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_evaluation_clock.py
+-rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_evaluation_engine.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_feedback.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_global_state.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_graph.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_graph_executor.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_graph_recorder.py
+-rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_graph_runner.py
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_lifecycle.py
+-rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_node.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_runtime/_operators.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/__init__.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_error_type.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_frame_scalar_type_meta_data.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ref_meta_data.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ref_type.py
+-rw-r--r--   0        0        0    35935 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_scalar_type_meta_data.py
+-rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_scalar_types.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_scalar_value.py
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_schema_type.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_time_series_meta_data.py
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_time_series_types.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ts_meta_data.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ts_signal_meta_data.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ts_type.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_ts_type_var_meta_data.py
+-rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsb_meta_data.py
+-rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsb_type.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsd_meta_data.py
+-rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsd_type.py
+-rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsl_meta_data.py
+-rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tsl_type.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tss_meta_data.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_tss_type.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_type_meta_data.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_types/_typing_utils.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/__init__.py
+-rw-r--r--   0        0        0    19268 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_decorators.py
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_dispatch.py
+-rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_exception_handling.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_graph_builder.py
+-rw-r--r--   0        0        0    28010 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_map.py
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_reduce.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_source_code_details.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_stub_wiring_node.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_switch.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_context.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_errors.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_instance.py
+-rw-r--r--   0        0        0    16810 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_signature.py
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_port.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_utils.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/__init__.py
+-rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_req_repl_service_node_service.py
+-rw-r--r--   0        0        0    15633 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_service_interface_node_class.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_subscription_service_node_service.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py
+-rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/__init__.py
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_analytical.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_compound_scalar_operators.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_conditional.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_const.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_data_source_polars.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_datetime_operators.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_drop_dups.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_format.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_frame_operators.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_graph.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_logical.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_math.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_null_sink.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_numpy.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_operators.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_pass_through.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_print.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_record.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_replay.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_service_utils.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_set_operators.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_stream_operators.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_tsb_operators.py
+-rw-r--r--   0        0        0    14011 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_tsd_operators.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_tsl_operators.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_tss_operators.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_tuple_operators.py
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/nodes/_window_operators.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/test/__init__.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/test/_node_printer.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/test/_node_unit_tester.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 hgraph-0.2.7/src/hgraph/test/testing.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/test_wiring.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_builder/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/test_node_impl.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_runtime/__init__.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_runtime/test_feedback.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_runtime/test_scheduler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_types/__init__.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_types/test_complex_types.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_types/test_operator_rank.py
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_types/test_type_meta_data.py
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_types/test_type_meta_resolve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/__init__.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_auto_const.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_auto_resolve.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_decorators.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_dispatch.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_error_handling.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_generic_graphs.py
+-rw-r--r--   0        0        0    14626 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_map.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_overloads.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_ref.py
+-rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_service.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_switch.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_ts_wiring.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tss.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/__init__.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_analytical.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_conditional.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_const.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_data_source_polars.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_drop_dups.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_format.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_frame.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_logical.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_math.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_numpy.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_operators.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_print.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_push_queue.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_recorder.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_replay.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_stream_operators.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsb_operators.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsd_operators.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsl_operators.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tss_operators.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_window_operators.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_wp_operators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/test/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/test/test_eval_node.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 hgraph-0.2.7/tests/python/unit/hgraph/test/test_node_printer.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 hgraph-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hgraph-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 hgraph-0.2.7/README.md
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 hgraph-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 hgraph-0.2.7/PKG-INFO
```

### Comparing `hgraph-0.2.6/CHANGELOG.md` & `hgraph-0.2.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -268,7 +268,16 @@
 * Fix min_of_two (from graph to compute_node)
 
 Version 0.2.6 (26-03-2024)
 --------------------------
 
 * Fix timing issue with tsd_rekey
 * Clean up imports and __all__ in nodes
+
+Version 0.2.7 (06-04-2024)
+--------------------------
+
+* Add support for multi-service implementations
+* Support multiple inputs in a request-reply service
+* nested tsd merge
+* constraint type wiring improvements
+
```

### Comparing `hgraph-0.2.6/ROADMAP.md` & `hgraph-0.2.7/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/.github/ISSUE_TEMPLATE/bug_report.md` & `hgraph-0.2.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/.github/ISSUE_TEMPLATE/feature_request.md` & `hgraph-0.2.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/index.md` & `hgraph-0.2.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/concepts/evaluation_clock_uml.png` & `hgraph-0.2.7/docs/concepts/evaluation_clock_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/concepts/evaluation_engine_api.png` & `hgraph-0.2.7/docs/concepts/evaluation_engine_api.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/concepts/forward_propagation_graph.md` & `hgraph-0.2.7/docs/concepts/forward_propagation_graph.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/concepts/graph_executor_uml.png` & `hgraph-0.2.7/docs/concepts/graph_executor_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/concepts/graph_runtime.md` & `hgraph-0.2.7/docs/concepts/graph_runtime.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/concepts/graph_uml.png` & `hgraph-0.2.7/docs/concepts/graph_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/concepts/node_uml.png` & `hgraph-0.2.7/docs/concepts/node_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/concepts/run_mode_uml.png` & `hgraph-0.2.7/docs/concepts/run_mode_uml.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/concepts/services.md` & `hgraph-0.2.7/docs/concepts/services.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/concepts/src_cmpt_snk_diagram.png` & `hgraph-0.2.7/docs/concepts/src_cmpt_snk_diagram.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/python/component_signature.md` & `hgraph-0.2.7/docs/python/component_signature.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/python/hg_types.md` & `hgraph-0.2.7/docs/python/hg_types.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/python/node_signature.md` & `hgraph-0.2.7/docs/python/node_signature.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/python/program_anatomy.md` & `hgraph-0.2.7/docs/python/program_anatomy.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/python/schema_based_types.md` & `hgraph-0.2.7/docs/python/schema_based_types.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/python/what_is_1_1.png` & `hgraph-0.2.7/docs/python/what_is_1_1.png`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/exception_handling.md` & `hgraph-0.2.7/docs/quick_start/exception_handling.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/exception_handling.py` & `hgraph-0.2.7/docs/quick_start/exception_handling.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/feedback.md` & `hgraph-0.2.7/docs/quick_start/feedback.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/generics.md` & `hgraph-0.2.7/docs/quick_start/generics.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/generics.py` & `hgraph-0.2.7/docs/quick_start/generics.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/graphs_and_nodes.md` & `hgraph-0.2.7/docs/quick_start/graphs_and_nodes.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/graphs_and_nodes.py` & `hgraph-0.2.7/docs/quick_start/graphs_and_nodes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/hello_world.md` & `hgraph-0.2.7/docs/quick_start/hello_world.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/injectable_attributes.md` & `hgraph-0.2.7/docs/quick_start/injectable_attributes.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/injectable_attributes.py` & `hgraph-0.2.7/docs/quick_start/injectable_attributes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/life_cycle.md` & `hgraph-0.2.7/docs/quick_start/life_cycle.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/map_reduce_switch.md` & `hgraph-0.2.7/docs/quick_start/map_reduce_switch.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/map_reduce_switch.py` & `hgraph-0.2.7/docs/quick_start/map_reduce_switch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/node_testing.md` & `hgraph-0.2.7/docs/quick_start/node_testing.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/push_source_node.md` & `hgraph-0.2.7/docs/quick_start/push_source_node.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/push_source_node.py` & `hgraph-0.2.7/docs/quick_start/push_source_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/docs/quick_start/quick_start.md` & `hgraph-0.2.7/docs/quick_start/quick_start.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/examples/monitoring/monitoring.md` & `hgraph-0.2.7/examples/monitoring/monitoring.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/examples/monitoring/phase_1/monitoring_api.py` & `hgraph-0.2.7/examples/monitoring/phase_1/monitoring_api.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/examples/web_api/web_api.py` & `hgraph-0.2.7/examples/web_api/web_api.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_builder/_builder.py` & `hgraph-0.2.7/src/hgraph/_builder/_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_builder/_graph_builder.py` & `hgraph-0.2.7/src/hgraph/_builder/_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_builder/_input_builder.py` & `hgraph-0.2.7/src/hgraph/_builder/_input_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_builder/_node_builder.py` & `hgraph-0.2.7/src/hgraph/_builder/_node_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_builder/_output_builder.py` & `hgraph-0.2.7/src/hgraph/_builder/_output_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_builder/_ts_builder.py` & `hgraph-0.2.7/src/hgraph/_builder/_ts_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/graph_construction.md` & `hgraph-0.2.7/src/hgraph/_impl/graph_construction.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_builder/_graph_builder.py` & `hgraph-0.2.7/src/hgraph/_impl/_builder/_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_builder/_map_builder.py` & `hgraph-0.2.7/src/hgraph/_impl/_builder/_map_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_builder/_node_builder.py` & `hgraph-0.2.7/src/hgraph/_impl/_builder/_node_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_builder/_node_impl_builder.py` & `hgraph-0.2.7/src/hgraph/_impl/_builder/_node_impl_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_builder/_reduce_builder.py` & `hgraph-0.2.7/src/hgraph/_impl/_builder/_reduce_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_builder/_service_impl_builder.py` & `hgraph-0.2.7/src/hgraph/_impl/_builder/_service_impl_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_builder/_switch_builder.py` & `hgraph-0.2.7/src/hgraph/_impl/_builder/_switch_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_builder/_try_except_builder.py` & `hgraph-0.2.7/src/hgraph/_impl/_builder/_try_except_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_builder/_ts_builder.py` & `hgraph-0.2.7/src/hgraph/_impl/_builder/_ts_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/__init__.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_common.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_common.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_data_writer.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_data_writer.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_evaluation_clock.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_evaluation_clock.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_evaluation_engine.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_graph.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,20 @@
             for i in range(self.push_source_nodes_end):
                 nodes[i].eval()  # This is only to move nodes on, won't call the before and after node eval here
 
         for i in range(self.push_source_nodes_end, len(nodes)):
             scheduled_time, node = schedule[i], nodes[i]
             if scheduled_time == now:
                 self._evaluation_engine.notify_before_node_evaluation(node)
-                node.eval()
+                from hgraph._types._error_type import NodeException
+                try:
+                    node.eval()
+                except NodeException as e:
+                    raise e
+                except Exception as e:
+                    raise NodeException.capture_error(e, node, 'During evaluation') from e
                 self._evaluation_engine.notify_after_node_evaluation(node)
             elif scheduled_time > now:
                 # If the node has a scheduled time in the future, we need to let the execution context know.
                 clock.update_next_scheduled_evaluation_time(scheduled_time)
 
         self._evaluation_engine.notify_after_graph_evaluation(self)
```

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_graph_executor.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph_executor.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_graph_recorder.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_graph_recorder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_map_node.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_map_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         # 1. All inputs should be reference, and we should only be active on the KEYS_ARG input
         keys: TSS[K] = self._kwargs[KEYS_ARG]
         if keys.modified:
             for k in keys.added():
                 self._create_new_graph(k)
             for k in keys.removed():
                 self._remove_graph(k)
+                self._scheduled_keys.pop(k, None)
         # 2. or one of the nested graphs has been scheduled for evaluation.
         scheduled_keys = self._scheduled_keys
         self._scheduled_keys = {}
         for k, dt in scheduled_keys.items():
             if dt == self.last_evaluation_time:
                 self._evaluate_graph(k)
             elif dt < self.last_evaluation_time:
```

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_nested_evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_node.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,21 +160,15 @@
             try:
                 self.do_eval()
             except Exception as e:
                 out = None
                 from hgraph._types._error_type import NodeError
                 self.error_output.apply_result(NodeError.capture_error(e, self))
         else:
-            from hgraph._types._error_type import NodeException
-            try:
-                self.do_eval()
-            except NodeException as e:
-                raise e
-            except Exception as e:
-                raise NodeException.capture_error(e, self, 'During evaluation') from e
+            self.do_eval()
         if scheduled:
             self._scheduler.advance()
         elif self.scheduler.is_scheduled:
             self.graph.schedule_node(self.node_ndx, self.scheduler.next_scheduled_time)
 
     @abstractmethod
     def do_start(self):
```

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_reduce_node.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_reduce_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_service_node_impl.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_service_node_impl.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_switch_node.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_switch_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_runtime/_try_except_node.py` & `hgraph-0.2.7/src/hgraph/_impl/_runtime/_try_except_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_types/_feature_extension.py` & `hgraph-0.2.7/src/hgraph/_impl/_types/_feature_extension.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_types/_input.py` & `hgraph-0.2.7/src/hgraph/_impl/_types/_input.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_types/_output.py` & `hgraph-0.2.7/src/hgraph/_impl/_types/_output.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_types/_ref.py` & `hgraph-0.2.7/src/hgraph/_impl/_types/_ref.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_types/_scalar_value.py` & `hgraph-0.2.7/src/hgraph/_impl/_types/_scalar_value.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_types/_signal.py` & `hgraph-0.2.7/src/hgraph/_impl/_types/_signal.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_types/_ts.py` & `hgraph-0.2.7/src/hgraph/_impl/_types/_ts.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_types/_tsb.py` & `hgraph-0.2.7/src/hgraph/_impl/_types/_tsb.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_types/_tsd.py` & `hgraph-0.2.7/src/hgraph/_impl/_types/_tsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     def apply_result(self, result: Any):
         if result is None:
             return
         self.value = result
 
     def _create(self, key: K):
         cast(TimeSeriesSetOutput, self.key_set).add(key)
-        self._ts_values[key] = output = self._ts_builder.make_instance(owning_output=self)
+        self._ts_values[key] = self._ts_builder.make_instance(owning_output=self)
         self._ref_ts_feature.update(key)
         for observer in self._key_observers:
             observer.on_key_added(key)
 
     def _clear_key_changes(self):
         self._removed_items = {}
         self._added_keys = set()
```

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_types/_tsl.py` & `hgraph-0.2.7/src/hgraph/_impl/_types/_tsl.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_impl/_types/_tss.py` & `hgraph-0.2.7/src/hgraph/_impl/_types/_tss.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/__init__.py` & `hgraph-0.2.7/src/hgraph/_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_data_writer.py` & `hgraph-0.2.7/src/hgraph/_runtime/_data_writer.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_evaluation_clock.py` & `hgraph-0.2.7/src/hgraph/_runtime/_evaluation_clock.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_evaluation_engine.py` & `hgraph-0.2.7/src/hgraph/_runtime/_evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_feedback.py` & `hgraph-0.2.7/src/hgraph/_runtime/_feedback.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_global_state.py` & `hgraph-0.2.7/src/hgraph/_runtime/_global_state.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_graph.py` & `hgraph-0.2.7/src/hgraph/_runtime/_graph.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_graph_executor.py` & `hgraph-0.2.7/src/hgraph/_runtime/_graph_executor.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_graph_recorder.py` & `hgraph-0.2.7/src/hgraph/_runtime/_graph_recorder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_graph_runner.py` & `hgraph-0.2.7/src/hgraph/_runtime/_graph_runner.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_lifecycle.py` & `hgraph-0.2.7/src/hgraph/_runtime/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_node.py` & `hgraph-0.2.7/src/hgraph/_runtime/_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_runtime/_operators.py` & `hgraph-0.2.7/src/hgraph/_runtime/_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/__init__.py` & `hgraph-0.2.7/src/hgraph/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_error_type.py` & `hgraph-0.2.7/src/hgraph/_types/_error_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_frame_scalar_type_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_frame_scalar_type_meta_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 if tp is None:
                     raise ParseError(f"Could not parse {value_tp.__args__[0]} as type from {value_tp}")
                 return HgDataFrameScalarTypeMetaData(tp)
 
         @classmethod
         def parse_value(cls, value) -> Optional["HgTypeMetaData"]:
             if isinstance(value, pl.DataFrame):
-                return HgDataFrameScalarTypeMetaData(HgScalarTypeVar.parse_type(COMPOUND_SCALAR))
+                return HgDataFrameScalarTypeMetaData(HgScalarTypeMetaData.parse_type(CompoundScalar))
 
         def __eq__(self, o: object) -> bool:
             return type(o) is HgDataFrameScalarTypeMetaData and self.schema == o.schema
 
         def __str__(self) -> str:
             return f'Frame[{str(self.schema)}]'
```

### Comparing `hgraph-0.2.6/src/hgraph/_types/_ref_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_ref_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_ref_type.py` & `hgraph-0.2.7/src/hgraph/_types/_ref_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_scalar_type_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_scalar_type_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_scalar_types.py` & `hgraph-0.2.7/src/hgraph/_types/_scalar_types.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_scalar_value.py` & `hgraph-0.2.7/src/hgraph/_types/_scalar_value.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_schema_type.py` & `hgraph-0.2.7/src/hgraph/_types/_schema_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_time_series_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_time_series_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_time_series_types.py` & `hgraph-0.2.7/src/hgraph/_types/_time_series_types.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_ts_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_ts_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_ts_signal_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_ts_signal_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_ts_type.py` & `hgraph-0.2.7/src/hgraph/_types/_ts_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_ts_type_var_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_ts_type_var_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_tsb_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_tsb_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_tsb_type.py` & `hgraph-0.2.7/src/hgraph/_types/_tsb_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     @classmethod
     def create(cls, **kwargs) -> Type["UnNamedTimeSeriesSchema"]:
         """Creates a type instance with root class UnNamedTimeSeriesSchema using the kwargs provided"""
         from hgraph._types._time_series_meta_data import HgTimeSeriesTypeMetaData
         schema = {k: HgTimeSeriesTypeMetaData.parse_type(v) for k, v in kwargs.items()}
         if any(v is None for v in schema.values()):
-            bad_inputs = {k: v for k, v in kwargs if schema[k] is None}
+            bad_inputs = {k: v for k, v in kwargs.items() if schema[k] is None}
             raise CustomMessageWiringError(f"The following inputs are not valid time-series types: {bad_inputs}")
         return cls.create_resolved_schema(schema)
 
     @classmethod
     def create_resolved_schema(cls, schema: Mapping[str, "HgTimeSeriesTypeMetaData"]) \
             -> Type["UnNamedTimeSeriesSchema"]:
         """Creates a type instance with root class UnNamedTimeSeriesSchema using the schema provided"""
```

### Comparing `hgraph-0.2.6/src/hgraph/_types/_tsd_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_tsd_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_tsd_type.py` & `hgraph-0.2.7/src/hgraph/_types/_tsd_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_tsl_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_tsl_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_tsl_type.py` & `hgraph-0.2.7/src/hgraph/_types/_tsl_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_tss_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_tss_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_tss_type.py` & `hgraph-0.2.7/src/hgraph/_types/_tss_type.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_type_meta_data.py` & `hgraph-0.2.7/src/hgraph/_types/_type_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_types/_typing_utils.py` & `hgraph-0.2.7/src/hgraph/_types/_typing_utils.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/__init__.py` & `hgraph-0.2.7/src/hgraph/_wiring/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_decorators.py` & `hgraph-0.2.7/src/hgraph/_wiring/_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,17 +263,16 @@
     :return:
     """
     from hgraph._wiring._wiring_node_class._service_impl_node_class import ServiceImplNodeClass
     if not isinstance(implementation, ServiceImplNodeClass):
         raise CustomMessageWiringError("The provided implementation is not a 'service_impl' wrapped function.")
 
     from hgraph import WiringGraphContext
-    assert len(implementation.interfaces) == 1, 'mutliservices are not implemented yet'
-    WiringGraphContext.instance().register_service_impl(implementation.interfaces[0], path or '', implementation,
-                                                        kwargs)
+    for i in implementation.interfaces:
+        WiringGraphContext.instance().register_service_impl(i, i.full_path(path), implementation, kwargs)
 
 
 def service_adaptor(interface):
     """
     @service
     def my_interface(ts1: TIME_SERIES, ...) -> OUT_TIME_SERIES:
         pass
```

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_dispatch.py` & `hgraph-0.2.7/src/hgraph/_wiring/_dispatch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_exception_handling.py` & `hgraph-0.2.7/src/hgraph/_wiring/_exception_handling.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_graph_builder.py` & `hgraph-0.2.7/src/hgraph/_wiring/_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_map.py` & `hgraph-0.2.7/src/hgraph/_wiring/_map.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_reduce.py` & `hgraph-0.2.7/src/hgraph/_wiring/_reduce.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_stub_wiring_node.py` & `hgraph-0.2.7/src/hgraph/_wiring/_stub_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_switch.py` & `hgraph-0.2.7/src/hgraph/_wiring/_switch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_context.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_context.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_errors.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,9 +151,10 @@
 class CustomMessageWiringError(WiringError):
     def __init__(self, message: str):
         self.message = message
         self.signature = WIRING_CONTEXT.current_signature
         super().__init__(self.message)
 
     def print_error(self):
-        msg = f"When resolving '{self.signature.signature}' \n{self.message}"
+        signature = self.signature.signature if self.signature else "unnamed graph"
+        msg = f"When resolving '{signature}' \n{self.message}"
         self._print_error(msg)
```

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_instance.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_instance.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_signature.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_signature.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_port.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_port.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,17 @@
             tp = input_wiring_port.output_type
             path = input_wiring_port.path
         return _wiring_port_for(tp, node_instance, path)
 
     def __getitem__(self, item):
         return self._wiring_port_for(item)
 
+    def as_dict(self):
+        return {k: self[k] for k in self.__schema__.__meta_data_schema__.keys()}
+
     def edges_for(self, node_map: Mapping["WiringNodeInstance", int], dst_node_ndx: int,
                   dst_path: tuple[SCALAR, ...]) -> \
             set["Edge"]:
         edges = set()
         if self.has_peer:
             from hgraph._builder._graph_builder import Edge
             edges.add(Edge(node_map[self.node_instance], self.path, dst_node_ndx, dst_path))
```

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_utils.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_utils.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/__init__.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_graph_wiring_node_class.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         If we are wiring the root graph, then there is no wiring node. In this case None is
         passed in.
         """
         self._wiring_node_signature: WiringNodeSignature = node_signature
         self._sink_nodes: ["WiringNodeInstance"] = []
         self._other_nodes: [Tuple["WiringPort", dict]] = []
         self._service_clients: [Tuple["WiringNodeClass", str]] = []
-        self._service_implementations: Dict[Tuple["WiringNodeClass", str], Tuple["ServiceImplNodeClass", dict]] = {}
+        self._service_implementations: Dict[str, Tuple["WiringNodeClass", "ServiceImplNodeClass", dict]] = {}
         self._built_services = {}
 
         self._current_frame = sys._getframe(1)
 
     @property
     def sink_nodes(self) -> tuple["WiringNodeInstance", ...]:
         return tuple(self._sink_nodes)
@@ -112,15 +112,15 @@
             prev_f = f
             i += 1
 
         self._other_nodes.append((node, prev_f.f_locals))
 
     def label_nodes(self):
         """
-        Label the nodes in the graph with the graph name
+        Label the nodes in the graph with the variable name if the output was assigned to a local variable
         """
         for port, locals in self._other_nodes:
             varname = next((k for k, v in locals.items() if v is port), None)
             if varname and port.path == ():
                 port.node_instance.set_label(varname)
 
     def register_service_client(self, service: "ServiceInterfaceNodeClass", path: str):
@@ -129,53 +129,73 @@
         """
         self._service_clients.append((service, path))
 
     def register_service_impl(self, service: "ServiceInterfaceNodeClass", path: str, impl: "ServiceImplNodeClass", kwargs):
         """
         Register a service client with the graph context
         """
-        self._service_implementations[(service, path)] = (impl, kwargs)
+        if prev_impl := self._service_implementations.get(path):
+            CustomMessageWiringError(f"Service implementation already registered for service at path: {path}: "
+                                     f"{prev_impl[0].signature.signature} with {prev_impl[1]}")
+
+        self._service_implementations[path] = (service, impl, kwargs)
+
+    def find_service_impl(self, path):
+        for c in WiringGraphContext.__stack__:
+            if item := c._service_implementations.get(path):
+                return item
+
+        raise CustomMessageWiringError(f"No service implementation found for path: {path}")
 
     def add_built_service_impl(self, path, node):
-        self.add_sink_node(node)
+        if node:
+            self.add_sink_node(node)
+
         self._built_services[path] = node
 
+    def built_services(self):
+        return self._built_services
+
     def build_services(self):
         """
         Build the service implementations for the graph
         """
         service_clients = copy(self._service_clients)
         dependencies = {}
         while True:
-            services_to_build_by_path = {}
+            services_to_build = set()
             for service, path in set(service_clients):
-                if item := self._service_implementations.get((service, path)):
-                    impl, kwargs = item
-                    services_to_build_by_path[path] = (service, impl, kwargs)
+                if item := self._service_implementations.get(path):
+                    interface, impl, kwargs = item
+                    if interface != service:
+                        raise CustomMessageWiringError(f"service implementation for path {path} implements "
+                                                       f"{interface.signature.signature} which does not match the client "
+                                                       f"expecting {service.signature.signature}")
+                    services_to_build.add(path)
                 else:
-                    CustomMessageWiringError(f'No implementation found for service: {service.signature.name} at path: {path}')
+                    raise CustomMessageWiringError(f'No implementation found for service: {service.signature.name} at path: {path}')
 
-            for path, (service, impl, kwargs) in services_to_build_by_path.items():
+            for path in services_to_build:
                 if path not in self._built_services:
                     clients_before = len(self._service_clients)
 
-                    impl, kwargs = self._service_implementations[(service, path)]
-                    impl(path=path, **kwargs)
+                    service, impl, kwargs = self._service_implementations[path]
+                    impl(path=path, __interface__=service, **kwargs)
 
                     new_clients = self._service_clients[clients_before:]
-                    dependencies.update({path: set(p for _, p in new_clients)})
+                    dependencies.update({path: set(p for _, p in new_clients if p != path)})
 
             if self._service_clients == service_clients:
                 break
             else:
                 service_clients = copy(self._service_clients)
 
         ordered = list(TopologicalSorter(dependencies).static_order())
         for i, path in enumerate(ordered):
-            object.__setattr__(self._built_services[path], 'rank', i + 1)
+            object.__setattr__(self._built_services[path], 'rank', i + 2)
 
 
     def __enter__(self):
         WiringGraphContext.__stack__.append(self)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_map_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_node_impl_wiring_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_pull_source_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_python_wiring_node_classes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_reduce_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_reference_service_node_class.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,10 +69,19 @@
             kwargs_, resolved_signature = self._validate_and_resolve_signature(*args,
                                                                                __pre_resolved_types__=__pre_resolved_types__,
                                                                                **kwargs)
 
             port = super().__call__(*args, __pre_resolved_types__=__pre_resolved_types__, **kwargs)
 
             from hgraph import WiringGraphContext
-            WiringGraphContext.instance().register_service_client(self, kwargs_.get("path") or '')
+            WiringGraphContext.instance().register_service_client(self, self.full_path(kwargs_.get("path")))
 
-            return port
+            return port
+
+    def wire_impl_out_stub(self, path, out):
+        from hgraph.nodes import capture_output_to_global_state
+        from hgraph import WiringGraphContext
+
+        full_path = self.full_path(path)
+        capture_output_to_global_state(full_path, out)
+
+        WiringGraphContext.instance().add_built_service_impl(full_path, None)
```

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_req_repl_service_node_service.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_subscription_service_node_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,70 @@
 from typing import Callable, TypeVar
 
 from frozendict import frozendict
 
-from hgraph import HgTypeMetaData, WiringContext, WiringGraphContext
+from hgraph import HgTypeMetaData, WiringContext, WiringGraphContext, TSS, TSB
+from hgraph._types._scalar_types import is_keyable_scalar
+from hgraph._types._ts_meta_data import HgTSTypeMetaData
 from hgraph._wiring._wiring_errors import CustomMessageWiringError
 from hgraph._wiring._wiring_node_class._service_interface_node_class import ServiceInterfaceNodeClass
 from hgraph._wiring._wiring_node_signature import WiringNodeSignature
 
-__all__ = ("RequestReplyServiceNodeClass",)
+__all__ = ("SubscriptionServiceNodeClass",)
 
+from hgraph._wiring._wiring_port import _wiring_port_for
 
-class RequestReplyServiceNodeClass(ServiceInterfaceNodeClass):
+
+class SubscriptionServiceNodeClass(ServiceInterfaceNodeClass):
 
     def __init__(self, signature: WiringNodeSignature, fn: Callable):
         if not signature.defaults.get("path"):
             signature = signature.copy_with(defaults=frozendict(signature.defaults | {"path": None}))
         super().__init__(signature, fn)
         if (l := len(signature.time_series_args)) != 1:
             raise CustomMessageWiringError(f"Expected 1 time-series argument, got {l}")
+        ts_type = signature.input_types[next(iter(signature.time_series_args))]
+        if type(ts_type) is not HgTSTypeMetaData or not is_keyable_scalar(ts_type.value_scalar_tp.py_type):
+            raise CustomMessageWiringError("The subscription property must be a TS[KEYABLE_SCALAR]")
 
     def full_path(self, user_path: str | None) -> str:
         if user_path is None:
             user_path = f"{self.fn.__module__}"
-        return f"reqrepl_svc://{user_path}/{self.fn.__name__}"
+        return f"subs_svc://{user_path}/{self.fn.__name__}"
 
     def __call__(self, *args, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable] = None, **kwargs) -> "WiringPort":
 
         with WiringContext(current_wiring_node=self, current_signature=self.signature):
             kwargs_, resolved_signature = self._validate_and_resolve_signature(*args,
                                                                                __pre_resolved_types__=__pre_resolved_types__,
                                                                                **kwargs)
 
             # But graph nodes are evaluated at wiring time, so this is the graph expansion happening here!
             with WiringGraphContext(self.signature) as g:
-                g.register_service_client(self, kwargs_.get("path") or '')
+                full_path = self.full_path(kwargs_.get("path"))
+                g.register_service_client(self, full_path)
 
-                from hgraph.nodes._service_utils import _request_service
-                from hgraph import TIME_SERIES_TYPE_1
-                return _request_service[TIME_SERIES_TYPE_1: resolved_signature.output_type](path=self.full_path(kwargs_["path"]),
-                                  request=kwargs_[next(iter(resolved_signature.time_series_args))])
+                from hgraph.nodes._service_utils import _subscribe
+                from hgraph import TIME_SERIES_TYPE
+                return _subscribe[TIME_SERIES_TYPE: resolved_signature.output_type](
+                    path=full_path,
+                    key=kwargs_[next(iter(resolved_signature.time_series_args))])
+
+    def wire_impl_inputs_stub(self, path):
+        from hgraph.nodes import capture_output_node_to_global_state
+        from hgraph import last_value_source_node, ts_schema
+
+        full_path = self.full_path(path)
+
+        arg = next(iter(self.signature.time_series_args))
+        subscriptions = last_value_source_node(f"{self.signature.name}_{arg}",
+                                               (tp := TSS[self.signature.input_types[arg].scalar_type().py_type]))
+        subscriptions = _wiring_port_for(tp, subscriptions, tuple())
+        capture_output_node_to_global_state(f"{full_path}_subs", subscriptions)
+
+        WiringGraphContext.instance().add_built_service_impl(full_path, None)
+
+        return TSB[ts_schema(**{arg: HgTypeMetaData.parse_type(tp)})].from_ts(**{arg: subscriptions})
+
+    def wire_impl_out_stub(self, path, out):
+        from hgraph.nodes import capture_output_to_global_state
+        capture_output_to_global_state(f"{self.full_path(path)}_out", out)
```

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_service_impl_node_class.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,46 @@
-from dataclasses import field, dataclass
-from typing import Callable, Mapping, Any, Sequence, TypeVar, Optional, Dict
+from typing import Callable, Mapping, Any, Sequence, TypeVar, Dict
 
 from frozendict import frozendict
 
-from hgraph._types._tsd_meta_data import HgTSDTypeMetaData
-from hgraph._wiring._wiring_node_class._pull_source_node_class import last_value_source_node
-from hgraph._types._tss_meta_data import HgTSSTypeMetaData
+from hgraph import TIME_SERIES_TYPE
 from hgraph._builder._graph_builder import GraphBuilder
 from hgraph._runtime._global_state import GlobalState
 from hgraph._types._scalar_type_meta_data import HgAtomicType, HgObjectType
+from hgraph._types._tss_meta_data import HgTSSTypeMetaData
 from hgraph._types._type_meta_data import HgTypeMetaData
 from hgraph._wiring._graph_builder import create_graph_builder
 from hgraph._wiring._wiring_context import WiringContext
-from hgraph._wiring._wiring_errors import CustomMessageWiringError, WiringError
+from hgraph._wiring._wiring_errors import CustomMessageWiringError
 from hgraph._wiring._wiring_node_class._graph_wiring_node_class import WiringGraphContext
+from hgraph._wiring._wiring_node_class._pull_source_node_class import last_value_source_node
 from hgraph._wiring._wiring_node_class._wiring_node_class import WiringNodeClass, \
     BaseWiringNodeClass
 from hgraph._wiring._wiring_node_instance import create_wiring_node_instance, WiringNodeInstanceContext
 from hgraph._wiring._wiring_node_signature import WiringNodeSignature, WiringNodeType
-
-__all__ = ("ServiceImplNodeClass",)
-
 from hgraph._wiring._wiring_port import _wiring_port_for
 
-from hgraph.nodes._service_utils import capture_output_node_to_global_state
+__all__ = ("ServiceImplNodeClass",)
 
 
 class ServiceImplNodeClass(BaseWiringNodeClass):
 
     def __init__(self, signature: WiringNodeSignature, fn: Callable, interfaces=None):
         # save original inputs
         self._original_signature = signature
         # Add "path" to the scalar signature
         # and remove time-series inputs
         time_series_args = signature.time_series_args
+        has_path = "path" in signature.args
         super().__init__(
             signature.copy_with(
-                args=('path',) + tuple(arg for arg in signature.args if arg not in time_series_args),
+                args=(('path',) if not has_path else ()) + tuple(arg for arg in signature.args if arg not in time_series_args),
 
                 input_types=frozendict(
-                    {k: v for k, v in (signature.input_types | {"path": HgAtomicType.parse_type(str)}).items() if
+                    {k: v for k, v in (signature.input_types | ({"path": HgAtomicType.parse_type(str)} if not has_path else {})).items() if
                      k not in time_series_args}),
                 time_series_args=tuple(),
             ), fn)
         if interfaces is None:
             raise CustomMessageWiringError("No interfaces provided")
 
         if not isinstance(interfaces, (tuple, list, set)):
@@ -60,42 +57,54 @@
             raise CustomMessageWiringError(
                 f"This path: '{path}' has already been registered for this service implementation")
         # Reserve the paths now
         for p in paths:
             gs[p] = self  # use this as a placeholder until we have built the node
 
     def __call__(self, *args, __pre_resolved_types__: dict[TypeVar, HgTypeMetaData | Callable] = None,
+                 __interface__: WiringNodeSignature = None,
                  **kwargs) -> "WiringPort":
 
         with WiringContext(current_wiring_node=self, current_signature=self._original_signature):
             path = kwargs.get("path")
-            self._validate_service_not_already_bound(path)
-            path = "" if path is None else path
+
+            if __interface__ is None:
+                __interface__ = self.interfaces[0]
+
+            if not __interface__.is_full_path(path):
+                full_path = __interface__.full_path(path)
+            else:
+                full_path = path
+                path = __interface__.path_from_full_path(full_path)
+
+            self._validate_service_not_already_bound(full_path)
             kwargs["path"] = path
 
             # TODO: This is only going to resolve scalars or output values, we need to
             # take a look at resolving the actual signature if there are pre-resolved-types.
             kwargs_, resolved_signature = self._validate_and_resolve_signature(
                 *args,
                 __pre_resolved_types__=__pre_resolved_types__,
                 **kwargs)
 
             resolved_signature = resolved_signature.copy_with(input_types=frozendict({
                         **resolved_signature.input_types,
                         'inner_graph': HgObjectType.parse_type(object)}))
 
             with WiringContext(current_wiring_node=self, current_signature=self.signature):
-                inner_graph = create_inner_graph(self._original_signature, self.fn, kwargs_, self.interfaces)
+                inner_graph, paths = create_inner_graph(self._original_signature, self.fn, kwargs_, self.interfaces)
                 kwargs_['inner_graph'] = inner_graph
 
             # We pass in rank of -1 because service implementations are ranked at the end of the graph build
             wiring_node_instance = create_wiring_node_instance(self, resolved_signature,
                                                                frozendict(kwargs_), rank=-1)
-            from hgraph._wiring._wiring_node_class._graph_wiring_node_class import WiringGraphContext
-            WiringGraphContext.instance().add_built_service_impl(path, wiring_node_instance)
+
+            for p in paths:
+                from hgraph._wiring._wiring_node_class._graph_wiring_node_class import WiringGraphContext
+                WiringGraphContext.instance().add_built_service_impl(p, wiring_node_instance)
 
     def create_node_builder_instance(self, node_signature: "NodeSignature",
                                      scalars: Dict[str, Any]) -> "NodeBuilder":
         # The service impl node should only take scalar values in. The rest will be a
         # graph where we will stub out the inputs and outputs.
         with WiringContext(current_wiring_node=self, current_signature=self.signature):
             from hgraph._impl._builder._service_impl_builder import PythonServiceImplNodeBuilder
@@ -145,111 +154,144 @@
                         (ts_int_type := next(iter(interface_sig.time_series_inputs.values()))).value_scalar_tp):
                     raise CustomMessageWiringError(
                         f"The implementation input {ts_type} scalar value does not match: {ts_int_type}")
                 if not signature.output_type.dereference().value_tp.matches(interface_sig.output_type.dereference()):
                     raise CustomMessageWiringError(
                         "The output type does not match that of the subscription service signature")
             case WiringNodeType.REQ_REP_SVC:
-                if len(signature.time_series_args) != 1:
-                    raise CustomMessageWiringError("The signature can only have one time-series input")
-                ts_type: HgTSDTypeMetaData = signature.input_types.get(arg := next(iter(signature.time_series_args)))
-                if not ts_type.value_tp.matches(
-                        (ts_int_type := next(iter(interface_sig.time_series_inputs.values())))):
-                    raise CustomMessageWiringError(
-                        f"The implementation input {ts_type} type value does not match: {ts_int_type}")
+                for arg, ts_type in signature.input_types.items():
+                    if not ts_type.value_tp.matches((ts_int_type := interface_sig.time_series_inputs.get(arg))):
+                        raise CustomMessageWiringError(
+                            f"The implementation input {ts_type} type value does not match: {ts_int_type}")
                 if not signature.output_type.dereference().value_tp.matches(interface_sig.output_type.dereference()):
                     raise CustomMessageWiringError(
                         "The output type does not match that of the subscription service signature")
             case _:
                 raise CustomMessageWiringError(f"Unknown service type: {interface_sig.node_type}")
     else:
-        raise CustomMessageWiringError("Unable to handle multiple interfaces yet")
+        pass # multiservice implementations use the interface stub APIs to wire up the service so checking happens there
 
 
 def create_inner_graph(wiring_signature: WiringNodeSignature, fn: Callable, scalars: Mapping[str, Any],
-                       interfaces: list[WiringNodeSignature]) -> GraphBuilder:
+                       interfaces: list[WiringNodeSignature]) -> (GraphBuilder, [str]):
     if len(interfaces) == 1:
         s: WiringNodeSignature = interfaces[0].signature
         match s.node_type:
             case WiringNodeType.REF_SVC:
                 return wire_reference_data_service(wiring_signature, fn, scalars, interfaces[0])
             case WiringNodeType.SUBS_SVC:
                 return wire_subscription_service(wiring_signature, fn, scalars, interfaces[0])
             case WiringNodeType.REQ_REP_SVC:
                 return wire_request_reply_service(wiring_signature, fn, scalars, interfaces[0])
             case _:
                 raise CustomMessageWiringError(f"Unknown service type: {s.node_type}")
+    else:
+        with WiringGraphContext(None) as context:
+            graph = wire_multi_service(fn, scalars)
+            for path, node in context.built_services().items():
+                if node:
+                    raise CustomMessageWiringError(f"Mitliservice implementations should not be registering service nodes")
+
+                s: WiringNodeClass = context.find_service_impl(path)[0]
+                match s.signature.node_type:
+                    case WiringNodeType.REF_SVC: # reference service does not require external stubs
+                        pass
+                    case WiringNodeType.SUBS_SVC: # subscription service does not require external stubs
+                        pass
+                    case WiringNodeType.REQ_REP_SVC:
+                        wire_request_reply_service_stubs(s.impl_signature, path, s)
+                    case _:
+                        raise CustomMessageWiringError(f"Unknown service type: {s.signature.node_type}")
+
+            return graph, list(context.built_services().keys())
+
+
+def wire_multi_service(fn: Callable, scalars: Mapping[str, Any]):
+    with WiringNodeInstanceContext(), WiringGraphContext(None) as context:
+        fn(**scalars)
+        sink_nodes = context.pop_sink_nodes()
+        return create_graph_builder(sink_nodes, False)
 
 
 def wire_subscription_service(wiring_signature: WiringNodeSignature, fn: Callable, scalars: Mapping[str, Any],
                               interface):
     path = (scalars := dict(scalars)).pop("path")
-    path = interface.full_path(path if path else None)
+    full_path = interface.full_path(path)
 
     from hgraph._wiring._decorators import graph
-    from hgraph.nodes._service_utils import capture_output_to_global_state
+    from hgraph.nodes._service_utils import capture_output_to_global_state, capture_output_node_to_global_state
 
     @graph
     def subscription_service():
+        subscriptions = interface.wire_impl_inputs_stub(path)
         # Call the implementation graph with the scalars provided
-        sn_arg = next(iter(wiring_signature.time_series_args))
-        subscriptions = last_value_source_node(f"{wiring_signature.name}_{sn_arg}",
-                                               (tp_ := wiring_signature.input_types[sn_arg]))
-        subscriptions = _wiring_port_for(tp_, subscriptions, tuple())
-        capture_output_node_to_global_state(f"{path}_subs", subscriptions)
-        out = fn(**{sn_arg: subscriptions} | scalars)
-        capture_output_to_global_state(f"{path}_out", out)
+        out = fn(**(subscriptions.as_dict() | scalars))
+        interface.wire_impl_out_stub(path, out)
 
     with WiringNodeInstanceContext(), WiringGraphContext(wiring_signature) as context:
         subscription_service()
         sink_nodes = context.pop_sink_nodes()
-        return create_graph_builder(sink_nodes, False)
+        return create_graph_builder(sink_nodes, False), [full_path]
+
+
+def wire_request_reply_service_stubs(wiring_signature: WiringNodeSignature, path, interface):
+    from hgraph.nodes._service_utils import capture_output_node_to_global_state, capture_output_to_global_state
+
+    for arg in wiring_signature.time_series_args:
+        tp = wiring_signature.input_types[arg]
+        request_node = last_value_source_node(f"{path}_request_{arg}", tp)
+        request = _wiring_port_for(tp, request_node, tuple())
+        capture_output_node_to_global_state(f"{path}_request_{arg}", request)
+        capture_output_to_global_state(f"{path}_request_{arg}_out", request)
+
+    if wiring_signature.output_type is not None:
+        replies_node = last_value_source_node(f"{path}_replies_fb", wiring_signature.output_type)
+        replies = _wiring_port_for(tp, replies_node, tuple())
+        capture_output_node_to_global_state(f"{path}_replies_fb", replies)
+        capture_output_to_global_state(f"{path}_replies", replies)
 
 
 def wire_request_reply_service(wiring_signature: WiringNodeSignature, fn: Callable, scalars: Mapping[str, Any],
-                              interface):
+                              interface) -> (GraphBuilder, [str]):
     path = (scalars := dict(scalars)).pop("path")
-    path = interface.full_path(path if path else None)
+    full_path = interface.full_path(path)
+
+    wire_request_reply_service_stubs(wiring_signature, full_path, interface)
 
     from hgraph._wiring._decorators import graph
-    from hgraph.nodes._service_utils import capture_output_to_global_state
 
     @graph
     def request_reply_service():
+        requests = interface.wire_impl_inputs_stub(path)
         # Call the implementation graph with the scalars provided
-        req_arg = next(iter(wiring_signature.time_series_args))
-        requests = last_value_source_node(f"{wiring_signature.name}_{req_arg}",
-                                               (tp_ := wiring_signature.input_types[req_arg]))
-        requests = _wiring_port_for(tp_, requests, tuple())
-        capture_output_node_to_global_state(f"{path}_requests", requests)
-        out = fn(**{req_arg: requests} | scalars)
-        capture_output_to_global_state(f"{path}_replies", out)
+        out = fn(**(requests.as_dict() | scalars))
+        interface.wire_impl_out_stub(path, out)
 
     with WiringNodeInstanceContext(), WiringGraphContext(wiring_signature) as context:
         request_reply_service()
         sink_nodes = context.pop_sink_nodes()
-        return create_graph_builder(sink_nodes, False)
+        return create_graph_builder(sink_nodes, False), [full_path]
 
 
 def wire_reference_data_service(
         wiring_signature: WiringNodeSignature,
         fn: Callable,
         scalars: Mapping[str, Any],
-        interface) -> GraphBuilder:
+        interface) -> (GraphBuilder, [str]):
     # The path was added to the scalars when initially wired to create the wiring node instance,
     # now we pop it off so that we can make use of both the scalars and the path.
     path = (scalars := dict(scalars)).pop("path")
-    path = interface.full_path(path if path else None)
+    full_path = interface.full_path(path)
 
     from hgraph._wiring._decorators import graph
     from hgraph.nodes._service_utils import capture_output_to_global_state
 
     @graph
     def ref_svc_inner_graph():
         # Call the implementation graph with the scalars provided
         out = fn(**scalars)
-        capture_output_to_global_state(path, out)
+        capture_output_to_global_state(full_path, out)
 
     with WiringNodeInstanceContext(), WiringGraphContext(wiring_signature) as context:
         ref_svc_inner_graph()
         sink_nodes = context.pop_sink_nodes()
-        return create_graph_builder(sink_nodes, False)
+        return create_graph_builder(sink_nodes, False), [full_path]
```

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_stub_wiring_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_switch_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_try_except_wiring_node.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py` & `hgraph-0.2.7/src/hgraph/_wiring/_wiring_node_class/_wiring_node_class.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/__init__.py` & `hgraph-0.2.7/src/hgraph/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_analytical.py` & `hgraph-0.2.7/src/hgraph/nodes/_analytical.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_compound_scalar_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_compound_scalar_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_conditional.py` & `hgraph-0.2.7/src/hgraph/nodes/_conditional.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from hgraph import TS, compute_node, TIME_SERIES_TYPE, REF
+from typing import cast
 
+from hgraph import TS, compute_node, TIME_SERIES_TYPE, REF, TSL, PythonTimeSeriesReference, Size
 
 __all__ = ("if_then_else", "if_true")
 
 
 @compute_node(valid=("condition",))
 def if_then_else(condition: TS[bool], true_value: REF[TIME_SERIES_TYPE], false_value: REF[TIME_SERIES_TYPE]) \
         -> REF[TIME_SERIES_TYPE]:
@@ -34,7 +35,13 @@
     If tick_once_only is True then this will only tick once, otherwise this will tick with every tick of the condition,
     when the condition is True.
     """
     if condition.value:
         if tick_once_only:
             condition.make_passive()
         return True
+
+
+@compute_node
+def route_ref(condition: TS[bool], ts: REF[TIME_SERIES_TYPE]) -> TSL[REF[TIME_SERIES_TYPE], Size[2]]:
+    return cast(TSL,
+                (ts.value, PythonTimeSeriesReference()) if condition.value else (PythonTimeSeriesReference(), ts.value))
```

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_const.py` & `hgraph-0.2.7/src/hgraph/nodes/_const.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_data_source_polars.py` & `hgraph-0.2.7/src/hgraph/nodes/_data_source_polars.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_datetime_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_datetime_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_format.py` & `hgraph-0.2.7/src/hgraph/nodes/_format.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_frame_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_frame_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_math.py` & `hgraph-0.2.7/src/hgraph/nodes/_math.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_numpy.py` & `hgraph-0.2.7/src/hgraph/nodes/_numpy.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_print.py` & `hgraph-0.2.7/src/hgraph/nodes/_print.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_record.py` & `hgraph-0.2.7/src/hgraph/nodes/_record.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_replay.py` & `hgraph-0.2.7/src/hgraph/nodes/_replay.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_service_utils.py` & `hgraph-0.2.7/src/hgraph/nodes/_service_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from typing import Mapping, Any, Type
 
 from hgraph import sink_node, REF, TIME_SERIES_TYPE, GlobalState, compute_node, SCALAR, TS, STATE, Removed, \
     pull_source_node, BaseWiringNodeClass, HgREFTypeMetaData, create_input_output_builders, \
     graph, AUTO_RESOLVE, TSD, TS_OUT, REMOVE_IF_EXISTS, TIME_SERIES_TYPE_1
 
 __all__ = ("capture_output_to_global_state", "capture_output_node_to_global_state", "write_subscription_key",
-           "write_service_request", "get_shared_reference_output")
+           "write_service_request", "get_shared_reference_output", "write_service_replies")
+
+from hgraph.nodes import null_sink
 
 
 @sink_node(active=tuple(), valid=tuple())
 def capture_output_to_global_state(path: str, ts: REF[TIME_SERIES_TYPE]):
     """This node serves to capture the output of a service node and record the output reference in the global state."""
 
 
@@ -89,43 +91,62 @@
     write_subscription_key(path, key)
     out = get_shared_reference_output[TIME_SERIES_TYPE: TSD[_s_tp, _ts_tp]](f"{path}_out")
     return out[key]
 
 
 @compute_node
 def write_service_request(path: str, request: TIME_SERIES_TYPE, _output: TS_OUT[int] = None, _state: STATE = None) -> \
-TS[int]:
+        TS[int]:
     """
-    Updates a TSD attached to the path with the data provided.
+    Updates TSDs attached to the path with the data provided.
     """
-    svc_node_in = GlobalState.instance().get(f"{path}_requests")
-    svc_node_in.apply_value({id(_state.requestor_id): request.delta_value})
+    for arg, ts in request.items():
+        if ts.modified:
+            svc_node_in = GlobalState.instance().get(f"{path}_request_{arg}")
+            svc_node_in.apply_value({id(_state.requestor_id): ts.delta_value})
 
     if not _output.valid:
         return id(_state.requestor_id)
 
 
 @write_service_request.start
 def write_service_request_start(path: str, _state: STATE):
     _state.requestor_id = object()
 
 
 @write_service_request.stop
 def write_service_request_stop(request: TIME_SERIES_TYPE, path: str, _state: STATE):
     if request.valid:
-        if svc_node_in := GlobalState.instance().get(f"{path}_requests"):
-            svc_node_in.apply_value({id(_state.requestor_id): REMOVE_IF_EXISTS})
+        for arg, i in request.items():
+            if i.valid:
+                if svc_node_in := GlobalState.instance().get(f"{path}_request_{arg}"):
+                    svc_node_in.apply_value({id(_state.requestor_id): REMOVE_IF_EXISTS})
+
+
+@sink_node
+def write_service_replies(path: str, response: TIME_SERIES_TYPE):
+    """
+    Updates TSDs attached to the path with the data provided.
+    """
+    svc_node_in = GlobalState.instance().get(f"{path}_replies_fb")
+    svc_node_in.apply_value(response.delta_value)
+
+
+@graph
+def _request_service(path: str, request: TIME_SERIES_TYPE):
+    null_sink(write_service_request(path, request))
 
 
 @graph
-def _request_service(path: str, request: TIME_SERIES_TYPE,
+def _request_reply_service(path: str, request: TIME_SERIES_TYPE,
                      tp_out: Type[TIME_SERIES_TYPE_1] = AUTO_RESOLVE) -> TIME_SERIES_TYPE_1:
     requestor_id = write_service_request(path, request)
-    out = get_shared_reference_output[TIME_SERIES_TYPE: TSD[int, tp_out]](f"{path}_replies")
-    return out[requestor_id]
+    if tp_out:
+        out = get_shared_reference_output[TIME_SERIES_TYPE: TSD[int, tp_out]](f"{path}_replies")
+        return out[requestor_id]
 
 
 class SharedReferenceNodeClass(BaseWiringNodeClass):
 
     def create_node_builder_instance(self, node_signature: "NodeSignature",
                                      scalars: Mapping[str, Any]) -> "NodeBuilder":
         output_type = node_signature.time_series_output
```

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_set_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_set_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_stream_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_stream_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_tsb_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_tsb_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_tsd_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_tsd_operators.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 from hgraph.nodes._const import const
 from hgraph.nodes._operators import len_
 from hgraph.nodes._set_operators import is_empty
 from hgraph.nodes._tsl_operators import merge
 
 __all__ = (
     "make_tsd", "make_tsd_scalar", "flatten_tsd", "extract_tsd", "tsd_get_item", "tsd_get_key_set", "tsd_contains",
-    "tsd_not", "tsd_is_empty", "tsd_len", "sum_tsd", "mul_tsd", "get_schema_type", "tsd_get_bundle_item",
-    "tsd_collapse_keys", "tsd_uncollapse_keys", "tsd_rekey", "tsd_flip", "tsd_flip_tsd", "merge_tsds", "tsd_partition")
+    "tsd_not", "tsd_is_empty", "tsd_len", "sum_tsd", "mul_tsd", "tsd_get_bundle_item",
+    "tsd_collapse_keys", "tsd_uncollapse_keys", "tsd_rekey", "tsd_flip", "tsd_flip_tsd", "merge_tsds",
+    "merge_nested_tsds", "tsd_partition", "get_schema_type")
 
 
 @compute_node(valid=("key",))
 def make_tsd(key: TS[K_1], value: TIME_SERIES_TYPE, remove_key: TS[bool] = None,
              ts_type: Type[TIME_SERIES_TYPE_1] = TIME_SERIES_TYPE) -> TSD[K_1, TIME_SERIES_TYPE_1]:
     """
     Make a TSD from a time-series of key and value, if either key or value ticks an entry in the TSD will be
@@ -188,16 +189,16 @@
         out.update({(k, k1): REMOVE_IF_EXISTS for k1 in v.removed_keys()})
 
     return out
 
 
 @compute_node
 def tsd_uncollapse_keys(ts: TSD[Tuple[K, K_1], REF[TIME_SERIES_TYPE]],
-                        _output: TSD[K, TSD[K_1, REF[TIME_SERIES_TYPE]]] = None) -> TSD[
-    K, TSD[K_1, REF[TIME_SERIES_TYPE]]]:
+                        _output: TSD[K, TSD[K_1, REF[TIME_SERIES_TYPE]]] = None) \
+        -> TSD[K, TSD[K_1, REF[TIME_SERIES_TYPE]]]:
     """
     Un-Collapse the nested TSDs to a TSD with a tuple key.
     """
     out = defaultdict(dict)
 
     removed_keys = defaultdict(set)
     for k in ts.removed_keys():
@@ -339,14 +340,47 @@
                 break
         else:
             out[k] = REMOVE_IF_EXISTS
 
     return out
 
 
+@compute_node(overloads=merge)
+def merge_nested_tsds(tsl: TSL[TSD[K, TSD[K_1, REF[TIME_SERIES_TYPE]]], SIZE]) -> TSD[K, TSD[K_1, REF[TIME_SERIES_TYPE]]]:
+    out = defaultdict(dict)
+    removals = set()
+    nested_removals = defaultdict(set)
+
+    for tsd in reversed(list(tsl.modified_values())):
+        for k, v in tsd.modified_items():
+            for k1, v1 in v.modified_items():
+                out[k].update({k1: v1.value})
+            nested_removals[k].update(v.removed_keys())
+            out[k].update({k1: REMOVE_IF_EXISTS for k1 in v.removed_keys()})
+        removals.update(tsd.removed_keys())
+        for k, v1 in tsd.removed_items():
+            nested_removals[k].update(v1.keys())
+
+    for k in removals:
+        for v in reversed(tsl.values()):
+            if k in v:
+                break
+        else:
+            out[k] = REMOVE_IF_EXISTS
+
+    for k, v in nested_removals.items():
+        for v1 in reversed(tsl.values()):
+            if k in v1:
+                for k1 in v:
+                    if k1 in v1[k] and out[k].get(k1, REMOVE_IF_EXISTS) is REMOVE_IF_EXISTS:
+                        out[k][k1] = v1[k][k1].value
+
+    return out
+
+
 @compute_node
 def tsd_partition(ts: TSD[K, REF[TIME_SERIES_TYPE]], partitions: TSD[K, TS[K_1]],
                   _state: STATE[TsdRekeyState] = None) -> TSD[K_1, TSD[K, REF[TIME_SERIES_TYPE]]]:
     """
     Partition a TSD into partitions by the given mapping.
     """
     out = defaultdict(dict)
```

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_tsl_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_tsl_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_tss_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_tss_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_tuple_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_tuple_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/nodes/_window_operators.py` & `hgraph-0.2.7/src/hgraph/nodes/_window_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/test/_node_printer.py` & `hgraph-0.2.7/src/hgraph/test/_node_printer.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/test/_node_unit_tester.py` & `hgraph-0.2.7/src/hgraph/test/_node_unit_tester.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/src/hgraph/test/testing.md` & `hgraph-0.2.7/src/hgraph/test/testing.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/test_wiring.py` & `hgraph-0.2.7/tests/python/unit/hgraph/test_wiring.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_impl/_builder/test_graph_builder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/test_graph_runner.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_impl/_runtime/test_record_replay.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_runtime/test_feedback.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_runtime/test_feedback.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_runtime/test_scheduler.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_runtime/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_types/test_complex_types.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_types/test_complex_types.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_types/test_operator_rank.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_types/test_operator_rank.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_types/test_type_meta_data.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_types/test_type_meta_data.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_types/test_type_meta_resolve.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_types/test_type_meta_resolve.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_auto_const.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_auto_const.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_auto_resolve.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_auto_resolve.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_de_dupping_of_nodes.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_decorators.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_dispatch.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_error_handling.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_map.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_map.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_overloads.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_overloads.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_ref.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_ref.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_service.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 from frozendict import frozendict
 
 from hgraph import reference_service, TSD, TS, service_impl, graph, register_service, default_path, \
-    subscription_service, TSS, map_, TSL, SIZE, request_reply_service
-from hgraph.nodes import const, pass_through
+    subscription_service, TSS, map_, TSL, SIZE, request_reply_service, contains_
+from hgraph.nodes import const, pass_through, merge, sample, tsd_flip
+from hgraph.nodes._conditional import route_ref
 from hgraph.test import eval_node
 
 
 def test_reference_service():
 
     @reference_service
     def my_service(path: str = None) -> TSD[str, TS[str]]:
@@ -65,15 +66,54 @@
         return map_(lambda x: x + 1, ts)
 
     @graph
     def main(x: TS[int]) -> TS[int]:
         register_service(default_path, add_one_service_impl)
         return add_one_service(default_path, x)
 
-    assert eval_node(main, [1]) == [None, 2]
+    assert eval_node(main, [1]) == [None, None, 2]
+
+
+def test_request_reply_service2():
+    @request_reply_service
+    def add_service(path: str, ts: TS[int], ts1: TS[int]) -> TS[int]:
+        """The service description"""
+
+    @service_impl(interfaces=add_service)
+    def add_service_impl(ts: TSD[int, TS[int]], ts1: TSD[int, TS[int]]) -> TSD[int, TS[int]]:
+        return map_(lambda x, y: x + y, ts, ts1)
+
+    @graph
+    def main(x: TS[int], y: TS[int]) -> TS[int]:
+        register_service(default_path, add_service_impl)
+        return add_service(default_path, x, y)
+
+    assert eval_node(main, [1], [2]) == [None, None, 3]
+
+
+def test_recursive_request_reply_service():
+    @request_reply_service
+    def add_one_service(path: str, ts: TS[int]) -> TS[int]:
+        """The service description"""
+
+    @graph
+    def _add_one_service_impl(ts: TS[int]) -> TS[int]:
+        z, nz = route_ref(ts == 0, ts)
+        return merge(TSL.from_ts(sample(z, 1), add_one_service('default_path', nz - 1) + 1))
+
+    @service_impl(interfaces=add_one_service)
+    def add_one_service_impl(ts: TSD[int, TS[int]]) -> TSD[int, TS[int]]:
+        return map_(_add_one_service_impl, ts)
+
+    @graph
+    def main(x: TS[int]) -> TS[int]:
+        register_service('default_path', add_one_service_impl)
+        return add_one_service('default_path', x)
+
+    assert eval_node(main, [3], __trace__=True)[-1] == 4
 
 
 def test_two_services():
     @request_reply_service
     def add_one_service(path: str, ts: TS[int]) -> TS[int]:
         """The service description"""
 
@@ -87,8 +127,39 @@
 
     @graph
     def main(x: TS[int]) -> TS[int]:
         register_service('another_path', add_one_service_impl_2)
         register_service('one_path', add_one_service_impl)
         return add_one_service('another_path', x)
 
-    assert eval_node(main, [1]) == [None, None, 3]
+    assert eval_node(main, [1]) == [None, None, None, None, 3]
+
+
+def test_mutltiservice():
+    @request_reply_service
+    def submit(path: str, ts: TS[int]):
+        ...
+
+    @reference_service
+    def receive(path: str) -> TSS[int]:
+        ...
+
+    @subscription_service
+    def subscribe(path: str, ts: TS[int]) -> TS[bool]:
+        ...
+
+    @service_impl(interfaces=(submit, receive, subscribe))
+    def impl(path: str):
+        submissions: TSD[int, TS[int]] = submit.wire_impl_inputs_stub(path).ts
+        items = tsd_flip(submissions).key_set
+        receive.wire_impl_out_stub(path, items)
+        subscribe.wire_impl_out_stub(path, map_(lambda key, i: contains_(i, key),
+                                                __keys__=subscribe.wire_impl_inputs_stub(path).ts, i=pass_through(items)))
+
+    @graph
+    def multiservice_test(ts1: TS[int], ts2: TS[int]) -> TSD[int, TS[bool]]:
+        register_service('submit', impl)
+        submit('submit', ts1)
+        submit('submit', ts2)
+        return map_(lambda key: subscribe('submit', key), __keys__=receive('submit'))
+
+    assert eval_node(multiservice_test, [1, None], [None, 2], __trace__=True) == [None, {}, {1: True}, {2: True}]
```

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_switch.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_switch.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsb_wiring.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsd_wiring.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tsl_wiring.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_tss.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_tss.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py` & `hgraph-0.2.7/tests/python/unit/hgraph/_wiring/test_wiring_node_signature.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_analytical.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_analytical.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_compound_scalar_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_conditional.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_conditional.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_const.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_const.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_data_source_polars.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_data_source_polars.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_format.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_format.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_frame.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_frame.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_math.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_math.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_numpy.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_numpy.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_operators.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_push_queue.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_push_queue.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_recorder.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_recorder.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_tsb_operators.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsb_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_tsd_operators.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsd_operators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pytest
 from frozendict import frozendict
 
 from hgraph import TS, graph, TIME_SERIES_TYPE, TSD, REMOVE, not_, SCALAR, K, TimeSeriesSchema, TSB, \
     compute_node, REF, TSS, Size, SIZE, K_1
 from hgraph.nodes import (make_tsd, extract_tsd, flatten_tsd, is_empty, sum_, tsd_get_item, const, tsd_rekey, tsd_flip,
-                          merge_tsds, tsd_partition, tsd_flip_tsd, tsd_collapse_keys, tsd_uncollapse_keys)
+                          merge_tsds, tsd_partition, tsd_flip_tsd, tsd_collapse_keys, tsd_uncollapse_keys,
+                          merge_nested_tsds)
 from hgraph.test import eval_node
 
 
 def test_make_tsd():
     assert eval_node(make_tsd, ['a', 'b', 'a'], [1, 2, 3]) == [{'a': 1}, {'b': 2}, {'a': 3}]
 
 
@@ -166,14 +167,20 @@
 
 def test_merge_tsd():
     assert eval_node(merge_tsds[K: int, TIME_SERIES_TYPE: TS[int], SIZE: Size[2]],
                      [({1: 1, 2: 2}, {1: 5, 3: 6}), ({2: 4}, {3: 8}), ({1: REMOVE}, {}), ({}, {1: REMOVE})]) == [
                {1: 1, 2: 2, 3: 6}, {2: 4, 3: 8}, {1: 5}, {1: REMOVE}]
 
 
+def test_merge_nested_tsd():
+    assert eval_node(merge_nested_tsds[K: int, K_1: int, TIME_SERIES_TYPE: TS[int], SIZE: Size[2]],
+                     [({1: {1: 1}, 2: {2: 2}}, {1: {1: 5}, 3: {3: 6}}), ({2: {2: 4}}, {3: {3: 8}}), ({1: REMOVE, 2: {2: REMOVE}}, {}), ({}, {1: REMOVE})]) == [
+        {1: {1: 1}, 2: {2: 2}, 3: {3: 6}}, {2: {2: 4}, 3: {3: 8}}, {1: {1: 5}, 2: {2: REMOVE}}, {1: REMOVE}]
+
+
 def test_tsd_partition():
     assert eval_node(tsd_partition[K: int, K_1: str, TIME_SERIES_TYPE: TS[int]],
                      [{1: 1, 2: 2, 3: 3}, {1: 4, 2: 5, 3: 6}, {1: REMOVE}],
                      [{1: 'odd'}, {2: 'even', 3: 'odd'}, None, {2: REMOVE}, {3: 'prime'}]) == [
                {'odd': {1: 1}},
                {'odd': {1: 4, 3: 6}, 'even': {2: 5}},
                {'odd': {1: REMOVE}},
```

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_tsl_operators.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tsl_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_tss_operators.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_tss_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_window_operators.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_window_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/nodes/test_wp_operators.py` & `hgraph-0.2.7/tests/python/unit/hgraph/nodes/test_wp_operators.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/tests/python/unit/hgraph/test/test_node_printer.py` & `hgraph-0.2.7/tests/python/unit/hgraph/test/test_node_printer.py`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/LICENSE` & `hgraph-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/README.md` & `hgraph-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/pyproject.toml` & `hgraph-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hgraph-0.2.6/PKG-INFO` & `hgraph-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgraph
-Version: 0.2.6
+Version: 0.2.7
 Summary: A functional reactive engine
 Project-URL: Homepage, https://github.com/hhenson/hgraph
 Project-URL: Repository, https://github.com/hhenson/hgraph.git
 Author-email: Howard Henson <howard@henson.me.uk>
 License: MIT License
         
         Copyright (c) 2023 Howard Henson
```

