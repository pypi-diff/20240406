# Comparing `tmp/pyscard-2.0.8.tar.gz` & `tmp/pyscard-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscard-2.0.8.tar", last modified: Sat Mar  9 17:26:47 2024, max compression
+gzip compressed data, was "pyscard-2.0.9.tar", last modified: Sat Apr  6 13:11:10 2024, max compression
```

## Comparing `pyscard-2.0.8.tar` & `pyscard-2.0.9.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.096717 pyscard-2.0.8/
--rw-r--r--   0 rousseau   (501) staff       (20)      401 2017-08-18 20:39:51.000000 pyscard-2.0.8/ACKS
--rw-r--r--   0 rousseau   (501) staff       (20)    11819 2024-03-09 17:21:23.000000 pyscard-2.0.8/ChangeLog
--rw-r--r--   0 rousseau   (501) staff       (20)     5233 2023-12-24 12:13:32.000000 pyscard-2.0.8/INSTALL.md
--rw-r--r--   0 rousseau   (501) staff       (20)    24827 2015-10-09 13:28:58.000000 pyscard-2.0.8/LICENSE
--rw-r--r--   0 rousseau   (501) staff       (20)      968 2023-03-29 15:12:06.000000 pyscard-2.0.8/MANIFEST.in
--rw-r--r--   0 rousseau   (501) staff       (20)      691 2023-12-24 12:13:32.000000 pyscard-2.0.8/Makefile
--rw-r--r--   0 rousseau   (501) staff       (20)     1339 2024-03-09 17:26:47.096288 pyscard-2.0.8/PKG-INFO
--rw-r--r--   0 rousseau   (501) staff       (20)      998 2023-12-24 12:13:32.000000 pyscard-2.0.8/README.md
--rw-r--r--   0 rousseau   (501) staff       (20)      415 2015-10-09 13:28:58.000000 pyscard-2.0.8/TODO
--rw-r--r--   0 rousseau   (501) staff       (20)       81 2023-12-24 12:13:32.000000 pyscard-2.0.8/pyproject.toml
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.095611 pyscard-2.0.8/pyscard.egg-info/
--rw-r--r--   0 rousseau   (501) staff       (20)     1339 2024-03-09 17:26:47.000000 pyscard-2.0.8/pyscard.egg-info/PKG-INFO
--rw-r--r--   0 rousseau   (501) staff       (20)     6442 2024-03-09 17:26:47.000000 pyscard-2.0.8/pyscard.egg-info/SOURCES.txt
--rw-r--r--   0 rousseau   (501) staff       (20)        1 2024-03-09 17:26:47.000000 pyscard-2.0.8/pyscard.egg-info/dependency_links.txt
--rw-r--r--   0 rousseau   (501) staff       (20)       29 2024-03-09 17:26:47.000000 pyscard-2.0.8/pyscard.egg-info/requires.txt
--rw-r--r--   0 rousseau   (501) staff       (20)       10 2024-03-09 17:26:47.000000 pyscard-2.0.8/pyscard.egg-info/top_level.txt
--rw-r--r--   0 rousseau   (501) staff       (20)       38 2024-03-09 17:26:47.096799 pyscard-2.0.8/setup.cfg
--rw-r--r--   0 rousseau   (501) staff       (20)     5852 2024-03-08 16:55:59.000000 pyscard-2.0.8/setup.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.048481 pyscard-2.0.8/smartcard/
--rw-r--r--   0 rousseau   (501) staff       (20)    10405 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/ATR.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3390 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/AbstractCardRequest.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2624 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/Card.py
--rw-r--r--   0 rousseau   (501) staff       (20)     9428 2023-05-01 14:00:01.000000 pyscard-2.0.8/smartcard/CardConnection.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3390 2021-03-19 10:29:46.000000 pyscard-2.0.8/smartcard/CardConnectionDecorator.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1481 2021-03-19 10:29:46.000000 pyscard-2.0.8/smartcard/CardConnectionEvent.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2418 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/CardConnectionObserver.py
--rw-r--r--   0 rousseau   (501) staff       (20)     9118 2024-03-04 17:44:32.000000 pyscard-2.0.8/smartcard/CardMonitoring.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3321 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/CardNames.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3365 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/CardRequest.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2339 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/CardService.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3698 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/CardType.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1697 2017-11-27 16:32:09.000000 pyscard-2.0.8/smartcard/ClassLoader.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.032081 pyscard-2.0.8/smartcard/Examples/
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.065119 pyscard-2.0.8/smartcard/Examples/framework/
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1469 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_ATR.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3793 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_CardConnectionDecorator.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1892 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_ConsoleConnectionTracer.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1718 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_CustomCardType.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2977 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_CustomErrorChecker.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3112 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_ErrorChecking.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2525 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_ExclusiveCardConnection.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2085 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_MonitorCards.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2855 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_MonitorCardsAndTransmit.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1926 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_MonitorReaders.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2364 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_TransmitCardObserver.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3040 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_apduTracerInterpreter.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2352 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/framework/sample_toHexString.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.069367 pyscard-2.0.8/smartcard/Examples/scard-api/
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4147 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_control.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3447 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_getATR.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     6535 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_getAttrib.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3937 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_getStatusChange.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3171 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_listCards.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4502 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_listInterfaces.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     5004 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_locateCards.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     5425 2023-03-02 20:26:06.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_pinpad.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     5988 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_readerGroups.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2256 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_readers.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4268 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_selectDFTelecom.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4202 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/scard-api/sample_transaction.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.071618 pyscard-2.0.8/smartcard/Examples/simple/
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1489 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/simple/getATR.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1628 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/simple/getATR_context.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2366 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/simple/selectDF_TELECOM.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1654 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/Examples/simple/simpleAPDU.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.032777 pyscard-2.0.8/smartcard/Examples/wx/
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.072592 pyscard-2.0.8/smartcard/Examples/wx/apdumanager/
--rwxr-xr-x   0 rousseau   (501) staff       (20)     8977 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/wx/apdumanager/SampleAPDUManagerPanel.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2001 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/wx/apdumanager/apdumanager.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.072886 pyscard-2.0.8/smartcard/Examples/wx/apdumanager/images/
--rw-r--r--   0 rousseau   (501) staff       (20)      318 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/Examples/wx/apdumanager/images/mysmartcard.ico
--rw-r--r--   0 rousseau   (501) staff       (20)     1383 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/wx/apdumanager/setup.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.073509 pyscard-2.0.8/smartcard/Examples/wx/cardmonitor/
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4723 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/wx/cardmonitor/cardmonitor.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.073817 pyscard-2.0.8/smartcard/Examples/wx/cardmonitor/images/
--rw-r--r--   0 rousseau   (501) staff       (20)      318 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/Examples/wx/cardmonitor/images/mysmartcard.ico
--rw-r--r--   0 rousseau   (501) staff       (20)     1372 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/wx/cardmonitor/setup.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.074111 pyscard-2.0.8/smartcard/Examples/wx/pcscdiag/
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3856 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/wx/pcscdiag/pcscdiag.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.074725 pyscard-2.0.8/smartcard/Examples/wx/readerviewer/
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.075043 pyscard-2.0.8/smartcard/Examples/wx/readerviewer/images/
--rw-r--r--   0 rousseau   (501) staff       (20)      318 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/Examples/wx/readerviewer/images/readerviewer.ico
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1887 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/wx/readerviewer/readerviewer.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1374 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/Examples/wx/readerviewer/setup.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3736 2023-03-29 15:12:06.000000 pyscard-2.0.8/smartcard/Exceptions.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3191 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/ExclusiveConnectCardConnection.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3506 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/ExclusiveTransmitCardConnection.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2120 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/Observer.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2256 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/PassThruCardService.py
--rw-r--r--   0 rousseau   (501) staff       (20)     8462 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/ReaderMonitoring.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3850 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/Session.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1376 2017-11-27 16:32:09.000000 pyscard-2.0.8/smartcard/Synchronization.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1921 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/System.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1123 2017-11-27 16:32:09.000000 pyscard-2.0.8/smartcard/__init__.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.033119 pyscard-2.0.8/smartcard/doc/
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.077264 pyscard-2.0.8/smartcard/doc/images/
--rw-r--r--   0 rousseau   (501) staff       (20)    25597 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/doc/images/pyscard.jpg
--rw-r--r--   0 rousseau   (501) staff       (20)     2897 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/doc/images/sflogo.php.png
--rw-r--r--   0 rousseau   (501) staff       (20)     2185 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/guid.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.050689 pyscard-2.0.8/smartcard/pcsc/
--rw-r--r--   0 rousseau   (501) staff       (20)    12293 2023-05-01 14:01:33.000000 pyscard-2.0.8/smartcard/pcsc/PCSCCardConnection.py
--rw-r--r--   0 rousseau   (501) staff       (20)    14112 2023-05-01 14:00:01.000000 pyscard-2.0.8/smartcard/pcsc/PCSCCardRequest.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2309 2019-03-25 19:45:41.000000 pyscard-2.0.8/smartcard/pcsc/PCSCContext.py
--rw-r--r--   0 rousseau   (501) staff       (20)     4057 2022-08-23 19:47:00.000000 pyscard-2.0.8/smartcard/pcsc/PCSCExceptions.py
--rw-r--r--   0 rousseau   (501) staff       (20)     9245 2023-06-13 19:33:17.000000 pyscard-2.0.8/smartcard/pcsc/PCSCPart10.py
--rw-r--r--   0 rousseau   (501) staff       (20)     5027 2023-04-23 21:12:07.000000 pyscard-2.0.8/smartcard/pcsc/PCSCReader.py
--rw-r--r--   0 rousseau   (501) staff       (20)     4091 2021-11-07 15:41:51.000000 pyscard-2.0.8/smartcard/pcsc/PCSCReaderGroups.py
--rw-r--r--   0 rousseau   (501) staff       (20)        0 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/pcsc/__init__.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.051170 pyscard-2.0.8/smartcard/pyro/
--rw-r--r--   0 rousseau   (501) staff       (20)     3212 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/pyro/PyroReader.py
--rw-r--r--   0 rousseau   (501) staff       (20)      890 2017-11-27 16:32:09.000000 pyscard-2.0.8/smartcard/pyro/__init__.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.052446 pyscard-2.0.8/smartcard/reader/
--rw-r--r--   0 rousseau   (501) staff       (20)     2058 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/reader/Reader.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2056 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/reader/ReaderFactory.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3687 2021-11-07 15:41:51.000000 pyscard-2.0.8/smartcard/reader/ReaderGroups.py
--rw-r--r--   0 rousseau   (501) staff       (20)        0 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/reader/__init__.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.084355 pyscard-2.0.8/smartcard/scard/
--rw-r--r--   0 rousseau   (501) staff       (20)    13642 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/scard/PcscDefs.i
--rw-r--r--   0 rousseau   (501) staff       (20)    14731 2023-03-29 15:12:06.000000 pyscard-2.0.8/smartcard/scard/PcscTypemaps.i
--rw-r--r--   0 rousseau   (501) staff       (20)       36 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/scard/__init__.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3557 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/scard/gemalto.ver
--rw-r--r--   0 rousseau   (501) staff       (20)    36718 2023-03-29 15:12:06.000000 pyscard-2.0.8/smartcard/scard/helpers.c
--rw-r--r--   0 rousseau   (501) staff       (20)     3783 2023-03-29 15:12:06.000000 pyscard-2.0.8/smartcard/scard/helpers.h
--rw-r--r--   0 rousseau   (501) staff       (20)     2074 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/scard/memlog.h
--rw-r--r--   0 rousseau   (501) staff       (20)     1457 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/scard/pcsctypes.h
--rw-r--r--   0 rousseau   (501) staff       (20)     5944 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/scard/pyscard-reader.h
--rw-r--r--   0 rousseau   (501) staff       (20)      120 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/scard/scard.def
--rw-r--r--   0 rousseau   (501) staff       (20)    75318 2023-08-23 19:38:47.000000 pyscard-2.0.8/smartcard/scard/scard.i
--rw-r--r--   0 rousseau   (501) staff       (20)      317 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/scard/scard.rc
--rw-r--r--   0 rousseau   (501) staff       (20)    28777 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/scard/winscarddll.c
--rw-r--r--   0 rousseau   (501) staff       (20)    11469 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/scard/winscarddll.h
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.055270 pyscard-2.0.8/smartcard/sw/
--rw-r--r--   0 rousseau   (501) staff       (20)     1777 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/sw/ErrorChecker.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3521 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/sw/ErrorCheckingChain.py
--rw-r--r--   0 rousseau   (501) staff       (20)     6711 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/sw/ISO7816_4ErrorChecker.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3372 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/sw/ISO7816_4_SW1ErrorChecker.py
--rw-r--r--   0 rousseau   (501) staff       (20)     5357 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/sw/ISO7816_8ErrorChecker.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3302 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/sw/ISO7816_9ErrorChecker.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2827 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/sw/SWExceptions.py
--rw-r--r--   0 rousseau   (501) staff       (20)      918 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/sw/__init__.py
--rw-r--r--   0 rousseau   (501) staff       (20)     4456 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/sw/op21_ErrorChecker.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.084706 pyscard-2.0.8/smartcard/test/
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2590 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/test/configcheck.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.089516 pyscard-2.0.8/smartcard/test/framework/
--rw-r--r--   0 rousseau   (501) staff       (20)      463 2021-03-18 17:21:40.000000 pyscard-2.0.8/smartcard/test/framework/local_config.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1628 2017-11-27 16:32:09.000000 pyscard-2.0.8/smartcard/test/framework/readme.txt
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2137 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_ATR.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4833 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_CAtr.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4496 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_Card.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     9685 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_CardConnection.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3224 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_CardMonitor.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     5263 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_CardRequest.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2528 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_CardService.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     5235 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_CardType.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)    13264 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_ErrorChecking.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4315 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_ExclusiveCardConnection.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     5700 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_readergroups.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3201 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_readermonitor.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     5902 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_readermonitorstress.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3753 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_readers.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4287 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/framework/testcase_ulist.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     5493 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/test/framework/testcase_utils.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1881 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/test/framework/testsuite_framework.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.090374 pyscard-2.0.8/smartcard/test/frameworkpcsc/
--rw-r--r--   0 rousseau   (501) staff       (20)     1649 2017-11-27 16:32:09.000000 pyscard-2.0.8/smartcard/test/frameworkpcsc/readme.txt
--rwxr-xr-x   0 rousseau   (501) staff       (20)     6228 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/frameworkpcsc/testcase_pcscreadergroups.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1429 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/test/frameworkpcsc/testsuite_frameworkpcsc.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.093249 pyscard-2.0.8/smartcard/test/scard/
--rw-r--r--   0 rousseau   (501) staff       (20)      463 2021-03-18 17:20:46.000000 pyscard-2.0.8/smartcard/test/scard/local_config.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1669 2017-11-27 16:32:09.000000 pyscard-2.0.8/smartcard/test/scard/readme.txt
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3016 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/scard/testcase_getatr.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3818 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/scard/testcase_getattrib.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     2447 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/scard/testcase_geterrormessage.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)    10007 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/scard/testcase_listcards.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4531 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/scard/testcase_locatecards.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     4578 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/scard/testcase_readergroups.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3598 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/scard/testcase_returncodes.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     3351 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/test/scard/testcase_transaction.py
--rwxr-xr-x   0 rousseau   (501) staff       (20)     1606 2021-11-03 17:56:31.000000 pyscard-2.0.8/smartcard/test/scard/testsuite_scard.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3882 2017-11-27 16:32:09.000000 pyscard-2.0.8/smartcard/ulist.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.055595 pyscard-2.0.8/smartcard/util/
--rw-r--r--   0 rousseau   (501) staff       (20)     8565 2022-12-30 14:58:48.000000 pyscard-2.0.8/smartcard/util/__init__.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.058366 pyscard-2.0.8/smartcard/wx/
--rw-r--r--   0 rousseau   (501) staff       (20)     2092 2017-01-06 12:33:20.000000 pyscard-2.0.8/smartcard/wx/APDUHexValidator.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2640 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/wx/APDUTracerPanel.py
--rw-r--r--   0 rousseau   (501) staff       (20)    16500 2017-01-06 12:33:20.000000 pyscard-2.0.8/smartcard/wx/CardAndReaderTreePanel.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3668 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/wx/ReaderToolbar.py
--rw-r--r--   0 rousseau   (501) staff       (20)     3157 2021-12-29 17:24:03.000000 pyscard-2.0.8/smartcard/wx/SimpleSCardApp.py
--rw-r--r--   0 rousseau   (501) staff       (20)     2140 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/wx/SimpleSCardAppEventObserver.py
--rw-r--r--   0 rousseau   (501) staff       (20)    13111 2017-01-06 12:33:20.000000 pyscard-2.0.8/smartcard/wx/SimpleSCardAppFrame.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1733 2023-12-22 12:00:33.000000 pyscard-2.0.8/smartcard/wx/__init__.py
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.059008 pyscard-2.0.8/smartcard/wx/resources/
--rw-r--r--   0 rousseau   (501) staff       (20)      318 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/wx/resources/reader.ico
--rw-r--r--   0 rousseau   (501) staff       (20)      318 2015-10-09 13:28:58.000000 pyscard-2.0.8/smartcard/wx/resources/smartcard.ico
-drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-03-09 17:26:47.095206 pyscard-2.0.8/test/
--rw-r--r--   0 rousseau   (501) staff       (20)        0 2015-10-09 13:28:58.000000 pyscard-2.0.8/test/__init__.py
--rw-r--r--   0 rousseau   (501) staff       (20)     4176 2021-11-03 17:56:31.000000 pyscard-2.0.8/test/test_ATR.py
--rw-r--r--   0 rousseau   (501) staff       (20)     4207 2023-05-01 14:00:52.000000 pyscard-2.0.8/test/test_Exceptions.py
--rw-r--r--   0 rousseau   (501) staff       (20)      721 2023-04-01 14:49:38.000000 pyscard-2.0.8/test/test_PCSC.py
--rw-r--r--   0 rousseau   (501) staff       (20)     4821 2022-08-28 16:38:10.000000 pyscard-2.0.8/test/test_PCSCExceptions.py
--rw-r--r--   0 rousseau   (501) staff       (20)     1012 2022-08-28 16:38:10.000000 pyscard-2.0.8/test/test_SCardGetErrorMessage.py
--rw-r--r--   0 rousseau   (501) staff       (20)     4943 2021-11-03 17:56:31.000000 pyscard-2.0.8/test/test_util.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.805106 pyscard-2.0.9/
+-rw-r--r--   0 rousseau   (501) staff       (20)      401 2017-08-18 20:39:51.000000 pyscard-2.0.9/ACKS
+-rw-r--r--   0 rousseau   (501) staff       (20)    11945 2024-04-05 20:30:03.000000 pyscard-2.0.9/ChangeLog
+-rw-r--r--   0 rousseau   (501) staff       (20)     5233 2023-12-24 12:13:32.000000 pyscard-2.0.9/INSTALL.md
+-rw-r--r--   0 rousseau   (501) staff       (20)    24827 2015-10-09 13:28:58.000000 pyscard-2.0.9/LICENSE
+-rw-r--r--   0 rousseau   (501) staff       (20)      968 2023-03-29 15:12:06.000000 pyscard-2.0.9/MANIFEST.in
+-rw-r--r--   0 rousseau   (501) staff       (20)      691 2023-12-24 12:13:32.000000 pyscard-2.0.9/Makefile
+-rw-r--r--   0 rousseau   (501) staff       (20)     1339 2024-04-06 13:11:10.804715 pyscard-2.0.9/PKG-INFO
+-rw-r--r--   0 rousseau   (501) staff       (20)      998 2023-12-24 12:13:32.000000 pyscard-2.0.9/README.md
+-rw-r--r--   0 rousseau   (501) staff       (20)      415 2015-10-09 13:28:58.000000 pyscard-2.0.9/TODO
+-rw-r--r--   0 rousseau   (501) staff       (20)       81 2023-12-24 12:13:32.000000 pyscard-2.0.9/pyproject.toml
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.804012 pyscard-2.0.9/pyscard.egg-info/
+-rw-r--r--   0 rousseau   (501) staff       (20)     1339 2024-04-06 13:11:10.000000 pyscard-2.0.9/pyscard.egg-info/PKG-INFO
+-rw-r--r--   0 rousseau   (501) staff       (20)     6442 2024-04-06 13:11:10.000000 pyscard-2.0.9/pyscard.egg-info/SOURCES.txt
+-rw-r--r--   0 rousseau   (501) staff       (20)        1 2024-04-06 13:11:10.000000 pyscard-2.0.9/pyscard.egg-info/dependency_links.txt
+-rw-r--r--   0 rousseau   (501) staff       (20)       29 2024-04-06 13:11:10.000000 pyscard-2.0.9/pyscard.egg-info/requires.txt
+-rw-r--r--   0 rousseau   (501) staff       (20)       10 2024-04-06 13:11:10.000000 pyscard-2.0.9/pyscard.egg-info/top_level.txt
+-rw-r--r--   0 rousseau   (501) staff       (20)       38 2024-04-06 13:11:10.805184 pyscard-2.0.9/setup.cfg
+-rw-r--r--   0 rousseau   (501) staff       (20)     5852 2024-04-05 20:30:24.000000 pyscard-2.0.9/setup.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.711316 pyscard-2.0.9/smartcard/
+-rw-r--r--   0 rousseau   (501) staff       (20)    10405 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/ATR.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3390 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/AbstractCardRequest.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2624 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/Card.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     9428 2023-05-01 14:00:01.000000 pyscard-2.0.9/smartcard/CardConnection.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3390 2021-03-19 10:29:46.000000 pyscard-2.0.9/smartcard/CardConnectionDecorator.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1481 2021-03-19 10:29:46.000000 pyscard-2.0.9/smartcard/CardConnectionEvent.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2418 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/CardConnectionObserver.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     9118 2024-03-04 17:44:32.000000 pyscard-2.0.9/smartcard/CardMonitoring.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3321 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/CardNames.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3365 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/CardRequest.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2339 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/CardService.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3698 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/CardType.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1697 2017-11-27 16:32:09.000000 pyscard-2.0.9/smartcard/ClassLoader.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.686330 pyscard-2.0.9/smartcard/Examples/
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.755684 pyscard-2.0.9/smartcard/Examples/framework/
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1469 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_ATR.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3793 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_CardConnectionDecorator.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1892 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_ConsoleConnectionTracer.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1718 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_CustomCardType.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2977 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_CustomErrorChecker.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3112 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_ErrorChecking.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2525 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_ExclusiveCardConnection.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2085 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_MonitorCards.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2855 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_MonitorCardsAndTransmit.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1926 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_MonitorReaders.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2364 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_TransmitCardObserver.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3040 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_apduTracerInterpreter.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2352 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/framework/sample_toHexString.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.761468 pyscard-2.0.9/smartcard/Examples/scard-api/
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4147 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_control.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3447 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_getATR.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     6535 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_getAttrib.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3937 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_getStatusChange.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3171 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_listCards.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4502 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_listInterfaces.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     5004 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_locateCards.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     5425 2023-03-02 20:26:06.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_pinpad.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     5988 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_readerGroups.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2256 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_readers.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4268 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_selectDFTelecom.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4202 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/scard-api/sample_transaction.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.763131 pyscard-2.0.9/smartcard/Examples/simple/
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1489 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/simple/getATR.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1628 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/simple/getATR_context.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2366 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/simple/selectDF_TELECOM.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1654 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/Examples/simple/simpleAPDU.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.687077 pyscard-2.0.9/smartcard/Examples/wx/
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.765008 pyscard-2.0.9/smartcard/Examples/wx/apdumanager/
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     8977 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/wx/apdumanager/SampleAPDUManagerPanel.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2001 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/wx/apdumanager/apdumanager.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.765430 pyscard-2.0.9/smartcard/Examples/wx/apdumanager/images/
+-rw-r--r--   0 rousseau   (501) staff       (20)      318 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/Examples/wx/apdumanager/images/mysmartcard.ico
+-rw-r--r--   0 rousseau   (501) staff       (20)     1383 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/wx/apdumanager/setup.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.766372 pyscard-2.0.9/smartcard/Examples/wx/cardmonitor/
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4723 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/wx/cardmonitor/cardmonitor.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.766792 pyscard-2.0.9/smartcard/Examples/wx/cardmonitor/images/
+-rw-r--r--   0 rousseau   (501) staff       (20)      318 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/Examples/wx/cardmonitor/images/mysmartcard.ico
+-rw-r--r--   0 rousseau   (501) staff       (20)     1372 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/wx/cardmonitor/setup.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.767407 pyscard-2.0.9/smartcard/Examples/wx/pcscdiag/
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3856 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/wx/pcscdiag/pcscdiag.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.768257 pyscard-2.0.9/smartcard/Examples/wx/readerviewer/
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.768655 pyscard-2.0.9/smartcard/Examples/wx/readerviewer/images/
+-rw-r--r--   0 rousseau   (501) staff       (20)      318 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/Examples/wx/readerviewer/images/readerviewer.ico
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1887 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/wx/readerviewer/readerviewer.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1374 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/Examples/wx/readerviewer/setup.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3801 2024-03-18 20:57:13.000000 pyscard-2.0.9/smartcard/Exceptions.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3191 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/ExclusiveConnectCardConnection.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3506 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/ExclusiveTransmitCardConnection.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2120 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/Observer.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2256 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/PassThruCardService.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     8462 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/ReaderMonitoring.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3850 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/Session.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1376 2017-11-27 16:32:09.000000 pyscard-2.0.9/smartcard/Synchronization.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1921 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/System.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1123 2017-11-27 16:32:09.000000 pyscard-2.0.9/smartcard/__init__.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.687426 pyscard-2.0.9/smartcard/doc/
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.770349 pyscard-2.0.9/smartcard/doc/images/
+-rw-r--r--   0 rousseau   (501) staff       (20)    25597 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/doc/images/pyscard.jpg
+-rw-r--r--   0 rousseau   (501) staff       (20)     2897 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/doc/images/sflogo.php.png
+-rw-r--r--   0 rousseau   (501) staff       (20)     2185 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/guid.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.717698 pyscard-2.0.9/smartcard/pcsc/
+-rw-r--r--   0 rousseau   (501) staff       (20)    12293 2023-05-01 14:01:33.000000 pyscard-2.0.9/smartcard/pcsc/PCSCCardConnection.py
+-rw-r--r--   0 rousseau   (501) staff       (20)    14112 2023-05-01 14:00:01.000000 pyscard-2.0.9/smartcard/pcsc/PCSCCardRequest.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2309 2019-03-25 19:45:41.000000 pyscard-2.0.9/smartcard/pcsc/PCSCContext.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     4057 2022-08-23 19:47:00.000000 pyscard-2.0.9/smartcard/pcsc/PCSCExceptions.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     9245 2023-06-13 19:33:17.000000 pyscard-2.0.9/smartcard/pcsc/PCSCPart10.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     5027 2023-04-23 21:12:07.000000 pyscard-2.0.9/smartcard/pcsc/PCSCReader.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     4091 2021-11-07 15:41:51.000000 pyscard-2.0.9/smartcard/pcsc/PCSCReaderGroups.py
+-rw-r--r--   0 rousseau   (501) staff       (20)        0 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/pcsc/__init__.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.718781 pyscard-2.0.9/smartcard/pyro/
+-rw-r--r--   0 rousseau   (501) staff       (20)     3212 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/pyro/PyroReader.py
+-rw-r--r--   0 rousseau   (501) staff       (20)      890 2017-11-27 16:32:09.000000 pyscard-2.0.9/smartcard/pyro/__init__.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.720882 pyscard-2.0.9/smartcard/reader/
+-rw-r--r--   0 rousseau   (501) staff       (20)     2058 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/reader/Reader.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2056 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/reader/ReaderFactory.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3687 2021-11-07 15:41:51.000000 pyscard-2.0.9/smartcard/reader/ReaderGroups.py
+-rw-r--r--   0 rousseau   (501) staff       (20)        0 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/reader/__init__.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.782571 pyscard-2.0.9/smartcard/scard/
+-rw-r--r--   0 rousseau   (501) staff       (20)    13642 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/scard/PcscDefs.i
+-rw-r--r--   0 rousseau   (501) staff       (20)    14746 2024-03-12 12:55:25.000000 pyscard-2.0.9/smartcard/scard/PcscTypemaps.i
+-rw-r--r--   0 rousseau   (501) staff       (20)       36 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/scard/__init__.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3557 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/scard/gemalto.ver
+-rw-r--r--   0 rousseau   (501) staff       (20)    36718 2023-03-29 15:12:06.000000 pyscard-2.0.9/smartcard/scard/helpers.c
+-rw-r--r--   0 rousseau   (501) staff       (20)     3783 2023-03-29 15:12:06.000000 pyscard-2.0.9/smartcard/scard/helpers.h
+-rw-r--r--   0 rousseau   (501) staff       (20)     2074 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/scard/memlog.h
+-rw-r--r--   0 rousseau   (501) staff       (20)     1457 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/scard/pcsctypes.h
+-rw-r--r--   0 rousseau   (501) staff       (20)     5944 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/scard/pyscard-reader.h
+-rw-r--r--   0 rousseau   (501) staff       (20)      120 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/scard/scard.def
+-rw-r--r--   0 rousseau   (501) staff       (20)    75318 2023-08-23 19:38:47.000000 pyscard-2.0.9/smartcard/scard/scard.i
+-rw-r--r--   0 rousseau   (501) staff       (20)      317 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/scard/scard.rc
+-rw-r--r--   0 rousseau   (501) staff       (20)    28777 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/scard/winscarddll.c
+-rw-r--r--   0 rousseau   (501) staff       (20)    11469 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/scard/winscarddll.h
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.725500 pyscard-2.0.9/smartcard/sw/
+-rw-r--r--   0 rousseau   (501) staff       (20)     1777 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/sw/ErrorChecker.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3521 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/sw/ErrorCheckingChain.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     6711 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/sw/ISO7816_4ErrorChecker.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3372 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/sw/ISO7816_4_SW1ErrorChecker.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     5357 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/sw/ISO7816_8ErrorChecker.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3302 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/sw/ISO7816_9ErrorChecker.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2827 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/sw/SWExceptions.py
+-rw-r--r--   0 rousseau   (501) staff       (20)      918 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/sw/__init__.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     4456 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/sw/op21_ErrorChecker.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.783363 pyscard-2.0.9/smartcard/test/
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2590 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/test/configcheck.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.792983 pyscard-2.0.9/smartcard/test/framework/
+-rw-r--r--   0 rousseau   (501) staff       (20)      463 2021-03-18 17:21:40.000000 pyscard-2.0.9/smartcard/test/framework/local_config.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1628 2017-11-27 16:32:09.000000 pyscard-2.0.9/smartcard/test/framework/readme.txt
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2137 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_ATR.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4833 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_CAtr.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4496 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_Card.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     9685 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_CardConnection.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3224 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_CardMonitor.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     5263 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_CardRequest.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2528 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_CardService.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     5235 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_CardType.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)    13264 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_ErrorChecking.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4315 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_ExclusiveCardConnection.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     5700 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_readergroups.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3201 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_readermonitor.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     5902 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_readermonitorstress.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3753 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_readers.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4287 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/framework/testcase_ulist.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     5493 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/test/framework/testcase_utils.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1881 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/test/framework/testsuite_framework.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.794595 pyscard-2.0.9/smartcard/test/frameworkpcsc/
+-rw-r--r--   0 rousseau   (501) staff       (20)     1649 2017-11-27 16:32:09.000000 pyscard-2.0.9/smartcard/test/frameworkpcsc/readme.txt
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     6228 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/frameworkpcsc/testcase_pcscreadergroups.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1429 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/test/frameworkpcsc/testsuite_frameworkpcsc.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.799155 pyscard-2.0.9/smartcard/test/scard/
+-rw-r--r--   0 rousseau   (501) staff       (20)      463 2021-03-18 17:20:46.000000 pyscard-2.0.9/smartcard/test/scard/local_config.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1669 2017-11-27 16:32:09.000000 pyscard-2.0.9/smartcard/test/scard/readme.txt
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3016 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/scard/testcase_getatr.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3818 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/scard/testcase_getattrib.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     2447 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/scard/testcase_geterrormessage.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)    10007 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/scard/testcase_listcards.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4531 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/scard/testcase_locatecards.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     4578 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/scard/testcase_readergroups.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3598 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/scard/testcase_returncodes.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     3351 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/test/scard/testcase_transaction.py
+-rwxr-xr-x   0 rousseau   (501) staff       (20)     1606 2021-11-03 17:56:31.000000 pyscard-2.0.9/smartcard/test/scard/testsuite_scard.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3882 2017-11-27 16:32:09.000000 pyscard-2.0.9/smartcard/ulist.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.725920 pyscard-2.0.9/smartcard/util/
+-rw-r--r--   0 rousseau   (501) staff       (20)     8565 2022-12-30 14:58:48.000000 pyscard-2.0.9/smartcard/util/__init__.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.745828 pyscard-2.0.9/smartcard/wx/
+-rw-r--r--   0 rousseau   (501) staff       (20)     2092 2017-01-06 12:33:20.000000 pyscard-2.0.9/smartcard/wx/APDUHexValidator.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2640 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/wx/APDUTracerPanel.py
+-rw-r--r--   0 rousseau   (501) staff       (20)    16500 2017-01-06 12:33:20.000000 pyscard-2.0.9/smartcard/wx/CardAndReaderTreePanel.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3668 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/wx/ReaderToolbar.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     3157 2021-12-29 17:24:03.000000 pyscard-2.0.9/smartcard/wx/SimpleSCardApp.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     2140 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/wx/SimpleSCardAppEventObserver.py
+-rw-r--r--   0 rousseau   (501) staff       (20)    13111 2017-01-06 12:33:20.000000 pyscard-2.0.9/smartcard/wx/SimpleSCardAppFrame.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1733 2023-12-22 12:00:33.000000 pyscard-2.0.9/smartcard/wx/__init__.py
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.746779 pyscard-2.0.9/smartcard/wx/resources/
+-rw-r--r--   0 rousseau   (501) staff       (20)      318 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/wx/resources/reader.ico
+-rw-r--r--   0 rousseau   (501) staff       (20)      318 2015-10-09 13:28:58.000000 pyscard-2.0.9/smartcard/wx/resources/smartcard.ico
+drwxr-xr-x   0 rousseau   (501) staff       (20)        0 2024-04-06 13:11:10.803254 pyscard-2.0.9/test/
+-rw-r--r--   0 rousseau   (501) staff       (20)        0 2015-10-09 13:28:58.000000 pyscard-2.0.9/test/__init__.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     4176 2021-11-03 17:56:31.000000 pyscard-2.0.9/test/test_ATR.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     5170 2024-03-18 20:57:13.000000 pyscard-2.0.9/test/test_Exceptions.py
+-rw-r--r--   0 rousseau   (501) staff       (20)      721 2023-04-01 14:49:38.000000 pyscard-2.0.9/test/test_PCSC.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     4821 2022-08-28 16:38:10.000000 pyscard-2.0.9/test/test_PCSCExceptions.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     1012 2022-08-28 16:38:10.000000 pyscard-2.0.9/test/test_SCardGetErrorMessage.py
+-rw-r--r--   0 rousseau   (501) staff       (20)     4943 2021-11-03 17:56:31.000000 pyscard-2.0.9/test/test_util.py
```

### Comparing `pyscard-2.0.8/ChangeLog` & `pyscard-2.0.9/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2.0.9 (April 2024)
+==================
+   * fix a bug with CardRequestTimeoutException introduced in 2.0.8
+   * Minor changes
+
 2.0.8 (march 2024)
 ==================
    * Make CardMonitor() thread safe on Python 3.12
    * Add hresult value in exceptions
    * Improve documentation
    * Check swig is installed on build
    * Remove use of imp module for wx (GUI)
