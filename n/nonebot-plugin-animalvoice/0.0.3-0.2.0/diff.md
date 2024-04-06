# Comparing `tmp/nonebot_plugin_animalVoice-0.0.3.tar.gz` & `tmp/nonebot_plugin_animalvoice-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_animalVoice-0.0.3.tar", last modified: Thu Dec 29 09:41:55 2022, max compression
+gzip compressed data, was "nonebot_plugin_animalvoice-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_animalVoice-0.0.3.tar` & `nonebot_plugin_animalvoice-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-12-29 09:41:55.243255 nonebot_plugin_animalVoice-0.0.3/
--rw-rw-rw-   0        0        0    35182 2022-12-26 14:44:31.000000 nonebot_plugin_animalVoice-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2454 2022-12-29 09:41:55.241253 nonebot_plugin_animalVoice-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1961 2022-12-29 07:50:54.000000 nonebot_plugin_animalVoice-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-12-29 09:41:55.216607 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/
-drwxrwxrwx   0        0        0        0 2022-12-29 09:41:55.237245 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/AnimalVoice/
--rw-rw-rw-   0        0        0     2416 2022-12-29 03:41:42.000000 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/AnimalVoice/__init__.py
--rw-rw-rw-   0        0        0      281 2022-12-29 09:15:54.000000 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/AnimalVoice/converter.py
-drwxrwxrwx   0        0        0        0 2022-12-29 09:41:55.239235 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/Cheru/
--rw-rw-rw-   0        0        0     1245 2022-12-29 09:02:50.000000 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/Cheru/__init__.py
--rw-rw-rw-   0        0        0      209 2022-12-29 09:06:53.000000 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/__init__.py
--rw-rw-rw-   0        0        0     2589 2022-12-29 09:33:05.000000 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/animalvoice_main.py
--rw-rw-rw-   0        0        0     2655 2022-12-29 09:36:19.000000 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/cheru_main.py
-drwxrwxrwx   0        0        0        0 2022-12-29 09:41:55.232516 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice.egg-info/
--rw-rw-rw-   0        0        0     2454 2022-12-29 09:41:54.000000 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2022-12-29 09:41:55.000000 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-29 09:41:54.000000 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-12-29 09:41:54.000000 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2022-12-29 09:41:54.000000 nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-29 09:41:55.243255 nonebot_plugin_animalVoice-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1211 2022-12-29 09:10:48.000000 nonebot_plugin_animalVoice-0.0.3/setup.py
+-rw-r--r--   0        0        0    35823 2024-04-06 13:00:03.100114 nonebot_plugin_animalvoice-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1623 2024-04-06 13:42:17.990781 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/__init__.py
+-rw-r--r--   0        0        0     2658 2024-04-06 13:28:58.815316 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/AnimalVoice/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-06 13:28:58.777210 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/AnimalVoice/converter.py
+-rw-r--r--   0        0        0     2836 2024-04-06 13:35:17.555281 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/animalvoice_main.py
+-rw-r--r--   0        0        0     1247 2024-04-06 13:28:58.800659 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/Cheru/__init__.py
+-rw-r--r--   0        0        0     2786 2024-04-06 13:35:17.555281 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/cheru_main.py
+-rw-r--r--   0        0        0      452 2024-04-06 13:31:08.659327 nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/config.py
+-rw-r--r--   0        0        0      421 2024-04-06 13:57:03.661347 nonebot_plugin_animalvoice-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2525 2024-04-06 13:00:03.102760 nonebot_plugin_animalvoice-0.2.0/README.md
+-rw-r--r--   0        0        0     3261 1970-01-01 00:00:00.000000 nonebot_plugin_animalvoice-0.2.0/setup.py
+-rw-r--r--   0        0        0     3031 1970-01-01 00:00:00.000000 nonebot_plugin_animalvoice-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_animalVoice-0.0.3/LICENSE` & `nonebot_plugin_animalvoice-0.2.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,82 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
-  The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
 
   The licenses for most software and other practical works are designed
 to take away your freedom to share and change the works.  By contrast,
