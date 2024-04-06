# Comparing `tmp/lamda-7.57.tar.gz` & `tmp/lamda-7.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lamda-7.57.tar", last modified: Sun Mar 31 15:21:29 2024, max compression
+gzip compressed data, was "dist/lamda-7.60.tar", last modified: Sat Apr  6 05:46:10 2024, max compression
```

## Comparing `lamda-7.57.tar` & `lamda-7.60.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-03-31 15:21:29.843830 lamda-7.57/
--rw-r--r--   0 whoami    (4096) whoami    (4096)      949 2024-03-31 15:21:29.843830 lamda-7.57/PKG-INFO
--rw-r--r--   0 whoami    (4096) whoami    (4096)     4229 2024-03-23 02:16:23.000000 lamda-7.57/README.md
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-03-31 15:21:29.839830 lamda-7.57/lamda/
--rw-r--r--   0 whoami    (4096) whoami    (4096)      205 2024-03-31 15:12:46.000000 lamda-7.57/lamda/__init__.py
--rw-r--r--   0 whoami    (4096) whoami    (4096)      894 2023-12-11 03:08:30.000000 lamda-7.57/lamda/bcast.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    74136 2024-03-31 05:08:50.000000 lamda-7.57/lamda/client.py
--rw-r--r--   0 whoami    (4096) whoami    (4096)     3167 2023-03-16 03:06:14.000000 lamda-7.57/lamda/const.py
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1603 2023-12-11 03:24:23.000000 lamda-7.57/lamda/exceptions.py
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-03-31 15:21:29.839830 lamda-7.57/lamda/google/
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-03-31 15:21:29.843830 lamda-7.57/lamda/google/protobuf/
--rw-r--r--   0 whoami    (4096) whoami    (4096)     5916 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/any.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     7734 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/api.proto
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-03-31 15:21:29.843830 lamda-7.57/lamda/google/protobuf/compiler/
--rw-r--r--   0 whoami    (4096) whoami    (4096)     8754 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/compiler/plugin.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    37969 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/descriptor.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     4895 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/duration.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2429 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/empty.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     8185 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/field_mask.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2341 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/source_context.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     3778 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/struct.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     6459 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/timestamp.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     6126 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/type.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     4042 2022-10-31 08:21:43.000000 lamda-7.57/lamda/google/protobuf/wrappers.proto
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-03-31 15:21:29.843830 lamda-7.57/lamda/rpc/
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2393 2024-03-17 15:58:16.000000 lamda-7.57/lamda/rpc/application.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      430 2024-01-06 00:45:44.000000 lamda-7.57/lamda/rpc/debug.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      710 2024-01-06 00:45:39.000000 lamda-7.57/lamda/rpc/file.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      391 2024-01-10 15:26:13.000000 lamda-7.57/lamda/rpc/policy.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2672 2024-01-13 06:01:07.000000 lamda-7.57/lamda/rpc/proxy.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    12143 2024-03-29 03:25:45.000000 lamda-7.57/lamda/rpc/services.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      478 2024-01-10 15:26:13.000000 lamda-7.57/lamda/rpc/settings.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      609 2024-01-10 15:26:13.000000 lamda-7.57/lamda/rpc/shell.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     2046 2024-01-10 15:26:13.000000 lamda-7.57/lamda/rpc/status.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      393 2023-12-11 03:09:19.000000 lamda-7.57/lamda/rpc/storage.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)      434 2024-01-10 15:26:13.000000 lamda-7.57/lamda/rpc/types.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)    19176 2024-03-31 05:08:50.000000 lamda-7.57/lamda/rpc/uiautomator.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1299 2024-01-10 15:26:13.000000 lamda-7.57/lamda/rpc/util.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1935 2024-01-10 15:26:13.000000 lamda-7.57/lamda/rpc/wifi.proto
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1007 2023-12-11 03:11:52.000000 lamda-7.57/lamda/types.py
-drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-03-31 15:21:29.843830 lamda-7.57/lamda.egg-info/
--rw-r--r--   0 whoami    (4096) whoami    (4096)      949 2024-03-31 15:21:29.000000 lamda-7.57/lamda.egg-info/PKG-INFO
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1062 2024-03-31 15:21:29.000000 lamda-7.57/lamda.egg-info/SOURCES.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)        1 2024-03-31 15:21:29.000000 lamda-7.57/lamda.egg-info/dependency_links.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)        1 2024-03-31 15:21:29.000000 lamda-7.57/lamda.egg-info/not-zip-safe
--rw-r--r--   0 whoami    (4096) whoami    (4096)      229 2024-03-31 15:21:29.000000 lamda-7.57/lamda.egg-info/requires.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)        6 2024-03-31 15:21:29.000000 lamda-7.57/lamda.egg-info/top_level.txt
--rw-r--r--   0 whoami    (4096) whoami    (4096)       38 2024-03-31 15:21:29.843830 lamda-7.57/setup.cfg
--rw-r--r--   0 whoami    (4096) whoami    (4096)     1635 2024-03-05 09:30:03.000000 lamda-7.57/setup.py
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.540284 lamda-7.60/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      949 2024-04-06 05:46:10.540284 lamda-7.60/PKG-INFO
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     4341 2024-04-06 02:54:54.000000 lamda-7.60/README.md
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.536284 lamda-7.60/lamda/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      205 2024-04-06 05:37:37.000000 lamda-7.60/lamda/__init__.py
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      894 2023-12-11 03:08:30.000000 lamda-7.60/lamda/bcast.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)    74749 2024-04-04 10:11:38.000000 lamda-7.60/lamda/client.py
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     3167 2023-03-16 03:06:14.000000 lamda-7.60/lamda/const.py
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1603 2023-12-11 03:24:23.000000 lamda-7.60/lamda/exceptions.py
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.536284 lamda-7.60/lamda/google/
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.540284 lamda-7.60/lamda/google/protobuf/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     5916 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/any.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     7734 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/api.proto
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.540284 lamda-7.60/lamda/google/protobuf/compiler/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     8754 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/compiler/plugin.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)    37969 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/descriptor.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     4895 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/duration.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     2429 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/empty.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     8185 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/field_mask.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     2341 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/source_context.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     3778 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/struct.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     6459 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/timestamp.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     6126 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/type.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     4042 2022-10-31 08:21:43.000000 lamda-7.60/lamda/google/protobuf/wrappers.proto
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.540284 lamda-7.60/lamda/rpc/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     2393 2024-03-17 15:58:16.000000 lamda-7.60/lamda/rpc/application.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      430 2024-01-06 00:45:44.000000 lamda-7.60/lamda/rpc/debug.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      710 2024-01-06 00:45:39.000000 lamda-7.60/lamda/rpc/file.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      391 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/policy.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     2672 2024-01-13 06:01:07.000000 lamda-7.60/lamda/rpc/proxy.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)    12143 2024-03-29 03:25:45.000000 lamda-7.60/lamda/rpc/services.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      478 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/settings.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      609 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/shell.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     2046 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/status.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      393 2023-12-11 03:09:19.000000 lamda-7.60/lamda/rpc/storage.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      434 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/types.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)    19642 2024-04-04 09:53:04.000000 lamda-7.60/lamda/rpc/uiautomator.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1299 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/util.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1935 2024-01-10 15:26:13.000000 lamda-7.60/lamda/rpc/wifi.proto
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1007 2023-12-11 03:11:52.000000 lamda-7.60/lamda/types.py
+drwxr-xr-x   0 whoami    (4096) whoami    (4096)        0 2024-04-06 05:46:10.540284 lamda-7.60/lamda.egg-info/
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      949 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/PKG-INFO
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1062 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/SOURCES.txt
+-rw-r--r--   0 whoami    (4096) whoami    (4096)        1 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/dependency_links.txt
+-rw-r--r--   0 whoami    (4096) whoami    (4096)        1 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/not-zip-safe
+-rw-r--r--   0 whoami    (4096) whoami    (4096)      229 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/requires.txt
+-rw-r--r--   0 whoami    (4096) whoami    (4096)        6 2024-04-06 05:46:10.000000 lamda-7.60/lamda.egg-info/top_level.txt
+-rw-r--r--   0 whoami    (4096) whoami    (4096)       38 2024-04-06 05:46:10.540284 lamda-7.60/setup.cfg
+-rw-r--r--   0 whoami    (4096) whoami    (4096)     1635 2024-03-05 09:30:03.000000 lamda-7.60/setup.py
```

### Comparing `lamda-7.57/PKG-INFO` & `lamda-7.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamda
-Version: 7.57
+Version: 7.60
 Summary: Android reverse engineering & automation framework
 Home-page: https://github.com/rev1si0n/lamda
 Author: rev1si0n
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `lamda-7.57/README.md` & `lamda-7.60/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 <p align="center"><a href="https://github.com/rev1si0n/lamda/wiki">使用文档</a> | <a href="https://t.me/lamda_dev">TELEGRAM</a> | <a href="https://lamda.run/join/qq">QQ 群组</a> | <a href="https://github.com/rev1si0n/lamda/blob/HEAD/CHANGELOG.txt">更新历史</a></p>
 
 LAMDA 是一个用于逆向及自动化的辅助框架，设计为减少安全分析以及应用测试人员的时间及琐碎问题，以编程化的接口替代大量手动操作，它并不是一个单一功能的框架，他是 Appium、uiautomator 的超集同时具备逆向领域的能力。为了让你大概了解它的用处：你是否会在手机上安装各类代理、插件或者点来点去的设置来完成你的工作？你是否要在异地操作远在千里之外的手机？你是否有编程控制手机的需求？是否还在某些云手机厂商那里购买昂贵的**IP切换**、**远程ADB调试**、**RPA自动化**甚至连 **logcat 日志**都要付费的服务？如果有，那么对了，只需一个 LAMDA 即可解决这些问题。并且，LAMDA 更注重**分布式**，事实上，你可以在一台公网服务器上管理散布在世界各地各种网络环境中的设备。当然，LAMDA 可以做到的不止于此。
 
 <p align="center">
 <img src="image/wx.png" alt="公众号" width="234">
 </p>
-<p align="center"><small>关注公众号查看视频教程以及更多使用方法</small><br><small><b>知识应该是共享的，我们不会要求你为相关知识付费</b></small><br><small>文字版文档请查看<a href="https://github.com/rev1si0n/lamda/wiki">使用文档</a></small></p>
+<p align="center"><small>关注公众号查看视频教程以及更多使用方法</small><br><small><b>知识应该是共享的，我们不会要求你为相关知识付费</b></small><br><br><small><a href="https://space.bilibili.com/1964784386/video">BILIBILI 同步发布</a></small><br><small>文字版文档请查看<a href="https://github.com/rev1si0n/lamda/wiki">使用文档</a></small></small>
+</p>
+
 
 经过超 500 台设备的稳定生产环境考验，具有近乎商业级软件的质量和稳定性，仅需 root 权限即可正常运行。具备 ARM/X86 全架构，安卓 6.0-14 的广泛兼容性，支持模拟器、真机、云手机、 WSA（Windows Subsystem for Android™️）、无头开发板以及 Redroid。提供大量可编程接口，支持界面布局检视、获取/重放系统中最近的 Activity、唤起应用的 Activity 等功能。除此之外，它支持大文件上传下载，远程桌面，以及UI自动化编程接口，点击、截图、获取界面元素、执行 shell 命令、设备状态、资源读取、系统配置、属性读写、一键中间人等，可通过 SSH 或内置 ADB 登录设备终端。具备 socks5、OpenVPN 代理并可通过接口轻松设置根证书，实现中间人攻击，以及 Frida、IDA 等工具等等，同时支持定时任务、Magisk开机自启动，你可以在任何地方通过网络连接运行着 LAMDA 设备。
 
 ![动图演示](image/demo.gif)
 
 ## 一键中间人流量分析
```

