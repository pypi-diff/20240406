# Comparing `tmp/sapiopylib-2024.2.7a178.tar.gz` & `tmp/sapiopylib-2024.4.5a179.tar.gz`

## Comparing `sapiopylib-2024.2.7a178.tar` & `sapiopylib-2024.4.5a179.tar`

### file list

```diff
@@ -1,126 +1,128 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/jarvis/QQPlotComputer.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    40379 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/DataService.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    21742 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/GroupManagerService.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/MessengerService.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/ReportManager.py
--rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/UserManagerService.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    25254 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/Message.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/UserInfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55797 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
--rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    29969 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    26958 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/field_set.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/protocol_template.py
--rw-r--r--   0        0        0    17530 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    23305 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/CompresionUtil.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    23715 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/autopaging.py
--rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recorddatasinks.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    44895 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    13745 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/ancestry.py
--rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/properties.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/src/sapiopylib/utils/string.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/EmailAttachmentDataTest.py
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/FR-51536_test.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/FR-51549_test.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/FR-51551_test.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/FR-51635_test.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/FR-51821_test.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/FR-51846_test.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/FR-51847_test.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/FR-51849_test.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/PR-51537_test.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/PR-51547.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/PR-51842_test.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/PR-51853_test.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/PR-51856_test.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/PR-51964_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/__init__.py
--rw-r--r--   0        0        0  1468866 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/data_type_models.py
--rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/tests/resources/fr-51846.ssg
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/LICENSE
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/README.md
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/pyproject.toml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 sapiopylib-2024.2.7a178/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0    12925 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/ClientCallbackService.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    48718 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataService.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    23745 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/GroupManagerService.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/MessengerService.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/ReportManager.py
+-rw-r--r--   0        0        0    13871 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/UserManagerService.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    25254 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Message.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/UserInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55797 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
+-rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    29969 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    26958 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/field_set.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/protocol_template.py
+-rw-r--r--   0        0        0    17530 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/CompresionUtil.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    23715 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/autopaging.py
+-rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recorddatasinks.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    44895 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    13745 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/ancestry.py
+-rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/properties.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/utils/string.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/EmailAttachmentDataTest.py
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51536_test.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51549_test.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51551_test.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51635_test.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51821_test.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51846_test.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51847_test.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51849_test.py
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-52100_test.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51537_test.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51547.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51842_test.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51853_test.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51856_test.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51964_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/__init__.py
+-rw-r--r--   0        0        0  1468866 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/data_type_models.py
+-rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/resources/fr-51846.ssg
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/LICENSE
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/README.md
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/pyproject.toml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/PKG-INFO
```

### Comparing `sapiopylib-2024.2.7a178/INSTALL.md` & `sapiopylib-2024.4.5a179/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/jarvis/QQPlotComputer.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/jarvis/QQPlotComputer.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/AccessionService.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,36 +5,40 @@
 from sapiopylib.rest.User import SapioUser
 from enum import Enum
 
 
 class AccessionCriteriaType(Enum):
     """
     Accessioning cache type.
-
-    SYSTEM: Global accessioning. Note that Accession Service from Sapio Foundations do not use this cache.
-
-    DATA_FIELD: Cached per data type's maximum value of a data field.
     """
     SYSTEM = 1
+    """Global accessioning. Note that the Accession Service from Sapio Foundations does not use this cache."""
     DATA_FIELD = 2
+    """Cached per data type's maximum value of a data field."""
 
 
 class AbstractAccessionCriteriaPojo:
     """
     Describes a criteria for server accession service request, in order to obtain a list of accession IDs.
     """
     criteria_type: AccessionCriteriaType
+    """The type of accessioning that is being requested."""
     prefix: Optional[str] = None
+    """If specified, the value returned will have this starting text."""
     suffix: Optional[str] = None
+    """If specified, the value returned will have this trailing text."""
     sequence_key: Optional[str]
+    """The key of the sequence. Each key holds separate cache of values. At minimum, for requests with different prefix,
+    suffix, data type name, or data field name, they should have different keys."""
     initial_sequence_value: int = 1
+    """If there are no value at all among all records in the field, start with this value."""
 
     def __init__(self, criteria_type: AccessionCriteriaType, sequence_key: str):
         """
-        INTERNAL ONLY. Use one of the sub-classes.
+        INTERNAL USE ONLY. Use one of the subclasses.
         """
         self.criteria_type = criteria_type
         self.sequence_key = sequence_key
 
     def from_pojo(self, json_dct: dict) -> None:
         self.prefix = json_dct.get('prefix')
         self.suffix = json_dct.get('suffix')
@@ -54,31 +58,37 @@
 class AccessionSystemCriteriaPojo(AbstractAccessionCriteriaPojo):
     """
     Describes request to accession a global (unrelated to data records) accession IDs.
     """
     def __init__(self, sequence_key: str):
         """
         Accession by sequence order in sequence key, regardless of existing record values.
+
         :param sequence_key: The sequence table ID to accession for. IDs in the same sequence will not duplicate.
         """
         super().__init__(AccessionCriteriaType.SYSTEM, sequence_key)
 
 
 class AccessionDataFieldCriteriaPojo(AbstractAccessionCriteriaPojo):
     """
     Describes request to accession data record's IDs for a data field under a specified format.
     """
     data_type_name: str
+    """The name of the data type that the data field name is under."""
     data_field_name: str
+    """The data field name of the field to accession. This field must have the "Unique" boolean set to true in the
+    data designer."""
 
     def __init__(self, data_type_name: str, data_field_name: str, sequence_key: str):
         """
         Accession for a data field's value
-        :param data_type_name: The data type name to accession
-        :param data_field_name: The data field name to accession
+
+        :param data_type_name: The data type name to accession for.
+        :param data_field_name: The data field name to accession for. This field must have the "Unique" boolean set
+            to true in the data designer.
         :param sequence_key: The sequence key that must be unique for the same formatting (prefix, suffix) of IDs.
         """
         super().__init__(AccessionCriteriaType.DATA_FIELD, sequence_key)
         self.data_type_name = data_type_name
         self.data_field_name = data_field_name
 
     def from_pojo(self, json_dct: dict):
@@ -100,52 +110,67 @@
     user: SapioUser
     __instances: WeakValueDictionary[SapioUser, AccessionManager] = WeakValueDictionary()
     __initialized: bool
 
     def __new__(cls, user: SapioUser):
         """
         Observes singleton pattern per record model manager object.
+
+        :param user: The user that will make the webservice request to the application.
         """
         obj = cls.__instances.get(user)
         if not obj:
             obj = object.__new__(cls)
             obj.__initialized = False
             cls.__instances[user] = obj
         return obj
 
     def __init__(self, user: SapioUser):
         """
         Obtains REST accession manager to perform accessioning operations.
+
+        :param user: The user that will make the webservice request to the application.
         """
         if self.__initialized:
             return
         self.user = user
         self.__initialized = True
 
     def accession_for_system(self, num_to_accession: int, criteria: AccessionSystemCriteriaPojo) -> List[str]:
         """
-        Accession IDs that do not need to get starting value from a data field.
-        :param num_to_accession: Number of IDs to return
-        :param criteria: The accession format.
-        :return: list if unique IDs that will never be generated with this method again.
+        Accession IDs that are not tied to a specific data type and field.
+
+        If this is the first time that the system is being accessioned with these criteria, the returned results
+        will start from the initial_sequence_value of the criteria. Otherwise, they will continue on from the previous
+        value.
+
+        :param num_to_accession: The number of new IDs to return.
+        :param criteria: The criteria by which the accession IDs will be generated.
+        :return: A list of unique IDs that will never be generated with this method again for the same criteria.
         """
         sub_path = self.user.build_url(['accession', 'accessionForSystem'])
         param = {'numToAccession': num_to_accession}
         payload = criteria.to_pojo()
         response = self.user.post(sub_path, param, payload)
         self.user.raise_for_status(response)
         return response.json()
 
     def accession_for_field(self, num_to_accession: int, criteria: AccessionDataFieldCriteriaPojo) -> List[str]:
         """
-        Accession IDs for the data fields.
-        If this is the first time, look up starting value to be greater than the maximum of existing ID (+1).
-        :param num_to_accession: Number of IDs to return
-        :param criteria: The rules on how an ID should be generated.
-        :return: List of generated IDs
+        Accession IDs that are tied to a specific data type and data field. The data field definition of the field that
+        is used must have the "Unique" boolean set to true in the data designer.
+
+        If this is the first time that this field is being accessioned with the given criteria, the returned results
+        will use the maximum value of the field across the records in the system that matches the criteria and add 1.
+        If there are no values that match the criteria, then the initial_sequence_value from the criteria is used. For
+        all subsequent calls, the returned results will continue on from the previous value.
+
+        :param num_to_accession: The number of new IDs to return.
+        :param criteria: The criteria by which the accession IDs will be generated.
+        :return: A list of unique IDs that will never be generated with this method again for the same criteria.
         """
         sub_path = self.user.build_url(['accession', 'accessionForField'])
         param = {'numToAccession': num_to_accession}
         payload = criteria.to_pojo()
         response = self.user.post(sub_path, param, payload)
         self.user.raise_for_status(response)
         return response.json()
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/DashboardManager.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,60 +15,69 @@
 
     __instances: WeakValueDictionary[SapioUser, DashboardManager] = WeakValueDictionary()
     __initialized: bool
 
     def __new__(cls, user: SapioUser):
         """
         Observes singleton pattern per record model manager object.
+
+        :param user: The user that will make the webservice request to the application.
         """
         obj = cls.__instances.get(user)
         if not obj:
             obj = object.__new__(cls)
             obj.__initialized = False
             cls.__instances[user] = obj
         return obj
 
     def __init__(self, user: SapioUser):
         """
         Obtain a dashboard manager to create, modify, or delete charts in Sapio.
-        :param user: The Sapio user context.
+
+        :param user: The user that will make the webservice request to the application.
         """
         if self.__initialized:
             return
         self.user = user
 
     def delete_dashboard_definition(self, dashboard_guid: str) -> None:
         """
         Delete an existing dashboard by the dashboard GUID.
+
+        :param dashboard_guid: The GUID of the dashboard to delete.
         """
         if not dashboard_guid:
             raise ValueError("Dashboard GUID must be specified.")
         url = self.user.build_url(['dashboard', dashboard_guid])
         response = self.user.delete(url)
         self.user.raise_for_status(response)
         return
 
     def get_dashboard(self, dashboard_guid: str) -> DashboardDefinition:
         """
         Get an existing dashboard stored in the system by its dashboard GUID.
+
+        :param dashboard_guid: The GUID of the dashboard to get.
+        :return: The dashboard definition for the matching GUID.
         """
         if not dashboard_guid:
             raise ValueError("Dashboard GUID must be specified.")
         url = self.user.build_url(['dashboard', dashboard_guid])
         response = self.user.get(url)
         self.user.raise_for_status(response)
         json = response.json()
         return DashboardDefinitionParser.parse_dashboard_definition(json)
 
     def store_dashboard_definition(self, dashboard: DashboardDefinition) -> DashboardDefinition:
         """
-        Store either a new or existing dashboard to the system.
-        :param dashboard: The dashboard object to be stored
-        :return: The returned dashboard object after store has completed.
-        If this is a new dashboard, the GUIDs, etc., will not be populated.
+        Add a new dashboard to the system or update an existing dashboard.
+
+        :param dashboard: The dashboard object to be stored.
+        :return: The returned dashboard object after store has completed. If this is a new dashboard, the GUIDs, etc.,
+            will not be populated.
         """
         url = self.user.build_url(['dashboard'])
         response = self.user.post(url, payload=dashboard.to_json())
         self.user.raise_for_status(response)
         json = response.json()
         return DashboardDefinitionParser.parse_dashboard_definition(json)
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,36 +22,44 @@
 
     __instances: WeakValueDictionary[SapioUser, DataRecordManager] = WeakValueDictionary()
     __initialized: bool
 
     def __new__(cls, user: SapioUser):
         """
         Observes singleton pattern per record model manager object.
+
+        :param user: The user that will make the webservice request to the application.
         """
         obj = cls.__instances.get(user)
         if not obj:
             obj = object.__new__(cls)
             obj.__initialized = False
             cls.__instances[user] = obj
         return obj
 
     def __init__(self, user: SapioUser):
+        """
+        Obtains data record manager to perform data record operations.
+
+        :param user: The user that will make the webservice request to the application.
+        """
         if self.__initialized:
             return
         self.user = user
         self.__initialized = True
 
     @staticmethod
     def get_data_frame(records: List[DataRecord]) -> DataFrame:
         """
         Get a pandas data frame for a list of records.
+
         :param records: The records to get data frames for.
         :return: A consolidated data frame among all columns across all data records.
-        The data records does not have to be of the same time, and records with same field names
-        will be joined under a single key.
+            The data records do not have to be of the same time, and records with same field names
+            will be joined under a single key.
         """
         data_dict: Dict[str, List[Any]] = dict()
         cur_length = 0
         for record in records:
             fields = record.get_fields()
             for key, value in fields.items():
                 if key not in data_dict:
@@ -61,73 +69,85 @@
             cur_length += 1
         return DataFrame.from_dict(data_dict, orient='columns')
 
     def query_data_records(self, data_type_name: str, data_field_name: str,
                            value_list: list,
                            paging_criteria: DataRecordPojoPageCriteria = None) -> DataRecordPojoListPageResult:
         """
-        Query the system for records of the given type that have values in the given field that match the given values
-        :param data_type_name: The data type name to use in the query for records.
+        Query the system for records of the given type that have values in the given field that match the given values.
+
+        :param data_type_name: The data type name of the records being queried for.
         :param data_field_name: The data field name that will be used when querying for records.
-        :param value_list: The list of values to be used in the query. Think of SQL "IN" Clause
-        :param paging_criteria optional paging criteria info for the current page.
-        :return: The result query of the current page.
+        :param value_list: The list of values to be used in the query. Similar in behavior to a SQL "IN" clause.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a list of the data records from the query,
+            the current page information, and whether more pages exist after it.
         """
         params = {'dataTypeName': data_type_name,
                   'dataFieldName': data_field_name}
         self._append_query_param(paging_criteria, params)
         sub_path = '/datarecordmanager/querydatarecords'
         response = self.user.post(sub_path, params, value_list)
         self.user.raise_for_status(response)
         json_dict = response.json()
         return DataRecordPojoListPageResult.from_json(json_dict)
 
     def query_data_records_by_id(self, data_type_name: str, record_id_list: List[int],
                                  paging_criteria: DataRecordPojoPageCriteria = None) -> DataRecordPojoListPageResult:
         """
-        Get a list of records given the given list of Record IDs provided in a comma delimited
-        list.  This method will only return records of the given type that have one of the
-        provided Record IDs.  The records are not guaranteed to be returned, in the same
+        Get a list of records given a list of their record IDs. This method will only return records of the given type
+        that have one of the provided record IDs. The records are not guaranteed to be returned in the same
         order as the provided list.
-        :param data_type_name: The data type name to use in the query for records.
-        :param record_id_list: Comma delimited list of Record IDs to be found in the system.
-        :param paging_criteria: optional paging criteria info for the current page.
-        :return:
+
+        :param data_type_name: The data type name of the records being queried for.
+        :param record_id_list: The list of record IDs to be used in the query.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a list of the data records from the query,
+            the current page information, and whether more pages exist after it.
         """
         record_id_list.sort()
         params = {'dataTypeName': data_type_name}
         self._append_query_param(paging_criteria, params)
         sub_path = '/datarecordlist'
         response = self.user.post(sub_path, params=params, payload=record_id_list)
         self.user.raise_for_status(response)
         json_dict = response.json()
         return DataRecordPojoListPageResult.from_json(json_dict)
 
     def query_all_records_of_type(self, data_type_name: str,
                                   paging_criteria: DataRecordPojoPageCriteria = None) -> DataRecordPojoListPageResult:
         """
         Get a list of all records of the given data type.
-        :param data_type_name: The data type name to retrieve for.
-        :param paging_criteria: The current page info.
-        :return: The paged data
+
+        :param data_type_name: The data type name of the records being queried for.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a list of the data records from the query,
+            the current page information, and whether more pages exist after it.
         """
         params = {'dataTypeName': data_type_name}
         self._append_query_param(paging_criteria, params)
         sub_path = '/datarecordlist/all'
         response = self.user.get(sub_path, params)
         self.user.raise_for_status(response)
         json_dict = response.json()
         return DataRecordPojoListPageResult.from_json(json_dict)
 
     def query_system_for_record(self, data_type_name: str,
                                 record_id: int) -> Optional[DataRecord]:
         """
-        Get the record of the given type that has the provided Record ID.
-        :param data_type_name: The Data Type Name of the record in the system.
-        :param record_id: The Record ID of the record in the system.
+        Get the record of the given type that has the provided record ID.
+
+        :param data_type_name: The data type name of the record being queried for.
+        :param record_id: The record ID of the record in the system.
         :return: The data record if available. None if not found.
         """
         params = {'dataTypeName': data_type_name,
                   'recordId': record_id}
         sub_path = '/datarecord'
         response = self.user.get(sub_path, params)
         self.user.raise_for_status(response)
@@ -135,20 +155,24 @@
             return None
         json_dict = response.json()
         return DataRecord.from_json(json_dict)
 
     def get_parents(self, record_id: int, child_type_name: str, parent_type_name: str,
                     paging_criteria: Optional[DataRecordPojoPageCriteria] = None) -> DataRecordPojoListPageResult:
         """
-        Get the parents of the given type above the record with the given Record ID.
-        :param record_id: The data type of the child record.
-        :param child_type_name: The data type name of the child of specified Record ID.
-        :param parent_type_name: The data type name of the parent to look for above he given Record ID.
-        :param paging_criteria: Optional criteria for next page info.
-        :return: The result of parents of the given child record, at the current page.
+        Get the parents of the given data type above the record with the given record ID and data type.
+
+        :param record_id: The record ID of the child record to search from.
+        :param child_type_name: The data type name of the child to search from.
+        :param parent_type_name: The data type name of the parents to look for above the given record ID.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a list of the data records from the query,
+            the current page information, and whether more pages exist after it.
         """
         params = {'recordId': record_id,
                   'childTypeName': child_type_name,
                   'parentTypeName': parent_type_name}
         self._append_query_param(paging_criteria, params)
         sub_path = '/datarecord/parents'
         response = self.user.get(sub_path, params)
@@ -156,21 +180,25 @@
         json_dict = response.json()
         return DataRecordPojoListPageResult.from_json(json_dict)
 
     def get_parents_list(self, record_id_list: List[int], child_type_name: Optional[str], parent_type_name: str,
                          paging_criteria: Optional[DataRecordPojoHierarchyPageCriteria] = None) -> \
             DataRecordPojoHierarchyListPageResult:
         """
-        Get the parents of the given type above the records with the given Record IDs.
-        :param record_id_list: The list of record IDs to retrieve parents for.
-        :param child_type_name: The child data type name of records in the record_id_list.
-        This is only required in high-performance high-volume data retrieval.
-        :param parent_type_name: The parent data type name to get for each child.
-        :param paging_criteria: Optionally specify the page to retrieve for. Note the page size may be enforced in SaaS.
-        :return: The current page's result.
+        Get the parents of the given type above the records with the given record IDs and data type.
+
+        :param record_id_list: The record IDs of the child records to search from.
+        :param child_type_name: The data type name of the children to search from.
+            This is only required in high-performance high-volume data retrieval.
+        :param parent_type_name: The data type name of the parents to look for above the given record IDs.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a dictionary of the data records from the query
+            mapped by their child record, the current page information, and whether more pages exist after it.
         """
         try:
             record_id_list.sort()
             params = {'childTypeName': child_type_name,
                       'parentTypeName': parent_type_name}
             self._append_query_param(paging_criteria, params)
             sub_path = '/datarecordlist/parents'
@@ -196,37 +224,46 @@
                 return DataRecordPojoHierarchyListPageResult.from_json(json_dict)
             else:
                 raise e
 
     def get_children(self, record_id: int, child_type_name: str,
                      paging_criteria: Optional[DataRecordPojoPageCriteria] = None) -> DataRecordPojoListPageResult:
         """
-        Get the children of the given type below the record with the given Record ID.
-        :param record_id: The Record ID of the parent record.
-        :param child_type_name: The data type name of the children to look for below the given Record ID.
-        :param paging_criteria: Optionally specify the page to retrieve for. Note the page size may be enforced in SaaS.
-        :return:
+        Get the children of the given data type below the record with the given record ID.
+
+        :param record_id: The record ID of the parent record to search from.
+        :param child_type_name: The data type name of the children to look for below the given record ID.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a list of the data records from the query,
+            the current page information, and whether more pages exist after it.
         """
         params = {'recordId': record_id,
                   'childTypeName': child_type_name}
         self._append_query_param(paging_criteria, params)
         sub_path = '/datarecord/children'
         response = self.user.get(sub_path, params)
         self.user.raise_for_status(response)
         json_dict = response.json()
         return DataRecordPojoListPageResult.from_json(json_dict)
 
     def get_children_list(self, record_id_list: List[int], child_type_name: str,
                           paging_criteria: Optional[DataRecordPojoHierarchyPageCriteria] = None) -> \
             DataRecordPojoHierarchyListPageResult:
         """
-        Get the children of the given type below the records with the given Record IDs.
-        :param record_id_list: Parent Record IDs to get children of.
-        :param child_type_name: The data type name of the children to look for below the given Record IDs.
-        :param paging_criteria: Optionally specify the page to retrieve for. Note the page size may be enforced in SaaS.
+        Get the children of the given type below the records with the given record IDs.
+
+        :param record_id_list: The record IDs of the parent records.
+        :param child_type_name: The data type name of the children to look for below the given record IDs.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a dictionary of the data records from the query
+            mapped by their parent record, the current page information, and whether more pages exist after it.
         """
         try:
             record_id_list.sort()
             params = {'childTypeName': child_type_name}
             self._append_query_param(paging_criteria, params)
             sub_path = '/datarecordlist/childrenbyid'
             response = self.user.post(sub_path, params=params, payload=record_id_list)
@@ -250,20 +287,24 @@
                 return DataRecordPojoHierarchyListPageResult.from_json(json_dict)
             else:
                 raise e
 
     def get_ancestors(self, record_id: int, descendant_type_name: str, ancestor_type_name: str,
                       paging_criteria: Optional[DataRecordPojoPageCriteria] = None) -> DataRecordPojoListPageResult:
         """
-        Get the ancestors of the given type above the records with the given Record ID.
-        :param record_id: The Record ID of the descendant record.
-        :param descendant_type_name: The data type name of descendants ancestors to look for above the given Record ID.
-        :param ancestor_type_name: The data type name of the ancestors to look for above the given Record ID.
-        :param paging_criteria: Optionally specify the page to retrieve for. Note the page size may be enforced in SaaS.
-        :return: ancestors of the current record at this page.
+        Get the ancestors of the given data type above the record with the given record ID and data type.
+
+        :param record_id: The record ID of the parent record to search from.
+        :param descendant_type_name: The data type name of the descendant to search from.
+        :param ancestor_type_name: The data type name of the ancestors to look for below the given record ID.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a list of the data records from the query,
+            the current page information, and whether more pages exist after it.
         """
         params = {'recordId': record_id,
                   'descendantTypeName': descendant_type_name,
                   "ancestorTypeName": ancestor_type_name}
         self._append_query_param(paging_criteria, params)
         sub_path = '/datarecord/ancestors'
         response = self.user.get(sub_path, params)
