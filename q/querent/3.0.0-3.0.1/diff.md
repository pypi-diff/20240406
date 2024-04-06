# Comparing `tmp/querent-3.0.0.tar.gz` & `tmp/querent-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querent-3.0.0.tar", last modified: Sun Mar 24 23:53:59 2024, max compression
+gzip compressed data, was "querent-3.0.1.tar", last modified: Sat Apr  6 14:19:49 2024, max compression
```

## Comparing `querent-3.0.0.tar` & `querent-3.0.1.tar`

### file list

```diff
@@ -1,266 +1,267 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.255647 querent-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-03-24 23:47:54.000000 querent-3.0.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    17136 2024-03-24 23:53:59.255647 querent-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-03-24 23:47:54.000000 querent-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.167647 querent-3.0.0/querent/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-24 23:47:54.000000 querent-3.0.0/querent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.171647 querent-3.0.0/querent/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-24 23:47:54.000000 querent-3.0.0/querent/callback/event_callback_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-24 23:47:54.000000 querent-3.0.0/querent/callback/event_callback_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.171647 querent-3.0.0/querent/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-24 23:47:54.000000 querent-3.0.0/querent/channel/channel_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.175647 querent-3.0.0/querent/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.175647 querent-3.0.0/querent/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.175647 querent-3.0.0/querent/collectors/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/aws/aws_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.179647 querent-3.0.0/querent/collectors/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/azure/azure_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/collector_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/collector_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/collector_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/collector_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.179647 querent-3.0.0/querent/collectors/drive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/drive/google_drive_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.179647 querent-3.0.0/querent/collectors/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/dropbox/dropbox_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.179647 querent-3.0.0/querent/collectors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/email/email_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/email/imap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.179647 querent-3.0.0/querent/collectors/fs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/fs/fs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.183647 querent-3.0.0/querent/collectors/gcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/gcs/gcs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.183647 querent-3.0.0/querent/collectors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/github/github_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.183647 querent-3.0.0/querent/collectors/jira/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/jira/jira_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.183647 querent-3.0.0/querent/collectors/news/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/news/news_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.183647 querent-3.0.0/querent/collectors/slack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/slack/slack_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.183647 querent-3.0.0/querent/collectors/webscaper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/webscaper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-03-24 23:47:54.000000 querent-3.0.0/querent/collectors/webscaper/web_scraper_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.187647 querent-3.0.0/querent/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/common_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.187647 querent-3.0.0/querent/common/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/errors/metric_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.195647 querent-3.0.0/querent/common/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/collected_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/collector_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/engine_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/file_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/ingested_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/ingested_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/ingested_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/ingested_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/querent_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/querent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/resource_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/types/workflow_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-24 23:47:54.000000 querent-3.0.0/querent/common/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.199647 querent-3.0.0/querent/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.199647 querent-3.0.0/querent/config/collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/collector/collector_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.199647 querent-3.0.0/querent/config/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/core/gpt_llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/core/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/core/opensource_llm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.199647 querent-3.0.0/querent/config/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/engine/engine_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/graph_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.203647 querent-3.0.0/querent/config/ingestor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/ingestor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/ingestor/ingestor_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.203647 querent-3.0.0/querent/config/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/logger/logger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.203647 querent-3.0.0/querent/config/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/metric/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.203647 querent-3.0.0/querent/config/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/resource/resource_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.203647 querent-3.0.0/querent/config/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-24 23:47:54.000000 querent-3.0.0/querent/config/workflow/workflow_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.203647 querent-3.0.0/querent/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.203647 querent-3.0.0/querent/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-03-24 23:47:54.000000 querent-3.0.0/querent/core/base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.207647 querent-3.0.0/querent/core/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/core/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13573 2024-03-24 23:47:54.000000 querent-3.0.0/querent/core/transformers/bert_ner_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-03-24 23:47:54.000000 querent-3.0.0/querent/core/transformers/fixed_entities_set_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-03-24 23:47:54.000000 querent-3.0.0/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    21230 2024-03-24 23:47:54.000000 querent-3.0.0/querent/core/transformers/gpt_llm_gpt_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-03-24 23:47:54.000000 querent-3.0.0/querent/core/transformers/relationship_extraction_llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.207647 querent-3.0.0/querent/dal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/dal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.207647 querent-3.0.0/querent/gnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/gnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.215647 querent-3.0.0/querent/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-24 23:47:54.000000 querent-3.0.0/querent/graph/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-03-24 23:47:54.000000 querent-3.0.0/querent/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-03-24 23:47:54.000000 querent-3.0.0/querent/graph/graph_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-24 23:47:54.000000 querent-3.0.0/querent/graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-24 23:47:54.000000 querent-3.0.0/querent/graph/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-03-24 23:47:54.000000 querent-3.0.0/querent/graph/shacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-03-24 23:47:54.000000 querent-3.0.0/querent/graph/subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-03-24 23:47:54.000000 querent-3.0.0/querent/graph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.215647 querent-3.0.0/querent/ingestors/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.215647 querent-3.0.0/querent/ingestors/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/audio/audio_ingestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/base_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.219647 querent-3.0.0/querent/ingestors/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/code/code_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.219647 querent-3.0.0/querent/ingestors/csv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/csv/csv_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.219647 querent-3.0.0/querent/ingestors/doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/doc/doc_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.219647 querent-3.0.0/querent/ingestors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/email/email_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/email/email_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.223647 querent-3.0.0/querent/ingestors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/github/github_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.223647 querent-3.0.0/querent/ingestors/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/html/html_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.223647 querent-3.0.0/querent/ingestors/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/images/image_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/ingestor_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/ingestor_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.223647 querent-3.0.0/querent/ingestors/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/json/json_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.223647 querent-3.0.0/querent/ingestors/pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/pdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/pdfs/pdf_ingestor_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.223647 querent-3.0.0/querent/ingestors/ppt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/ppt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/ppt/ppt_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.227647 querent-3.0.0/querent/ingestors/texts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/texts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/texts/text_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.227647 querent-3.0.0/querent/ingestors/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/video/video_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.227647 querent-3.0.0/querent/ingestors/xlsx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/xlsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/xlsx/xlsx_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.227647 querent-3.0.0/querent/ingestors/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-03-24 23:47:54.000000 querent-3.0.0/querent/ingestors/xml/xml_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.227647 querent-3.0.0/querent/insights/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/insights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.227647 querent-3.0.0/querent/kg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.231647 querent-3.0.0/querent/kg/ner_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/ner_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/ner_helperfunctions/attn_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/ner_helperfunctions/contextual_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/ner_helperfunctions/dependency_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/ner_helperfunctions/filter_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/ner_helperfunctions/fixed_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/ner_helperfunctions/fixed_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/ner_helperfunctions/ner_llm_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/querent_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.239647 querent-3.0.0/querent/kg/rel_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/contextual_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/embedding_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/filter_semantic_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/fixed_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/openai_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/openllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/questionanswer_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/rag_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/rel_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-24 23:47:54.000000 querent-3.0.0/querent/kg/rel_helperfunctions/triple_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.243647 querent-3.0.0/querent/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-24 23:47:54.000000 querent-3.0.0/querent/logging/custom_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-24 23:47:54.000000 querent-3.0.0/querent/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-24 23:47:54.000000 querent-3.0.0/querent/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-24 23:47:54.000000 querent-3.0.0/querent/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.243647 querent-3.0.0/querent/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.243647 querent-3.0.0/querent/metric/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/metric/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-24 23:47:54.000000 querent-3.0.0/querent/metric/adapters/promethus_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-24 23:47:54.000000 querent-3.0.0/querent/metric/base_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-24 23:47:54.000000 querent-3.0.0/querent/metric/metric_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-24 23:47:54.000000 querent-3.0.0/querent/metric/metric_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.247647 querent-3.0.0/querent/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-24 23:47:54.000000 querent-3.0.0/querent/processors/async_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-24 23:47:54.000000 querent-3.0.0/querent/processors/text_cleanup_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-03-24 23:47:54.000000 querent-3.0.0/querent/processors/text_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.247647 querent-3.0.0/querent/querent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/querent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-03-24 23:47:54.000000 querent-3.0.0/querent/querent/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-03-24 23:47:54.000000 querent-3.0.0/querent/querent/querent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-24 23:47:54.000000 querent-3.0.0/querent/querent/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/querent/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.247647 querent-3.0.0/querent/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.247647 querent-3.0.0/querent/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-24 23:47:54.000000 querent-3.0.0/querent/storage/milvus_vectorevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-24 23:47:54.000000 querent-3.0.0/querent/storage/neo4j_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-24 23:47:54.000000 querent-3.0.0/querent/storage/postgres_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-03-24 23:47:54.000000 querent-3.0.0/querent/storage/s3-data-management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.251647 querent-3.0.0/querent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-03-24 23:47:54.000000 querent-3.0.0/querent/tools/web_page_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.251647 querent-3.0.0/querent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:47:54.000000 querent-3.0.0/querent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-03-24 23:47:54.000000 querent-3.0.0/querent/utils/webpage_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.251647 querent-3.0.0/querent/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-24 23:47:54.000000 querent-3.0.0/querent/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-03-24 23:47:54.000000 querent-3.0.0/querent/workflow/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-03-24 23:47:54.000000 querent-3.0.0/querent/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:53:59.251647 querent-3.0.0/querent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17136 2024-03-24 23:53:59.000000 querent-3.0.0/querent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-03-24 23:53:59.000000 querent-3.0.0/querent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 23:53:59.000000 querent-3.0.0/querent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-24 23:53:59.000000 querent-3.0.0/querent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-24 23:53:59.000000 querent-3.0.0/querent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 23:53:59.255647 querent-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-03-24 23:47:54.000000 querent-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.556272 querent-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-06 14:13:26.000000 querent-3.0.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    17135 2024-04-06 14:19:49.556272 querent-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-06 14:13:26.000000 querent-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.476271 querent-3.0.1/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-06 14:13:26.000000 querent-3.0.1/querent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.480271 querent-3.0.1/querent/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-06 14:13:26.000000 querent-3.0.1/querent/callback/event_callback_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-06 14:13:26.000000 querent-3.0.1/querent/callback/event_callback_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.484271 querent-3.0.1/querent/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-06 14:13:26.000000 querent-3.0.1/querent/channel/channel_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.484271 querent-3.0.1/querent/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.488271 querent-3.0.1/querent/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.488271 querent-3.0.1/querent/collectors/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/aws/aws_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.488271 querent-3.0.1/querent/collectors/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/azure/azure_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/collector_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/collector_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/collector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/collector_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.488271 querent-3.0.1/querent/collectors/drive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/drive/google_drive_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.492271 querent-3.0.1/querent/collectors/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/dropbox/dropbox_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.492271 querent-3.0.1/querent/collectors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/email/email_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/email/imap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.492271 querent-3.0.1/querent/collectors/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/fs/fs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.492271 querent-3.0.1/querent/collectors/gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/gcs/gcs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.492271 querent-3.0.1/querent/collectors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/github/github_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/collectors/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/jira/jira_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/collectors/news/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/news/news_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/collectors/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/slack/slack_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/collectors/webscaper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/webscaper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/webscaper/web_scraper_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/common_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/common/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/errors/metric_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.504271 querent-3.0.1/querent/common/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/collected_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/collector_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/engine_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/file_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/ingested_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/ingested_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/ingested_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/ingested_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/querent_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/querent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/resource_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/workflow_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.504271 querent-3.0.1/querent/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.504271 querent-3.0.1/querent/config/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/collector/collector_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.504271 querent-3.0.1/querent/config/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/core/gpt_llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/core/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/core/opensource_llm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.504271 querent-3.0.1/querent/config/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/engine/engine_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/graph_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/config/ingestor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/ingestor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/ingestor/ingestor_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/config/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/logger/logger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/config/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/metric/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/config/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/resource/resource_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/config/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/workflow/workflow_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.512272 querent-3.0.1/querent/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/bert_ner_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/fixed_entities_set_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16808 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21403 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/gpt_llm_gpt_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/relationship_extraction_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.512272 querent-3.0.1/querent/dal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/dal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.512272 querent-3.0.1/querent/gnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/gnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.516271 querent-3.0.1/querent/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/graph_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/shacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.516271 querent-3.0.1/querent/ingestors/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.516271 querent-3.0.1/querent/ingestors/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/audio/audio_ingestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/base_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/code/code_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/csv/csv_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/doc/doc_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/email/email_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/email/email_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/github/github_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/html/html_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/images/image_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/ingestor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/ingestor_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/json/json_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/pdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/pdfs/pdf_ingestor_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/ppt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/ppt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/ppt/ppt_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/texts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/texts/text_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/video/video_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/xlsx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/xlsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/xlsx/xlsx_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.528272 querent-3.0.1/querent/ingestors/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/xml/xml_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.528272 querent-3.0.1/querent/insights/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/insights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.528272 querent-3.0.1/querent/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.532272 querent-3.0.1/querent/kg/ner_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/attn_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/contextual_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/dependency_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/filter_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/fixed_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/fixed_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/ner_llm_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/querent_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.536272 querent-3.0.1/querent/kg/rel_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/contextual_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/embedding_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/filter_semantic_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/fixed_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/openai_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/openllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/questionanswer_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/rag_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/rel_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/triple_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.544272 querent-3.0.1/querent/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-06 14:13:26.000000 querent-3.0.1/querent/logging/custom_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-06 14:13:26.000000 querent-3.0.1/querent/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-06 14:13:26.000000 querent-3.0.1/querent/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-06 14:13:26.000000 querent-3.0.1/querent/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.548272 querent-3.0.1/querent/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.548272 querent-3.0.1/querent/metric/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/adapters/promethus_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/base_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/metric_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/metric_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.548272 querent-3.0.1/querent/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 14:13:26.000000 querent-3.0.1/querent/processors/async_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-06 14:13:26.000000 querent-3.0.1/querent/processors/text_cleanup_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-06 14:13:26.000000 querent-3.0.1/querent/processors/text_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.552272 querent-3.0.1/querent/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/querent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-06 14:13:26.000000 querent-3.0.1/querent/querent/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-06 14:13:26.000000 querent-3.0.1/querent/querent/querent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-06 14:13:26.000000 querent-3.0.1/querent/querent/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/querent/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.552272 querent-3.0.1/querent/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.552272 querent-3.0.1/querent/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/gcs_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/milvus_vectorevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/neo4j_graphevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/postgres_graphevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/s3-data-management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.552272 querent-3.0.1/querent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-06 14:13:26.000000 querent-3.0.1/querent/tools/web_page_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.556272 querent-3.0.1/querent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-06 14:13:26.000000 querent-3.0.1/querent/utils/webpage_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.556272 querent-3.0.1/querent/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 14:13:26.000000 querent-3.0.1/querent/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-06 14:13:26.000000 querent-3.0.1/querent/workflow/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-06 14:13:26.000000 querent-3.0.1/querent/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.556272 querent-3.0.1/querent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17135 2024-04-06 14:19:49.000000 querent-3.0.1/querent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-06 14:19:49.000000 querent-3.0.1/querent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 14:19:49.000000 querent-3.0.1/querent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-06 14:19:49.000000 querent-3.0.1/querent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 14:19:49.000000 querent-3.0.1/querent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 14:19:49.556272 querent-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-06 14:13:26.000000 querent-3.0.1/setup.py
```

### Comparing `querent-3.0.0/LICENCE` & `querent-3.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/PKG-INFO` & `querent-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.0
+Version: 3.0.1
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -36,27 +36,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: cachetools==5.3.3
-Requires-Dist: aiohttp==3.9.2
+Requires-Dist: aiohttp==3.9.3
 Requires-Dist: attrs==23.1.0
