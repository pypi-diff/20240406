# Comparing `tmp/metabeaver-0.4.1.tar.gz` & `tmp/metabeaver-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabeaver-0.4.1.tar", last modified: Thu Apr  4 20:44:22 2024, max compression
+gzip compressed data, was "metabeaver-0.4.2.tar", last modified: Sat Apr  6 15:33:40 2024, max compression
```

## Comparing `metabeaver-0.4.1.tar` & `metabeaver-0.4.2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:22.070084 metabeaver-0.4.1/
--rw-rw-rw-   0        0        0      682 2024-04-04 20:44:22.066075 metabeaver-0.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.690356 metabeaver-0.4.1/metabeaver/
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.721691 metabeaver-0.4.1/metabeaver/BeaverTown/
--rw-rw-rw-   0        0        0       54 2024-02-20 17:36:10.000000 metabeaver-0.4.1/metabeaver/BeaverTown/__init__.py
--rw-rw-rw-   0        0        0      523 2024-02-20 17:54:11.000000 metabeaver-0.4.1/metabeaver/BeaverTown/abstractBeaver.py
--rw-rw-rw-   0        0        0      928 2023-11-01 11:25:56.000000 metabeaver-0.4.1/metabeaver/BeaverTown/beaverOn.py
--rw-rw-rw-   0        0        0       54 2023-11-28 08:40:24.000000 metabeaver-0.4.1/metabeaver/BeaverTown/pumpkinPie.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.721691 metabeaver-0.4.1/metabeaver/Binary/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/Binary/__init__.py
--rw-rw-rw-   0        0        0     3173 2024-02-10 12:14:12.000000 metabeaver-0.4.1/metabeaver/Binary/binaryOperations.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.734314 metabeaver-0.4.1/metabeaver/Caching/
--rw-rw-rw-   0        0        0     2084 2023-10-15 13:36:19.000000 metabeaver-0.4.1/metabeaver/Caching/LeastRecentlyUsed.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/Caching/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.765154 metabeaver-0.4.1/metabeaver/DataManipulation/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.1/metabeaver/DataManipulation/__init__.py
--rw-rw-rw-   0        0        0     1737 2024-04-02 20:33:27.000000 metabeaver-0.4.1/metabeaver/DataManipulation/filterPandas.py
--rw-rw-rw-   0        0        0      859 2023-05-22 12:30:24.000000 metabeaver-0.4.1/metabeaver/DataManipulation/localPickle.py
--rw-rw-rw-   0        0        0      831 2023-05-15 09:25:04.000000 metabeaver-0.4.1/metabeaver/DataManipulation/universalResourceLinkHandler.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.781035 metabeaver-0.4.1/metabeaver/DataStructures/
--rw-rw-rw-   0        0        0     3440 2023-12-30 09:15:13.000000 metabeaver-0.4.1/metabeaver/DataStructures/BinarySearchTree.py
--rw-rw-rw-   0        0        0      182 2023-12-28 08:32:20.000000 metabeaver-0.4.1/metabeaver/DataStructures/Node.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/DataStructures/__init__.py
--rw-rw-rw-   0        0        0      400 2023-09-27 14:26:46.000000 metabeaver-0.4.1/metabeaver/DataStructures/firstInFirstOutQueue.py
--rw-rw-rw-   0        0        0        0 2023-10-16 07:07:41.000000 metabeaver-0.4.1/metabeaver/DataStructures/firstInLastOut.py
--rw-rw-rw-   0        0        0        0 2023-10-16 07:07:21.000000 metabeaver-0.4.1/metabeaver/DataStructures/linkedList.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.781035 metabeaver-0.4.1/metabeaver/DatabaseFunctionality/
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.790129 metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQL/
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQL/__init__.py
--rw-rw-rw-   0        0        0     1051 2024-03-08 12:25:31.000000 metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQL/rawSQL.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.830293 metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQLite/
--rw-rw-rw-   0        0        0    32341 2023-12-21 09:23:48.000000 metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQLite/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-11-28 08:53:13.000000 metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py
--rw-rw-rw-   0        0        0     1854 2023-11-28 11:03:59.000000 metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py
--rw-rw-rw-   0        0        0       54 2023-12-20 14:54:15.000000 metabeaver-0.4.1/metabeaver/DatabaseFunctionality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.830293 metabeaver-0.4.1/metabeaver/DatesAndTime/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.1/metabeaver/DatesAndTime/__init__.py
--rw-rw-rw-   0        0        0      692 2024-03-06 21:17:29.000000 metabeaver-0.4.1/metabeaver/DatesAndTime/getToday.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.837805 metabeaver-0.4.1/metabeaver/Dynamic Programming/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/Dynamic Programming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.843903 metabeaver-0.4.1/metabeaver/FileIO/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/FileIO/__init__.py
--rw-rw-rw-   0        0        0      389 2024-04-03 15:41:35.000000 metabeaver-0.4.1/metabeaver/FileIO/pickleObject.py
--rw-rw-rw-   0        0        0      966 2024-03-02 22:41:17.000000 metabeaver-0.4.1/metabeaver/FileIO/yamlIO.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.850076 metabeaver-0.4.1/metabeaver/Formatting/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.1/metabeaver/Formatting/__init__.py
--rw-rw-rw-   0        0        0      450 2023-09-02 17:13:50.000000 metabeaver-0.4.1/metabeaver/Formatting/printControl.py
--rw-rw-rw-   0        0        0     1063 2023-10-04 07:18:25.000000 metabeaver-0.4.1/metabeaver/Formatting/printControlTest.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.850076 metabeaver-0.4.1/metabeaver/GoogleCloudPlatform/
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.859918 metabeaver-0.4.1/metabeaver/GoogleCloudPlatform/BigQuery/
--rw-rw-rw-   0        0        0     7543 2024-04-04 20:44:03.000000 metabeaver-0.4.1/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.1/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
--rw-rw-rw-   0        0        0     3388 2024-04-04 19:42:42.000000 metabeaver-0.4.1/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py
--rw-rw-rw-   0        0        0      144 2024-01-05 19:00:29.000000 metabeaver-0.4.1/metabeaver/GoogleCloudPlatform/BigQuery/credentialsFromEnv.py
--rw-rw-rw-   0        0        0     4872 2024-04-02 20:16:43.000000 metabeaver-0.4.1/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.1/metabeaver/GoogleCloudPlatform/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.879903 metabeaver-0.4.1/metabeaver/Graph Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/Graph Algorithms/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:48:31.000000 metabeaver-0.4.1/metabeaver/Graph Algorithms/bellmanFord.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:43:10.000000 metabeaver-0.4.1/metabeaver/Graph Algorithms/breadthFirstSearch.py
--rw-rw-rw-   0        0        0      990 2024-02-13 10:13:17.000000 metabeaver-0.4.1/metabeaver/Graph Algorithms/depthFirstSearch.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:48:06.000000 metabeaver-0.4.1/metabeaver/Graph Algorithms/dijkstra.py
--rw-rw-rw-   0        0        0        0 2023-10-11 14:43:34.000000 metabeaver-0.4.1/metabeaver/Graph Algorithms/monteCarloTreeSearch.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.879903 metabeaver-0.4.1/metabeaver/Graphing/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.1/metabeaver/Graphing/__init__.py
--rw-rw-rw-   0        0        0      824 2023-05-26 14:44:50.000000 metabeaver-0.4.1/metabeaver/Graphing/markdownGenerator.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.900029 metabeaver-0.4.1/metabeaver/InstallationScripts/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.1/metabeaver/InstallationScripts/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.4.1/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.900029 metabeaver-0.4.1/metabeaver/InterviewQuestions/
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.915301 metabeaver-0.4.1/metabeaver/InterviewQuestions/Arrays/
--rw-rw-rw-   0        0        0       54 2024-03-06 21:33:39.000000 metabeaver-0.4.1/metabeaver/InterviewQuestions/Arrays/__init__.py
--rw-rw-rw-   0        0        0     1100 2024-01-16 09:07:23.000000 metabeaver-0.4.1/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py
--rw-rw-rw-   0        0        0     2374 2024-02-12 11:00:27.000000 metabeaver-0.4.1/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py
--rw-rw-rw-   0        0        0     3115 2024-01-10 09:29:29.000000 metabeaver-0.4.1/metabeaver/InterviewQuestions/Arrays/twoSum.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.930496 metabeaver-0.4.1/metabeaver/InterviewQuestions/Stacks/
--rw-rw-rw-   0        0        0       54 2024-03-06 21:34:35.000000 metabeaver-0.4.1/metabeaver/InterviewQuestions/Stacks/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-10-24 15:28:24.000000 metabeaver-0.4.1/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/InterviewQuestions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.930496 metabeaver-0.4.1/metabeaver/LearnPython/
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.950034 metabeaver-0.4.1/metabeaver/LearnPython/ControlFlow/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/LearnPython/ControlFlow/__init__.py
--rw-rw-rw-   0        0        0     2615 2024-03-01 09:39:54.000000 metabeaver-0.4.1/metabeaver/LearnPython/ControlFlow/ifelifelse.py
--rw-rw-rw-   0        0        0       54 2024-02-20 17:10:29.000000 metabeaver-0.4.1/metabeaver/LearnPython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.964878 metabeaver-0.4.1/metabeaver/Machine Learning/
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.971532 metabeaver-0.4.1/metabeaver/Machine Learning/LLM/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/Machine Learning/LLM/__init__.py
--rw-rw-rw-   0        0        0       54 2024-03-28 19:26:50.000000 metabeaver-0.4.1/metabeaver/Machine Learning/LLM/loadWithLlamaCPP.py
--rw-rw-rw-   0        0        0     1996 2024-04-02 16:08:53.000000 metabeaver-0.4.1/metabeaver/Machine Learning/LLM/loadWithTransformers.py
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/Machine Learning/__init__.py
--rw-rw-rw-   0        0        0     2915 2024-02-18 11:36:59.000000 metabeaver-0.4.1/metabeaver/Machine Learning/lassoRegression.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.987279 metabeaver-0.4.1/metabeaver/Mathematical Operations/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/Mathematical Operations/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-16 16:20:54.000000 metabeaver-0.4.1/metabeaver/Mathematical Operations/greatestCommonDenominator.py
--rw-rw-rw-   0        0        0     1072 2024-03-01 15:21:44.000000 metabeaver-0.4.1/metabeaver/Mathematical Operations/vectorDotProduct.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.990290 metabeaver-0.4.1/metabeaver/MetaProgramming/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.1/metabeaver/MetaProgramming/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.990290 metabeaver-0.4.1/metabeaver/OperationBeaver/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.1/metabeaver/OperationBeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:21.990290 metabeaver-0.4.1/metabeaver/Search Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/Search Algorithms/__init__.py
--rw-rw-rw-   0        0        0     2686 2023-11-01 10:30:45.000000 metabeaver-0.4.1/metabeaver/Search Algorithms/binarySearch.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:22.010351 metabeaver-0.4.1/metabeaver/Set Theory/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/Set Theory/__init__.py
--rw-rw-rw-   0        0        0     5497 2023-10-06 17:16:32.000000 metabeaver-0.4.1/metabeaver/Set Theory/findAllSubsets.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:22.040113 metabeaver-0.4.1/metabeaver/Sorting Algorithms/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/Sorting Algorithms/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-12-12 09:32:50.000000 metabeaver-0.4.1/metabeaver/Sorting Algorithms/heapSort.py
--rw-rw-rw-   0        0        0     1539 2023-10-15 18:11:43.000000 metabeaver-0.4.1/metabeaver/Sorting Algorithms/insertionSort.py
--rw-rw-rw-   0        0        0     1275 2024-01-09 08:35:40.000000 metabeaver-0.4.1/metabeaver/Sorting Algorithms/mergeSort.py
--rw-rw-rw-   0        0        0     1136 2023-10-13 07:08:11.000000 metabeaver-0.4.1/metabeaver/Sorting Algorithms/quickSort.py
--rw-rw-rw-   0        0        0     3213 2023-10-12 10:18:23.000000 metabeaver-0.4.1/metabeaver/Sorting Algorithms/timsort.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:22.040113 metabeaver-0.4.1/metabeaver/Testing/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.1/metabeaver/Testing/__init__.py
--rw-rw-rw-   0        0        0     3544 2023-11-03 10:47:27.000000 metabeaver-0.4.1/metabeaver/Testing/scratchPad.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:22.050333 metabeaver-0.4.1/metabeaver/TextValidation/
--rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.1/metabeaver/TextValidation/__init__.py
--rw-rw-rw-   0        0        0     1418 2023-09-27 14:33:38.000000 metabeaver-0.4.1/metabeaver/TextValidation/closureChecker.py
--rw-rw-rw-   0        0        0     4004 2023-11-01 10:50:46.000000 metabeaver-0.4.1/metabeaver/TextValidation/establishLargestPalindrome.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:22.059913 metabeaver-0.4.1/metabeaver/WebScraping/
--rw-rw-rw-   0        0        0       54 2023-11-28 09:31:41.000000 metabeaver-0.4.1/metabeaver/WebScraping/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-11-28 09:40:35.000000 metabeaver-0.4.1/metabeaver/WebScraping/simpleRequests.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.1/metabeaver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 20:44:22.066075 metabeaver-0.4.1/metabeaver.egg-info/
--rw-rw-rw-   0        0        0      682 2024-04-04 20:44:21.000000 metabeaver-0.4.1/metabeaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4078 2024-04-04 20:44:21.000000 metabeaver-0.4.1/metabeaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 20:44:21.000000 metabeaver-0.4.1/metabeaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-04 20:44:21.000000 metabeaver-0.4.1/metabeaver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-04 20:44:21.000000 metabeaver-0.4.1/metabeaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 20:44:22.070084 metabeaver-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1299 2024-04-04 20:44:03.000000 metabeaver-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:40.141210 metabeaver-0.4.2/
+-rw-rw-rw-   0        0        0      615 2024-04-06 15:33:40.141210 metabeaver-0.4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.301213 metabeaver-0.4.2/metabeaver/
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.407046 metabeaver-0.4.2/metabeaver/BeaverTown/
+-rw-rw-rw-   0        0        0       54 2024-02-20 17:36:10.000000 metabeaver-0.4.2/metabeaver/BeaverTown/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-02-20 17:54:11.000000 metabeaver-0.4.2/metabeaver/BeaverTown/abstractBeaver.py
+-rw-rw-rw-   0        0        0      928 2023-11-01 11:25:56.000000 metabeaver-0.4.2/metabeaver/BeaverTown/beaverOn.py
+-rw-rw-rw-   0        0        0       54 2023-11-28 08:40:24.000000 metabeaver-0.4.2/metabeaver/BeaverTown/pumpkinPie.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.422474 metabeaver-0.4.2/metabeaver/Binary/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/Binary/__init__.py
+-rw-rw-rw-   0        0        0     3173 2024-02-10 12:14:12.000000 metabeaver-0.4.2/metabeaver/Binary/binaryOperations.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.441409 metabeaver-0.4.2/metabeaver/Caching/
+-rw-rw-rw-   0        0        0     2084 2023-10-15 13:36:19.000000 metabeaver-0.4.2/metabeaver/Caching/LeastRecentlyUsed.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/Caching/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.502878 metabeaver-0.4.2/metabeaver/DataManipulation/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.2/metabeaver/DataManipulation/__init__.py
+-rw-rw-rw-   0        0        0     1737 2024-04-02 20:33:27.000000 metabeaver-0.4.2/metabeaver/DataManipulation/filterPandas.py
+-rw-rw-rw-   0        0        0      859 2023-05-22 12:30:24.000000 metabeaver-0.4.2/metabeaver/DataManipulation/localPickle.py
+-rw-rw-rw-   0        0        0      831 2023-05-15 09:25:04.000000 metabeaver-0.4.2/metabeaver/DataManipulation/universalResourceLinkHandler.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.551131 metabeaver-0.4.2/metabeaver/DataStructures/
+-rw-rw-rw-   0        0        0     3440 2023-12-30 09:15:13.000000 metabeaver-0.4.2/metabeaver/DataStructures/BinarySearchTree.py
+-rw-rw-rw-   0        0        0      182 2023-12-28 08:32:20.000000 metabeaver-0.4.2/metabeaver/DataStructures/Node.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0      400 2023-09-27 14:26:46.000000 metabeaver-0.4.2/metabeaver/DataStructures/firstInFirstOutQueue.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 07:07:41.000000 metabeaver-0.4.2/metabeaver/DataStructures/firstInLastOut.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 07:07:21.000000 metabeaver-0.4.2/metabeaver/DataStructures/linkedList.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.561408 metabeaver-0.4.2/metabeaver/DatabaseFunctionality/
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.581615 metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQL/
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQL/__init__.py
+-rw-rw-rw-   0        0        0     1051 2024-03-08 12:25:31.000000 metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQL/rawSQL.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.636158 metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQLite/
+-rw-rw-rw-   0        0        0    32341 2023-12-21 09:23:48.000000 metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:31.000000 metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQLite/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-11-28 08:53:13.000000 metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py
+-rw-rw-rw-   0        0        0     1854 2023-11-28 11:03:59.000000 metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py
+-rw-rw-rw-   0        0        0       54 2023-12-20 14:54:15.000000 metabeaver-0.4.2/metabeaver/DatabaseFunctionality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.645776 metabeaver-0.4.2/metabeaver/DatesAndTime/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.2/metabeaver/DatesAndTime/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-03-06 21:17:29.000000 metabeaver-0.4.2/metabeaver/DatesAndTime/getToday.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.651327 metabeaver-0.4.2/metabeaver/Dynamic Programming/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/Dynamic Programming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.674808 metabeaver-0.4.2/metabeaver/FileIO/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/FileIO/__init__.py
+-rw-rw-rw-   0        0        0      389 2024-04-03 15:41:35.000000 metabeaver-0.4.2/metabeaver/FileIO/pickleObject.py
+-rw-rw-rw-   0        0        0      966 2024-03-02 22:41:17.000000 metabeaver-0.4.2/metabeaver/FileIO/yamlIO.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.701467 metabeaver-0.4.2/metabeaver/Formatting/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.2/metabeaver/Formatting/__init__.py
+-rw-rw-rw-   0        0        0      450 2023-09-02 17:13:50.000000 metabeaver-0.4.2/metabeaver/Formatting/printControl.py
+-rw-rw-rw-   0        0        0     1063 2023-10-04 07:18:25.000000 metabeaver-0.4.2/metabeaver/Formatting/printControlTest.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.701467 metabeaver-0.4.2/metabeaver/GoogleCloudPlatform/
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.761448 metabeaver-0.4.2/metabeaver/GoogleCloudPlatform/BigQuery/
+-rw-rw-rw-   0        0        0     7543 2024-04-04 20:44:03.000000 metabeaver-0.4.2/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.2/metabeaver/GoogleCloudPlatform/BigQuery/__init__.py
+-rw-rw-rw-   0        0        0     3388 2024-04-04 19:42:42.000000 metabeaver-0.4.2/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py
+-rw-rw-rw-   0        0        0      144 2024-01-05 19:00:29.000000 metabeaver-0.4.2/metabeaver/GoogleCloudPlatform/BigQuery/credentialsFromEnv.py
+-rw-rw-rw-   0        0        0     5440 2024-04-06 15:32:03.000000 metabeaver-0.4.2/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.2/metabeaver/GoogleCloudPlatform/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.789180 metabeaver-0.4.2/metabeaver/Graph Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/Graph Algorithms/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:48:31.000000 metabeaver-0.4.2/metabeaver/Graph Algorithms/bellmanFord.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:43:10.000000 metabeaver-0.4.2/metabeaver/Graph Algorithms/breadthFirstSearch.py
+-rw-rw-rw-   0        0        0      990 2024-02-13 10:13:17.000000 metabeaver-0.4.2/metabeaver/Graph Algorithms/depthFirstSearch.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:48:06.000000 metabeaver-0.4.2/metabeaver/Graph Algorithms/dijkstra.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 14:43:34.000000 metabeaver-0.4.2/metabeaver/Graph Algorithms/monteCarloTreeSearch.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.804464 metabeaver-0.4.2/metabeaver/Graphing/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:45:09.000000 metabeaver-0.4.2/metabeaver/Graphing/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-05-26 14:44:50.000000 metabeaver-0.4.2/metabeaver/Graphing/markdownGenerator.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.821561 metabeaver-0.4.2/metabeaver/InstallationScripts/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.2/metabeaver/InstallationScripts/__init__.py
+-rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.4.2/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.821561 metabeaver-0.4.2/metabeaver/InterviewQuestions/
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.852322 metabeaver-0.4.2/metabeaver/InterviewQuestions/Arrays/
+-rw-rw-rw-   0        0        0       54 2024-03-06 21:33:39.000000 metabeaver-0.4.2/metabeaver/InterviewQuestions/Arrays/__init__.py
+-rw-rw-rw-   0        0        0     1100 2024-01-16 09:07:23.000000 metabeaver-0.4.2/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py
+-rw-rw-rw-   0        0        0     2374 2024-02-12 11:00:27.000000 metabeaver-0.4.2/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py
+-rw-rw-rw-   0        0        0     3115 2024-01-10 09:29:29.000000 metabeaver-0.4.2/metabeaver/InterviewQuestions/Arrays/twoSum.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.884179 metabeaver-0.4.2/metabeaver/InterviewQuestions/Stacks/
+-rw-rw-rw-   0        0        0       54 2024-03-06 21:34:35.000000 metabeaver-0.4.2/metabeaver/InterviewQuestions/Stacks/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-10-24 15:28:24.000000 metabeaver-0.4.2/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/InterviewQuestions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.884179 metabeaver-0.4.2/metabeaver/LearnPython/
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.901090 metabeaver-0.4.2/metabeaver/LearnPython/ControlFlow/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/LearnPython/ControlFlow/__init__.py
+-rw-rw-rw-   0        0        0     2615 2024-03-01 09:39:54.000000 metabeaver-0.4.2/metabeaver/LearnPython/ControlFlow/ifelifelse.py
+-rw-rw-rw-   0        0        0       54 2024-02-20 17:10:29.000000 metabeaver-0.4.2/metabeaver/LearnPython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.921411 metabeaver-0.4.2/metabeaver/Machine Learning/
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.941644 metabeaver-0.4.2/metabeaver/Machine Learning/LLM/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/Machine Learning/LLM/__init__.py
+-rw-rw-rw-   0        0        0       54 2024-03-28 19:26:50.000000 metabeaver-0.4.2/metabeaver/Machine Learning/LLM/loadWithLlamaCPP.py
+-rw-rw-rw-   0        0        0     1996 2024-04-02 16:08:53.000000 metabeaver-0.4.2/metabeaver/Machine Learning/LLM/loadWithTransformers.py
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/Machine Learning/__init__.py
+-rw-rw-rw-   0        0        0     2915 2024-02-18 11:36:59.000000 metabeaver-0.4.2/metabeaver/Machine Learning/lassoRegression.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.951567 metabeaver-0.4.2/metabeaver/Mathematical Operations/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/Mathematical Operations/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 16:20:54.000000 metabeaver-0.4.2/metabeaver/Mathematical Operations/greatestCommonDenominator.py
+-rw-rw-rw-   0        0        0     1072 2024-03-01 15:21:44.000000 metabeaver-0.4.2/metabeaver/Mathematical Operations/vectorDotProduct.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.951567 metabeaver-0.4.2/metabeaver/MetaProgramming/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.2/metabeaver/MetaProgramming/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.963806 metabeaver-0.4.2/metabeaver/OperationBeaver/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.2/metabeaver/OperationBeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.975079 metabeaver-0.4.2/metabeaver/Search Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/Search Algorithms/__init__.py
+-rw-rw-rw-   0        0        0     2686 2023-11-01 10:30:45.000000 metabeaver-0.4.2/metabeaver/Search Algorithms/binarySearch.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:40.001470 metabeaver-0.4.2/metabeaver/Set Theory/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/Set Theory/__init__.py
+-rw-rw-rw-   0        0        0     5497 2023-10-06 17:16:32.000000 metabeaver-0.4.2/metabeaver/Set Theory/findAllSubsets.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:40.066406 metabeaver-0.4.2/metabeaver/Sorting Algorithms/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/Sorting Algorithms/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-12-12 09:32:50.000000 metabeaver-0.4.2/metabeaver/Sorting Algorithms/heapSort.py
+-rw-rw-rw-   0        0        0     1539 2023-10-15 18:11:43.000000 metabeaver-0.4.2/metabeaver/Sorting Algorithms/insertionSort.py
+-rw-rw-rw-   0        0        0     1275 2024-01-09 08:35:40.000000 metabeaver-0.4.2/metabeaver/Sorting Algorithms/mergeSort.py
+-rw-rw-rw-   0        0        0     1136 2023-10-13 07:08:11.000000 metabeaver-0.4.2/metabeaver/Sorting Algorithms/quickSort.py
+-rw-rw-rw-   0        0        0     3213 2023-10-12 10:18:23.000000 metabeaver-0.4.2/metabeaver/Sorting Algorithms/timsort.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:40.081606 metabeaver-0.4.2/metabeaver/Testing/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.2/metabeaver/Testing/__init__.py
+-rw-rw-rw-   0        0        0     3544 2023-11-03 10:47:27.000000 metabeaver-0.4.2/metabeaver/Testing/scratchPad.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:40.111527 metabeaver-0.4.2/metabeaver/TextValidation/
+-rw-rw-rw-   0        0        0        0 2023-11-01 10:48:19.000000 metabeaver-0.4.2/metabeaver/TextValidation/__init__.py
+-rw-rw-rw-   0        0        0     1418 2023-09-27 14:33:38.000000 metabeaver-0.4.2/metabeaver/TextValidation/closureChecker.py
+-rw-rw-rw-   0        0        0     4004 2023-11-01 10:50:46.000000 metabeaver-0.4.2/metabeaver/TextValidation/establishLargestPalindrome.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:40.141210 metabeaver-0.4.2/metabeaver/WebScraping/
+-rw-rw-rw-   0        0        0       54 2023-11-28 09:31:41.000000 metabeaver-0.4.2/metabeaver/WebScraping/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-11-28 09:40:35.000000 metabeaver-0.4.2/metabeaver/WebScraping/simpleRequests.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.4.2/metabeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:39.351562 metabeaver-0.4.2/metabeaver.egg-info/
+-rw-rw-rw-   0        0        0      615 2024-04-06 15:33:38.000000 metabeaver-0.4.2/metabeaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4078 2024-04-06 15:33:38.000000 metabeaver-0.4.2/metabeaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 15:33:38.000000 metabeaver-0.4.2/metabeaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-06 15:33:38.000000 metabeaver-0.4.2/metabeaver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-06 15:33:38.000000 metabeaver-0.4.2/metabeaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 15:33:40.141210 metabeaver-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1299 2024-04-06 15:32:30.000000 metabeaver-0.4.2/setup.py
```

### Comparing `metabeaver-0.4.1/PKG-INFO` & `metabeaver-0.4.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: metabeaver
-Version: 0.4.1
+Version: 0.4.2
 Summary: Beaverish about data. Metabeaver originally started as a "glue" project to bring together commonly used code. It has since expanded to contain common operations, metaprogramming, and Computer Sci resources. It is intended a resource to learn computer science, Python, and limit the need to rebuild the wheel. For development operations, please see Operation Beaver.
 Home-page: https://github.com/rainbowpusheenthe3rd/dataBeaver
 Author: Luke Anthony Pollen
 Author-email: luke@pollenanalytics.com