@@ -271,198 +312,225 @@
         json_dict = response.json()
         return DataRecordPojoListPageResult.from_json(json_dict)
 
     def get_ancestors_list(self, record_id_list: List[int], descendant_type_name: str, ancestor_type_name: str,
                            paging_criteria: Optional[DataRecordPojoHierarchyPageCriteria] = None) -> \
             DataRecordPojoHierarchyListPageResult:
         """
-        Get the ancestors of the given type above the records with the given Record IDs.
-        :param record_id_list: Record IDs to get ancestors of.
-        :param descendant_type_name: The data type name of the descendants to look for above the given Record IDs.
-        :param ancestor_type_name: The data type name of the ancestors to look for above the given Record IDs.
-        :param paging_criteria: Optionally specify the page to retrieve for. Note the page size may be enforced in SaaS.
-        :return: Current page's result, ancestors of the records.
+        Get the ancestors of the given type above the records with the given record IDs and data type.
+
+        :param record_id_list: The record IDs of the descendant records to search from.
+        :param descendant_type_name: The data type name of the descendants to search from.
+        :param ancestor_type_name: The data type name of the ancestors to look for above the given record IDs.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a dictionary of the data records from the query
+            mapped by their descendant record, the current page information, and whether more pages exist after it.
         """
         record_id_list.sort()
         params = {'descendantTypeName': descendant_type_name,
                   "ancestorTypeName": ancestor_type_name}
         self._append_query_param(paging_criteria, params)
         sub_path = '/datarecordlist/ancestors'
         response = self.user.post(sub_path, params=params, payload=record_id_list)
         self.user.raise_for_status(response)
         json_dict = response.json()
         return DataRecordPojoHierarchyListPageResult.from_json(json_dict)
 
     def get_descendants(self, record_id: int, descendant_type_name: str,
                         paging_criteria: Optional[DataRecordPojoPageCriteria] = None) -> DataRecordPojoListPageResult:
         """
-        Get the descendants of the given type below the records with the given Record ID.
-        :param record_id: The Record ID of the ancestor record.
-        :param descendant_type_name: The data type name of the descendants to look for above the given Record ID.
-        :param paging_criteria: Optionally specify the page to retrieve for. Note the page size may be enforced in SaaS.
-        :return: The result descendants, of current page.
+        Get the descendants of the given data type below the record with the given record ID.
+
+        :param record_id: The record ID of the ancestor record to search from.
+        :param descendant_type_name: The data type name of the descendants to look for below the given record ID.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a list of the data records from the query,
+            the current page information, and whether more pages exist after it.
         """
         params = {'recordId': record_id,
                   'descendantTypeName': descendant_type_name}
         self._append_query_param(paging_criteria, params)
         sub_path = '/datarecord/descendants'
         response = self.user.get(sub_path, params)
         self.user.raise_for_status(response)
         json_dict = response.json()
         return DataRecordPojoListPageResult.from_json(json_dict)
 
     def get_descendants_list(self, record_id_list: List[int], descendant_type_name: str,
                              paging_criteria: Optional[DataRecordPojoHierarchyPageCriteria] = None) -> \
             DataRecordPojoHierarchyListPageResult:
         """
-        Get the descendants of the given type below the records with the given Record IDs.
-        :param record_id_list: Record IDs to get descendants of.
-        :param descendant_type_name: The data type name of the descendants to look for above the given Record ID.
-        :param paging_criteria: Optionally specify the page to retrieve for. Note the page size may be enforced in SaaS.
-        :return: The result descendants, of current page.
+        Get the descendants of the given type below the records with the given record IDs.
+
+        :param record_id_list: The record IDs of the ancestor records.
+        :param descendant_type_name: The data type name of the descendants to look for below the given record IDs.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a dictionary of the data records from the query
+            mapped by their ancestor record, the current page information, and whether more pages exist after it.
         """
         record_id_list.sort()
         params = {'descendantTypeName': descendant_type_name}
         self._append_query_param(paging_criteria, params)
         sub_path = '/datarecordlist/descendants'
         response = self.user.post(sub_path, params=params, payload=record_id_list)
         self.user.raise_for_status(response)
         json_dict = response.json()
         return DataRecordPojoHierarchyListPageResult.from_json(json_dict)
 
     def add_data_record(self, data_type_name: str) -> DataRecord:
         """
-        Create a new record of the provided data type.  Only default values and system fields will be set on the record
-        before it is stored.
+        Create a single new record of the provided data type. Only default values and system fields will be set on the
+        record before it is stored.
 
-        The record will be filled with default value, followed by changes by on-save plugins.
-        You may want to use a record setter method in this manager following this call
-        :param data_type_name: The data type of the record to create in the system.
-        :return: The record pojo representing the record that was created.
+        :param data_type_name: The data type name of the record to create in the system.
+        :return: The record object representing the data record in the system.
         """
         sub_path = '/datarecord/' + urllib.parse.quote(data_type_name)
         response = self.user.post(sub_path)
         self.user.raise_for_status(response)
         json_dict = response.json()
         return DataRecord.from_json(json_dict)
 
     def add_data_records(self, data_type_name: str, num_to_add: int) -> List[DataRecord]:
         """
-        Add multiple data records and create them with default values.
-        :param data_type_name: The data type name of added records.
-        :param num_to_add: The number of records to be added.
-        :return: The new data record pojo list.
+        Create multiple new record of the provided data type. Only default values and system fields will be set on the
+        record before it is stored.
+
+        :param data_type_name: The data type name of the records to create in the system.
+        :param num_to_add: The number of records to create.
+        :return: A list of record objects representing the data records in the system.
         """
         sub_path = '/datarecordlist/' + urllib.parse.quote(data_type_name)
         params = {'numberToAdd': num_to_add}
         response = self.user.post(sub_path, params)
         self.user.raise_for_status(response)
         json_list = response.json()
         return [DataRecord.from_json(json) for json in json_list]
 
     def add_data_records_with_data(self, data_type_name: str,
                                    field_map_list: List[Dict[str, Any]]
                                    ) -> List[DataRecord]:
         """
-        A shortcut to add data records in a list and provide data as field map list in a single call.
-        :param data_type_name: The data type name of added records.
-        :param field_map_list: The field map list of the data of the data records to be added.
+        Create new records of the provided data type in the system while also setting fields on the records before
+        they are stored.
+
+        :param data_type_name: The data type name of the records to create in the system.
+        :param field_map_list: The list of field maps of the data records to be added. Each dictionary in the list
+            represents the fields for a new record. The dictionary keys are the data field names of the fields on the
+            data type, with the dictionary values being the values that those data fields will be set to.
+        :return: A list of record objects representing the data records in the system.
         """
         sub_path = '/datarecordlist/fields/' + urllib.parse.quote(data_type_name)
         response = self.user.post(sub_path, payload=field_map_list)
         self.user.raise_for_status(response)
         json_list = response.json()
         return [DataRecord.from_json(json) for json in json_list]
 
     def set_attachment_data(self, record: DataRecord,
                             file_name: str, data_stream: IO) -> None:
         """
         Upload file bytes to be used as the attachment data for the given record.
+
         :param record: The attachment record to upload the file bytes to.
         :param file_name: The name of the file being uploaded as the attachment data.
-        :param data_stream: The stream to be consumed as upload binary data.
+        :param data_stream: The stream to be consumed as uploaded binary data.
         """
         data_type_name = record.get_data_type_name()
         record_id = record.get_record_id()
         sub_path = '/datarecord/attachment/' + urllib.parse.quote(data_type_name) + "/" + \
                    urllib.parse.quote(str(record_id)) + "/" + urllib.parse.quote(file_name)
         response = self.user.post_data_stream(sub_path, data_stream)
         self.user.raise_for_status(response)
 
     def get_attachment_data(self, record: DataRecord,
                             data_sink: Callable[[bytes], None]) -> None:
         """
         Take the attachment data stream and consume the data in a data sink method.
+
         :param record: The record to obtain attachment data from.
-        :param data_sink: The data sink method to consume data stream
+        :param data_sink: The data sink method to consume the data stream of the attachment.
         """
         data_type_name = record.get_data_type_name()
         record_id = record.get_record_id()
         sub_path = '/datarecord/attachment/' + urllib.parse.quote(data_type_name) + "/" + \
                    urllib.parse.quote(str(record_id))
         self.user.consume_octet_stream_get(sub_path, data_sink)
 
     def set_record_image(self, record: DataRecord,
                          data_stream: IO) -> None:
         """
-        Set the record image on the record defined by the data type name and record ID parameters.
-        :param record: The record to set image for.
-        :param data_stream: The stream to be consumed as upload image data.
+        Set the record image of the given data record.
+
+        :param record: The record to set the image for.
+        :param data_stream: The stream to be consumed as uploaded image data.
         """
         data_type_name = record.get_data_type_name()
         record_id = record.get_record_id()
         sub_path = '/datarecord/image/' + urllib.parse.quote(data_type_name) + "/" + \
                    urllib.parse.quote(str(record_id))
         response = self.user.post_data_stream(sub_path, data_stream)
         self.user.raise_for_status(response)
 
     def get_record_image(self, record: DataRecord,
                          data_sink: Callable[[bytes], None]) -> None:
         """
-        Get the data record image and consume it with data sink.
+        Get the record image of the given data record.
+
         :param record: The record to get image from.
-        :param data_sink: The data sink to consume image data.
+        :param data_sink: The data sink method to consume the data stream of the image.
         """
         data_type_name = record.get_data_type_name()
         record_id = record.get_record_id()
         sub_path = '/datarecord/image/' + urllib.parse.quote(data_type_name) + "/" + urllib.parse.quote(str(record_id))
         self.user.consume_octet_stream_get(sub_path, data_sink)
 
     def delete_data_record(self, record: DataRecord, recursive_delete: bool = False) -> None:
         """
-        Delete a single data record from Sapio.
+        Delete a single data record from the system.
+
         :param record: The record to be deleted.
-        :param recursive_delete: Whether we will delete the record's descendants if there is no other lineage.
+        :param recursive_delete: Whether to delete the record's descendants if there is no other lineage to those
+            records.
         """
         data_type_name = record.get_data_type_name()
         record_id = record.get_record_id()
         sub_path = '/datarecord/' + urllib.parse.quote(data_type_name) + "/" + urllib.parse.quote(str(record_id))
         params = {'recursiveDelete': recursive_delete}
         response = self.user.delete(sub_path, params)
         self.user.raise_for_status(response)
 
     def delete_data_record_list(self, delete_list: List[DataRecord], recursive_delete: bool = False) -> None:
         """
-        Recurisvely delete a list of data records.
+        Delete a list of data records from the system.
+
         :param delete_list: The record list to be deleted from Sapio.
-        :param recursive_delete: Whether we will delete the record's descendants if there is no other lineage.
+        :param recursive_delete: Whether to delete the record's descendants if there is no other lineage to those
+            records.
         """
         sub_path = '/datarecordlist/delete/'
         params = {'recursiveDelete': recursive_delete}
         response = self.user.post(sub_path, params, to_record_json_list(delete_list))
         self.user.raise_for_status(response)
 
     # noinspection PyProtectedMember,PyUnresolvedReferences
     def commit_data_records(self, records_to_update: List[DataRecord]) -> None:
         """
-        Update a list of records with their new field maps within each pojo.
-        Unlike the regular web service 'set fields for records' method, only fields that has been changed will be set.
+        Update a list of records in the system with their new field maps from the given record objects.
+
+        Unlike the regular web service 'set fields for records' method, only fields that have been changed will be set.
         Should this commit operation be successful, the field data changes being tracked will be cleared,
         and the new field maps will be committed.
-        :param records_to_update: The records to be updated.
+
+        :param records_to_update: A list of data records to be updated in the system.
         """
         sub_path = '/datarecordlist/fields'
         changed_record_list: List[DataRecord] = list()
         for record in records_to_update:
             changed_record = DataRecord(record.get_data_type_name(), record.get_record_id(),
                                         record.get_changed_fields_clone())
             changed_record_list.append(changed_record)
@@ -476,116 +544,137 @@
             for record in records_to_update:
                 record.rollback()
             raise e
 
     def add_child(self, parent_record: DataRecord, child_record: DataRecord) -> Optional[DataRecord]:
         """
         Add an existing record as a child of another existing record.
+
         :param parent_record: The parent data record to add the child record to.
         :param child_record: The child data record to be added under the parent.
+        :return: The child record that was added, expected to not be None.
         """
         sub_path = self.user.build_url(['datarecord', 'child',
                                         parent_record.get_data_type_name(), str(parent_record.get_record_id())])
         params = {'childTypeName': child_record.get_data_type_name(),
                   'childRecordId': child_record.get_record_id()}
         response = self.user.post(sub_path, params)
         self.user.raise_for_status(response)
         if self.user.is_null_response(response):
             return None
         json = response.json()
         return DataRecord.from_json(json)
 
     def add_children(self, parent_children_map: Dict[DataRecord, List[DataRecord]]) -> None:
         """
-        Add children to the parents.
-        :param parent_children_map: The map of (parent) -> (All children to be added to this parent)
+        Create multiple parent/child relationships between existing records in the system at once.
+
+        :param parent_children_map: A dictionary where the keys are the parent data records and the values are a list
+            of data records to be added as children of the key data record.
         """
         payload = dict()
         for parent, children_list in parent_children_map.items():
             if parent is None:
                 continue
             if children_list is None or len(children_list) == 0:
                 continue
             payload[parent.get_map_key_reference()] = to_record_json_list(children_list)
         sub_path = '/datarecordlist/children'
         response = self.user.put(sub_path, payload=payload)
         self.user.raise_for_status(response)
 
     def remove_children(self, parent_children_map: Dict[DataRecord, List[DataRecord]]) -> None:
         """
-        Remove children from parents.
-        :param parent_children_map: The map of (parent) -> (All children to be removed from this parent)
+        Remove multiple parent/child relationships between existing records in the system at once.
+
+        :param parent_children_map: A dictionary where the keys are the parent data records and the values are a list
+            of data records to be removed as children of the key data record.
         """
         payload = dict()
         for parent, children_list in parent_children_map.items():
             if parent is None:
                 continue
             if children_list is None or len(children_list) == 0:
                 continue
             payload[parent.get_map_key_reference()] = to_record_json_list(children_list)
         sub_path = '/datarecordlist/children/delete'
         response = self.user.post(sub_path, payload=payload)
         self.user.raise_for_status(response)
 
     def add_children_for_record(self, parent: DataRecord, child_list: List[DataRecord]) -> None:
         """
-        Add children of a data record POJO.
-        :param parent: The parent record.
-        :param child_list: The children list to be added to this parent record.
+        Add a list of existing records as children of another existing record.
+
+        :param parent: The parent data record to add the child record to.
+        :param child_list: A list of the children data records to be added under the parent.
         """
         data_type_name = parent.get_data_type_name()
         record_id = parent.get_record_id()
         sub_path = '/datarecord/children/' + urllib.parse.quote(data_type_name) + \
                    "/" + urllib.parse.quote(str(record_id))
         response = self.user.put(sub_path, payload=to_record_json_list(child_list))
         self.user.raise_for_status(response)
 
     def create_children_for_record(self, parent: DataRecord,
                                    child_type_name: str, num_to_add: int) -> List[DataRecord]:
         """
-        Add new children for a parent record.
-        :param parent: The parent data record.
-        :param child_type_name: The child data type name.
-        :param num_to_add: The number of children to be created.
+        Create multiple new record of the provided data type while at the same time adding them as children of an
+        existing data record. Only default values and system fields will be set on the record before it is stored.
+
+        :param parent: The existing parent data record.
+        :param child_type_name: The data type name of the child records that will be created.
+        :param num_to_add: The number of child records to be created.
+        :return: A list of record objects representing the child data records in the system.
         """
         sub_path = self.user.build_url(['datarecord', 'children',
                                         parent.get_data_type_name(), str(parent.get_record_id())])
         params = {'childTypeName': child_type_name, 'numberToAdd': num_to_add}
         response = self.user.post(sub_path, params=params)
         self.user.raise_for_status(response)
         json_list = response.json()
         return [DataRecord.from_json(json) for json in json_list]
 
     def create_children_fields_for_record(self, parent: DataRecord, child_type_name: str,
                                           child_field_list: List[Dict[str, Any]]) -> \
             List[DataRecord]:
         """
-        Create children prefilled with values in field map list.
+        Create new records of the provided data type in the system while also setting fields on the records before
+        they are stored and adding them as children of an existing data record.
+
         :param parent: The parent to create children for.
-        :param child_type_name: The children's data type name.
-        :param child_field_list: The field map list of data in the new children.
-        :return: The newly created children records.
+        :param child_type_name: The data type name of the child records to create in the system.
+        :param child_field_list: The list of field maps of the data records to be added. Each dictionary in the list
+            represents the fields for a new record. The dictionary keys are the data field names of the fields on the
+            data type, with the dictionary values being the values that those data fields will be set to.
+        :return: A list of record objects representing the child data records in the system.
         """
         sub_path = self.user.build_url(['datarecord', 'children', 'fields',
                                         parent.get_data_type_name(), str(parent.get_record_id())])
         params = {'childTypeName': child_type_name}
         response = self.user.post(sub_path, params, child_field_list)
         self.user.raise_for_status(response)
         json_list = response.json()
         return [DataRecord.from_json(json) for json in json_list]
 
     def create_children_fields_for_parents(self, child_type_name: str,
                                            children_field_map_list_by_parent:
                                            Dict[DataRecord, List[Dict[str, Any]]]
                                            ) -> Dict[DataRecord, List[DataRecord]]:
         """
-        Create new children for parents.
-        :param child_type_name The data type name for all new children records.
-        :param children_field_map_list_by_parent: a map of (parent) -> (list of new children data field map list)
-        :return: a map of (parent) -> (newly created children data record list)
+        Create new records of the provided data type in the system while also setting fields on the records before
+        they are stored and creating multiple parent/child relationships between the new records and existing records
+        in the system at once.
+        
+        :param child_type_name: The data type name of the child records to create in the system.
+        :param children_field_map_list_by_parent: A dictionary where the keys are the parent data records and the values
+            are a list of field maps to create records that will be added as children of the key data record. Each
+            dictionary in this list represents the fields for a new record. The dictionary keys are the data field names
+            of the fields on the data type, with the dictionary values being the values that those data fields will be
+            set to.
+        :return: A dictionary mapping each parent record to a list of their newly created child data records.
         """
         parent_record_by_map_key = {rec.get_map_key_reference(): rec for rec in
                                     children_field_map_list_by_parent.keys()}
 
         sub_path = self.user.build_url(['datarecordlist', 'children'])
         params = {'childTypeName': child_type_name}
         payload: Dict[str, List[Dict[str, Any]]] = dict()
