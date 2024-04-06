# Comparing `tmp/symbol_shoestring-0.1.0.tar.gz` & `tmp/symbol_shoestring-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol_shoestring-0.1.0.tar", max compression
+gzip compressed data, was "symbol_shoestring-0.1.1.tar", max compression
```

## Comparing `symbol_shoestring-0.1.0.tar` & `symbol_shoestring-0.1.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0    12333 2023-08-18 12:24:41.515536 symbol_shoestring-0.1.0/README.md
--rw-r--r--   0        0        0      960 2023-08-18 12:28:45.291319 symbol_shoestring-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-18 12:24:41.515536 symbol_shoestring-0.1.0/shoestring/__init__.py
--rw-r--r--   0        0        0     1937 2023-08-18 12:24:41.515536 symbol_shoestring-0.1.0/shoestring/__main__.py
--rw-r--r--   0        0        0        0 2023-08-18 12:24:41.515536 symbol_shoestring-0.1.0/shoestring/commands/__init__.py
--rw-r--r--   0        0        0     1552 2023-08-18 12:24:41.515536 symbol_shoestring-0.1.0/shoestring/commands/announce_transaction.py
--rw-r--r--   0        0        0     2475 2023-08-18 12:24:41.515536 symbol_shoestring-0.1.0/shoestring/commands/health.py
--rw-r--r--   0        0        0     1417 2023-08-18 12:24:41.515536 symbol_shoestring-0.1.0/shoestring/commands/import_bootstrap.py
--rw-r--r--   0        0        0     1025 2023-08-18 12:24:41.515536 symbol_shoestring-0.1.0/shoestring/commands/init.py
--rw-r--r--   0        0        0     1692 2023-08-18 12:24:41.515536 symbol_shoestring-0.1.0/shoestring/commands/min_cosignatures_count.py
--rw-r--r--   0        0        0     1733 2023-08-18 12:24:41.515536 symbol_shoestring-0.1.0/shoestring/commands/pemtool.py
--rw-r--r--   0        0        0     1569 2023-08-18 12:24:41.515536 symbol_shoestring-0.1.0/shoestring/commands/renew_certificates.py
--rw-r--r--   0        0        0     5270 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/commands/renew_voting_keys.py
--rw-r--r--   0        0        0     3071 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/commands/reset_data.py
--rw-r--r--   0        0        0     5507 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/commands/setup.py
--rw-r--r--   0        0        0     3332 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/commands/signer.py
--rw-r--r--   0        0        0     2246 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/commands/upgrade.py
--rw-r--r--   0        0        0        0 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/healthagents/__init__.py
--rw-r--r--   0        0        0      594 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/healthagents/peer_api.py
--rw-r--r--   0        0        0     3586 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/healthagents/peer_certificate.py
--rw-r--r--   0        0        0      644 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/healthagents/rest_api.py
--rw-r--r--   0        0        0     2985 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/healthagents/rest_https_certificate.py
--rw-r--r--   0        0        0     1686 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/healthagents/voting_keys.py
--rw-r--r--   0        0        0     1573 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/healthagents/websockets.py
--rw-r--r--   0        0        0     5055 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/CertificateFactory.py
--rw-r--r--   0        0        0     3233 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/ConfigurationManager.py
--rw-r--r--   0        0        0     1656 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/FileDownloader.py
--rw-r--r--   0        0        0      360 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/FileTemplater.py
--rw-r--r--   0        0        0     1961 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/HarvesterConfigurator.py
--rw-r--r--   0        0        0      830 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/HeightGrouping.py
--rw-r--r--   0        0        0     3089 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/LinkTransactionBuilder.py
--rw-r--r--   0        0        0      655 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/MultisigAnalyzer.py
--rw-r--r--   0        0        0     2789 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/NodeDownloader.py
--rw-r--r--   0        0        0      578 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/NodeFeatures.py
--rw-r--r--   0        0        0     1412 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/NodewatchClient.py
--rw-r--r--   0        0        0     1381 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/OpensslExecutor.py
--rw-r--r--   0        0        0     3060 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/PackageResolver.py
--rw-r--r--   0        0        0     2139 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/PeerDownloader.py
--rw-r--r--   0        0        0     2372 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/PemUtils.py
--rw-r--r--   0        0        0    12793 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/Preparer.py
--rw-r--r--   0        0        0     3509 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/ShoestringConfiguration.py
--rw-r--r--   0        0        0      371 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/TransactionSerializer.py
--rw-r--r--   0        0        0     3947 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/VoterConfigurator.py
--rw-r--r--   0        0        0        0 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/internal/__init__.py
--rw-r--r--   0        0        0    16279 2023-08-18 12:26:50.515417 symbol_shoestring-0.1.0/shoestring/lang/en/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    25799 2023-08-18 12:26:49.811417 symbol_shoestring-0.1.0/shoestring/lang/en/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      438 2023-08-18 12:26:50.531417 symbol_shoestring-0.1.0/shoestring/lang/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    19137 2023-08-18 12:26:50.159417 symbol_shoestring-0.1.0/shoestring/lang/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    18924 2023-08-18 12:26:49.323418 symbol_shoestring-0.1.0/shoestring/lang/messages.pot
--rw-r--r--   0        0        0      213 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/lang/po.header.txt
--rw-r--r--   0        0        0      270 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/startup/delayrestapi.sh
--rw-r--r--   0        0        0      565 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/startup/mongors.sh
--rw-r--r--   0        0        0      190 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/startup/startBroker.sh
--rw-r--r--   0        0        0      272 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/startup/startServer.sh
--rw-r--r--   0        0        0      102 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/startup/wait.sh
--rw-r--r--   0        0        0     2830 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/templates/docker-compose-dual.yaml
--rw-r--r--   0        0        0      629 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/templates/docker-compose-peer.yaml
--rw-r--r--   0        0        0      299 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/templates/nginx.conf.erb
--rw-r--r--   0        0        0     1004 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/Screen.py
--rw-r--r--   0        0        0     2102 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/ScreenContainer.py
--rw-r--r--   0        0        0     1781 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/ShoestringOperation.py
--rw-r--r--   0        0        0     4774 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/TabbedView.py
--rw-r--r--   0        0        0      843 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/TitleBar.py
--rw-r--r--   0        0        0     2708 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/ValidatingTextBox.py
--rw-r--r--   0        0        0        0 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/__init__.py
--rw-r--r--   0        0        0     3664 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/__main__.py
--rw-r--r--   0        0        0     1917 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/buttons.py
--rw-r--r--   0        0        0      484 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/keybindings.py
--rw-r--r--   0        0        0     1553 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/navigation.py
--rw-r--r--   0        0        0     1635 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screen_loader.py
--rw-r--r--   0        0        0        0 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/__init__.py
--rw-r--r--   0        0        0     1890 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/certificates.py
--rw-r--r--   0        0        0      652 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/end_screen.py
--rw-r--r--   0        0        0     6498 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/harvesting.py
--rw-r--r--   0        0        0     1625 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/modal.py
--rw-r--r--   0        0        0      799 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/network_type.py
--rw-r--r--   0        0        0     2981 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/node_settings.py
--rw-r--r--   0        0        0      757 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/node_type.py
--rw-r--r--   0        0        0     6789 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/obligatory.py
--rw-r--r--   0        0        0      827 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/root_check.py
--rw-r--r--   0        0        0      799 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/voting.py
--rw-r--r--   0        0        0     1835 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/screens/welcome.py
--rw-r--r--   0        0        0     3810 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/setup_file_generator.py
--rw-r--r--   0        0        0     1744 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/shoestring_dispatcher.py
--rw-r--r--   0        0        0     1095 2023-08-18 12:24:41.519536 symbol_shoestring-0.1.0/shoestring/wizard/styles.py
--rw-r--r--   0        0        0    13500 1970-01-01 00:00:00.000000 symbol_shoestring-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    12333 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/README.md
+-rw-r--r--   0        0        0      957 2024-04-06 16:25:10.478720 symbol_shoestring-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/commands/__init__.py
+-rw-r--r--   0        0        0     1552 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/commands/announce_transaction.py
+-rw-r--r--   0        0        0     2475 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/commands/health.py
+-rw-r--r--   0        0        0     1417 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/commands/import_bootstrap.py
+-rw-r--r--   0        0        0     1025 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/commands/init.py
+-rw-r--r--   0        0        0     1692 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/commands/min_cosignatures_count.py
+-rw-r--r--   0        0        0     1733 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/commands/pemtool.py
+-rw-r--r--   0        0        0     1569 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/commands/renew_certificates.py
+-rw-r--r--   0        0        0     5270 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/commands/renew_voting_keys.py
+-rw-r--r--   0        0        0     3071 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/commands/reset_data.py
+-rw-r--r--   0        0        0     5507 2024-04-06 16:10:17.894030 symbol_shoestring-0.1.1/shoestring/commands/setup.py
+-rw-r--r--   0        0        0     3332 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/commands/signer.py
+-rw-r--r--   0        0        0     2246 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/commands/upgrade.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/healthagents/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/healthagents/peer_api.py
+-rw-r--r--   0        0        0     3586 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/healthagents/peer_certificate.py
+-rw-r--r--   0        0        0      644 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/healthagents/rest_api.py
+-rw-r--r--   0        0        0     2985 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/healthagents/rest_https_certificate.py
+-rw-r--r--   0        0        0     1686 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/healthagents/voting_keys.py
+-rw-r--r--   0        0        0     1573 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/healthagents/websockets.py
+-rw-r--r--   0        0        0     5055 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/CertificateFactory.py
+-rw-r--r--   0        0        0     3233 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/ConfigurationManager.py
+-rw-r--r--   0        0        0     1656 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/FileDownloader.py
+-rw-r--r--   0        0        0      360 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/FileTemplater.py
+-rw-r--r--   0        0        0     1961 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/HarvesterConfigurator.py
+-rw-r--r--   0        0        0      830 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/HeightGrouping.py
+-rw-r--r--   0        0        0     3089 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/LinkTransactionBuilder.py
+-rw-r--r--   0        0        0      655 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/MultisigAnalyzer.py
+-rw-r--r--   0        0        0     2789 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/NodeDownloader.py
+-rw-r--r--   0        0        0     1128 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/NodeFeatures.py
+-rw-r--r--   0        0        0     1412 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/NodewatchClient.py
+-rw-r--r--   0        0        0     1381 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/OpensslExecutor.py
+-rw-r--r--   0        0        0     3060 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/PackageResolver.py
+-rw-r--r--   0        0        0     2139 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/PeerDownloader.py
+-rw-r--r--   0        0        0     2372 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/PemUtils.py
+-rw-r--r--   0        0        0    12793 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/Preparer.py
+-rw-r--r--   0        0        0     3291 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/ShoestringConfiguration.py
+-rw-r--r--   0        0        0      371 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/TransactionSerializer.py
+-rw-r--r--   0        0        0     3947 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/VoterConfigurator.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/internal/__init__.py
+-rw-r--r--   0        0        0    16279 2024-04-06 16:23:59.406344 symbol_shoestring-0.1.1/shoestring/lang/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    25799 2024-04-06 16:23:59.190343 symbol_shoestring-0.1.1/shoestring/lang/en/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      438 2024-04-06 16:23:59.406344 symbol_shoestring-0.1.1/shoestring/lang/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    19137 2024-04-06 16:23:59.270343 symbol_shoestring-0.1.1/shoestring/lang/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    18924 2024-04-06 16:23:59.090342 symbol_shoestring-0.1.1/shoestring/lang/messages.pot
+-rw-r--r--   0        0        0      213 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/lang/po.header.txt
+-rw-r--r--   0        0        0      270 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/startup/delayrestapi.sh
+-rw-r--r--   0        0        0      571 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/startup/mongors.sh
+-rw-r--r--   0        0        0      190 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/startup/startBroker.sh
+-rw-r--r--   0        0        0      272 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/startup/startServer.sh
+-rw-r--r--   0        0        0      102 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/startup/wait.sh
+-rw-r--r--   0        0        0     2868 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/templates/docker-compose-dual.yaml
+-rw-r--r--   0        0        0      648 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/templates/docker-compose-peer.yaml
+-rw-r--r--   0        0        0      299 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/templates/nginx.conf.erb
+-rw-r--r--   0        0        0     1004 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/Screen.py
+-rw-r--r--   0        0        0     2102 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/ScreenContainer.py
+-rw-r--r--   0        0        0     1781 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/ShoestringOperation.py
+-rw-r--r--   0        0        0     4837 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/TabbedView.py
+-rw-r--r--   0        0        0      843 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/TitleBar.py
+-rw-r--r--   0        0        0     2708 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/ValidatingTextBox.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/__init__.py
+-rw-r--r--   0        0        0     3664 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/__main__.py
+-rw-r--r--   0        0        0     1917 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/buttons.py
+-rw-r--r--   0        0        0      484 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/keybindings.py
+-rw-r--r--   0        0        0     1553 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/navigation.py
+-rw-r--r--   0        0        0     1635 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screen_loader.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/__init__.py
+-rw-r--r--   0        0        0     1890 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/certificates.py
+-rw-r--r--   0        0        0      652 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/end_screen.py
+-rw-r--r--   0        0        0     6498 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/harvesting.py
+-rw-r--r--   0        0        0     1625 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/modal.py
+-rw-r--r--   0        0        0      799 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/network_type.py
+-rw-r--r--   0        0        0     2981 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/node_settings.py
+-rw-r--r--   0        0        0      757 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/node_type.py
+-rw-r--r--   0        0        0     6789 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/obligatory.py
+-rw-r--r--   0        0        0      827 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/root_check.py
+-rw-r--r--   0        0        0      799 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/voting.py
+-rw-r--r--   0        0        0     1835 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/screens/welcome.py
+-rw-r--r--   0        0        0     3750 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/setup_file_generator.py
+-rw-r--r--   0        0        0     1744 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/shoestring_dispatcher.py
+-rw-r--r--   0        0        0     1095 2024-04-06 16:10:17.898030 symbol_shoestring-0.1.1/shoestring/wizard/styles.py
+-rw-r--r--   0        0        0    13497 1970-01-01 00:00:00.000000 symbol_shoestring-0.1.1/PKG-INFO
```

### Comparing `symbol_shoestring-0.1.0/README.md` & `symbol_shoestring-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/pyproject.toml` & `symbol_shoestring-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'symbol-shoestring'
-version = '0.1.0'
+version = '0.1.1'
 description = 'Symbol Shoestring Deployment Tool'
 authors = ['Symbol Contributors <contributors@symbol.dev>']
 maintainers = ['Symbol Contributors <contributors@symbol.dev>']
 license = 'MIT'
 
 readme = 'README.md'
 