#### html2text {}

```diff
@@ -15,14 +15,16 @@
 æ¥å¿**é½è¦ä»è´¹çæå¡ï¼å¦ææï¼é£ä¹å¯¹äºï¼åªéä¸ä¸ª LAMDA
 å³å¯è§£å³è¿äºé®é¢ãå¹¶ä¸ï¼LAMDA
 æ´æ³¨é**åå¸å¼**ï¼äºå®ä¸ï¼ä½ å¯ä»¥å¨ä¸å°å¬ç½æå¡å¨ä¸ç®¡çæ£å¸å¨ä¸çåå°åç§ç½ç»ç¯å¢ä¸­çè®¾å¤ãå½ç¶ï¼LAMDA
 å¯ä»¥åå°çä¸æ­¢äºæ­¤ã
                                   [å¬ä¼å·]
            å³æ³¨å¬ä¼å·æ¥çè§é¢æç¨ä»¥åæ´å¤ä½¿ç¨æ¹æ³
      ?ç??¥?è?¯??å?º??è?¯?¥?æ??¯?å??±?ä?º?«?ç???ï?¼??æ???ä?»?¬?ä?¸??ä?¼??è?¦??æ?±??ä?½? ?ä?¸?º?ç??¸?å??³?ç??¥?è?¯??ä?»??è?´?¹
+
+                             _B_I_L_I_B_I_L_I_ _å___æ_­_¥_å___å_¸_
                      æå­çææ¡£è¯·æ¥ç_ä_½_¿_ç__¨_æ___æ_¡_£
 ç»è¿è¶ 500
 å°è®¾å¤çç¨³å®çäº§ç¯å¢èéªï¼å·æè¿ä¹åä¸çº§è½¯ä»¶çè´¨éåç¨³å®æ§ï¼ä»é
 root æéå³å¯æ­£å¸¸è¿è¡ãå·å¤ ARM/X86 å¨æ¶æï¼å®å 6.0-14
 çå¹¿æ³å¼å®¹æ§ï¼æ¯ææ¨¡æå¨ãçæºãäºææºã WSAï¼Windows
 Subsystem for Androidâ¢ï¸ï¼ãæ å¤´å¼åæ¿ä»¥å
 Redroidãæä¾å¤§éå¯ç¼ç¨æ¥å£ï¼æ¯æçé¢å¸å±æ£è§ãè·å/
```