@@ -604,57 +693,68 @@
             value_list = from_json_record_list(value)
             ret[key_pojo] = value_list
         return ret
 
     def has_access(self, access_type: SapioAccessType, record_list: List[DataRecord]) -> \
             List[DataRecord]:
         """
-        Check to see if the user requesting the operation has the requested access to the provided records.
-        :param access_type: The type of access to check for.
-        :param record_list: List of records to check access for.
-        :return: A sub-list of original list of records that have the requested access.
+        Check if the user has the given access type to the provided records.
+
+        :param access_type: The type of access to check for. Access types that can be checked are read, write, and
+            delete permissions.
+        :param record_list: The list of records to check access for.
+        :return: A sub-list of the original list of records that have the requested access; if the input and output
+            are equivalent then the user has the requested access for all records of the input, while if the output
+            is empty then the user has access to none of the input records.
         """
         sub_path = self.user.build_url(['datarecord', 'access', access_type.name])
         payload = to_record_json_list(record_list)
         response = self.user.post(sub_path, payload=payload)
         self.user.raise_for_status(response)
         json = response.json()
         return from_json_record_list(json)
 
     def add_data_records_data_pump(self, data_type_name: str, field_map_list: List[Dict[str, Any]]) -> List[int]:
         """
-        Create New High Volume Records Via Data Pump With Field Maps.
+        Create new high volume data type records in the system while also setting their fields.
 
-        This method can only be used to support the creation of High Volume data types.
+        This call will bypass overhead surrounding the creation of data records in the server and directly stream data
+        to the database. Intended for creating a large number of HVDT records at once.
 
-        It will bypass many overheads surrounding object creations of data records in server and directly stream data
-        to the database. This method cannot return DataRecord objects and can only provide you the new record id list.
-        :param data_type_name: The data type name to insert records for.
-        :param field_map_list: The field map list to add to data type.
-        :return: The ordered list of record IDs that are added to DB, in the same order as original field map list data.
+        :param data_type_name: The data type name to insert records for. The data type must be a high volume data type.
+        :param field_map_list: The list of field maps of the data records to be added. Each dictionary in the list
+            represents the fields for a new record. The dictionary keys are the data field names of the fields on the
+            data type, with the dictionary values being the values that those data fields will be set to.
+        :return: An ordered list of record IDs of the records that were added to the database, in the same order as
+            the input field map list data.
         """
         sub_path = self.user.build_url(['datarecordlist', 'fields', data_type_name, 'datapump'])
         response = self.user.post(sub_path, payload=field_map_list)
         self.user.raise_for_status(response)
         ret: List[int] = response.json()
         return ret
 
     def add_children_data_pump(self, child_type_name: str,
                                parent_child_field_map: Dict[DataRecord, List[Dict[str, Any]]]) \
             -> Dict[DataRecord, List[int]]:
         """
-        Create New High Volume Children Via Data Pump For Parent List.
+        Create new high volume data type records in the system while also setting their fields and creating multiple
+        parent/child relationships between the new records and existing records in the system at once.
 
-        This method can only be used to support the creation of High Volume data types.
+        This call will bypass overhead surrounding the creation of data records in the server and directly stream data
+        to the database. Intended for creating a large number of HVDT records at once.
 
-        It will bypass many overheads surrounding object creations of data records in server and directly stream data
-        to the database. This method cannot return DataRecord objects and can only provide you the new record id list.
-        :param child_type_name: The data type name of the new children for these data records.
-        :param parent_child_field_map: The dictionary of (Parent Data Record) -> (List of new children field map data)
-        :return: The dictionary of (Parent Data Record) -> (List of new children record ID in order of field map list)
+        :param child_type_name: The data type name to insert records for. The data type must be a high volume data type.
+        :param parent_child_field_map: A dictionary where the keys are the parent data records and the values
+            are a list of field maps to create records that will be added as children of the key data record. Each
+            dictionary in this list represents the fields for a new record. The dictionary keys are the data field names
+            of the fields on the data type, with the dictionary values being the values that those data fields will be
+            set to.
+        :return: A dictionary mapping each parent record to a list of the record IDs of their newly created children.
+            The record ID lists are in the same order as the field map lists from the input.
         """
         sub_path = self.user.build_url(['datarecordlist', 'children', 'datapump'])
         params = {
             'childTypeName': child_type_name
         }
         map_key_to_record: Dict[str, DataRecord] = dict()
         parent_child_field_map_pojo: Dict[str, List[Dict[str, Any]]] = dict()
@@ -672,21 +772,25 @@
         return ret
 
     def get_side_link_to_list(self, data_record_list: List[DataRecord], linked_data_type_name: str,
                               side_link_field_name: str, paging_criteria: Optional[DataRecordSideLinkToPageCriteria]
                               = None) -> DataRecordSideLinkToListPageResult:
         """
         Get the side linked records of the given type that point back to the given records.
+        
         :param data_record_list: The list of records to retrieve side links to.
         :param linked_data_type_name: The data type name of the side linked records.
-        :param side_link_field_name: The data field name on the linkedDataTypeName that points back to the given records.
-        :param paging_criteria: The current page to retrieve.
-        :return:  An object containing a map from the record key 'DataTypeName:RecordId' to arrays of data records that
-         are side linked to the provided list of Records as well as a criteria object that details how to retrieve the
-         next page of data.
+        :param side_link_field_name: The data field name on the linked_data_type_name that points back to the given
+            records.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a dictionary from the record key
+            'DataTypeName:RecordId' to arrays of data records that are side linked to the provided list of records,
+            the current page information, and whether more pages exist after it.
         """
         data_record_list.sort()
         params = {'linkedDataTypeName': linked_data_type_name,
                   'sideLinkedFieldName': side_link_field_name}
         self._append_query_param(paging_criteria, params)
         sub_path = '/datarecordlist/sidelinksto'
         request_body = [x.to_json() for x in data_record_list]
@@ -696,20 +800,23 @@
         return DataRecordSideLinkToListPageResult.from_json(json_dict)
 
     def get_side_link_from_list(self, data_record_list: List[DataRecord], side_link_field_name: str,
                                 paging_criteria: Optional[DataRecordSideLinkFromPageCriteria] = None) -> \
             DataRecordSideLinkFromListPageResult:
         """
         Get the side linked records from the given records referenced by the given field name.
-        :param data_record_list: The list of records to retrieve side links.
+        
+        :param data_record_list: The list of records to retrieve side links from.
         :param side_link_field_name: The data field name on the given record that points to the records to retrieve.
-        :param paging_criteria: The current page to retrieve.
-        :return: An object containing a map from the record key 'DataTypeName:RecordId'
-        to arrays of data records that are side linked from the provided list of Records as well as a criteria object
-        that details how to retrieve the next page of data.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a dictionary from the record key
+            'DataTypeName:RecordId' to arrays of data records that are side linked from the provided list of records,
+            the current page information, and whether more pages exist after it.
         """
         data_record_list.sort()
         params = {'sideLinkedFieldName': side_link_field_name}
         self._append_query_param(paging_criteria, params)
         sub_path = '/datarecordlist/sidelinksfrom'
         request_body = [x.to_json() for x in data_record_list]
         response = self.user.post(sub_path, params, request_body)
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/DataService.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataService.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,34 +15,40 @@
 
     __instances: WeakValueDictionary[SapioUser, DataManager] = WeakValueDictionary()
     __initialized: bool
 
     def __new__(cls, user: SapioUser):
         """
         Observes singleton pattern per record model manager object.
+
+        :param user: The user that will make the webservice request to the application.
         """
         obj = cls.__instances.get(user)
         if not obj:
             obj = object.__new__(cls)
             obj.__initialized = False
             cls.__instances[user] = obj
         return obj
 
     def __init__(self, user: SapioUser):