-our General Public Licenses are intended to guarantee your freedom to
+the GNU General Public License is intended to guarantee your freedom to
 share and change all versions of a program--to make sure it remains free
-software for all its users.
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
 
   When we speak of free software, we are referring to freedom, not
 price.  Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 them if you wish), that you receive source code or can get it if you
 want it, that you can change the software or use pieces of it in new
 free programs, and that you know you can do these things.
 
-  Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-  A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate.  Many developers of free software are heartened and
-encouraged by the resulting cooperation.  However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-  The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community.  It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server.  Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-  An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals.  This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing under
-this license.
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
 
   The precise terms and conditions for copying, distribution and
 modification follow.
 
                        TERMS AND CONDITIONS
 
   0. Definitions.
 
-  "This License" refers to version 3 of the GNU Affero General Public License.
+  "This License" refers to version 3 of the GNU General Public License.
 
   "Copyright" also means copyright-like laws that apply to other kinds of
 works, such as semiconductor masks.
 
   "The Program" refers to any copyrightable work licensed under this
 License.  Each licensee is addressed as "you".  "Licensees" and
 "recipients" may be individuals or organizations.
@@ -533,53 +545,43 @@
 covered work so as to satisfy simultaneously your obligations under this
 License and any other pertinent obligations, then as a consequence you may
 not convey it at all.  For example, if you agree to terms that obligate you
 to collect a royalty for further conveying from those to whom you convey
 the Program, the only way you could satisfy both those terms and this
 License would be to refrain entirely from conveying the Program.
 
-  13. Remote Network Interaction; Use with the GNU General Public License.
-
-  Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your version
-supports such interaction) an opportunity to receive the Corresponding
-Source of your version by providing access to the Corresponding Source
-from a network server at no charge, through some standard or customary
-means of facilitating copying of software.  This Corresponding Source
-shall include the Corresponding Source for any work covered by version 3
-of the GNU General Public License that is incorporated pursuant to the
-following paragraph.
+  13. Use with the GNU Affero General Public License.
 
   Notwithstanding any other provision of this License, you have
 permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
+under version 3 of the GNU Affero General Public License into a single
 combined work, and to convey the resulting work.  The terms of this
 License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
 
   14. Revised Versions of this License.
 
   The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time.  Such new versions
-will be similar in spirit to the present version, but may differ in detail to
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
 address new problems or concerns.
 
   Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU Affero General
+Program specifies that a certain numbered version of the GNU General
 Public License "or any later version" applies to it, you have the
 option of following the terms and conditions either of that numbered
 version or of any later version published by the Free Software
 Foundation.  If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
+GNU General Public License, you may choose any version ever published
 by the Free Software Foundation.
 
   If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
+versions of the GNU General Public License can be used, that proxy's
 public statement of acceptance of a version permanently authorizes you
 to choose that version for the Program.
 
   Later license versions may give you additional or different
 permissions.  However, no additional obligations are imposed on any
 author or copyright holder as a result of your choosing to follow a
 later version.
@@ -629,33 +631,44 @@
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     <one line to give the program's name and a brief idea of what it does.>
     Copyright (C) <year>  <name of author>
 
     This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published
-    by the Free Software Foundation, either version 3 of the License, or
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
+    GNU General Public License for more details.
 
-    You should have received a copy of the GNU Affero General Public License
+    You should have received a copy of the GNU General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source.  For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code.  There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
-<https://www.gnu.org/licenses/>.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `nonebot_plugin_animalVoice-0.0.3/PKG-INFO` & `nonebot_plugin_animalvoice-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot_plugin_animalVoice
-Version: 0.0.3
-Summary: _✨Nonebot兽语译者插件✨_
-Home-page: https://github.com/ANGJustinl/nonebot_plugin_animalVoice_main
-Author: ANGJustinl
-Author-email: angjustin@163.com
-Keywords: pip,nonebot2,nonebot,nonebot_plugin
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
   
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 
 