### Comparing `lamda-7.57/lamda/bcast.proto` & `lamda-7.60/lamda/bcast.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/client.py` & `lamda-7.60/lamda/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,16 @@
                 "MetaKeyCode",
                 "MetaKeyCodes",
                 "BaseCryptor",
                 "FernetCryptor",
                 "OpenVPNAuth",
                 "OpenVPNEncryption",
                 "OpenVPNKeyDirection",
+                "FindImageMethod",
+                "FindImageArea",
                 "ToastDuration",
                 "OpenVPNCipher",
                 "OpenVPNProto",
                 "Orientation",
                 "OpenVPNProfile",
                 "GproxyProfile",
                 "Selector",
@@ -226,27 +228,27 @@
 TouchDown.shiftY = touchMoveShiftY
 
 TouchAction.type = property(touchActionType)
 TouchAction.action = property(touchActionRealAction)
 
 TouchSequence.load = classmethod(touchSequenceLoad)
 TouchSequence.save = touchSequenceSave
-
 TouchSequence.appendAction = touchSequenceAppendAction
 TouchSequence.appendDown = touchSequenceAppendDown
 TouchSequence.appendWait = touchSequenceAppendWait
 TouchSequence.appendUp = touchSequenceAppendUp
 
 TouchSequence.__getitem__ = touchSequenceIndexer
 TouchSequence.__iter__ = touchSequenceIter
 
 Bound.width = property(width)
 Bound.height = property(height)
 
 FindImageMethod = protos.FindImageMethod