```

### Comparing `pyscard-2.0.8/INSTALL.md` & `pyscard-2.0.9/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/LICENSE` & `pyscard-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/MANIFEST.in` & `pyscard-2.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/Makefile` & `pyscard-2.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/PKG-INFO` & `pyscard-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyscard
-Version: 2.0.8
+Version: 2.0.9
 Summary: Smartcard module for Python.
 Home-page: https://github.com/LudovicRousseau/pyscard
-Download-URL: http://sourceforge.net/projects/pyscard/files/pyscard/pyscard%202.0.8/pyscard-2.0.8.tar.gz/download
+Download-URL: http://sourceforge.net/projects/pyscard/files/pyscard/pyscard%202.0.9/pyscard-2.0.9.tar.gz/download
 Author: Ludovic Rousseau
 Author-email: ludovic.rousseau@free.fr
 Platform: linux
 Platform: win32
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
```

### Comparing `pyscard-2.0.8/README.md` & `pyscard-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/pyscard.egg-info/PKG-INFO` & `pyscard-2.0.9/pyscard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyscard
-Version: 2.0.8
+Version: 2.0.9
 Summary: Smartcard module for Python.
 Home-page: https://github.com/LudovicRousseau/pyscard
-Download-URL: http://sourceforge.net/projects/pyscard/files/pyscard/pyscard%202.0.8/pyscard-2.0.8.tar.gz/download
+Download-URL: http://sourceforge.net/projects/pyscard/files/pyscard/pyscard%202.0.9/pyscard-2.0.9.tar.gz/download
 Author: Ludovic Rousseau
 Author-email: ludovic.rousseau@free.fr
 Platform: linux
 Platform: win32
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Intended Audience :: Developers
```

### Comparing `pyscard-2.0.8/pyscard.egg-info/SOURCES.txt` & `pyscard-2.0.9/pyscard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/setup.py` & `pyscard-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     platform_swig_opts = ['-DPCSCLITE']
     try:
         pkg_config_cflags = subprocess.check_output(['pkg-config', '--cflags', 'libpcsclite'])
         platform_extra_compile_args += shlex.split(pkg_config_cflags.decode())
     except:
         platform_include_dirs = ['/usr/include/PCSC', '/usr/local/include/PCSC']
 