-Requires-Dist: beautifulsoup4==4.12.2
+Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: boto3==1.26.146
 Requires-Dist: botocore==1.29.146
 Requires-Dist: bs4==0.0.1
 Requires-Dist: faiss-cpu==1.7.4
 Requires-Dist: gensim==4.3.2
 Requires-Dist: hdbscan==0.8.33
 Requires-Dist: jira==3.6.0
 Requires-Dist: jmespath==1.0.1
 Requires-Dist: joblib==1.2.0
-Requires-Dist: json5==0.9.14
+Requires-Dist: json5==0.9.24
 Requires-Dist: jsonmerge==1.9.0
 Requires-Dist: jsonschema==4.17.3
 Requires-Dist: kombu==5.2.4
 Requires-Dist: llama_cpp_python==0.2.15
 Requires-Dist: lxml==4.9.2
 Requires-Dist: newspaper3k==0.2.8
 Requires-Dist: nltk==3.8.1
@@ -66,29 +66,29 @@
 Requires-Dist: PyJWT==2.4.0
 Requires-Dist: pytest==7.3.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: redis==5.0.3
 Requires-Dist: regex==2023.5.5
 Requires-Dist: sentence-transformers==2.2.2
 Requires-Dist: spacy==3.7.2
-Requires-Dist: uvicorn==0.22.0
+Requires-Dist: uvicorn==0.29.0
 Requires-Dist: slack-sdk==3.26.1
 Requires-Dist: pylint==2.17.4
 Requires-Dist: pytest-cov==4.1.0
 Requires-Dist: pytest-mock==3.11.1
 Requires-Dist: tensorflow==2.14.0
 Requires-Dist: transformers==4.36.0
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: prometheus-client==0.17.1
 Requires-Dist: rdflib==7.0.0
 Requires-Dist: pytest-asyncio==0.23.2
 Requires-Dist: pyshacl==0.25.0
 Requires-Dist: google-cloud-storage==2.14.0