-Requires-Dist: google-cloud-bigquery
-Requires-Dist: google-cloud-core
-Requires-Dist: numpy
-Requires-Dist: pandas
+License: UNKNOWN
+Platform: UNKNOWN
+
+UNKNOWN
+
```

### Comparing `metabeaver-0.4.1/metabeaver/BeaverTown/abstractBeaver.py` & `metabeaver-0.4.2/metabeaver/BeaverTown/abstractBeaver.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/BeaverTown/beaverOn.py` & `metabeaver-0.4.2/metabeaver/BeaverTown/beaverOn.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Binary/binaryOperations.py` & `metabeaver-0.4.2/metabeaver/Binary/binaryOperations.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Caching/LeastRecentlyUsed.py` & `metabeaver-0.4.2/metabeaver/Caching/LeastRecentlyUsed.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/DataManipulation/filterPandas.py` & `metabeaver-0.4.2/metabeaver/DataManipulation/filterPandas.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/DataManipulation/localPickle.py` & `metabeaver-0.4.2/metabeaver/DataManipulation/localPickle.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/DataManipulation/universalResourceLinkHandler.py` & `metabeaver-0.4.2/metabeaver/DataManipulation/universalResourceLinkHandler.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/DataStructures/BinarySearchTree.py` & `metabeaver-0.4.2/metabeaver/DataStructures/BinarySearchTree.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQL/rawSQL.py` & `metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQL/rawSQL.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py` & `metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQLite/SQLiteDatabase.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py` & `metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQLite/commonCreateUpdate.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py` & `metabeaver-0.4.2/metabeaver/DatabaseFunctionality/SQLite/inspectTable.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/DatesAndTime/getToday.py` & `metabeaver-0.4.2/metabeaver/DatesAndTime/getToday.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/FileIO/yamlIO.py` & `metabeaver-0.4.2/metabeaver/FileIO/yamlIO.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Formatting/printControlTest.py` & `metabeaver-0.4.2/metabeaver/Formatting/printControlTest.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py` & `metabeaver-0.4.2/metabeaver/GoogleCloudPlatform/BigQuery/TableManagement.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py` & `metabeaver-0.4.2/metabeaver/GoogleCloudPlatform/BigQuery/clientFromCredentials.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py` & `metabeaver-0.4.2/metabeaver/GoogleCloudPlatform/BigQuery/getTableData.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 import datetime as dt
 import json
 import pandas as pd
 import yaml
 from google.cloud import bigquery
 
 