@@ -35,43 +20,62 @@
 <a href="https://www.python.org">
     <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
 </a>
 
 ---  
  </div> 
   
+## ✔ 使用例
+
+![3`$HP~HVN%SK(IV@2HO7X{M](https://user-images.githubusercontent.com/96008766/210118707-b00e90ff-ce8c-4fdb-bcd9-f3a18c2ebc50.png)
+
+![OYJ5N2~Z@XZ)B6FL %MEIKA](https://user-images.githubusercontent.com/96008766/210118729-8e8a6ff0-f911-4514-aac9-a87f714051e9.png)
+  
 ## 💿 安装
 
 ### 1. nb-cli安装（推荐）
-bot根目录下打开命令行，执行nb命令安装插件，插件配置会自动添加至配置文件  
+bot根目录下打开命令行，执行nb命令安装插件，插件配置会自动添加至配置文件 
+ 
 ```
-nb plugin install nonebot_plugin_face2cartoonpic
+nb plugin install nonebot_plugin_animalVoice
 ```
 
 ### 2. pip安装
+
 ```
-pip install nonebot_plugin_face2cartoonpic --upgrade
+pip install nonebot_plugin_animalVoice --upgrade
+
 ```  
+
 打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  
 ```nonebot.load_plugin('nonebot_plugin_animalVoice')```  
   
 或在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_animalVoice```即可  
-pyproject.toml配置例如：  
+pyproject.toml配置例如： 
+
 ``` 
+
 [tool.nonebot]
 plugin_dirs = ["src/plugins"]
 plugins = ["nonebot_plugin_animalVoice","xxxxx"]
+
 ```
-  
 
-```  
+
 ## 🎉 使用
 ### 指令表
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | [兽音加密]/[convert] | 否 | 群聊/私聊 | 发送需要加密的文字 |
 | [兽音解密]/[deconvert] | 否 | 群聊/私聊 | 发送需要解密的文字 |
+| [切噜一下]/[cherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |
+| [切噜～]/[decherulize] | 否 | 群聊/私聊 | 发送需要解密的文字 |
 
 
 **注意**
 
 默认情况下, 您应该在指令前加上命令前缀, 通常是 /
+
+
+### 🧡特别感谢 
+
+HoshinoBot: https://github.com/Ice-Cirno/HoshinoBot 提供了切噜切噜的算法
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_animalVoice Version: 0.0.3 Summary:
-_â¨Nonebotå½è¯­è¯èæä»¶â¨_ Home-page: https://github.com/ANGJustinl/
-nonebot_plugin_animalVoice_main Author: ANGJustinl Author-email:
-angjustin@163.com Keywords: pip,nonebot2,nonebot,nonebot_plugin Platform: any
-Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
-OS Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # nonebot_plugin_animalVoice _â¨Nonebotå½è¯­è¯èæä»¶â¨_ --- _[_l_i_c_e_n_s_e_]
                                _[_p_y_p_i_]_[_p_y_t_h_o_n_]---
-## ð¿ å®è£ ### 1. nb-cliå®è£ï¼æ¨èï¼
+## â ä½¿ç¨ä¾ ![3`$HP~HVN%SK(IV@2HO7X{M](https://user-
+images.githubusercontent.com/96008766/210118707-b00e90ff-ce8c-4fdb-bcd9-
+f3a18c2ebc50.png) ![OYJ5N2~Z@XZ)B6FL %MEIKA](https://user-
+images.githubusercontent.com/96008766/210118729-8e8a6ff0-f911-4514-aac9-
+a87f714051e9.png) ## ð¿ å®è£ ### 1. nb-cliå®è£ï¼æ¨èï¼
 botæ ¹ç®å½ä¸æå¼å½ä»¤è¡ï¼æ§è¡nbå½ä»¤å®è£æä»¶ï¼æä»¶éç½®ä¼èªå¨æ·»å è³éç½®æä»¶
-``` nb plugin install nonebot_plugin_face2cartoonpic ``` ### 2. pipå®è£ ```
-pip install nonebot_plugin_face2cartoonpic --upgrade ``` æå¼ nonebot2
-é¡¹ç®ç ```bot.py``` æä»¶, å¨å¶ä¸­åå¥ ```nonebot.load_plugin
+``` nb plugin install nonebot_plugin_animalVoice ``` ### 2. pipå®è£ ``` pip
+install nonebot_plugin_animalVoice --upgrade ``` æå¼ nonebot2 é¡¹ç®ç
+```bot.py``` æä»¶, å¨å¶ä¸­åå¥ ```nonebot.load_plugin
 ('nonebot_plugin_animalVoice')``` æå¨botè·¯å¾```pyproject.toml```ç```
 [tool.nonebot]```ç```plugins```ä¸­æ·»å ```nonebot_plugin_animalVoice```å³å¯
 pyproject.tomléç½®ä¾å¦ï¼ ``` [tool.nonebot] plugin_dirs = ["src/plugins"]
-plugins = ["nonebot_plugin_animalVoice","xxxxx"] ``` ``` ## ð ä½¿ç¨ ###
+plugins = ["nonebot_plugin_animalVoice","xxxxx"] ``` ## ð ä½¿ç¨ ###
 æä»¤è¡¨ | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:----:|:----:
 | | [å½é³å å¯]/[convert] | å¦ | ç¾¤è/ç§è |
 åééè¦å å¯çæå­ | | [å½é³è§£å¯]/[deconvert] | å¦ | ç¾¤è/
-ç§è | åééè¦è§£å¯çæå­ | **æ³¨æ** é»è®¤æåµä¸,
-æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼, éå¸¸æ¯ /
+ç§è | åééè¦è§£å¯çæå­ | | [ååä¸ä¸]/[cherulize] | å¦ |
+ç¾¤è/ç§è | åééè¦è§£å¯çæå­ | | [ååï½]/[decherulize] | å¦
+| ç¾¤è/ç§è | åééè¦è§£å¯çæå­ | **æ³¨æ** é»è®¤æåµä¸,
+æ¨åºè¯¥å¨æä»¤åå ä¸å½ä»¤åç¼, éå¸¸æ¯ / ### ð§¡ç¹å«æè°¢
+HoshinoBot: https://github.com/Ice-Cirno/HoshinoBot
+æä¾äºååååçç®æ³
```

### Comparing `nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/Cheru/__init__.py` & `nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/Cheru/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import re
 from itertools import zip_longest
 
-CHERU_SET = '切卟叮咧哔唎啪啰啵嘭噜噼巴拉蹦铃'
+CHERU_SET = "切卟叮咧哔唎啪啰啵嘭噜噼巴拉蹦铃"
 CHERU_DIC = {c: i for i, c in enumerate(CHERU_SET)}
-ENCODING = 'gb18030'
-rex_split = re.compile(r'\b', re.U)
-rex_word = re.compile(r'^\w+$', re.U)
-rex_cheru_word: re.Pattern = re.compile(rf'切[{CHERU_SET}]+', re.U)
+ENCODING = "gb18030"
+rex_split = re.compile(r"\b", re.U)
+rex_word = re.compile(r"^\w+$", re.U)
+rex_cheru_word: re.Pattern = re.compile(rf"切[{CHERU_SET}]+", re.U)
 
 
 def grouper(iterable, n, fillvalue=None):
     args = [iter(iterable)] * n
     return zip_longest(*args, fillvalue=fillvalue)
 
 
 def word2cheru(w: str) -> str:
-    c = ['切']
+    c = ["切"]
     for b in w.encode(ENCODING):
-        c.append(CHERU_SET[b & 0xf])
-        c.append(CHERU_SET[(b >> 4) & 0xf])
-    return ''.join(c)
+        c.append(CHERU_SET[b & 0xF])
+        c.append(CHERU_SET[(b >> 4) & 0xF])
+    return "".join(c)
 
 
 def cheru2word(c: str) -> str:
-    if not c[0] == '切' or len(c) < 2:
+    if not c[0] == "切" or len(c) < 2:
         return c
     b = []
-    for b1, b2 in grouper(c[1:], 2, '切'):
+    for b1, b2 in grouper(c[1:], 2, "切"):
         x = CHERU_DIC.get(b2, 0)
         x = x << 4 | CHERU_DIC.get(b1, 0)
         b.append(x)
-    return bytes(b).decode(ENCODING, 'replace')
+    return bytes(b).decode(ENCODING, "replace")
 
 
 def str2cheru(s: str) -> str:
     c = []
     for w in rex_split.split(s):
         if rex_word.search(w):
             w = word2cheru(w)
         c.append(w)
-    return ''.join(c)
+    return "".join(c)
 
 
 def cheru2str(c: str) -> str:
-    return rex_cheru_word.sub(lambda w: cheru2word(w.group()), c)
+    return rex_cheru_word.sub(lambda w: cheru2word(w.group()), c)
```

### Comparing `nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/animalvoice_main.py` & `nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/animalvoice_main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,97 @@
 from nonebot import on_command
-from nonebot.params import CommandArg,Arg
+from nonebot.params import Arg
 from nonebot.adapters.onebot.v11 import MessageEvent, Message, Bot
 from nonebot.typing import T_State
 
-from .AnimalVoice.converter import msg_convert,msg_deconvert
+from .config import Config
+from .AnimalVoice.converter import msg_convert, msg_deconvert
+
+convert = on_command(
+    Config.customize_cmd_animalconvert,
+    aliases={"animalvoice", "convert"},
+    priority=5,
+    block=True,
+)
+deconvert = on_command(
+    Config.customize_cmd_animaldeconvert,
+    aliases={"deanimalvoice", "deconvert"},
+    priority=5,
+    block=True,
+)
+if_at_sender = Config.at_sender
 
-convert = on_command('兽音加密',aliases={'animalvoice','convert'}, priority=5, block=True)
-deconvert = on_command('兽音解密',aliases={'deanimalvoice','deconvert'}, priority=5, block=True)
 
 @convert.handle()
-async def _(state: T_State): 
+async def _(state: T_State):
     return
-#这里用got是因为必须单独消息发送否则容易乱
+
+
+# 这里用got是因为必须单独消息发送否则容易乱
 @convert.got("msg", prompt="请发送加密前文字")
-async def get_image(state: T_State,msgs: Message = Arg()):
+async def get_image(state: T_State, msgs: Message = Arg()):
     msg_input = msgs
     if not str:
-        await convert.send("不是文字啊")
+        await convert.send("不是文字啊", at_sender=if_at_sender)
         msg_input = str(msg_input)
     state["msg"] = msg_input
-    
-@convert.handle()  
-async def _(bot:Bot,state: T_State,event:MessageEvent):  
+
+
+@convert.handle()
+async def _(bot: Bot, state: T_State, event: MessageEvent):
     msg_input = str(state["msg"][0])
     try:
         msg = msg_convert(msg_input)
     except Exception as e:
-        await convert.finish("寄，加密失败了，报错为{}".format(e), reply_message=True) 
-    
+        await convert.finish("寄，加密失败了，报错为{}".format(e), reply_message=True)
+
     msgs = []
-    msgs.append({
-		        "type": "node",
-		        "data": {
-			        "name": "昂昂兽音译者bot",
-			        "uin": bot.self_id,
-			        "content": "加密结果\n{}".format(msg)
-		    }
+    msgs.append(
+        {
+            "type": "node",
+            "data": {
+                "name": "兽音译者bot",
+                "uin": bot.self_id,
+                "content": "加密结果\n{}".format(msg),
+            },
         }
     )
-    await bot.call_api('send_group_forward_msg', group_id=event.group_id, messages=msgs)
+    await bot.call_api("send_group_forward_msg", group_id=event.group_id, messages=msgs)
     await convert.finish()
-    
-    
+
+
 @deconvert.handle()
-async def _(state: T_State): 
+async def _(state: T_State):
     return
-#这里用got是因为必须单独消息发送否则容易乱
+
+
+# 这里用got是因为必须单独消息发送否则容易乱
 @deconvert.got("msg", prompt="请发送需要解密的文字")
-async def get_image(state: T_State,msgs: Message = Arg()):
+async def get_image(state: T_State, msgs: Message = Arg()):
     msg_input = msgs
     if not str:
-        await deconvert.send("不是文字啊")
+        await deconvert.send("不是文字啊", at_sender=if_at_sender)
         msg_input = str(msg_input)
     state["msg"] = msg_input
-    
-@deconvert.handle()  
-async def _(bot:Bot,state: T_State,event:MessageEvent):  
+
+
+@deconvert.handle()
+async def _(bot: Bot, state: T_State, event: MessageEvent):
     msg_input = str(state["msg"][0])
     try:
         msg = msg_deconvert(msg_input)
     except Exception as e:
-        await deconvert.finish("寄，解密失败了，报错为{}".format(e), reply_message=True) 
-    
+        await deconvert.finish("寄，解密失败了，报错为{}".format(e), reply_message=True)
+
     msgs = []
-    msgs.append({
-		        "type": "node",
-		        "data": {
-			        "name": "昂昂兽音译者bot",
-			        "uin": bot.self_id,
-			        "content": "解密结果\n{}".format(msg)
-		    }
+    msgs.append(
+        {
+            "type": "node",
+            "data": {
+                "name": "兽音译者bot",
+                "uin": bot.self_id,
+                "content": "解密结果\n{}".format(msg),
+            },
         }
     )
-    await bot.call_api('send_group_forward_msg', group_id=event.group_id, messages=msgs)
-    await deconvert.finish()
+    await bot.call_api("send_group_forward_msg", group_id=event.group_id, messages=msgs)
+    await deconvert.finish()
```

### Comparing `nonebot_plugin_animalVoice-0.0.3/nonebot_plugin_animalVoice/cheru_main.py` & `nonebot_plugin_animalvoice-0.2.0/nonebot_plugin_animalVoice/cheru_main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,87 @@
 from nonebot import on_command
-from nonebot.params import CommandArg,Arg
+from nonebot.params import Arg
 from nonebot.adapters.onebot.v11 import MessageEvent, Message, Bot
 from nonebot.typing import T_State
 
-from .Cheru import cheru2str,str2cheru
+from .config import Config
+from .Cheru import cheru2str, str2cheru
 
-cherulizing = on_command('切噜一下',aliases={'cherulize'}, priority=5, block=True)
-decherulizing = on_command('切噜～',aliases={'decherulize'}, priority=5, block=True)
+cherulizing = on_command(
+    Config.customize_cmd_cherulizing, aliases={"cherulize"}, priority=5, block=True
+)
+decherulizing = on_command(
+    Config.customize_cmd_decherulizing, aliases={"decherulize"}, priority=5, block=True
+)
+if_at_sender = Config.at_sender
 
 
 @cherulizing.handle()
-async def _(): 
+async def _():
     return
-#这里用got是因为必须单独消息发送否则容易乱
+
+
+# 这里用got是因为必须单独消息发送否则容易乱
 @cherulizing.got("msg", prompt="切噜什么切噜～♪")
-async def get_image(bot:Bot,state: T_State,msgs: Message = Arg()):
+async def get_image(bot: Bot, state: T_State, msgs: Message = Arg()):
     msg_input = msgs
     if len(msg_input) > 500:
-        await bot.send('切、切噜太长切不动勒切噜噜...', at_sender=True)
+        await bot.send("切、切噜太长切不动勒切噜噜...", at_sender=if_at_sender)
         return
     state["msg"] = msg_input
-    
-@cherulizing.handle()  
-async def _(bot:Bot,state: T_State,event:MessageEvent):  
+
+
+@cherulizing.handle()
+async def _(bot: Bot, state: T_State, event: MessageEvent):
     msg_input = str(state["msg"][0])
     try:
         msg = str2cheru(msg_input)
     except Exception as e:
-        await cherulizing.finish("切、切噜报错切不动勒切噜噜{}".format(e), reply_message=True) 
-    
+        await cherulizing.finish("切、切噜报错切不动勒切噜噜{}".format(e), reply_message=True)
+
     msgs = []
-    msgs.append({
-		        "type": "node",
-		        "data": {
-			        "name": "昂昂切噜bot",
-			        "uin": bot.self_id,
-			        "content": '切噜～♪\n{}'.format(msg)
-		    }
+    msgs.append(
+        {
+            "type": "node",
+            "data": {
+                "name": "风间千爱瑠",
+                "uin": bot.self_id,
+                "content": "切噜～♪\n{}".format(msg),
+            },
         }
     )
-    await bot.call_api('send_group_forward_msg', group_id=event.group_id, messages=msgs)
+    await bot.call_api("send_group_forward_msg", group_id=event.group_id, messages=msgs)
     await cherulizing.finish()
 
-    
+
 @decherulizing.handle()
-async def _(state: T_State): 
+async def _(state: T_State):
     return
-#这里用got是因为必须单独消息发送否则容易乱
+
+
+# 这里用got是因为必须单独消息发送否则容易乱
 @decherulizing.got("msg", prompt="请发送需要解密的文字")
-async def get_image(bot:Bot,state: T_State,msgs: Message = Arg()):
+async def get_image(bot: Bot, state: T_State, msgs: Message = Arg()):
     msg_input = msgs
     if len(msg_input) > 1501:
-        await bot.send('切、切噜太长切不动勒切噜噜...', at_sender=True)
+        await bot.send("切、切噜太长切不动勒切噜噜...", at_sender=if_at_sender)
         return
     state["msg"] = msg_input
-    
-@decherulizing.handle()  
-async def _(bot:Bot,state: T_State,event:MessageEvent):  
+
+
+@decherulizing.handle()
+async def _(bot: Bot, state: T_State, event: MessageEvent):
     msg_input = str(state["msg"][0])
     try:
-        msg = '你的的切噜噜是：\n{}'.format(cheru2str(msg_input))
+        msg = "你的的切噜噜是：\n{}".format(cheru2str(msg_input))
     except Exception as e:
-        await decherulizing.finish("切、切噜报错切不动勒切噜噜{}".format(e), reply_message=True) 
-    
+        await decherulizing.finish("切、切噜报错切不动勒切噜噜{}".format(e), reply_message=True)
+
     msgs = []
-    msgs.append({
-		        "type": "node",
-		        "data": {
-			        "name": "昂昂切噜bot",
-			        "uin": bot.self_id,
-			        "content": msg
-		    }
+    msgs.append(
+        {
+            "type": "node",
+            "data": {"name": "风间千爱瑠", "uin": bot.self_id, "content": msg},
         }
     )
-    await bot.call_api('send_group_forward_msg', group_id=event.group_id, messages=msgs)
-    await decherulizing.finish()
+    await bot.call_api("send_group_forward_msg", group_id=event.group_id, messages=msgs)
+    await decherulizing.finish()
```