-Requires-Dist: PyMuPDF==1.23.26
+Requires-Dist: PyMuPDF==1.24.0
 Requires-Dist: pydub==0.25.1
 Requires-Dist: SpeechRecognition==3.10.1
 Requires-Dist: pytesseract==0.3.10
 Requires-Dist: pytextract==2.0.1
 Requires-Dist: pandas==2.1.4
 Requires-Dist: python-pptx==0.6.23
 Requires-Dist: tika==2.6.0
```

### Comparing `querent-3.0.0/README.md` & `querent-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/__init__.py` & `querent-3.0.1/querent/__init__.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/callback/event_callback_dispatcher.py` & `querent-3.0.1/querent/callback/event_callback_dispatcher.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/callback/event_callback_interface.py` & `querent-3.0.1/querent/callback/event_callback_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/channel/channel_interface.py` & `querent-3.0.1/querent/channel/channel_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/aws/aws_collector.py` & `querent-3.0.1/querent/collectors/aws/aws_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/azure/azure_collector.py` & `querent-3.0.1/querent/collectors/azure/azure_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/collector_errors.py` & `querent-3.0.1/querent/collectors/collector_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/collector_factory.py` & `querent-3.0.1/querent/collectors/collector_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/collector_resolver.py` & `querent-3.0.1/querent/collectors/collector_resolver.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/drive/google_drive_collector.py` & `querent-3.0.1/querent/collectors/drive/google_drive_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/dropbox/dropbox_collector.py` & `querent-3.0.1/querent/collectors/dropbox/dropbox_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/email/email_collector.py` & `querent-3.0.1/querent/collectors/email/email_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/email/imap.py` & `querent-3.0.1/querent/collectors/email/imap.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/fs/fs_collector.py` & `querent-3.0.1/querent/collectors/fs/fs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/gcs/gcs_collector.py` & `querent-3.0.1/querent/collectors/gcs/gcs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/github/github_collector.py` & `querent-3.0.1/querent/collectors/github/github_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/jira/jira_collector.py` & `querent-3.0.1/querent/collectors/jira/jira_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/slack/slack_collector.py` & `querent-3.0.1/querent/collectors/slack/slack_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/collectors/webscaper/web_scraper_collector.py` & `querent-3.0.1/querent/collectors/webscaper/web_scraper_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/common/common_errors.py` & `querent-3.0.1/querent/common/common_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/common/errors/metric_errors.py` & `querent-3.0.1/querent/common/errors/metric_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/common/types/collected_bytes.py` & `querent-3.0.1/querent/common/types/collected_bytes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/common/types/file_buffer.py` & `querent-3.0.1/querent/common/types/file_buffer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/common/types/ingested_code.py` & `querent-3.0.1/querent/common/types/ingested_code.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/common/types/ingested_images.py` & `querent-3.0.1/querent/common/types/ingested_images.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/common/types/ingested_messages.py` & `querent-3.0.1/querent/common/types/ingested_messages.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/common/types/ingested_tokens.py` & `querent-3.0.1/querent/common/types/ingested_tokens.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/common/types/querent_queue.py` & `querent-3.0.1/querent/common/types/querent_queue.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/common/uri.py` & `querent-3.0.1/querent/common/uri.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/config/collector/collector_config.py` & `querent-3.0.1/querent/config/collector/collector_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/config/config.py` & `querent-3.0.1/querent/config/config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/config/core/gpt_llm_config.py` & `querent-3.0.1/querent/config/core/gpt_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/config/core/llm_config.py` & `querent-3.0.1/querent/config/core/llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/config/core/opensource_llm_config.py` & `querent-3.0.1/querent/config/core/opensource_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/config/engine/engine_config.py` & `querent-3.0.1/querent/config/engine/engine_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/config/graph_config.py` & `querent-3.0.1/querent/config/graph_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/config/ingestor/ingestor_config.py` & `querent-3.0.1/querent/config/ingestor/ingestor_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,7 +28,8 @@
     AVI = "avi"
     WAV = "wav"
     GITHUB = "github"
     Unsupported = "unsupported"
     Email = "email"
     Slack = "slack"
     Jira = "jira"