+FindImageArea = protos.FindImageArea
 
 Bound.center = center
 Bound.corner = corner
 
 
 def load_proto(name):
     """ 载入包下面的相关 proto 文件 """
@@ -851,24 +853,34 @@
         return r.value
     def get_clipboard(self):
         """
         获取剪切板文字（小于 Android10）
         """
         r = self.stub.getClipboard(protos.Empty())
         return r.value
-    def find_similar_image(self, data, threshold=0,
-                           max_distance=0, bound=None,
-                           method=FindImageMethod.FI_TEMPLATE):
+    def _set_target_Area(self, req, area):
+        req.area = area
+    def _set_target_Bound(self, req, bound):
+        req.bound.CopyFrom(bound)
+    def find_similar_image(self, data, threshold=0.0, distance=250,
+                           scale=1.0, area=FindImageArea.FIA_WHOLE_SCREEN,
+                           method=FindImageMethod.FIM_TEMPLATE):
         """
         根据提供的目标图片从屏幕中获取相似图片位置
         """
-        req = protos.FindImageRequest(bound=bound)
+        req = protos.FindImageRequest()
+        checkArgumentTyp(area, (Bound, int))
+        name = getattr(getattr(area, "DESCRIPTOR", None),
+                                         "name", "Area")
+        func = "_set_target_{}".format(name)
+        getattr(self, func)(req, area)
         req.method = method