-# Assume a config-yaml file with valid GCP credentials.json filepath, used to get X rows of data.
-def getData(x):
+def getData(x,
+            project_name=None, # GCP project to target. Defaults to config-yaml.yaml value if not over-ridden.
+            dataset=None, # GCP BigQuery dataset to target. Defaults to yaml value if not over-ridden.
+            table_name=None, # GCP BigQuery dataset-table to target. Defaults to yaml value if not over-ridden.
+            credentials_file_loc=None, # Valid credentials.json for GCP. Default to yaml value if not over-ridden.
+            ):
 
     # Get the credentials for the API calls
     with open('config-yaml.yaml', 'r') as file:
         configuration = yaml.safe_load(file)
 
     # Get the path of the credentials and the project name for dynamically requesting a GCP BigQuery client
-    credentials_path = configuration['GCP']['credentials_file_loc']
-    gcp_project = configuration['GCP']['project_name']
+    if credentials_file_loc is None:
+        credentials_file_loc = configuration['GCP'].get('credentials_file_loc')
+    if project_name is None:
+        project_name = configuration['GCP'].get('project_name')
+
+    # Check if dataset and table_name are provided and, if not, use values from configuration, our config-yaml file.
+    if dataset is None:
+        dataset = configuration['GCP']['dataset']
+    if table_name is None:
+        table_name = configuration['GCP']['table_name']
 