+    News = "news"
```

### Comparing `querent-3.0.0/querent/config/metric/prometheus.py` & `querent-3.0.1/querent/config/metric/prometheus.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/config/resource/resource_config.py` & `querent-3.0.1/querent/config/resource/resource_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/config/workflow/workflow_config.py` & `querent-3.0.1/querent/config/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/core/base_engine.py` & `querent-3.0.1/querent/core/base_engine.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/core/transformers/bert_ner_opensourcellm.py` & `querent-3.0.1/querent/core/transformers/bert_ner_opensourcellm.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,21 +205,24 @@
                     relationships = self.semantic_extractor.process_tokens(filtered_triples)
                     relationships = self.semantictriplefilter.filter_triples(relationships)
                     if len(relationships) > 0:
                         embedding_triples = self.create_emb.generate_embeddings(relationships)
                         if self.sample_relationships:
                             embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
                         for triple in embedding_triples:
-                            graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
-                            if graph_json:
-                                current_state = EventState(EventType.Graph,1.0, graph_json, file)
-                                await self.set_state(new_state=current_state)
-                            vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
-                            if vector_json:
-                                current_state = EventState(EventType.Vector,1.0, vector_json, file)
-                                await self.set_state(new_state=current_state)
+                            if not self.termination_event.is_set():
+                                graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
+                                if graph_json:
+                                    current_state = EventState(EventType.Graph,1.0, graph_json, file)
+                                    await self.set_state(new_state=current_state)
+                                vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
+                                if vector_json:
+                                    current_state = EventState(EventType.Vector,1.0, vector_json, file)
+                                    await self.set_state(new_state=current_state)
+                            else:
+                                return
                     else:
                         return
                 else:
                     return filtered_triples, file
         except Exception as e:
             self.logger.debug(f"Invalid {self.__class__.__name__} configuration. Unable to process tokens. {e}")
```

### Comparing `querent-3.0.0/querent/core/transformers/fixed_entities_set_opensourcellm.py` & `querent-3.0.1/querent/core/transformers/fixed_entities_set_opensourcellm.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,22 +169,25 @@
                     self.logger.debug(f"length of relationships {len(relationships)}")
                     relationships = self.semantictriplefilter.filter_triples(relationships)
                     if len(relationships) > 0:
                         embedding_triples = self.create_emb.generate_embeddings(relationships)
                         if self.sample_relationships:
                             embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
                         for triple in embedding_triples:
-                            graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
-                            if graph_json:
-                                current_state = EventState(EventType.Graph,1.0, graph_json, file)
-                                await self.set_state(new_state=current_state)
-                            vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
-                            if vector_json:
-                                current_state = EventState(EventType.Vector,1.0, vector_json, file)
-                                await self.set_state(new_state=current_state)
+                            if not self.termination_event.is_set():
+                                graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
+                                if graph_json:
+                                    current_state = EventState(EventType.Graph,1.0, graph_json, file)
+                                    await self.set_state(new_state=current_state)
+                                vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
+                                if vector_json:
+                                    current_state = EventState(EventType.Vector,1.0, vector_json, file)
+                                    await self.set_state(new_state=current_state)
+                            else:
+                                return
                     else:
                         return
                 else:
                     return filtered_triples, file
             else:
                 return
         except Exception as e:
```

### Comparing `querent-3.0.0/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py` & `querent-3.0.1/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,21 +273,24 @@
                         output_tuple = self.generate_output_tuple(result, context_json)
                         relationships.append(output_tuple)
                 if len(relationships) > 0:
                     embedding_triples = self.create_emb.generate_embeddings(relationships)
                     if self.sample_relationships:
                             embedding_triples = self.predicate_context_extractor.process_predicate_types(embedding_triples)
                     for triple in embedding_triples:
-                        graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
-                        if graph_json:
-                                current_state = EventState(EventType.Graph,1.0, graph_json, file)
-                                await self.set_state(new_state=current_state)
-                        vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
-                        if vector_json:
-                                current_state = EventState(EventType.Vector,1.0, vector_json, file)
-                                await self.set_state(new_state=current_state)
+                        if not self.termination_event.is_set():
+                            graph_json = json.dumps(TripleToJsonConverter.convert_graphjson(triple))
+                            if graph_json:
+                                    current_state = EventState(EventType.Graph,1.0, graph_json, file)
+                                    await self.set_state(new_state=current_state)
+                            vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson(triple))
+                            if vector_json:
+                                    current_state = EventState(EventType.Vector,1.0, vector_json, file)
+                                    await self.set_state(new_state=current_state)
+                        else:
+                            return
         except Exception as e:
             self.logger.error(f"Invalid {self.__class__.__name__} configuration. Unable to extract predicates using GPT. {e}")
             raise Exception(f"An error occurred while extracting predicates using GPT: {e}")
 
     async def process_messages(self, data: IngestedMessages):
         raise NotImplementedError
```

### Comparing `querent-3.0.0/querent/core/transformers/gpt_llm_gpt_ner.py` & `querent-3.0.1/querent/core/transformers/gpt_llm_gpt_ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,24 +239,27 @@
                         continue
                     if len(relevant_triples)>0:
                         final_triples.extend(relevant_triples)
                 #final_triples = [{'subject': 'paleocene–eocene thermal maximum (petm) record', 'predicate': 'is present in', 'object': '543-m-thick (1780 ft) deep-marine section in the gulf of mexico (gom)', 'subject_type': 'event', 'object_type': 'location', 'predicate_type': 'occurrence', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM.'}, {'subject': 'climate and tectonic perturbations', 'predicate': 'can induce', 'object': 'a substantial response', 'subject_type': 'process', 'object_type': 'event', 'predicate_type': 'causative', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM.'}, {'subject': 'gulf coastal plain', 'predicate': 'is', 'object': 'ultimately in the gom', 'subject_type': 'location', 'object_type': 'location', 'predicate_type': 'ownership', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM.'}, {'subject': 'paleocene–eocene thermal maximum (petm) record', 'predicate': 'is present in', 'object': '543-m-thick (1780 ft) deep-marine section in the gulf of mexico (gom)', 'subject_type': 'event', 'object_type': 'location', 'predicate_type': 'occurrence', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin.'}, {'subject': 'climate and tectonic perturbations', 'predicate': 'can induce', 'object': 'a substantial response', 'subject_type': 'process', 'object_type': 'event', 'predicate_type': 'causative', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin.'}, {'subject': 'upstream north american catchments', 'predicate': 'can induce', 'object': 'a substantial response', 'subject_type': 'location', 'object_type': 'event', 'predicate_type': 'causative', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin.'}, {'subject': 'downstream sectors of the gulf coastal plain', 'predicate': 'can be impacted by', 'object': 'upstream north american catchments', 'subject_type': 'location', 'object_type': 'location', 'predicate_type': 'causative', 'sentence': 'ABSTRACT In this study, we present evidence of a Paleocene–Eocene Thermal Maximum (PETM) record within a 543-m-thick (1780 ft) deep-marine section in the Gulf of Mexico (GoM) using organic carbon stable isotopes and biostratigraphic constraints. We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin.'}, {'subject': 'climate and tectonic perturbations', 'predicate': 'can induce', 'object': 'a substantial response', 'subject_type': 'process', 'object_type': 'event', 'predicate_type': 'causative', 'sentence': 'We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin. Despite other thick PETM sections being observed elsewhere in the world, the one described in this study links with a continental- scale paleo-drainage, which makes it of particular interest for paleoclimate and source- to-sink reconstructions.'}, {'subject': 'upstream north american catchments', 'predicate': 'can induce', 'object': 'a substantial response', 'subject_type': 'location', 'object_type': 'event', 'predicate_type': 'causative', 'sentence': 'We suggest that climate and tectonic perturbations in the upstream North American catchments can induce a substantial response in the downstream sectors of the Gulf Coastal Plain and ultimately in the GoM. This relationship is illustrated in the deep-water basin by (1) a high accom- modation and deposition of a shale interval when coarse-grained terrigenous material was trapped upstream at the onset of the PETM, and (2) a considerable increase in sedi- ment supply during the PETM, which is archived as a particularly thick sedimentary section in the deep-sea fans of the GoM basin. Despite other thick PETM sections being observed elsewhere in the world, the one described in this study links with a continental- scale paleo-drainage, which makes it of particular interest for paleoclimate and source- to-sink reconstructions.'}]
                 final_triples = self.remove_duplicate_triplets(final_triples)
                 if len(final_triples) > 0:
                     for triple in final_triples:
-                        graph_json = json.dumps(triple)
-                        if graph_json:
-                            current_state = EventState(EventType.Graph,1.0, graph_json, file)
-                            await self.set_state(new_state=current_state)
-                        context_embeddings = self.create_emb.get_embeddings([triple['sentence']])[0]
-                        triple['context_embeddings'] = context_embeddings
-                        triple['context'] = triple['sentence']
-                        vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson((triple['subject'],json.dumps(triple), triple['object'])))
-                        if vector_json:
-                                current_state = EventState(EventType.Vector,1.0, vector_json, file)
+                        if not self.termination_event.is_set():
+                            graph_json = json.dumps(triple)
+                            if graph_json:
+                                current_state = EventState(EventType.Graph,1.0, graph_json, file)
                                 await self.set_state(new_state=current_state)