-VERSION_INFO = (2, 0, 8, 0)
+VERSION_INFO = (2, 0, 9, 0)
 VERSION_STR = '%i.%i.%i' % VERSION_INFO[:3]
 VERSION_ALT = '%i,%01i,%01i,%04i' % VERSION_INFO
 
 
 class BuildPyBuildExtFirst(build_py):
     """Workaround substitude `build_py` command for SWIG"""
     def run(self):
```

### Comparing `pyscard-2.0.8/smartcard/ATR.py` & `pyscard-2.0.9/smartcard/ATR.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/AbstractCardRequest.py` & `pyscard-2.0.9/smartcard/AbstractCardRequest.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Card.py` & `pyscard-2.0.9/smartcard/Card.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/CardConnection.py` & `pyscard-2.0.9/smartcard/CardConnection.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/CardConnectionDecorator.py` & `pyscard-2.0.9/smartcard/CardConnectionDecorator.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/CardConnectionEvent.py` & `pyscard-2.0.9/smartcard/CardConnectionEvent.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/CardConnectionObserver.py` & `pyscard-2.0.9/smartcard/CardConnectionObserver.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/CardMonitoring.py` & `pyscard-2.0.9/smartcard/CardMonitoring.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/CardNames.py` & `pyscard-2.0.9/smartcard/CardNames.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/CardRequest.py` & `pyscard-2.0.9/smartcard/CardRequest.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/CardService.py` & `pyscard-2.0.9/smartcard/CardService.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/CardType.py` & `pyscard-2.0.9/smartcard/CardType.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/ClassLoader.py` & `pyscard-2.0.9/smartcard/ClassLoader.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_ATR.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_ATR.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_CardConnectionDecorator.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_CardConnectionDecorator.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_ConsoleConnectionTracer.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_ConsoleConnectionTracer.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_CustomCardType.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_CustomCardType.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_CustomErrorChecker.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_CustomErrorChecker.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_ErrorChecking.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_ErrorChecking.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_ExclusiveCardConnection.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_ExclusiveCardConnection.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_MonitorCards.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_MonitorCards.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_MonitorCardsAndTransmit.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_MonitorCardsAndTransmit.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_MonitorReaders.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_MonitorReaders.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_TransmitCardObserver.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_TransmitCardObserver.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_apduTracerInterpreter.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_apduTracerInterpreter.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/framework/sample_toHexString.py` & `pyscard-2.0.9/smartcard/Examples/framework/sample_toHexString.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_control.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_control.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_getATR.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_getATR.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_getAttrib.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_getAttrib.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_getStatusChange.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_getStatusChange.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_listCards.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_listCards.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_listInterfaces.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_listInterfaces.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_locateCards.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_locateCards.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_pinpad.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_pinpad.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_readerGroups.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_readerGroups.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_readers.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_readers.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_selectDFTelecom.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_selectDFTelecom.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/scard-api/sample_transaction.py` & `pyscard-2.0.9/smartcard/Examples/scard-api/sample_transaction.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/simple/getATR.py` & `pyscard-2.0.9/smartcard/Examples/simple/getATR.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/simple/getATR_context.py` & `pyscard-2.0.9/smartcard/Examples/simple/getATR_context.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/simple/selectDF_TELECOM.py` & `pyscard-2.0.9/smartcard/Examples/simple/selectDF_TELECOM.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/simple/simpleAPDU.py` & `pyscard-2.0.9/smartcard/Examples/simple/simpleAPDU.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/wx/apdumanager/SampleAPDUManagerPanel.py` & `pyscard-2.0.9/smartcard/Examples/wx/apdumanager/SampleAPDUManagerPanel.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/wx/apdumanager/apdumanager.py` & `pyscard-2.0.9/smartcard/Examples/wx/apdumanager/apdumanager.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/wx/apdumanager/setup.py` & `pyscard-2.0.9/smartcard/Examples/wx/apdumanager/setup.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/wx/cardmonitor/cardmonitor.py` & `pyscard-2.0.9/smartcard/Examples/wx/cardmonitor/cardmonitor.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/wx/cardmonitor/setup.py` & `pyscard-2.0.9/smartcard/Examples/wx/cardmonitor/setup.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/wx/pcscdiag/pcscdiag.py` & `pyscard-2.0.9/smartcard/Examples/wx/pcscdiag/pcscdiag.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/wx/readerviewer/readerviewer.py` & `pyscard-2.0.9/smartcard/Examples/wx/readerviewer/readerviewer.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Examples/wx/readerviewer/setup.py` & `pyscard-2.0.9/smartcard/Examples/wx/readerviewer/setup.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Exceptions.py` & `pyscard-2.0.9/smartcard/Exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,18 @@
     """Raised when a CardRequest wait fails."""
     pass
 
 
 class CardRequestTimeoutException(SmartcardException):
     """Raised when a CardRequest times out."""
 