-        req.max_distance = max_distance
+        req.distance = distance
         req.threshold = threshold
+        req.scale = scale
         req.partial = data
         r = self.stub.findSimilarImage(req)
         return r.bounds
     def freeze_rotation(self, freeze=True):
         """
         锁定屏幕旋转
         """
@@ -2033,19 +2045,20 @@
         return self.stub("UiAutomator").screenshot(quality, bound=bound)
     def dump_window_hierarchy(self, compressed=False):
         return self.stub("UiAutomator").dump_window_hierarchy(compressed=compressed)
     def wait_for_idle(self, timeout):
         return self.stub("UiAutomator").wait_for_idle(timeout)
     def get_last_toast(self):
         return self.stub("UiAutomator").get_last_toast()
-    def find_similar_image(self, data, threshold=0,
-                                max_distance=0, bound=None,
-                                method=FindImageMethod.FI_TEMPLATE):
+    def find_similar_image(self, data, threshold=0.0, distance=250,
+                                scale=1.0, area=FindImageArea.FIA_WHOLE_SCREEN,
+                                method=FindImageMethod.FIM_TEMPLATE):
         return self.stub("UiAutomator").find_similar_image(data, threshold=threshold,
-                                max_distance=max_distance, bound=bound, method=method)
+                                distance=distance, scale=scale,
+                                area=area, method=method)
     # watcher
     def remove_all_watchers(self):
         return self.stub("UiAutomator").remove_all_watchers()
     def set_watcher_loop_enabled(self, enabled):
         return self.stub("UiAutomator").set_watcher_loop_enabled(enabled)
     def get_watcher_loop_enabled(self):
         return self.stub("UiAutomator").get_watcher_loop_enabled()
@@ -2113,11 +2126,10 @@
     parser.add_argument("-port", type=int, default=port,
                                    help="service port")
     parser.add_argument("-cert", type=str, default=crt,
                                    help="ssl cert")
     args = parser.parse_args()
 
     readline.parse_and_bind("tab: complete")
-
     d = Device(args.device, port=args.port,
-                    certificate=args.cert)
+                        certificate=args.cert)
     code.interact(local=globals())