+        """
+        :param user: The user that will make the webservice request to the application.
+        """
         if self.__initialized:
             return
         self.user = user
         self.__initialized = True
 
     def export_to_xml(self, records: List[DataRecord],
                       data_sink: Callable[[bytes], None],
                       recursive: bool = True,
                       data_types_to_exclude: Optional[List[str]] = None) -> None:
         """
         Export records into zipped XML. The format will be .xml.gz
+
         :param records: The records to be exported.
         :param data_sink: The sink to receive exported data.
         :param recursive: whether to recursively export all descendant records.
         :param data_types_to_exclude: a black list of data type names.
         """
         sub_path = self.user.build_url(['datamanager', 'exportxml'])
         params = {'dataTypesToExclude': data_types_to_exclude,
@@ -53,14 +59,15 @@
             payload.append(desc.to_json())
         self.user.consume_octet_stream_post(sub_path, data_sink, params=params, payload=payload)
 
     def import_from_xml(self, parent_record: DataRecord, data_stream: IO,
                         skip_top_level: bool = False) -> None:
         """
         Import records as children of a parent data record from a .xml.gz file
+
         :param parent_record: The parent record to import under.
         :param data_stream: The data IO containing the zipped xml
         :param skip_top_level: Whether to skip top-level records we are importing in XML.
         """
         sub_path = self.user.build_url(['datamanager', 'importxml',
                                         parent_record.data_type_name, str(parent_record.record_id)])
         params = {'skipTopLevel': skip_top_level}
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataTypeService.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 from typing import Any, Dict, List
 from weakref import WeakValueDictionary
 
 from sapiopylib.rest.User import SapioUser
 from sapiopylib.rest.pojo.datatype.DataType import DataTypeDefinition, DataTypeParser
-from sapiopylib.rest.pojo.datatype.DataTypeLayout import DataTypeLayoutParser
+from sapiopylib.rest.pojo.datatype.DataTypeLayout import DataTypeLayoutParser, DataTypeLayout
 from sapiopylib.rest.pojo.datatype.FieldDefinition import FieldDefinitionParser, AbstractVeloxFieldDefinition
 
 
 class DataTypeManager:
     """
     Obtain information about data types in the system.
     """
@@ -16,66 +16,83 @@
 
     __instances: WeakValueDictionary[SapioUser, DataTypeManager] = WeakValueDictionary()
     __initialized: bool
 
     def __new__(cls, user: SapioUser):
         """
         Observes singleton pattern per record model manager object.
+
+        :param user: The user that will make the webservice request to the application.
         """
         obj = cls.__instances.get(user)
         if not obj:
             obj = object.__new__(cls)
             obj.__initialized = False
             cls.__instances[user] = obj
         return obj
 
     def __init__(self, user: SapioUser):
+        """
+        Obtains a data type manager to query data type definitions.
+
+        :param user: The user that will make the webservice request to the application.
+        """
         if self.__initialized:
             return
         self.user = user
         self.__initialized = True
 
     def get_field_definition_list(self, data_type_name: str) -> List[AbstractVeloxFieldDefinition]:
         """
-        Get the list of field definitions that back the provided data type. These fields can be
+        Get the field definitions for every field on the provided data type. These fields can be
         used to know what fields will be returned when getting records of this type.
-        :param data_type_name: The data type name of the type containing the field definitions to return.
+
+        :param data_type_name: The data type name of a data type in the system.
+        :return: A list of the field definitions for every field on the provided dat type.
         """
         sub_path: str = self.user.build_url(['datatypemanager', 'veloxfieldlist', data_type_name])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         json_list: List[Dict[str, Any]] = response.json()
         return [FieldDefinitionParser.to_field_definition(x) for x in json_list]
 
     def get_data_type_name_list(self) -> List[str]:
         """
-        The list of all data type names that exist in the system.
-        These data type names can be used to query for fields and records of that type.
-        The names can also be used to get field definitions of the type to know what fields can be retrieved.
+        Get all data type names that exist in the system. These data type names can be used to determine which
+        data record can be queried or created in the system and to query information about specific data types.
+
+        :return: A list of all data type names from the system.
         """
         sub_path: str = '/datatypemanager/datatypenamelist'
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         json_list: List[str] = response.json()
         return json_list
 
     def get_data_type_definition(self, data_type_name: str) -> DataTypeDefinition:
         """
-        Get Data Type Definition
-        :param data_type_name: The data type name of the data type definition to return.
+        Get the data type definition for the given data type. The data type definition can be used to determine a data
+        type's display name, plural name, allowable record relationships, and more.
+
+        :param data_type_name: The data type name of a data type in the system.
+        :return: The data type definition of the given data type.
         """
         sub_path: str = self.user.build_url(['datatypemanager', 'datatypedefinition', data_type_name])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         json_dct = response.json()
         return DataTypeParser.parse_data_type_definition(json_dct)
 
-    def get_data_type_layout_list(self, data_type_name: str):
+    def get_data_type_layout_list(self, data_type_name: str) -> List[DataTypeLayout]:
         """
-        Get all available layouts for the provided data type name.
-        :param data_type_name: The data type name to get layouts for.
+        Get all available layouts for the provided data type name. Layouts are how records are displayed to users in the
+        system. They can be used by TemporaryDataTypes and DataRecordDialogRequests to control how client callbacks are
+        displayed to the user.
+
+        :param data_type_name: The data type name of a data type in the system.
+        :return: A list of all data type layouts for the provided data type.
         """
         sub_path: str = self.user.build_url(['datatypemanager', 'layout', data_type_name])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         json_list: List[Dict[str, Any]] = response.json()
         return [DataTypeLayoutParser.parse_layout(x) for x in json_list]
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/ELNService.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,381 +23,428 @@
 
     __instances: WeakValueDictionary[SapioUser, ElnManager] = WeakValueDictionary()
     __initialized: bool
 
     def __new__(cls, user: SapioUser):
         """
         Observes singleton pattern per record model manager object.
+
+        :param user: The user that will make the webservice request to the application.
         """
         obj = cls.__instances.get(user)
         if not obj:
             obj = object.__new__(cls)
             obj.__initialized = False
             cls.__instances[user] = obj
         return obj
 
     def __init__(self, user: SapioUser):
+        """
+        Obtain an ELN manager to perform ELN operations.
+
+        :param user: The user that will make the webservice request to the application.
+        """
         if self.__initialized:
             return
         self.user = user
         self.__initialized = True
 
     def create_notebook_experiment(self, pojo: InitializeNotebookExperimentPojo) -> ElnExperiment:
         """
-        Use the provided criteria to create a new Notebook Experiment.
-        :param pojo: The details about how to create the experiment.
-        :return: The new experiment's info data.
+        Use the provided criteria to create a new notebook experiment.
+
+        :param pojo: The criteria for the creation of the new experiment.
+        :return: An object representing the new experiment that was created in the system.
         """
         sub_path = '/eln/notebookexperiment/'
         response = self.user.post(sub_path, payload=pojo.to_json())
         self.user.raise_for_status(response)
         json_dict = response.json()
         return ELNExperimentParser.parse_eln_experiment(json_dict)
 
     def delete_notebook_experiment(self, notebook_experiment_id: int) -> None:
         """
         Delete a notebook experiment when providing a notebook experiment ID.
+
+        :param notebook_experiment_id: The notebook experiment ID of the experiment to delete.
         """
         subpath = self.user.build_url(['eln', 'experiment', str(notebook_experiment_id)])
         response = self.user.delete(subpath)
         self.user.raise_for_status(response)
 
     def get_template_experiment_list(self, query: TemplateExperimentQueryPojo) -> List[ElnTemplate]:
         """
-        Get a list of TemplateExperimentPojo objects using the provided criteria object to search
-        the templates in the app.
-        :return: List of templates matching the provided criteria in the system.
+        Get a list of experiment template from the system that match the provided query criteria.
+
+        :param query: Search criteria for finding experiment templates.
+        :return: A list of templates matching the provided criteria in the system.
         """
         sub_path = "/eln/templateexperiment/"
         response = self.user.post(sub_path, payload=query.to_json())
         self.user.raise_for_status(response)
         json_list: List[Dict[str, Any]] = response.json()
         return [ELNExperimentParser.parse_template_experiment(x) for x in json_list]
 
     def get_experiment_entry_list(self, eln_experiment_id: int, to_retrieve_field_definitions: bool = False) \
             -> List[ExperimentEntry]:
         """
-        Get all experiment entries for an ELN experiment.
-        :param eln_experiment_id: The ELN experiment ID these entries are made under.
-        :param to_retrieve_field_definitions: If true, the resulting entries will be filled with field definition data.
-        :return: The experiment entry data list.
+        Get all the experiment entries for an ELN experiment.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param to_retrieve_field_definitions: If true, the returned experiment entry objects will contain field
+            definitions for the fields that are present in the entry (e.g. the columns of a table entry or fields of a
+            form entry).
+        :return: A list of experiment entries from the given experiment.
         """
         sub_path = self.user.build_url(['eln', 'getExperimentEntryList', str(eln_experiment_id)])
         params = {
             'retrieveDataDefinitions': to_retrieve_field_definitions
         }
         response = self.user.get(sub_path, params)
         self.user.raise_for_status(response)
         json_list: List[Dict[str, Any]] = response.json()
         return [ExperimentEntryParser.parse_experiment_entry(x) for x in json_list]
 
     def get_experiment_entry(self, eln_experiment_id: int, entry_id: int,
                              to_retrieve_field_definitions: bool = False) -> Optional[ExperimentEntry]:
         """
-        Get a specific entry from ELN experiment.
-        :param eln_experiment_id: The ELN experiment ID the entry was created under.
-        :param entry_id: The Experiment ID entry we are searching for.
-        :param to_retrieve_field_definitions:  If true, the resulting entries will be filled with field definition data.
-        :return: The experiment entry if exists, or None if not.
+        Get a specific entry from an ELN experiment given its entry ID.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param entry_id: The entry ID of the entry.
+        :param to_retrieve_field_definitions: If true, the returned experiment entry objects will contain field
+            definitions for the fields that are present in the entry (e.g. the columns of a table entry or fields of a
+            form entry).
+        :return: The experiment entry that matches the input if it exists, or None if it does not.
         """
         sub_path = self.user.build_url(['eln', 'getExperimentEntry', str(eln_experiment_id), str(entry_id)])
         params = {
             'retrieveDataDefinitions': to_retrieve_field_definitions
         }
         response = self.user.get(sub_path, params)
         self.user.raise_for_status(response)
         json_dct: Optional[Dict[str, Any]] = response.json()
         if json_dct is None:
             return None
         return ExperimentEntryParser.parse_experiment_entry(json_dct)
 
-    def get_eln_experiment_by_record_id(self, record_id: int):
+    def get_eln_experiment_by_record_id(self, record_id: int) -> ElnExperiment:
         """
-        Given the record ID of the data record that is the title record of the experiment entry, find the experiment.
+        Given the record ID of the experiment data record for a notebook, find the ELN experiment.
+        This can be useful when trying to retrieve ELN experiments from the global data type hierarchy.
 
-        This can be useful when trying to retrieve ELN experiment from global data type hierarchy.
+        :param record_id: The record ID of the experiment record.
+        :return: The ELN experiment for the matching experiment record.
         """
         sub_path = '/eln/queryExperimentByRecordId'
         params = {
             'recordId': record_id
         }
         response = self.user.get(sub_path, params)
         self.user.raise_for_status(response)
         return ELNExperimentParser.parse_eln_experiment(response.json())
 
     def get_eln_experiment_list(self, owner_username: Optional[str] = None,
                                 status_types: Optional[List[ExperimentEntryStatus]] = None) \
             -> List[ElnExperiment]:
         """
-        Retrieves the metadata of notebook experiments in the system. It may run faster when filters are specified.
-        :param owner_username: The owner filter specifies that notebook experiment must be owned by
-        this user to be retrieved.
-        :param status_types: The status type specifies the notebook experiment must have one of
-        these statuses to be retrieved.
-        :return:
+        Get the ELN experiments from the system that match the basic input parameters.
+
+        :param owner_username: If specified, filter to only those experiments that are owned by the user with this name.
+        :param status_types: If specified, filter to only those experiments with the matching status.
+        :return: A list of ELN experiments that match the input search criteria.
         """
         sub_path = '/eln/getExperimentInfoList'
         params = dict()
         if owner_username is not None:
             params['ownerUsername'] = owner_username
         if status_types is not None:
             params['statusTypes'] = [x.name for x in status_types]
         response = self.user.get(sub_path, params)
         self.user.raise_for_status(response)
         json_list: List[Dict[str, Any]] = response.json()
         return [ELNExperimentParser.parse_eln_experiment(x) for x in json_list]
 
     def get_eln_experiment_by_criteria(self, criteria: ElnExperimentQueryCriteria) -> List[ElnExperiment]:
         """
-        Searches ELN experiment by a complex query criteria object
-        :param criteria: The search request details
-        :return: A list of ELN experiments.
+        Get the ELN experiments from the system that match the complex search criteria.
+
+        :param criteria: The complex search criteria for the experiments.
+        :return: A list of ELN experiments that match the input search criteria.
         """
         sub_path = '/eln/queryExperimentByCriteria'
         response = self.user.post(sub_path, payload=criteria.to_json())
         self.user.raise_for_status(response)
         json_list: List[Dict[str, Any]] = response.json()
         return [ELNExperimentParser.parse_eln_experiment(x) for x in json_list]
 
     def get_eln_experiment_by_id(self, eln_experiment_id: int) -> Optional[ElnExperiment]:
         """
-        Get the ELN experiment by its experiment ID.
-        :param eln_experiment_id: The experiment ID to search for.
+        Get an ELN experiment by its notebook experiment ID.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
         :return: The ELN experiment object. Returns None if it does not exist, or the current user does not have access.
         """
         criteria = ElnExperimentQueryCriteria(notebook_experiment_id_white_list=[eln_experiment_id])
         results = self.get_eln_experiment_by_criteria(criteria)
         if results:
             return results[0]
         return None
 
     def add_experiment_entry(self, eln_experiment_id: int, entry_criteria: ElnEntryCriteria) -> ExperimentEntry:
         """
-        Creates a new entry under the ELN experiment. May pre-populate with data.
-        :param eln_experiment_id: The experiment ID to create the entry under.
-        :param entry_criteria The criteria specifies how we the new entry should be.
-        :return:the entry created if successful, without field definitions.
+        Create a new entry under in an ELN experiment.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param entry_criteria: The creation criteria for the new experiment entry.
+        :return: The experiment entry that was created. This entry object will not contain field definitions.
         """
         sub_path = self.user.build_url(['eln', 'addExperimentEntry', str(eln_experiment_id)])
         response = self.user.post(sub_path, payload=entry_criteria.to_json())
         self.user.raise_for_status(response)
         json_dct: Dict[str, Any] = response.json()
         return ExperimentEntryParser.parse_experiment_entry(json_dct)
 
     def add_predefined_entry_fields(self, eln_experiment_id: int, entry_id: int,
                                     predefined_field_name_list: List[str]) -> ExperimentEntry:
         """
-        Add additional predefined fields to ELN experiment entry.
-        :param eln_experiment_id: The experiment ID the entry is under.
-        :param entry_id: The entry ID in experiment to modify.
-        :param predefined_field_name_list: The predefined field list to be added to experiment entry.
-        :return: The entry with field definitions filled in after processing.
+        Add additional predefined fields to an ELN experiment entry.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param entry_id: The entry ID of the entry.
+        :param predefined_field_name_list: A list of the predefined fields to be added to the experiment entry.
+        :return: The entry that the fields were added to with updated field definitions.
         """
         sub_path = self.user.build_url(['eln', 'addPredefinedEntryFields', str(eln_experiment_id), str(entry_id)])
         response = self.user.post(sub_path, payload=predefined_field_name_list)
         self.user.raise_for_status(response)
         json_dct: Dict[str, Any] = response.json()
         return ExperimentEntryParser.parse_experiment_entry(json_dct)
 
     def get_predefined_fields(self, eln_base_data_type: ElnBaseDataType) -> List[AbstractVeloxFieldDefinition]:
         """
-        Given the base ELN data type, what are the available pre-defined fields in the system?
-        :param eln_base_data_type: The base data type to query.
-        :return: All defined field definitions for this ELN data type.
+        Determine what the available predefined fields in the system are for an entry given its base ELN data type.
+
+        :param eln_base_data_type: The base data type of the ELN entry. This includes ELNExperiment,
+            ELNExperimentDetail, and ELNSampleDetail entries.
+        :return: All predefined field definitions for this ELN data type.
         """
         sub_path = self.user.build_url(['eln', 'getPredefinedFields', eln_base_data_type.data_type_name])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         json_list: List[Dict[str, Any]] = response.json()
         return [FieldDefinitionParser.to_field_definition(x) for x in json_list]
 
     def get_predefined_field_by_id(self, field_id: int) -> AbstractVeloxFieldDefinition:
         """
-        Given the base ELN data type and the predefined field ID, retrieve its full definition. Error 422 if not found.
+        Given a predefined field ID, retrieve its full field definition.
+
         :param field_id: The system generated ID for the predefined field.
-        :return: The field definition.
+        :return: The field definition for the matching predefined field.
         """
         sub_path = self.user.build_url(['eln', 'getPredefinedFieldById', str(field_id)])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         json_dct: Dict[str, Any] = response.json()
         return FieldDefinitionParser.to_field_definition(json_dct)
 
     def get_predefined_field_by_name(self, eln_base_data_type: ElnBaseDataType, field_name: str) \
             -> AbstractVeloxFieldDefinition:
         """
-        Given the base ELN data type and name created by administrator, retrieve its full definition.
-        Error 422 if not found.
-        :param eln_base_data_type: The base data type to query.
-        :param field_name: The unique identifier defined by administrator for the field.
-        :return: The field definition.
+        Given the base ELN data type and data field name of a predefined field, retrieve its full field definition.
+
+        :param eln_base_data_type: The base data type of the entry type that the predefined field is for. This includes
+            ELNExperiment, ELNExperimentDetail, and ELNSampleDetail entries.
+        :param field_name: The data field name of the predefined field.
+        :return: The field definition for the matching predefined field.
         """
         sub_path = self.user.build_url(['eln', 'getPredefinedFieldByName', eln_base_data_type.data_type_name,
                                         field_name])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         json_dct: Dict[str, Any] = response.json()
         return FieldDefinitionParser.to_field_definition(json_dct)
 
     def get_data_records_for_entry(self, eln_experiment_id: int, entry_id: int,
                                    paging_criteria: DataRecordPojoPageCriteria = None) -> DataRecordPojoListPageResult:
         """
-        Retrieve the data records that will be displayed inside the entry.
-        :param eln_experiment_id: The experiment ID the entry is under.
-        :param entry_id: The entry ID in experiment to get records for
-        :param paging_criteria: Optional criteria for next page info, when retrieving the next page.
-        :return: The current page of data record results.
+        Get the data records that are associated with the given entry.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param entry_id: The entry ID of the entry.
+        :param paging_criteria: Optional paging criteria info for the current page. Note the maximum page size may be
+            enforced by the system. If it is, a page size must be given that is less than or equal to the maximum.
+            If not provided, returns the first page of results.
+        :return: The query results from the current page, containing a list of the data records from the query,
+            the current page information, and whether more pages exist after it.
         """
         sub_path = self.user.build_url(['eln', 'getDataRecordsForEntry', str(eln_experiment_id), str(entry_id)])
         params = dict()
         if paging_criteria is not None:
             params['lastRetrievedRecordId'] = paging_criteria.last_retrieved_record_id
             params['pageSize'] = paging_criteria.page_size
         response = self.user.get(sub_path, params)
         self.user.raise_for_status(response)
         json_dct: Dict[str, Any] = response.json()
         return DataRecordPojoListPageResult.from_json(json_dct)
 
     def submit_experiment_entry(self, eln_experiment_id: int, entry_id: int) -> None:
         """
-        Submitting an entry locks down the entry. If the entry enters completed status (default),
-        then dependent steps becomes available.
-        :param eln_experiment_id: The experiment ID the entry is under.
-        :param entry_id: The entry ID of the entry to be locked down.
+        Submit the given experiment entry. This locks down the entry and will cause any entries that are dependent
+        upon this one to become enabled.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param entry_id: The entry ID of the entry.
         """
         sub_path = self.user.build_url(['eln', 'submitExperimentEntry', str(eln_experiment_id), str(entry_id)])
         response = self.user.post(sub_path)
         self.user.raise_for_status(response)
 
     def add_records_to_table_entry(self, eln_experiment_id: int, entry_id: int,
                                    records_to_add: List[DataRecord]) -> None:
         """
-        Add one or more data records to an experiment table entry.
-        :param eln_experiment_id: The experiment ID the entry is under.
-        :param entry_id: The entry ID in experiment to modify. Must be a table entry.
-        :param records_to_add: These may be new or existing records. To add an existing record, fill in the record ID.
-        If the record ID is not specified, it is assumed that this is a new record.
-        Any field updates will be in the field map of the DataRecordPojo.
-        If the field do not exist, then the service do not perform field updates on the data record.
+        Add data records to an experiment table entry.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param entry_id: The entry ID of the entry. This ID must correspond to a table entry.
+        :param records_to_add: A list of data records to add to the corresponding experiment table entry. These data
+            records do not need to already exist in the system. If the data record objects lack record IDs, then
+            the system will create the data records alongside adding them to the experiment entry. If the data records
+            do already exist, then the records are only added to the entry; no field updates will be performed.
         """
         sub_path = self.user.build_url(['eln', 'addRecordsToTableEntry', str(eln_experiment_id), str(entry_id)])
         record_pojo_list = [x.to_json() for x in records_to_add]
         response = self.user.post(sub_path, payload=record_pojo_list)
         self.user.raise_for_status(response)
 
     def remove_records_from_table_entry(self, eln_experiment_id: int, entry_id: int,
                                         record_id_remove_list: List[int]) -> None:
         """
-        Remove one or more data records from an experiment entry
-        :param eln_experiment_id: The experiment ID the entry is under.
-        :param entry_id: The entry ID in experiment to modify. Must be a table entry.
-        :param record_id_remove_list: A list of record ID integers to remove.
+        Remove data records from an experiment table entry.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param entry_id: The entry ID of the entry. This ID must correspond to a table entry.
+        :param record_id_remove_list: A list of record IDs corresponding to the records that should be removed from the
+            entry.
         """
         sub_path = self.user.build_url(['eln', 'removeRecordsFromTableEntry', str(eln_experiment_id), str(entry_id)])
         response = self.user.post(sub_path, payload=record_id_remove_list)
         self.user.raise_for_status(response)
 
     def update_experiment_entry(self, eln_experiment_id: int, entry_id: int,
                                 entry_update_criteria: AbstractElnEntryUpdateCriteria) -> None:
         """
-        Updates some metadata of an experiment entry.
-        :param eln_experiment_id: The experiment ID the entry is under.
-        :param entry_id: The entry ID in experiment to modify. Must be a table entry.
-        :param entry_update_criteria: The update fields are all optional.
-        If the update is only to be performed on some properties, may leave out the unrelated properties from the
-        JSON passed in.
+        Update the metadata of an experiment entry. Possible metadata changes include the entry's name, status,
+        entry options, and more.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param entry_id: The entry ID of the entry.
+        :param entry_update_criteria: The update criteria for the experiment entry.
         """
         sub_path = self.user.build_url(['eln', 'updateExperimentEntry', str(eln_experiment_id), str(entry_id)])
         response = self.user.post(sub_path, payload=entry_update_criteria.to_json())
         self.user.raise_for_status(response)
 
     def update_notebook_experiment(self, eln_experiment_id: int,
                                    experiment_update_criteria: ElnExperimentUpdateCriteria) -> None:
         """
-        Updates some metadata of a notebook experiment.
-        :param eln_experiment_id: The experiment ID of the experiment being edited.
-        :param experiment_update_criteria:The update fields are all optional.
-        If the update is only to be performed on some properties, may leave out the unrelated properties as 'None'
+        Update the metadata of a notebook experiment. Possible metadata changes include the experiment's name, status,
+        and experiment options.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param experiment_update_criteria: The update criteria for the ELN experiment.
         """
         sub_path = self.user.build_url(['eln', 'updateNotebookExperiment', str(eln_experiment_id)])
         response = self.user.post(sub_path, payload=experiment_update_criteria.to_json())
         self.user.raise_for_status(response)
 
     def get_experiment_entry_options(self, eln_experiment_id: int, entry_id: int) -> Dict[str, str]:
         """
-        Get the current experiment entry options. These may be used to store plugin data or configurations.
-        :param eln_experiment_id: The ELN experiment ID the entry is under.
-        :param entry_id: The entry ID of the entry to get options for.
+        Get the entry options from an experiment entry. These may be used to store plugin or configuration data.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param entry_id: The entry ID of the entry.
+        :return: A dictionary of the experiment entry options.
         """
         sub_path = self.user.build_url(['eln', 'getExperimentEntryOptions', str(eln_experiment_id), str(entry_id)])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         return response.json()
 
     def get_notebook_experiment_options(self, eln_experiment_id: int) -> Dict[str, str]:
         """
-        Get the current notebook experiment options. These may be used to store plugin data or configurations.
-        :param eln_experiment_id: The ELN experiment ID to get the options for.
-        :return:
+        Get the experiment options from an ELN experiment. These may be used to store plugin or configuration data.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :return: A dictionary of the experiment entry options.
         """
         sub_path = self.user.build_url(['eln', 'getNotebookExperimentOptions', str(eln_experiment_id)])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         return response.json()
 
     # FR-51551 Added method
     def transfer_ownership(self, eln_experiment_id: int, new_owner_username: str) -> None:
         """
         Transfer ownership of an experiment to a new user.
-        :param eln_experiment_id: The ELN experiment ID to transfer ownership.
-        :param new_owner_username: The new owner username.
+
+        :param eln_experiment_id: The notebook experiment ID of the experiment.
+        :param new_owner_username: The new owner's username.
         """
         sub_path: str = self.user.build_url(['eln', 'changeOwner', str(eln_experiment_id), new_owner_username])
         response = self.user.post(sub_path)
         self.user.raise_for_status(response)
 
     def get_protocol_template_info_list(self, query: ProtocolTemplateQuery) -> list[ProtocolTemplateInfo]:
         """
-        Get a list of ProtocolTemplateInfoPojo objects using the provided criteria object to search the templates in the app.
+        Get a list of protocol templates using the provided criteria to search for templates in the app.
+
+        :param query: The search criteria for the protocol templates.
+        :return: A list of protocol templates matching the search criteria.
         """
         sub_path: str = self.user.build_url(['eln', 'protocoltemplate'])
         response = self.user.post(sub_path, payload=query.to_json())
         self.user.raise_for_status(response)
         json_list: list[dict[str, Any]] = response.json()
         return [ProtocolTemplateInfo.from_json(x) for x in json_list]
 
     def add_protocol_template(self, exp_id: int, protocol_template: int, position: ElnEntryPosition) -> list[ExperimentEntry]:
         """
-        Adds the entries from the protocol template to the given Eln Experiment.
-        The payload must be a ElnExperimentEntryPositionPojo defining where in the experiment the protocol should be added.
-        :param exp_id: The experiment ID to add the protocol template to.
-        :param protocol_template: The Protocol Template ID to add.
+        Adds the entries from a protocol template to the given ELN experiment at the given position.
+
+        :param exp_id: The notebook experiment ID of the experiment.
+        :param protocol_template: The ID of the protocol template to add to the experiment.
         :param position: The position in the experiment where the protocol template should be added to the experiment.
-        The first entry from the template will be added in thisposition and all subsequent entries will be added after it.
-        :return: list of newly added experiment entry objects in the ELN experiment.
+            The first entry from the template will be added in this position and all subsequent entries will be added
+            after it.
+        :return: A list of the newly added experiment entries in the ELN experiment.
         """
         sub_path = self.user.build_url(['eln', 'addProtocolTemplate', str(exp_id), str(protocol_template)])
         response = self.user.post(sub_path, payload=position.to_json())
         self.user.raise_for_status(response)
         json_list: list[dict[str, Any]] = response.json()
         return [ExperimentEntryParser.parse_experiment_entry(x) for x in json_list]
 
     def get_field_set_info_list(self) -> List[ElnFieldSetInfo]:
         """
-        Get a list of EnbFieldSetInfoPojo objects from the app.
+        Get a list of field set info from the system.
+
+        :return: A list of all field set info in the system.
         """
         sub_path = self.user.build_url(['eln', 'enbFieldSet', 'infolist'])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         json_list: list[dict[str, Any]] = response.json()
         return [ElnFieldSetInfo.from_json(x) for x in json_list]
 
     def get_predefined_fields_from_field_set_id(self, field_set_id: int) -> list[AbstractVeloxFieldDefinition]:
         """
-        Get a list of VeloxFieldDefinitionPojo objects from the field set.
+        Get a list of field definitions for the fields that are present in a field set.
+
         :param field_set_id: The system generated ID for the field set.
+        :return: A list of field definitions for the fields in the matching field set.
         """
         sub_path = self.user.build_url(['eln', 'enbFieldSet', 'fields', str(field_set_id)])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         json_list: list[dict[str, Any]] = response.json()
         return [FieldDefinitionParser.to_field_definition(x) for x in json_list]
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/GroupManagerService.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/GroupManagerService.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,90 +15,114 @@
 
     __instances: WeakValueDictionary[SapioUser, VeloxGroupManager] = WeakValueDictionary()
     __initialized: bool
 
     def __new__(cls, user: SapioUser):
         """
         Observes singleton pattern per record model manager object.
+
+        :param user: The user that will make the webservice request to the application.
         """
         obj = cls.__instances.get(user)
         if not obj:
             obj = object.__new__(cls)
             obj.__initialized = False
             cls.__instances[user] = obj
         return obj
 
     def __init__(self, user: SapioUser):
+        """
+        Obtains a group manager to perform queries on group membership and info.
+
+        :param user: The user that will make the webservice request to the application.
+        """
         if self.__initialized:
             return
         self.user = user
         self.__initialized = True
 
     def get_user_group_name_list(self) -> List[str]:
         """
-        Get the list of all user group names in the system.
+        Get the names of all groups in the system.
+
+        :return: A list of the names for all user groups in the system.
         """
         sub_path = '/usergroup/namelist/'
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         return response.json()
 
     def get_user_group_info_list(self) -> List[UserGroupInfo]:
         """
-        Get the list of all User Group Info objects representing all User Groups in the system.
+        Get the user group info for all groups in the system.
+
+        :return: A list of user group info for all user groups in the system.
         """
         sub_path = '/usergroup/infolist/'
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         return [UserGroupInfo.parse(x) for x in response.json()]
 
     def get_user_group_info_by_id(self, group_id: int) -> UserGroupInfo:
         """
-        Get a user group info by its group id
-        :param group_id: The group ID we are getting info for.
+        Get a user group's info by its group ID.
+
+        :param group_id: The ID of a group in the system.
+        :return: The user group info that matches the provided group ID.
         """
         sub_path = self.user.build_url(['usergroup', 'info', 'id', str(group_id)])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         return UserGroupInfo.parse(response.json())
 
     def get_user_group_info_by_name(self, group_name: str) -> UserGroupInfo:
         """
-        Get a user group info by its name
+        Get a user group's info by its group name.
+
+        :param group_name: The name of a group in the system.
+        :return: The user group info that matches the provided group name.
         """
         sub_path = self.user.build_url(['usergroup', 'info', 'name', group_name])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         return UserGroupInfo.parse(response.json())
 
-    def get_user_info_list_for_group(self, group_name: str) -> List[UserGroupInfo]:
+    def get_user_info_list_for_group(self, group_name: str) -> List[UserInfo]:
         """
-        Given the group name, retrieve user info list of all users who have membership to the given group.
+        Given the group name, retrieve the user info list of all users who have membership in that group.
+
+        :param group_name: The name of a group in the system.
+        :return: A list of user info for every member in the provided group.
         """
         sub_path = self.user.build_url(['usergroup', 'userassignment', group_name])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         return [UserInfo.parse(x) for x in response.json()]
 
     def get_user_info_map_for_groups(self, group_names: List[str]) -> Dict[str, List[UserInfo]]:
         """
-        Given a collection of group names, retrieve a user info list for each group, mapped by group names.
+        Given a list of group names, retrieve the user info list of all users who have membership in those groups.
+
+        :param group_names: A list of names of groups in the system.
+        :return: A dictionary of user info for every member in the provided groups, mapped by group name.
         """
         sub_path = '/usergroup/userassignment/'
         response = self.user.post(sub_path, payload=group_names)
         self.user.raise_for_status(response)
         raw_json: Dict[str, List[Dict[str, Any]]] = response.json()
         ret: Dict[str, List[UserInfo]] = dict()
         for key, value in raw_json.items():
             user_info_list = [UserInfo.parse(x) for x in value]
             ret[key] = user_info_list
         return ret
 
     def get_user_group_info_list_for_user(self, username: str) -> List[UserGroupInfo]:
         """
         Get a list of user groups the given user has membership of.
-        :param username The username to search membership for.
+
+        :param username: The username of a user in the system.
+        :return: A list of user group info for every group that the given user is a member of.
         """
         sub_path = self.user.build_url(['usergroup', 'groupassignment', username])
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
-        return [UserGroupInfo.parse(x) for x in response.json()]
+        return [UserGroupInfo.parse(x) for x in response.json()]
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/PicklistService.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,46 +13,56 @@
     user: SapioUser
     __instances: WeakValueDictionary[SapioUser, PicklistManager] = WeakValueDictionary()
     __initialized: bool
 
     def __new__(cls, user: SapioUser):
         """
         Observes singleton pattern per record model manager object.
+
+        :param user: The user that will make the webservice request to the application.
         """
         obj = cls.__instances.get(user)
         if not obj:
             obj = object.__new__(cls)
             obj.__initialized = False
             cls.__instances[user] = obj
         return obj
 
     def __init__(self, user: SapioUser):
+        """
+        Obtain a pick list manager for reading from and writing to or creating pick lists in the system.
+
+        :param user: The user that will make the webservice request to the application.
+        """
         if self.__initialized:
             return
         self.user = user
         self.__initialized = True
 
     def get_picklist_config_list(self) -> List[PickListConfig]:
         """
-        Get a list of all pick list configurations in the system.
+        Get every pick list configuration in the system.
+
+        :return: A list of all pick list configurations from the system.
         """
         sub_path: str = '/picklist/getConfigList'
         response = self.user.get(sub_path)
         self.user.raise_for_status(response)
         json_list: List[Dict[str, Any]] = response.json()
         return [PicklistParser.parse_picklist_config(x) for x in json_list]
 
     def update_picklist_value_list(self, pick_list_name: str, pick_list_new_value_list: List[str]) \
             -> PickListConfig:
         """
         Update the specified pick list config in the system.
-        :param pick_list_name: Name of the pick list to update.
-        If there is no picklist by this pick list name, will create a new picklist with this name.
-        :param pick_list_new_value_list: The list of values in the pick list
-        :return: The new picklist config object.
+
+        :param pick_list_name: The name of the pick list to update. If there is no picklist with this name, then a new
+            pick list will be created with this name.
+        :param pick_list_new_value_list: The list of values in the pick list.
+        :return: The updated or new pick list configuration object.
         """
         sub_path = self.user.build_url(['picklist', 'updateConfigValueList', pick_list_name])
         response = self.user.post(sub_path, payload=pick_list_new_value_list)
         self.user.raise_for_status(response)
         json_dct = response.json()
         return PicklistParser.parse_picklist_config(json_dct)
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/ReportManager.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/ReportManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,82 +26,98 @@
     user: SapioUser
     __instances: WeakValueDictionary[SapioUser, ReportManager] = WeakValueDictionary()
     __initialized: bool
 
     def __new__(cls, user: SapioUser):
         """
         Observes singleton pattern per record model manager object.
+
+        :param user: The user that will make the webservice request to the application.
         """
         obj = cls.__instances.get(user)
         if not obj:
             obj = object.__new__(cls)
             obj.__initialized = False
             cls.__instances[user] = obj
         return obj
 
     def __init__(self, user: SapioUser):
         """
-        Obtains REST accession manager to perform accessioning operations.
+        Obtains REST report manager to perform reporting operations.
+
+        :param user: The user that will make the webservice request to the application.
         """
         if self.__initialized:
             return
         self.user = user
         self.__initialized = True
 
     def get_report_template_info_list(self) -> list[ReportTemplateInfo]:
         """
-        Select the details about the Report templates currently in the system.
+        Get the details about the report templates currently in the system.
+
+        :return: A list of report template info for every report template in the system.
         """
         url = self.user.build_url(['reporttemplate'])
         response = self.user.get(url)
         json_data = response.json()
         template_info_list = []
         for template_json in json_data:
             template_info = VeloxReportBuilderParser.parse_report_template_info(template_json)
             template_info_list.append(template_info)
         return template_info_list
 
     def get_report_entry_info_list(self, template_id: str) -> list[ReportEntryInfo]:
         """
-        Select the details about the Report entries contained in the Report Template with the provided ID currently in the system.
-        :param template_id: The ID of the Report Template from which to retrieve the entries.
+        Get the details about the report entries contained in the report template with the provided ID currently in
+        the system.
+
+        :param template_id: The ID of the report template from which to retrieve the entries.
+        :return: A list of report entry info for the matching report template ID.
         """
         url = self.user.build_url(['reporttemplate', 'entries', template_id])
         response = self.user.get(url)
         json_data = response.json()
         entry_info_list = []
         for entry_json in json_data:
             entry_info = VeloxReportBuilderParser.parse_report_entry_info(entry_json)
             entry_info_list.append(entry_info)
         return entry_info_list
 
     def generate_report_pdf(self, template_id: str, attachment_data_type: str, data_context: ReportDataContext) -> None:
         """
         Generate a Report PDF in the system using the provided template and data.
-        This method will start an asynchronous process to generate the Report PDF and store it as a record in the system using the provided attachment data type.
-        Optionally, a parent record can be provided to identify where the newly created attachment data type will be stored.
+        This method will start an asynchronous process to generate the Report PDF and store it as a record in the system
+        using the provided attachment data type.
+        Optionally, a parent record can be provided to identify where the newly created attachment data type will be
+        stored.
         If no parent data record is provided, then the attachment record will be stored in the aether with no parents.
+
         :param template_id: The ID of the Report Template from which the PDF will be generated.
-        :param attachment_data_type: The attachment data type name that defines the type of attachment record that will be created to store the generated PDF.  This data type must exist in the system and must be a valid attachment data type.
+        :param attachment_data_type: The attachment data type name that defines the type of attachment record that will
+            be created to store the generated PDF.  This data type must exist in the system and must be a valid
+            attachment data type.
         :param data_context: The data context that should be used when generating the PDF from the Report Template.
         """
         url = self.user.build_url(['reporttemplate', 'pdf', template_id, attachment_data_type])
         payload = data_context.to_json()
         response = self.user.post(url, payload=payload)
         self.user.raise_for_status(response)
 
     def initialize_report_data_context(self, record_models: Iterable[PyRecordModel | WrappedRecordModel], template_id: str,
                                        parent_model: PyRecordModel | WrappedRecordModel | None = None,
                                        attachment_file_name: str | None = None) -> ReportDataContext:
         """
         This is a helper tool that allows you to quickly set up a new report data context.
+
         :param record_models: The record models that participate in this report.
         :param template_id: The template ID to retrieve entry definition.
         :param parent_model: If specified, the PDF attachment will be attached as child of this record.
         :param attachment_file_name: The file name of the attachment.
+        :return: A newly constructed report data context.
         """
         unwrapped_models = RecordModelWrapperUtil.unwrap_list(record_models)
         RecordModelUtil.validate_backing_records(unwrapped_models)
         parent_model_unwrapped: PyRecordModel | None = None
         if parent_model:
             parent_model_unwrapped = RecordModelWrapperUtil.unwrap(parent_model)
             RecordModelUtil.validate_backing_records([parent_model_unwrapped])
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/User.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/User.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,20 +12,27 @@
 
 class UserSessionAdditionalData:
     """
     The session info for the current session. This is not necessary to establish connection from client to server,
     but can provide useful info for a webservice user program.
     """
     current_group_id: Optional[int]
+    """The group ID of the group that the user currently has selected"""
     current_group_name: Optional[str]
+    """The group name of the group that the user currently has selected"""
     first_name: Optional[str]
+    """The user's first name as specified in the user manager."""
     middle_name: Optional[str]
+    """The user's first name as specified in the user manager."""
     last_name: Optional[str]
+    """The user's first name as specified in the user manager."""
     email: Optional[str]
+    """The user's email address as specified in the user manager."""
     utc_offset_seconds: int
+    """The UTC offset in seconds of the user. Can be used to determine the user's local time."""
 
     def __init__(self, current_group_id: Optional[int], current_group_name: Optional[str],
                  first_name: Optional[str], middle_name: Optional[str], last_name: Optional[str], email: Optional[str],
                  utc_offset_seconds: int):
         self.current_group_id = current_group_id
         self.current_group_name = current_group_name
         self.first_name = first_name
@@ -82,41 +89,55 @@
 
 class SapioUser:
     """
     The Sapio REST API Client stores the REST connection info for each new requests.
     There are two main ways to authenticate, with API token, and with username/password.
     """
     url: str
+    """The URL that will be called by this user when making webservice requests."""
     api_token: Optional[str]
+    """The API token used to authenticate requests to the system."""
     username: Optional[str]
+    """The user's username in the system. May be used for authentication of requests when using username/password
+    authentication."""
     password: Optional[str]
+    """The user's password for the system. May be used for authentication of requests when using username/password
+    authentication."""
     guid: Optional[str]
+    """The GUID of the system being communicated with."""
     account_name: Optional[str]
+    """The name of the account of the system being communicated with."""
     verify_ssl_cert: bool
+    """Whether to verify SSL certificates of the server. This will throw SSLError if the server is self-signed."""
     timeout_seconds: int
+    """The number of seconds that this user will wait for a response from the server before timing out."""
     __next_temp_record_id: int
     logger: logging.Logger
 
     _session_additional_data: Optional[UserSessionAdditionalData]
 
     def __init__(self, url: str,
                  verify_ssl_cert: bool = True, timeout_seconds: int = 60,
                  api_token: str = None, username: str = None, password: str = None,
                  guid: str = None, account_name: str = None,
                  session_additional_data: Optional[UserSessionAdditionalData] = None):
         """
         Create a new Sapio REST API Client object using API Token. Typically ends with "/webservice/api".
 
         :param url: The URL of root of REST API APPLICATION. For example: https://localhost/webservice/api
+        :param verify_ssl_cert: Whether to verify SSL certificates of the server. This will throw SSLError if the server
+            is self-signed.
+        :param timeout_seconds: The wait timeout of the request, in seconds. Default: 60 (1 minute)
         :param api_token: The API token to authenticate the platform API user. Use App Config Manager to obtain this.
-        :param guid: When using username/password authentication, provide GUID of the app. Obtain from Sapio Portal.
         :param username: When using username/password authentication, the username of the credential.
         :param password: When using username/password authentication, the password of the credential.
-        :param verify_ssl_cert: Whether to verify SSL certificates. This will throw SSLError if the server self-signed.
-        :param timeout_seconds: The wait timeout of the request, in seconds. Default: 60 (1 minute)
+        :param guid: When using username/password authentication, provide GUID of the app. Obtain from Sapio Portal.
+        :param account_name: The name of the account of the system being communicated with.
+        :param session_additional_data: Additional data for this user's current session, including info about the user
+            from the user manager, the user's currently selected group, and more.
         """
         self.url = url
         self.api_token = api_token
         self.guid = guid
         self.username = username
         self.password = password
         self.verify_ssl_cert = verify_ssl_cert
@@ -172,39 +193,41 @@
         return requests.get(self.url + url_sub_path, params=params,
                             headers=self.get_http_headers(), verify=self.verify_ssl_cert,
                             timeout=self.timeout_seconds)
 
     def consume_octet_stream_get(self, url_sub_path: str,
                                  data_sink: Callable[[bytes], None],
                                  params: Optional[dict] = None,
-                                 chunk_size=1024 * 1024) -> None:
+                                 chunk_size=1024 * 1024) -> Response:
         session = requests.Session()
         url = self.url + url_sub_path
         headers = self.get_http_headers()
         response = session.get(url=url, params=params,
                                headers=headers, verify=self.verify_ssl_cert,
                                timeout=self.timeout_seconds, stream=True)
         self.raise_for_status(response)
         for chunk in response.iter_content(chunk_size=chunk_size):
             data_sink(chunk)