-    # Load the credentials from the file path location specified in the yaml.
-    with open(credentials_path, 'r') as file:
+    # Load the credentials from the file path location specified in the yaml, or by user.
+    with open(credentials_file_loc, 'r') as file:
         credentials_info = json.load(file)
 
     # Use the 'from_service_account_info' method to dynamically load credentials from a file
     client = bigquery.Client.from_service_account_info(
         credentials_info,
-        project=gcp_project
+        project=project_name
     )
 
     # Get the first x rows from the table.
-    df = get_first_n_rows(client,
-                          configuration['GCP']['project_name'],
-                          configuration['GCP']['dataset'],
-                          configuration['GCP']['table_name'],
-                          x)
+    df = get_first_n_rows(client, project_name, dataset, table_name, x)
 
     return df
 
 
 # Fetches the first n rows from a bigquery table. Must receive a valid instantiated client
 def get_first_n_rows(client, project_id, dataset_id, table_id, n):
     """
```

### Comparing `metabeaver-0.4.1/metabeaver/Graph Algorithms/depthFirstSearch.py` & `metabeaver-0.4.2/metabeaver/Graph Algorithms/depthFirstSearch.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Graphing/markdownGenerator.py` & `metabeaver-0.4.2/metabeaver/Graphing/markdownGenerator.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/InstallationScripts/autoGenerateRequirementsText.py` & `metabeaver-0.4.2/metabeaver/InstallationScripts/autoGenerateRequirementsText.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py` & `metabeaver-0.4.2/metabeaver/InterviewQuestions/Arrays/bestTimeSellStock.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py` & `metabeaver-0.4.2/metabeaver/InterviewQuestions/Arrays/removeThirdDuplicate.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/InterviewQuestions/Arrays/twoSum.py` & `metabeaver-0.4.2/metabeaver/InterviewQuestions/Arrays/twoSum.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py` & `metabeaver-0.4.2/metabeaver/InterviewQuestions/Stacks/calculateFromSymbols.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/LearnPython/ControlFlow/ifelifelse.py` & `metabeaver-0.4.2/metabeaver/LearnPython/ControlFlow/ifelifelse.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Machine Learning/LLM/loadWithTransformers.py` & `metabeaver-0.4.2/metabeaver/Machine Learning/LLM/loadWithTransformers.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Machine Learning/lassoRegression.py` & `metabeaver-0.4.2/metabeaver/Machine Learning/lassoRegression.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Mathematical Operations/vectorDotProduct.py` & `metabeaver-0.4.2/metabeaver/Mathematical Operations/vectorDotProduct.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Search Algorithms/binarySearch.py` & `metabeaver-0.4.2/metabeaver/Search Algorithms/binarySearch.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Set Theory/findAllSubsets.py` & `metabeaver-0.4.2/metabeaver/Set Theory/findAllSubsets.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Sorting Algorithms/heapSort.py` & `metabeaver-0.4.2/metabeaver/Sorting Algorithms/heapSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Sorting Algorithms/insertionSort.py` & `metabeaver-0.4.2/metabeaver/Sorting Algorithms/insertionSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Sorting Algorithms/mergeSort.py` & `metabeaver-0.4.2/metabeaver/Sorting Algorithms/mergeSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Sorting Algorithms/quickSort.py` & `metabeaver-0.4.2/metabeaver/Sorting Algorithms/quickSort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Sorting Algorithms/timsort.py` & `metabeaver-0.4.2/metabeaver/Sorting Algorithms/timsort.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/Testing/scratchPad.py` & `metabeaver-0.4.2/metabeaver/Testing/scratchPad.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/TextValidation/closureChecker.py` & `metabeaver-0.4.2/metabeaver/TextValidation/closureChecker.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/TextValidation/establishLargestPalindrome.py` & `metabeaver-0.4.2/metabeaver/TextValidation/establishLargestPalindrome.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver/WebScraping/simpleRequests.py` & `metabeaver-0.4.2/metabeaver/WebScraping/simpleRequests.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/metabeaver.egg-info/PKG-INFO` & `metabeaver-0.4.2/metabeaver.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: metabeaver
-Version: 0.4.1
+Version: 0.4.2
 Summary: Beaverish about data. Metabeaver originally started as a "glue" project to bring together commonly used code. It has since expanded to contain common operations, metaprogramming, and Computer Sci resources. It is intended a resource to learn computer science, Python, and limit the need to rebuild the wheel. For development operations, please see Operation Beaver.
 Home-page: https://github.com/rainbowpusheenthe3rd/dataBeaver
 Author: Luke Anthony Pollen
 Author-email: luke@pollenanalytics.com
-Requires-Dist: google-cloud-bigquery
-Requires-Dist: google-cloud-core
-Requires-Dist: numpy
-Requires-Dist: pandas
+License: UNKNOWN
+Platform: UNKNOWN
+
+UNKNOWN
+
```

### Comparing `metabeaver-0.4.1/metabeaver.egg-info/SOURCES.txt` & `metabeaver-0.4.2/metabeaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metabeaver-0.4.1/setup.py` & `metabeaver-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metabeaver',
-    version='0.4.1', # Major, minor, patch
+    version='0.4.2', # Major, minor, patch
     packages=find_packages(exclude=['Testing', '*.xlsx', '*.xls']),
     install_requires=[
         'google-cloud-bigquery',
         'google-cloud-core',
         'numpy',
         'pandas',
         #transformers,
```