-    def __init__(self, *args):
+    def __init__(self, hresult=-1, *args):
         SmartcardException.__init__(self,
-                                    "Time-out during card request", *args)
+                                    "Time-out during card request",
+                                    hresult=hresult, *args)
 
 
 class CardServiceException(SmartcardException):
     """Raised when a CardService class method fails."""
     pass
```

### Comparing `pyscard-2.0.8/smartcard/ExclusiveConnectCardConnection.py` & `pyscard-2.0.9/smartcard/ExclusiveConnectCardConnection.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/ExclusiveTransmitCardConnection.py` & `pyscard-2.0.9/smartcard/ExclusiveTransmitCardConnection.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Observer.py` & `pyscard-2.0.9/smartcard/Observer.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/PassThruCardService.py` & `pyscard-2.0.9/smartcard/PassThruCardService.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/ReaderMonitoring.py` & `pyscard-2.0.9/smartcard/ReaderMonitoring.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Session.py` & `pyscard-2.0.9/smartcard/Session.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/Synchronization.py` & `pyscard-2.0.9/smartcard/Synchronization.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/System.py` & `pyscard-2.0.9/smartcard/System.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/__init__.py` & `pyscard-2.0.9/smartcard/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/doc/images/pyscard.jpg` & `pyscard-2.0.9/smartcard/doc/images/pyscard.jpg`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/doc/images/sflogo.php.png` & `pyscard-2.0.9/smartcard/doc/images/sflogo.php.png`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/guid.py` & `pyscard-2.0.9/smartcard/guid.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/pcsc/PCSCCardConnection.py` & `pyscard-2.0.9/smartcard/pcsc/PCSCCardConnection.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/pcsc/PCSCCardRequest.py` & `pyscard-2.0.9/smartcard/pcsc/PCSCCardRequest.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/pcsc/PCSCContext.py` & `pyscard-2.0.9/smartcard/pcsc/PCSCContext.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/pcsc/PCSCExceptions.py` & `pyscard-2.0.9/smartcard/pcsc/PCSCExceptions.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/pcsc/PCSCPart10.py` & `pyscard-2.0.9/smartcard/pcsc/PCSCPart10.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/pcsc/PCSCReader.py` & `pyscard-2.0.9/smartcard/pcsc/PCSCReader.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/pcsc/PCSCReaderGroups.py` & `pyscard-2.0.9/smartcard/pcsc/PCSCReaderGroups.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/pyro/PyroReader.py` & `pyscard-2.0.9/smartcard/pyro/PyroReader.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/pyro/__init__.py` & `pyscard-2.0.9/smartcard/pyro/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/reader/Reader.py` & `pyscard-2.0.9/smartcard/reader/Reader.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/reader/ReaderFactory.py` & `pyscard-2.0.9/smartcard/reader/ReaderFactory.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/reader/ReaderGroups.py` & `pyscard-2.0.9/smartcard/reader/ReaderGroups.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/scard/PcscDefs.i` & `pyscard-2.0.9/smartcard/scard/PcscDefs.i`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/scard/PcscTypemaps.i` & `pyscard-2.0.9/smartcard/scard/PcscTypemaps.i`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,15 @@
 {
     $1 = &temp;
 }
 
 %typemap(in) SCARDDWORDARG INPUT(SCARDDWORDARG)
 {
     $1 =  SCardHelper_PySCardDwordArgToSCARDDWORDARG( $input );
-    if (-1 == $1)
+    if ((SCARDDWORDARG)-1 == $1)
         goto fail;
 }
 
 %typemap(argout) SCARDDWORDARG* OUTPUT
 {
     SCardHelper_AppendSCardDwordArgToPyObject( *$1, &$result );
 }