+        return response
 
     def consume_octet_stream_post(self, url_sub_path: str,
                                   data_sink: Callable[[bytes], None],
                                   params: Optional[dict] = None,
                                   payload = None,
-                                  chunk_size=1024 * 1024) -> None:
+                                  chunk_size=1024 * 1024) -> Response:
         session = requests.Session()
         url = self.url + url_sub_path
         headers = self.get_http_headers()
         response = session.post(url=url, params=params, json=payload,
                                 headers=headers, verify=self.verify_ssl_cert,
                                 timeout=self.timeout_seconds, stream=True)
         self.raise_for_status(response)
         for chunk in response.iter_content(chunk_size=chunk_size):
             data_sink(chunk)
+        return response
 
     def delete(self, url_sub_path: str, params: Optional[dict] = None, payload=None) -> Response:
         return requests.delete(self.url + url_sub_path, params=params, json=payload,
                                headers=self.get_http_headers(), verify=self.verify_ssl_cert,
                                timeout=self.timeout_seconds)
 
     def put(self, url_sub_path: str, params: Optional[dict] = None, payload=None) -> Response:
@@ -244,14 +267,15 @@
         """
         prefix = self.get_logging_prefix()
         self.logger.info(prefix + msg)
 
     def log_error(self, msg: str, exc_info=True) -> None:
         """
         Log an error message