+                            context_embeddings = self.create_emb.get_embeddings([triple['sentence']])[0]
+                            triple['context_embeddings'] = context_embeddings
+                            triple['context'] = triple['sentence']
+                            vector_json = json.dumps(TripleToJsonConverter.convert_vectorjson((triple['subject'],json.dumps(triple), triple['object'])))
+                            if vector_json:
+                                    current_state = EventState(EventType.Vector,1.0, vector_json, file)
+                                    await self.set_state(new_state=current_state)
+                        else:
+                            return
 
         except Exception as e:
             self.logger.debug(f"Invalid {self.__class__.__name__} configuration. Unable to extract predicates using GPT NER LLM class. {e}")
     
     async def process_messages(self, data: IngestedMessages):
         raise NotImplementedError
```

### Comparing `querent-3.0.0/querent/core/transformers/relationship_extraction_llm.py` & `querent-3.0.1/querent/core/transformers/relationship_extraction_llm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/graph/errors.py` & `querent-3.0.1/querent/graph/errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/graph/graph.py` & `querent-3.0.1/querent/graph/graph.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/graph/graph_namespace.py` & `querent-3.0.1/querent/graph/graph_namespace.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/graph/ontology.py` & `querent-3.0.1/querent/graph/ontology.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/graph/schema.py` & `querent-3.0.1/querent/graph/schema.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/graph/shacl.py` & `querent-3.0.1/querent/graph/shacl.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/graph/subject.py` & `querent-3.0.1/querent/graph/subject.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/graph/utils.py` & `querent-3.0.1/querent/graph/utils.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/audio/audio_ingestors.py` & `querent-3.0.1/querent/ingestors/audio/audio_ingestors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/base_ingestor.py` & `querent-3.0.1/querent/ingestors/base_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/code/code_ingestor.py` & `querent-3.0.1/querent/ingestors/code/code_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/csv/csv_ingestor.py` & `querent-3.0.1/querent/ingestors/csv/csv_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/doc/doc_ingestor.py` & `querent-3.0.1/querent/ingestors/doc/doc_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/email/email_ingestor.py` & `querent-3.0.1/querent/ingestors/email/email_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/email/email_reader.py` & `querent-3.0.1/querent/ingestors/email/email_reader.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/github/github_ingestor.py` & `querent-3.0.1/querent/ingestors/github/github_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/html/html_ingestor.py` & `querent-3.0.1/querent/ingestors/html/html_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/images/image_ingestor.py` & `querent-3.0.1/querent/ingestors/images/image_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/ingestor_factory.py` & `querent-3.0.1/querent/ingestors/ingestor_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/ingestor_manager.py` & `querent-3.0.1/querent/ingestors/ingestor_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,15 @@
             IngestorBackend.XML.value: XmlIngestorFactory(),
             IngestorBackend.HTML.value: HtmlIngestorFactory(),
             IngestorBackend.MP4.value: VideoIngestorFactory(),
             IngestorBackend.GITHUB.value: GithubIngestorFactory(),
             IngestorBackend.Slack.value: TextIngestorFactory(is_token_stream=True),
             IngestorBackend.Email.value: EmailIngestorFactory(),
             IngestorBackend.Jira.value: JsonIngestorFactory(),
+            IngestorBackend.News.value: TextIngestorFactory(is_token_stream=True)
             # Add more mappings as needed
         }
         self.file_caches = LRUCache(maxsize=cache_size)
         self.result_queue = result_queue
         self.tokens_feader = tokens_feader
         self.logger = setup_logger(__name__, "IngestorFactoryManager")
```

### Comparing `querent-3.0.0/querent/ingestors/json/json_ingestor.py` & `querent-3.0.1/querent/ingestors/json/json_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/pdfs/pdf_ingestor_v1.py` & `querent-3.0.1/querent/ingestors/pdfs/pdf_ingestor_v1.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/ppt/ppt_ingestor.py` & `querent-3.0.1/querent/ingestors/ppt/ppt_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/texts/text_ingestor.py` & `querent-3.0.1/querent/ingestors/texts/text_ingestor.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from querent.config.ingestor.ingestor_config import IngestorBackend
 from querent.common import common_errors
 from querent.common.types.ingested_tokens import IngestedTokens
 from querent.logging.logger import setup_logger
 
 
 class TextIngestorFactory(IngestorFactory):
-    SUPPORTED_EXTENSIONS = {"txt", "slack", ""}
+    SUPPORTED_EXTENSIONS = {"txt", "slack", "", "news"}
 
     def __init__(self, is_token_stream=False):
         self.is_token_stream = is_token_stream
 
     async def supports(self, file_extension: str) -> bool:
         return file_extension.lower() in self.SUPPORTED_EXTENSIONS