```

### Comparing `pyscard-2.0.8/smartcard/scard/gemalto.ver` & `pyscard-2.0.9/smartcard/scard/gemalto.ver`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/scard/helpers.c` & `pyscard-2.0.9/smartcard/scard/helpers.c`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/scard/helpers.h` & `pyscard-2.0.9/smartcard/scard/helpers.h`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/scard/memlog.h` & `pyscard-2.0.9/smartcard/scard/memlog.h`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/scard/pcsctypes.h` & `pyscard-2.0.9/smartcard/scard/pcsctypes.h`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/scard/pyscard-reader.h` & `pyscard-2.0.9/smartcard/scard/pyscard-reader.h`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/scard/scard.i` & `pyscard-2.0.9/smartcard/scard/scard.i`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/scard/winscarddll.c` & `pyscard-2.0.9/smartcard/scard/winscarddll.c`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/scard/winscarddll.h` & `pyscard-2.0.9/smartcard/scard/winscarddll.h`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/sw/ErrorChecker.py` & `pyscard-2.0.9/smartcard/sw/ErrorChecker.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/sw/ErrorCheckingChain.py` & `pyscard-2.0.9/smartcard/sw/ErrorCheckingChain.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/sw/ISO7816_4ErrorChecker.py` & `pyscard-2.0.9/smartcard/sw/ISO7816_4ErrorChecker.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/sw/ISO7816_4_SW1ErrorChecker.py` & `pyscard-2.0.9/smartcard/sw/ISO7816_4_SW1ErrorChecker.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/sw/ISO7816_8ErrorChecker.py` & `pyscard-2.0.9/smartcard/sw/ISO7816_8ErrorChecker.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/sw/ISO7816_9ErrorChecker.py` & `pyscard-2.0.9/smartcard/sw/ISO7816_9ErrorChecker.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/sw/SWExceptions.py` & `pyscard-2.0.9/smartcard/sw/SWExceptions.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/sw/__init__.py` & `pyscard-2.0.9/smartcard/sw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/sw/op21_ErrorChecker.py` & `pyscard-2.0.9/smartcard/sw/op21_ErrorChecker.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/configcheck.py` & `pyscard-2.0.9/smartcard/test/configcheck.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/readme.txt` & `pyscard-2.0.9/smartcard/test/framework/readme.txt`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_ATR.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_ATR.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_CAtr.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_CAtr.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_Card.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_Card.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_CardConnection.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_CardConnection.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_CardMonitor.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_CardMonitor.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_CardRequest.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_CardRequest.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_CardService.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_CardService.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_CardType.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_CardType.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_ErrorChecking.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_ErrorChecking.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_ExclusiveCardConnection.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_ExclusiveCardConnection.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_readergroups.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_readergroups.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_readermonitor.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_readermonitor.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_readermonitorstress.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_readermonitorstress.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_readers.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_readers.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_ulist.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_ulist.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testcase_utils.py` & `pyscard-2.0.9/smartcard/test/framework/testcase_utils.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/framework/testsuite_framework.py` & `pyscard-2.0.9/smartcard/test/framework/testsuite_framework.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/frameworkpcsc/readme.txt` & `pyscard-2.0.9/smartcard/test/frameworkpcsc/readme.txt`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/frameworkpcsc/testcase_pcscreadergroups.py` & `pyscard-2.0.9/smartcard/test/frameworkpcsc/testcase_pcscreadergroups.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/frameworkpcsc/testsuite_frameworkpcsc.py` & `pyscard-2.0.9/smartcard/test/frameworkpcsc/testsuite_frameworkpcsc.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/scard/readme.txt` & `pyscard-2.0.9/smartcard/test/scard/readme.txt`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/scard/testcase_getatr.py` & `pyscard-2.0.9/smartcard/test/scard/testcase_getatr.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/scard/testcase_getattrib.py` & `pyscard-2.0.9/smartcard/test/scard/testcase_getattrib.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/scard/testcase_geterrormessage.py` & `pyscard-2.0.9/smartcard/test/scard/testcase_geterrormessage.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/scard/testcase_listcards.py` & `pyscard-2.0.9/smartcard/test/scard/testcase_listcards.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/scard/testcase_locatecards.py` & `pyscard-2.0.9/smartcard/test/scard/testcase_locatecards.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/scard/testcase_readergroups.py` & `pyscard-2.0.9/smartcard/test/scard/testcase_readergroups.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/scard/testcase_returncodes.py` & `pyscard-2.0.9/smartcard/test/scard/testcase_returncodes.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/scard/testcase_transaction.py` & `pyscard-2.0.9/smartcard/test/scard/testcase_transaction.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/test/scard/testsuite_scard.py` & `pyscard-2.0.9/smartcard/test/scard/testsuite_scard.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/ulist.py` & `pyscard-2.0.9/smartcard/ulist.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/util/__init__.py` & `pyscard-2.0.9/smartcard/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/wx/APDUHexValidator.py` & `pyscard-2.0.9/smartcard/wx/APDUHexValidator.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/wx/APDUTracerPanel.py` & `pyscard-2.0.9/smartcard/wx/APDUTracerPanel.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/wx/CardAndReaderTreePanel.py` & `pyscard-2.0.9/smartcard/wx/CardAndReaderTreePanel.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/wx/ReaderToolbar.py` & `pyscard-2.0.9/smartcard/wx/ReaderToolbar.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/wx/SimpleSCardApp.py` & `pyscard-2.0.9/smartcard/wx/SimpleSCardApp.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/wx/SimpleSCardAppEventObserver.py` & `pyscard-2.0.9/smartcard/wx/SimpleSCardAppEventObserver.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/wx/SimpleSCardAppFrame.py` & `pyscard-2.0.9/smartcard/wx/SimpleSCardAppFrame.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/smartcard/wx/__init__.py` & `pyscard-2.0.9/smartcard/wx/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/test/test_ATR.py` & `pyscard-2.0.9/test/test_ATR.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/test/test_Exceptions.py` & `pyscard-2.0.9/test/test_Exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -106,9 +106,29 @@
         if platform.system() == 'Windows':
             expected = "An attempt was made to end a non-existent transaction. "
         else:
             expected = "Transaction failed."
         expected = "foo: " + expected + " (0x80100016)"
         self.assertEqual(text, expected)
 