+
         :param msg: The message to log error for
         :param exc_info: If true, it will also print the stack trace.
         """
         prefix = self.get_logging_prefix()
         self.logger.error(prefix + msg, exc_info=exc_info)
 
     def get_logging_prefix(self):
@@ -261,14 +285,18 @@
         prefix: str = "<" + self.url + "> "
         if self.username:
             prefix = self.username + ": "
         return prefix
 
     @property
     def session_additional_data(self) -> UserSessionAdditionalData:
+        """
+        :return: Additional data for this user's current session, including info about the user from the user manager,
+            the user's currently selected group, and more.
+        """
         if self._session_additional_data is not None:
             return self._session_additional_data
         sub_url = '/user/currentsession/additionaldata'
         response = self.get(sub_url)
         self.raise_for_status(response)
         self._session_additional_data = parse_session_additional_data(response.json())
         return self._session_additional_data
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/UserManagerService.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/UserManagerService.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,44 +15,55 @@
 
     __instances: WeakValueDictionary[SapioUser, VeloxUserManager] = WeakValueDictionary()
     __initialized: bool
 
     def __new__(cls, user: SapioUser):
         """
         Observes singleton pattern per record model manager object.
+
+        :param user: The user that will make the webservice request to the application.
         """
         obj = cls.__instances.get(user)
         if not obj:
             obj = object.__new__(cls)
             obj.__initialized = False
             cls.__instances[user] = obj
         return obj
 
     def __init__(self, user: SapioUser):
+        """
+        Obtain a user manager for retrieving information about users in the system.
+
+        :param user: The user that will make the webservice request to the application.
+        """
         if self.__initialized:
             return
         self.user = user
         self.__initialized = True
 
     def get_user_info_list(self, criteria: UserInfoCriteria = UserInfoCriteria()) -> List[UserInfo]:
         """