```

### Comparing `querent-3.0.0/querent/ingestors/video/video_ingestor.py` & `querent-3.0.1/querent/ingestors/video/video_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/xlsx/xlsx_ingestor.py` & `querent-3.0.1/querent/ingestors/xlsx/xlsx_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/ingestors/xml/xml_ingestor.py` & `querent-3.0.1/querent/ingestors/xml/xml_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/ner_helperfunctions/attn_scores.py` & `querent-3.0.1/querent/kg/ner_helperfunctions/attn_scores.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/ner_helperfunctions/contextual_embeddings.py` & `querent-3.0.1/querent/kg/ner_helperfunctions/contextual_embeddings.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/ner_helperfunctions/dependency_parsing.py` & `querent-3.0.1/querent/kg/ner_helperfunctions/dependency_parsing.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/ner_helperfunctions/filter_triples.py` & `querent-3.0.1/querent/kg/ner_helperfunctions/filter_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/ner_helperfunctions/fixed_entities.py` & `querent-3.0.1/querent/kg/ner_helperfunctions/fixed_entities.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/ner_helperfunctions/fixed_predicate.py` & `querent-3.0.1/querent/kg/ner_helperfunctions/fixed_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/ner_helperfunctions/ner_llm_transformer.py` & `querent-3.0.1/querent/kg/ner_helperfunctions/ner_llm_transformer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/querent_kg.py` & `querent-3.0.1/querent/kg/querent_kg.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/rel_helperfunctions/contextual_predicate.py` & `querent-3.0.1/querent/kg/rel_helperfunctions/contextual_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/rel_helperfunctions/embedding_store.py` & `querent-3.0.1/querent/kg/rel_helperfunctions/embedding_store.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/rel_helperfunctions/filter_semantic_triples.py` & `querent-3.0.1/querent/kg/rel_helperfunctions/filter_semantic_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/rel_helperfunctions/fixed_relationships.py` & `querent-3.0.1/querent/kg/rel_helperfunctions/fixed_relationships.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py` & `querent-3.0.1/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/rel_helperfunctions/openai_functions.py` & `querent-3.0.1/querent/kg/rel_helperfunctions/openai_functions.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/rel_helperfunctions/questionanswer_llama2.py` & `querent-3.0.1/querent/kg/rel_helperfunctions/questionanswer_llama2.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/rel_helperfunctions/rag_retriever.py` & `querent-3.0.1/querent/kg/rel_helperfunctions/rag_retriever.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/rel_helperfunctions/rel_normalize.py` & `querent-3.0.1/querent/kg/rel_helperfunctions/rel_normalize.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/kg/rel_helperfunctions/triple_to_json.py` & `querent-3.0.1/querent/kg/rel_helperfunctions/triple_to_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def convert_vectorjson(triple):
         try:
             subject, json_str, object_ = triple
             data = TripleToJsonConverter._parse_json_str(json_str)
             if data is None:
                 return {}
 
-            id_format = f"{TripleToJsonConverter._normalize_text(subject)}_{TripleToJsonConverter._normalize_text(data.get('predicate', ''))}_{TripleToJsonConverter._normalize_text(object_)}"
+            id_format = f"{TripleToJsonConverter._normalize_text(subject)}-{TripleToJsonConverter._normalize_text(data.get('predicate', ''))}-{TripleToJsonConverter._normalize_text(object_)}"
             json_object = {
                 "id": TripleToJsonConverter._normalize_text(id_format,replace_space=True).replace(",","_"),
                 "embeddings": data.get("context_embeddings", []),
                 "size": len(data.get("context_embeddings", [])),
                 "namespace": TripleToJsonConverter._normalize_text(data.get("predicate", ""),replace_space=True),
                 "sentence": data.get("context", "").lower()
             }
@@ -72,12 +72,12 @@
         except Exception as e:
             raise Exception(f"Error in convert_vectorjson: {e}")
         
 
     @staticmethod
     def replace_special_chars_with_underscore(data):
         # This pattern will match anything that is not a letter, number, or underscore
-        pattern = r'[^a-zA-Z0-9_]'
+        pattern = r'[^-a-zA-Z0-9_]'
         # Replace matched patterns with an underscore
         return re.sub(pattern, '_', data)
```

### Comparing `querent-3.0.0/querent/logging/filters.py` & `querent-3.0.1/querent/logging/filters.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/logging/handlers.py` & `querent-3.0.1/querent/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/logging/logger.py` & `querent-3.0.1/querent/logging/logger.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/metric/adapters/promethus_adapter.py` & `querent-3.0.1/querent/metric/adapters/promethus_adapter.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/metric/metric_logging_handler.py` & `querent-3.0.1/querent/metric/metric_logging_handler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/metric/metric_registry.py` & `querent-3.0.1/querent/metric/metric_registry.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/processors/text_cleanup_processor.py` & `querent-3.0.1/querent/processors/text_cleanup_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/processors/text_processor.py` & `querent-3.0.1/querent/processors/text_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/querent/auto_scaler.py` & `querent-3.0.1/querent/querent/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/querent/querent.py` & `querent-3.0.1/querent/querent/querent.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/querent/resource_manager.py` & `querent-3.0.1/querent/querent/resource_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/storage/milvus_vectorevent_storage.py` & `querent-3.0.1/querent/storage/milvus_vectorevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/storage/neo4j_graphevent_storage.py` & `querent-3.0.1/querent/storage/neo4j_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/storage/postgres_graphevent_storage.py` & `querent-3.0.1/querent/storage/postgres_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/storage/s3-data-management.py` & `querent-3.0.1/querent/storage/s3-data-management.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/tools/web_page_extractor.py` & `querent-3.0.1/querent/tools/web_page_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/utils/webpage_extractor.py` & `querent-3.0.1/querent/utils/webpage_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/workflow/_helpers.py` & `querent-3.0.1/querent/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent/workflow/workflow.py` & `querent-3.0.1/querent/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.0/querent.egg-info/PKG-INFO` & `querent-3.0.1/querent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.0
+Version: 3.0.1
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -36,27 +36,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: cachetools==5.3.3
-Requires-Dist: aiohttp==3.9.2
+Requires-Dist: aiohttp==3.9.3
 Requires-Dist: attrs==23.1.0
-Requires-Dist: beautifulsoup4==4.12.2
+Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: boto3==1.26.146
 Requires-Dist: botocore==1.29.146
 Requires-Dist: bs4==0.0.1
 Requires-Dist: faiss-cpu==1.7.4
 Requires-Dist: gensim==4.3.2
 Requires-Dist: hdbscan==0.8.33
 Requires-Dist: jira==3.6.0
 Requires-Dist: jmespath==1.0.1
 Requires-Dist: joblib==1.2.0
-Requires-Dist: json5==0.9.14
+Requires-Dist: json5==0.9.24
 Requires-Dist: jsonmerge==1.9.0
 Requires-Dist: jsonschema==4.17.3
 Requires-Dist: kombu==5.2.4
 Requires-Dist: llama_cpp_python==0.2.15
 Requires-Dist: lxml==4.9.2
 Requires-Dist: newspaper3k==0.2.8
 Requires-Dist: nltk==3.8.1
@@ -66,29 +66,29 @@
 Requires-Dist: PyJWT==2.4.0
 Requires-Dist: pytest==7.3.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: redis==5.0.3
 Requires-Dist: regex==2023.5.5
 Requires-Dist: sentence-transformers==2.2.2
 Requires-Dist: spacy==3.7.2