+    def test_wrongType(self):
+        # SCardEstablishContext() argument should be int or long
+        with self.assertRaises(TypeError):
+            hresult, hcontext = SCardEstablishContext([0])
+
+        with self.assertRaises(TypeError):
+            hresult, hcontext = SCardEstablishContext("foo")
+
+    def test_CardRequestTimeoutException(self):
+        exc = CardRequestTimeoutException()
+        self.assertEqual(str(exc), "Time-out during card request")
+        exc = CardRequestTimeoutException(SCARD_E_NOT_TRANSACTED)
+        if platform.system() == 'Windows':
+            expected = "Time-out during card request: An attempt was made to end a non-existent transaction.  (0x80100016)"
+        else:
+            expected = "Time-out during card request: Transaction failed. (0x80100016)"
+        self.assertEqual(str(exc), expected)
+        exc = CardRequestTimeoutException(hresult=SCARD_E_NOT_TRANSACTED)
+        self.assertEqual(str(exc), expected)
+
 if __name__ == '__main__':
     unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyscard-2.0.8/test/test_PCSC.py` & `pyscard-2.0.9/test/test_PCSC.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/test/test_PCSCExceptions.py` & `pyscard-2.0.9/test/test_PCSCExceptions.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/test/test_SCardGetErrorMessage.py` & `pyscard-2.0.9/test/test_SCardGetErrorMessage.py`

 * *Files identical despite different names*

### Comparing `pyscard-2.0.8/test/test_util.py` & `pyscard-2.0.9/test/test_util.py`

 * *Files identical despite different names*