```

### Comparing `lamda-7.57/lamda/const.py` & `lamda-7.60/lamda/const.py`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/exceptions.py` & `lamda-7.60/lamda/exceptions.py`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/any.proto` & `lamda-7.60/lamda/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/api.proto` & `lamda-7.60/lamda/google/protobuf/api.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/compiler/plugin.proto` & `lamda-7.60/lamda/google/protobuf/compiler/plugin.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/descriptor.proto` & `lamda-7.60/lamda/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/duration.proto` & `lamda-7.60/lamda/google/protobuf/duration.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/empty.proto` & `lamda-7.60/lamda/google/protobuf/empty.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/field_mask.proto` & `lamda-7.60/lamda/google/protobuf/field_mask.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/source_context.proto` & `lamda-7.60/lamda/google/protobuf/source_context.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/struct.proto` & `lamda-7.60/lamda/google/protobuf/struct.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/timestamp.proto` & `lamda-7.60/lamda/google/protobuf/timestamp.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/type.proto` & `lamda-7.60/lamda/google/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/google/protobuf/wrappers.proto` & `lamda-7.60/lamda/google/protobuf/wrappers.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/rpc/application.proto` & `lamda-7.60/lamda/rpc/application.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/rpc/file.proto` & `lamda-7.60/lamda/rpc/file.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/rpc/proxy.proto` & `lamda-7.60/lamda/rpc/proxy.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/rpc/services.proto` & `lamda-7.60/lamda/rpc/services.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/rpc/shell.proto` & `lamda-7.60/lamda/rpc/shell.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/rpc/status.proto` & `lamda-7.60/lamda/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/rpc/uiautomator.proto` & `lamda-7.60/lamda/rpc/uiautomator.proto`

 * *Files 2% similar despite different names*

```diff
@@ -552,22 +552,38 @@
         oneof _target {
                 Selector target = 3;
                 Key key = 4;
         }
 }
 
 enum FindImageMethod {
-        FI_TEMPLATE             = 0;
-        FI_FEATURE_POINT        = 1;
+        FIM_TEMPLATE            = 0;
+        FIM_FEATURE             = 1;
+}
+
+enum FindImageArea {
+        FIA_WHOLE_SCREEN        = 0;
+        FIA_LEFT                = 1;
+        FIA_TOP_LEFT            = 2;
+        FIA_TOP                 = 3;
+        FIA_TOP_RIGHT           = 4;
+        FIA_RIGHT               = 5;
+        FIA_BOTTOM_RIGHT        = 6;
+        FIA_BOTTOM              = 7;
+        FIA_BOTTOM_LEFT         = 8;
 }
 
 message FindImageRequest {
-        FindImageMethod method  = 1;
-        Bound bound             = 2;
-        bytes partial           = 3;
-        uint32 max_distance     = 4;
-        float threshold         = 5;
+        bytes partial           = 1;
+        FindImageMethod method  = 2;
+        oneof _area {
+                FindImageArea area = 3;
+                Bound bound     = 4;
+        }
+        uint32 distance         = 5;
+        float threshold         = 6;
+        float scale             = 7;
 }
 
 message FindImageResponse {
         repeated Bound bounds = 1;
 }
```

### Comparing `lamda-7.57/lamda/rpc/util.proto` & `lamda-7.60/lamda/rpc/util.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/rpc/wifi.proto` & `lamda-7.60/lamda/rpc/wifi.proto`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda/types.py` & `lamda-7.60/lamda/types.py`

 * *Files identical despite different names*

### Comparing `lamda-7.57/lamda.egg-info/PKG-INFO` & `lamda-7.60/lamda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamda
-Version: 7.57
+Version: 7.60
 Summary: Android reverse engineering & automation framework
 Home-page: https://github.com/rev1si0n/lamda
 Author: rev1si0n
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `lamda-7.57/lamda.egg-info/SOURCES.txt` & `lamda-7.60/lamda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lamda-7.57/setup.py` & `lamda-7.60/setup.py`

 * *Files identical despite different names*