-        Retrieve list of user info data.
-        :param criteria filters for the results.
+        Retrieve a list of user info data based on the given criteria.
+
+        :param criteria: Search criteria that can be used to filter the search results.
+        :return: A list of user info that matches the search criteria.
         """
         sub_path = '/user/infolist/'
         response = self.user.post(sub_path, payload=criteria.to_json())
         self.user.raise_for_status(response)
         json_dct_list = response.json()
         return [UserInfo.parse(x) for x in json_dct_list]
 
     def get_user_name_list(self, include_deactivated_users: bool = False) -> List[str]:
         """
         Get a list of all available usernames in the Sapio system.
+
         :param include_deactivated_users: Whether to include the users that are deactivated.
+        :return: A list of all usernames in the system that match the search criteria.
         """
         sub_path = '/user/namelist/'
         params = {
             'includeDeactivatedUsers': include_deactivated_users
         }
         response = self.user.get(sub_path, params=params)
         self.user.raise_for_status(response)
-        return response.json()
+        return response.json()
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/WebhookService.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,15 @@
             traceback.print_exc()
             return SapioWebhookResult(False, display_text="Error occurred during webhook execution.").to_json()
 
     @abstractmethod
     def run(self, context: SapioWebhookContext) -> SapioWebhookResult:
         """
         The execution details for this service.
+
         :param context: The webhook context provided to you when it is called.
         :return: The webhook result to send back to Sapio.
         """
         pass
 
 
 class WebhookConfiguration:
@@ -64,28 +65,36 @@
                  client_timeout_seconds: int = 60, debug=False):
         self.verify_sapio_cert = verify_sapio_cert
         self.client_timeout_seconds = client_timeout_seconds
         self.debug = debug
         self._handlers_by_sub_path = dict()
 
     def register(self, url_path, handler_clazz: Type[AbstractWebhookHandler]):
+        """
+        Register a new webhook endpoint.
+
+        :param url_path: The endpoint that will be used to invoke the given class.
+        :param handler_clazz: The webhook handler class that will be run when this endpoint is called.
+        """
         self._handlers_by_sub_path[url_path] = handler_clazz
 
     @property
     def handlers_by_sub_path(self):
         return self._handlers_by_sub_path
 
 
 class WebhookServerFactory:
     @staticmethod
     def configure_flask_app(app: Optional[Flask], config: WebhookConfiguration) -> Flask:
         """
         Configure a new or existing flask server.
-        :param app: The existing flask server. If None is specified, a new server is created with default configs.
-        :param config: The Sapio webhook configurations for flask server.
+
+        :param app: The existing Flask server. If None is specified, a new server is created with default configs.
+        :param config: The Sapio webhook configurations for the Flask server.
+        :return: The input Flask app, or a new one if no input was provided.
         """
         if app is None:
             app = Flask('SapioWebhookServer')
         app.debug = config.debug
         for url, handler_clazz in config.handlers_by_sub_path.items():
             if config.debug:
                 print("Register POST: " + url)
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/Message.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Message.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/UserInfo.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/UserInfo.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     _field_definition_map: Dict[str, AbstractVeloxFieldDefinition]
     data_type_name: str
     display_name: str
     plural_display_name: str
     attachment: bool
     record_image_assignable: bool
 
+    def get_field_def_list(self):
+        return list(self._field_definition_map.values())
+
     def set_field_definition(self, field_def: AbstractVeloxFieldDefinition):
         """
         Replace existing field with the same field name with the new field definition.
         """
         field_def._data_type_name = self.data_type_name
         self._field_definition_map[field_def.get_data_field_name().upper()] = field_def
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/field_set.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/field_set.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/eln/protocol_template.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/protocol_template.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,50 @@
 import base64
 from abc import ABC, abstractmethod
+from enum import Enum
 from typing import Any, List, Dict, Optional
 
 from sapiopylib.rest.pojo.datatype.DataTypeLayout import DataTypeLayout
 
 from sapiopylib.rest.pojo.DataRecord import DataRecord
 
 from sapiopylib.rest.pojo.CustomReport import CustomReport
 
 from sapiopylib.rest.pojo.datatype.FieldDefinition import AbstractVeloxFieldDefinition
 from sapiopylib.rest.pojo.datatype.TemporaryDataType import TemporaryDataType
 from sapiopylib.rest.pojo.webhook.WebhookEnums import CallbackType, SearchType, ScanToSelectCriteria, FormAccessLevel
 
+class PopupType(Enum):
+    """
+    The different client callback toastr pop up types.
+    """
+    Success = 0
+    Info = 1
+    Warning = 2
+    Error = 3
+
+class DisplayPopupRequest:
+    """
+    A request payload to indicate what toastr message we want to send to human end user.
+    """
+    title: str
+    message: str
+    popup_type: PopupType
+
+    def __init__(self, title: str, message: str, popup_type: PopupType):
+        self.title = title
+        self.message = message
+        self.popup_type = popup_type
+
+    def to_json(self) -> dict[str, Any]:
+        return {
+            "title": self.title,
+            "message": self.message,
+            "popupType": self.popup_type.name
+        }
 
 class AbstractClientCallbackRequest(ABC):
     """
     A request for a client callback to be shown to the user that invoked the webhook.
     """
     callback_context_data: Optional[str]
```

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/CompresionUtil.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/CompresionUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/Protocols.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/autopaging.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/autopaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recorddatasinks.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recorddatasinks.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/ancestry.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/ancestry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/rest/utils/recordmodel/properties.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/properties.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/src/sapiopylib/utils/string.py` & `sapiopylib-2024.4.5a179/src/sapiopylib/utils/string.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/EmailAttachmentDataTest.py` & `sapiopylib-2024.4.5a179/tests/EmailAttachmentDataTest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/FR-51536_test.py` & `sapiopylib-2024.4.5a179/tests/FR-51536_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/FR-51549_test.py` & `sapiopylib-2024.4.5a179/tests/FR-51549_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/FR-51551_test.py` & `sapiopylib-2024.4.5a179/tests/FR-51551_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/FR-51635_test.py` & `sapiopylib-2024.4.5a179/tests/FR-51635_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/FR-51821_test.py` & `sapiopylib-2024.4.5a179/tests/FR-51821_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/FR-51846_test.py` & `sapiopylib-2024.4.5a179/tests/FR-51846_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/FR-51847_test.py` & `sapiopylib-2024.4.5a179/tests/FR-51847_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/FR-51849_test.py` & `sapiopylib-2024.4.5a179/tests/FR-51849_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/PR-51537_test.py` & `sapiopylib-2024.4.5a179/tests/PR-51537_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/PR-51547.py` & `sapiopylib-2024.4.5a179/tests/PR-51547.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/PR-51842_test.py` & `sapiopylib-2024.4.5a179/tests/PR-51842_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/PR-51853_test.py` & `sapiopylib-2024.4.5a179/tests/PR-51853_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/PR-51856_test.py` & `sapiopylib-2024.4.5a179/tests/PR-51856_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/PR-51964_test.py` & `sapiopylib-2024.4.5a179/tests/PR-51964_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/data_type_models.py` & `sapiopylib-2024.4.5a179/tests/data_type_models.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/tests/resources/fr-51846.ssg` & `sapiopylib-2024.4.5a179/tests/resources/fr-51846.ssg`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/LICENSE` & `sapiopylib-2024.4.5a179/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/README.md` & `sapiopylib-2024.4.5a179/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.2.7a178/pyproject.toml` & `sapiopylib-2024.4.5a179/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2024.02.07a178'
+version='2024.04.05a179'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `sapiopylib-2024.2.7a178/PKG-INFO` & `sapiopylib-2024.4.5a179/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sapiopylib
-Version: 2024.2.7a178
+Version: 2024.4.5a179
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sapiopylib Version: 2024.2.7a178 Summary: Official
+Metadata-Version: 2.3 Name: sapiopylib Version: 2024.4.5a179 Summary: Official
 Sapio Informatics Platform Python API Project-URL: Homepage, https://
 github.com/sapiosciences Project-URL: Bug Tracker, https://github.com/
 sapiosciences/sapio-py-tutorials/issues Author-email: Yechen Qiao
 sapiosciences.com> License-Expression: MPL-2.0 License-File: LICENSE Keywords:
 eln,lims,rest,sapio Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Healthcare Industry Classifier: Intended Audience :: Science/Research
```