-Requires-Dist: uvicorn==0.22.0
+Requires-Dist: uvicorn==0.29.0
 Requires-Dist: slack-sdk==3.26.1
 Requires-Dist: pylint==2.17.4
 Requires-Dist: pytest-cov==4.1.0
 Requires-Dist: pytest-mock==3.11.1
 Requires-Dist: tensorflow==2.14.0
 Requires-Dist: transformers==4.36.0
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: prometheus-client==0.17.1
 Requires-Dist: rdflib==7.0.0
 Requires-Dist: pytest-asyncio==0.23.2
 Requires-Dist: pyshacl==0.25.0
 Requires-Dist: google-cloud-storage==2.14.0
-Requires-Dist: PyMuPDF==1.23.26
+Requires-Dist: PyMuPDF==1.24.0
 Requires-Dist: pydub==0.25.1
 Requires-Dist: SpeechRecognition==3.10.1
 Requires-Dist: pytesseract==0.3.10
 Requires-Dist: pytextract==2.0.1
 Requires-Dist: pandas==2.1.4
 Requires-Dist: python-pptx==0.6.23
 Requires-Dist: tika==2.6.0
```

### Comparing `querent-3.0.0/querent.egg-info/SOURCES.txt` & `querent-3.0.1/querent.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,15 @@
 querent/querent/__init__.py
 querent/querent/auto_scaler.py
 querent/querent/querent.py
 querent/querent/resource_manager.py
 querent/querent/worker.py
 querent/search/__init__.py
 querent/storage/__init__.py
+querent/storage/gcs_query.py
 querent/storage/milvus_vectorevent_storage.py
 querent/storage/neo4j_graphevent_storage.py
 querent/storage/postgres_graphevent_storage.py
 querent/storage/s3-data-management.py
 querent/tools/__init__.py
 querent/tools/web_page_extractor.py
 querent/utils/__init__.py
```

### Comparing `querent-3.0.0/querent.egg-info/requires.txt` & `querent-3.0.1/querent.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 cachetools==5.3.3
-aiohttp==3.9.2
+aiohttp==3.9.3
 attrs==23.1.0
-beautifulsoup4==4.12.2
+beautifulsoup4==4.12.3
 boto3==1.26.146
 botocore==1.29.146
 bs4==0.0.1
 faiss-cpu==1.7.4
 gensim==4.3.2
 hdbscan==0.8.33
 jira==3.6.0
 jmespath==1.0.1
 joblib==1.2.0
-json5==0.9.14
+json5==0.9.24
 jsonmerge==1.9.0
 jsonschema==4.17.3
 kombu==5.2.4
 llama_cpp_python==0.2.15
 lxml==4.9.2
 newspaper3k==0.2.8
 nltk==3.8.1
@@ -25,29 +25,29 @@
 PyJWT==2.4.0
 pytest==7.3.2
 python-dotenv==1.0.0
 redis==5.0.3
 regex==2023.5.5
 sentence-transformers==2.2.2
 spacy==3.7.2
-uvicorn==0.22.0
+uvicorn==0.29.0
 slack-sdk==3.26.1
 pylint==2.17.4
 pytest-cov==4.1.0
 pytest-mock==3.11.1
 tensorflow==2.14.0
 transformers==4.36.0
 asyncio==3.4.3
 aiofiles==23.2.1
 prometheus-client==0.17.1
 rdflib==7.0.0
 pytest-asyncio==0.23.2
 pyshacl==0.25.0
 google-cloud-storage==2.14.0
-PyMuPDF==1.23.26
+PyMuPDF==1.24.0
 pydub==0.25.1
 SpeechRecognition==3.10.1
 pytesseract==0.3.10
 pytextract==2.0.1
 pandas==2.1.4
 python-pptx==0.6.23
 tika==2.6.0
```

### Comparing `querent-3.0.0/setup.py` & `querent-3.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
     Querent AI: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 """
 
 from setuptools import setup, find_packages
 
 requirements = [
     "cachetools==5.3.3",
-    "aiohttp==3.9.2",
+    "aiohttp==3.9.3",
     "attrs==23.1.0",
-    "beautifulsoup4==4.12.2",
+    "beautifulsoup4==4.12.3",
     "boto3==1.26.146",
     "botocore==1.29.146",
     "bs4==0.0.1",
     "faiss-cpu==1.7.4",
     "gensim==4.3.2",
     "hdbscan==0.8.33",
     "jira==3.6.0",
     "jmespath==1.0.1",
     "joblib==1.2.0",
-    "json5==0.9.14",
+    "json5==0.9.24",
     "jsonmerge==1.9.0",
     "jsonschema==4.17.3",
     "kombu==5.2.4",
     "llama_cpp_python==0.2.15",
     "lxml==4.9.2",
     "newspaper3k==0.2.8",
     "nltk==3.8.1",
@@ -32,29 +32,29 @@
     "PyJWT==2.4.0",
     "pytest==7.3.2",
     "python-dotenv==1.0.0",
     "redis==5.0.3",
     "regex==2023.5.5",
     "sentence-transformers==2.2.2",
     "spacy==3.7.2",
-    "uvicorn==0.22.0",
+    "uvicorn==0.29.0",
     "slack-sdk==3.26.1",
     "pylint==2.17.4",
     "pytest-cov==4.1.0",
     "pytest-mock==3.11.1",
     "tensorflow==2.14.0",
     "transformers==4.36.0",
     "asyncio==3.4.3",
     "aiofiles==23.2.1",
     "prometheus-client==0.17.1",
     "rdflib==7.0.0",
     "pytest-asyncio==0.23.2",
     "pyshacl==0.25.0",
     "google-cloud-storage==2.14.0",
-    "PyMuPDF==1.23.26",
+    "PyMuPDF==1.24.0",
     "pydub==0.25.1",
     "SpeechRecognition==3.10.1",
     "pytesseract==0.3.10",
     "pytextract==2.0.1",
     "pandas==2.1.4",
     "python-pptx==0.6.23",
     "tika==2.6.0",
@@ -80,15 +80,15 @@
 ]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="querent",
-    version="3.0.0",
+    version="3.0.1",
     author="Querent AI",
     description="The Asynchronous Data Dynamo and Graph Neural Network Catalyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Querent-ai/querent-ai",
     project_urls={
         "Documentation": "https://github.com/Querent-ai/querent-ai/docs",
```