@@ -16,16 +16,16 @@
 
 classifiers = ['Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11']
 
 include = ['shoestring/lang/*/LC_MESSAGES/messages.mo']
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aiohttp = ">=3.8.5,<3.9.0"
+aiohttp = ">=3.9.0,<3.10.0"
 jinja2 = ">=3.1.2,<3.2.0"
 prompt-toolkit = ">=3.0.39,<3.1.0"
 pyyaml = ">=6.0.1,<6.1.0"
 requests = ">=2.31.0,<2.32.0"
 symbol-lightapi = ">=0.0.5,<0.1.0"
 symbol-sdk-python = ">=3.1.0,<3.2.0"
-websockets = ">=11.0.3,<11.1.0"
+websockets = ">=12.0,<13.0"
 zenlog = ">=1.1,<2.0"
```

### Comparing `symbol_shoestring-0.1.0/shoestring/__main__.py` & `symbol_shoestring-0.1.1/shoestring/__main__.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/announce_transaction.py` & `symbol_shoestring-0.1.1/shoestring/commands/announce_transaction.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/health.py` & `symbol_shoestring-0.1.1/shoestring/commands/health.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/import_bootstrap.py` & `symbol_shoestring-0.1.1/shoestring/commands/import_bootstrap.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/init.py` & `symbol_shoestring-0.1.1/shoestring/commands/init.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/min_cosignatures_count.py` & `symbol_shoestring-0.1.1/shoestring/commands/min_cosignatures_count.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/pemtool.py` & `symbol_shoestring-0.1.1/shoestring/commands/pemtool.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/renew_certificates.py` & `symbol_shoestring-0.1.1/shoestring/commands/renew_certificates.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/renew_voting_keys.py` & `symbol_shoestring-0.1.1/shoestring/commands/renew_voting_keys.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/reset_data.py` & `symbol_shoestring-0.1.1/shoestring/commands/reset_data.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/setup.py` & `symbol_shoestring-0.1.1/shoestring/commands/setup.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/signer.py` & `symbol_shoestring-0.1.1/shoestring/commands/signer.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/commands/upgrade.py` & `symbol_shoestring-0.1.1/shoestring/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/healthagents/peer_api.py` & `symbol_shoestring-0.1.1/shoestring/healthagents/peer_api.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/healthagents/peer_certificate.py` & `symbol_shoestring-0.1.1/shoestring/healthagents/peer_certificate.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/healthagents/rest_api.py` & `symbol_shoestring-0.1.1/shoestring/healthagents/rest_api.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/healthagents/rest_https_certificate.py` & `symbol_shoestring-0.1.1/shoestring/healthagents/rest_https_certificate.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/healthagents/voting_keys.py` & `symbol_shoestring-0.1.1/shoestring/healthagents/voting_keys.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/healthagents/websockets.py` & `symbol_shoestring-0.1.1/shoestring/healthagents/websockets.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/CertificateFactory.py` & `symbol_shoestring-0.1.1/shoestring/internal/CertificateFactory.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/ConfigurationManager.py` & `symbol_shoestring-0.1.1/shoestring/internal/ConfigurationManager.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/FileDownloader.py` & `symbol_shoestring-0.1.1/shoestring/internal/FileDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/HarvesterConfigurator.py` & `symbol_shoestring-0.1.1/shoestring/internal/HarvesterConfigurator.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/HeightGrouping.py` & `symbol_shoestring-0.1.1/shoestring/internal/HeightGrouping.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/LinkTransactionBuilder.py` & `symbol_shoestring-0.1.1/shoestring/internal/LinkTransactionBuilder.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/MultisigAnalyzer.py` & `symbol_shoestring-0.1.1/shoestring/internal/MultisigAnalyzer.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/NodeDownloader.py` & `symbol_shoestring-0.1.1/shoestring/internal/NodeDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/NodewatchClient.py` & `symbol_shoestring-0.1.1/shoestring/internal/NodewatchClient.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/OpensslExecutor.py` & `symbol_shoestring-0.1.1/shoestring/internal/OpensslExecutor.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/PackageResolver.py` & `symbol_shoestring-0.1.1/shoestring/internal/PackageResolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 from aiohttp import ClientSession
 
 from .FileDownloader import download_file
 
 SYMBOL_GITHUB_URI = 'https://api.github.com/repos/symbol/symbol/releases'
 OFFICIAL_HASHES = {
-	'client/catapult/v1.0.3.6': (
-		'A1D3BE805B43E8B8D2490EE1F04709C9067E151EAB4E8A2F6492BCA2A781403A'
-		'573BCE2765A84C989E0EBE3CD494CAE66132EA3145572DEF8F937F46E5E6E4BA'
+	'client/catapult/v1.0.3.7': (
+		'B75A54DA8DA3D4E09640B22190883214FF6BF5EFBA943CCA279B6B4FF8F3DBB0'
+		'9D9C5C2FC6233DCF299417AB11D2632E9BD21903B2B49E3DF113C0E0B2CFC267'
 	)
 }
 
 
 async def _get_releases(releases_uri):
 	async with ClientSession() as session:
 		async with session.get(releases_uri) as response:
```

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/PeerDownloader.py` & `symbol_shoestring-0.1.1/shoestring/internal/PeerDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/PemUtils.py` & `symbol_shoestring-0.1.1/shoestring/internal/PemUtils.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/Preparer.py` & `symbol_shoestring-0.1.1/shoestring/internal/Preparer.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/ShoestringConfiguration.py` & `symbol_shoestring-0.1.1/shoestring/internal/ShoestringConfiguration.py`

 * *Files 13% similar despite different names*

```diff
@@ -65,22 +65,15 @@
 
 	return ImportsConfiguration(config['harvester'], config['voter'])
 
 
 def parse_node_configuration(config):
 	"""Parses node configuration."""
 
-	features = NodeFeatures(0)
-	for feature in config['features'].split('|'):
-		try:
-			features |= NodeFeatures[feature.strip()]
-		except KeyError as ex:
-			# rethrow KeyError as ValueError for consistency with other value parsing errors
-			raise ValueError(ex) from ex
-
+	features = NodeFeatures.parse(config['features'])
 	user_id = int(config['userId'])
 	group_id = int(config['groupId'])
 	ca_password = config['caPassword']
 	api_https = config['apiHttps'].lower() == 'true'
 	ca_common_name = config['caCommonName']
 	node_common_name = config['nodeCommonName']
```

### Comparing `symbol_shoestring-0.1.0/shoestring/internal/VoterConfigurator.py` & `symbol_shoestring-0.1.1/shoestring/internal/VoterConfigurator.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/lang/en/LC_MESSAGES/messages.mo` & `symbol_shoestring-0.1.1/shoestring/lang/en/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-08-18 12:26+0000\n"
+"POT-Creation-Date: 2024-04-06 16:23+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.14.0\n"
 
 msgid "announce-transaction-announce-successful"
 msgstr "transaction was successfully sent to the network"
 
 msgid "announce-transaction-preparing-to-announce"
 msgstr ""
 "preparing to announce transaction {transaction_hash} of type "
```

### Comparing `symbol_shoestring-0.1.0/shoestring/lang/en/LC_MESSAGES/messages.po` & `symbol_shoestring-0.1.1/shoestring/lang/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/lang/ja/LC_MESSAGES/messages.po` & `symbol_shoestring-0.1.1/shoestring/lang/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/lang/messages.pot` & `symbol_shoestring-0.1.1/shoestring/lang/messages.pot`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/startup/mongors.sh` & `symbol_shoestring-0.1.1/shoestring/startup/mongors.sh`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 state_filename=$1
 shift
 
 pwd
 
 while true;
 do
-	if mongo --eval "db.runCommand( { serverStatus: 1 } )" db/local > /dev/null 2>&1; then
+	if mongosh --eval "db.runCommand( { serverStatus: 1 } )" db/local > /dev/null 2>&1; then
 		break;
 	fi
 	echo "waiting for mongod start..."
 	sleep 1
 done
 
 echo " [+] Preparing db5"
 cd /mongo
-mongo db/catapult < mongoDbPrepare.js
+mongosh db/catapult < mongoDbPrepare.js
 echo " [.] (exit code: $?)"
 cd -
 
 echo " [+] db prepared, checking account indexes"
-mongo --eval 'db.accounts.getIndexes()' db/catapult
+mongosh --eval 'db.accounts.getIndexes()' db/catapult
 
 trap 'echo "exiting"; exit 0' SIGTERM
 mkdir -p "$(dirname "${state_filename}")"
 touch "${state_filename}"
 
 sleep infinity & wait
```

### Comparing `symbol_shoestring-0.1.0/shoestring/templates/docker-compose-dual.yaml` & `symbol_shoestring-0.1.1/shoestring/templates/docker-compose-dual.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ---
 version: '2'
 services:
   db:
-    image: mongo:5.0.15
+    image: mongo:6.0.14
     user: '{{ user }}'
     command: mongod --dbpath=/dbdata
     stop_signal: SIGINT
     ports:
       - 127.0.0.1:27017:27017
     volumes:
       - ./dbdata:/dbdata:rw
       - ./dbdata:/data:rw
 
   initiate:
-    image: mongo:5.0.15
+    image: mongo:6.0.14
     user: '{{ user }}'
     command: /bin/bash /startup/mongors.sh /real_data/startup/mongo-initialized
     volumes:
       - ./startup:/startup:ro
       - ./mongo:/mongo:ro
       - ./dbdata:/dbdata:rw
       - ./dbdata:/data:rw
@@ -36,14 +36,15 @@
     command: /bin/bash /startup/wait.sh /data/startup/mongo-initialized /startup/startServer.sh
     environment:
       - LD_LIBRARY_PATH=/usr/catapult/lib:/usr/catapult/deps
     stop_signal: SIGINT
     stop_grace_period: 300s
     ports:
       - 7900:7900
+    working_dir: /
     volumes:
       - ./startup:/startup:ro
       - ./userconfig:/userconfig:ro
       - ./seed:/seed:ro
       - ./keys/cert:/certificates:ro
       - ./data:/data
       - ./logs:/logs
@@ -54,15 +55,16 @@
     user: '{{ user }}'
     cap_add:
       - SYS_PTRACE
     command: /bin/bash /startup/wait.sh /data/startup/datadir-initialized /startup/startBroker.sh
     environment:
       - LD_LIBRARY_PATH=/usr/catapult/lib:/usr/catapult/deps
     stop_signal: SIGINT
-    stop_grace_period: 20s
+    stop_grace_period: 60s
+    working_dir: /
     volumes:
       - ./startup:/startup:ro
       - ./userconfig:/userconfig:ro
       - ./keys/cert:/certificates:ro
       - ./data:/data
       - ./logs:/logs
```

### Comparing `symbol_shoestring-0.1.0/shoestring/templates/docker-compose-peer.yaml` & `symbol_shoestring-0.1.1/shoestring/templates/docker-compose-peer.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     command: /usr/catapult/bin/catapult.server /userconfig
     environment:
       - LD_LIBRARY_PATH=/usr/catapult/lib:/usr/catapult/deps
     stop_signal: SIGINT
     stop_grace_period: 300s
     ports:
       - 7900:7900
+    working_dir: /
     volumes:
       - ./startup:/startup:ro
       - ./userconfig:/userconfig:ro
       - ./seed:/seed:ro
       - ./data:/data
       - ./logs:/logs
       - ./keys/voting:/votingkeys
```

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/Screen.py` & `symbol_shoestring-0.1.1/shoestring/wizard/Screen.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/ScreenContainer.py` & `symbol_shoestring-0.1.1/shoestring/wizard/ScreenContainer.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/ShoestringOperation.py` & `symbol_shoestring-0.1.1/shoestring/wizard/ShoestringOperation.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/TabbedView.py` & `symbol_shoestring-0.1.1/shoestring/wizard/TabbedView.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,21 @@
 class TabList(RadioList):
 	"""
 	List of tab buttons. Only one can be selected at the same time.
 
 	:param values: List of (value, label) tuples.
 	"""
 
+	# pylint: disable=invalid-name
 	container_style = 'class:tab-list'
 	default_style = 'class:tab'
 	selected_style = 'class:tab-selected'
 	checked_style = 'class:tab-checked'
 	multiple_selection = False
+	# pylint: enable=invalid-name
 
 	def __init__(self, values, default=None):
 		super().__init__(values, default)
 		self.show_scrollbar = False
 
 		# add left + right key bindings
 		# proper bindings are actually at the end of returned lists
```

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/TitleBar.py` & `symbol_shoestring-0.1.1/shoestring/wizard/TitleBar.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/ValidatingTextBox.py` & `symbol_shoestring-0.1.1/shoestring/wizard/ValidatingTextBox.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/__main__.py` & `symbol_shoestring-0.1.1/shoestring/wizard/__main__.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/buttons.py` & `symbol_shoestring-0.1.1/shoestring/wizard/buttons.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/navigation.py` & `symbol_shoestring-0.1.1/shoestring/wizard/navigation.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screen_loader.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screen_loader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screens/certificates.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screens/certificates.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screens/end_screen.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screens/end_screen.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screens/harvesting.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screens/harvesting.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screens/modal.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screens/modal.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screens/network_type.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screens/network_type.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screens/node_settings.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screens/node_settings.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screens/node_type.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screens/node_type.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screens/obligatory.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screens/obligatory.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screens/root_check.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screens/root_check.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screens/voting.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screens/voting.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/screens/welcome.py` & `symbol_shoestring-0.1.1/shoestring/wizard/screens/welcome.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/setup_file_generator.py` & `symbol_shoestring-0.1.1/shoestring/wizard/setup_file_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 	if voting.active:
 		node_features = node_features | NodeFeatures.VOTER
 
 	replacements = [
 		('node', 'apiHttps', _to_bool_string(node_settings.api_https)),
 		('node', 'caCommonName', certificates.ca_common_name),
 		('node', 'nodeCommonName', certificates.node_common_name),
-		('node', 'features', ','.join(node_feature[len('NodeFeatures.'):] for node_feature in str(node_features).split(',')))
+		('node', 'features', node_features.to_formatted_string())
 	]
 
 	if harvesting.active:
 		config_harvesting_filepath = None
 		if not harvesting.auto_harvest:
 			config_harvesting_filepath = 'none'
 		elif not harvesting.generate_keys:
```

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/shoestring_dispatcher.py` & `symbol_shoestring-0.1.1/shoestring/wizard/shoestring_dispatcher.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/shoestring/wizard/styles.py` & `symbol_shoestring-0.1.1/shoestring/wizard/styles.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.1.0/PKG-INFO` & `symbol_shoestring-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: symbol-shoestring
-Version: 0.1.0
+Version: 0.1.1
 Summary: Symbol Shoestring Deployment Tool
 Home-page: https://github.com/symbol/product/tree/main/tools/shoestring
 License: MIT
 Keywords: symbol,shoestring,deployment,node
 Author: Symbol Contributors
 Author-email: contributors@symbol.dev
 Maintainer: Symbol Contributors
 Maintainer-email: contributors@symbol.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.5,<3.9.0)
+Requires-Dist: aiohttp (>=3.9.0,<3.10.0)
 Requires-Dist: jinja2 (>=3.1.2,<3.2.0)
 Requires-Dist: prompt-toolkit (>=3.0.39,<3.1.0)
 Requires-Dist: pyyaml (>=6.0.1,<6.1.0)
 Requires-Dist: requests (>=2.31.0,<2.32.0)
 Requires-Dist: symbol-lightapi (>=0.0.5,<0.1.0)
 Requires-Dist: symbol-sdk-python (>=3.1.0,<3.2.0)
-Requires-Dist: websockets (>=11.0.3,<11.1.0)
+Requires-Dist: websockets (>=12.0,<13.0)
 Requires-Dist: zenlog (>=1.1,<2.0)
 Project-URL: Repository, https://github.com/symbol/product/tree/main/tools/shoestring
 Description-Content-Type: text/markdown
 
 # shoestring
 
 # Security
```

