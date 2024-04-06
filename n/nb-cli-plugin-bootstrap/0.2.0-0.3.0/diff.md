# Comparing `tmp/nb_cli_plugin_bootstrap-0.2.0.tar.gz` & `tmp/nb_cli_plugin_bootstrap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_cli_plugin_bootstrap-0.2.0.tar", last modified: Tue Mar  5 15:57:46 2024, max compression
+gzip compressed data, was "nb_cli_plugin_bootstrap-0.3.0.tar", last modified: Sat Apr  6 16:23:40 2024, max compression
```

## Comparing `nb_cli_plugin_bootstrap-0.2.0.tar` & `nb_cli_plugin_bootstrap-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0     1069 2024-03-05 15:57:30.202974 nb_cli_plugin_bootstrap-0.2.0/LICENSE
--rw-r--r--   0        0        0     3597 2024-03-05 15:57:30.202974 nb_cli_plugin_bootstrap-0.2.0/README.md
--rw-r--r--   0        0        0       22 2024-03-05 15:57:30.202974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 15:57:30.202974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/handlers/__init__.py
--rw-r--r--   0        0        0    16654 2024-03-05 15:57:30.202974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/handlers/bootstrap.py
--rw-r--r--   0        0        0     6199 2024-03-05 15:57:30.202974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/handlers/update_project.py
--rw-r--r--   0        0        0     1029 2024-03-05 15:57:30.202974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/plugin.py
--rw-r--r--   0        0        0      722 2024-03-05 15:57:30.202974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/cookiecutter.json
--rw-r--r--   0        0        0      683 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/hooks/post_gen_project.py
--rw-r--r--   0        0        0      285 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      117 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/!run.sh
--rw-r--r--   0        0        0       71 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/!update-project.sh
--rw-r--r--   0        0        0      105 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/#启动.bat
--rw-r--r--   0        0        0       59 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/#更新所有插件.bat
--rw-r--r--   0        0        0       36 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/#进入虚拟环境.bat
--rw-r--r--   0        0        0     3199 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/.env.prod
--rw-r--r--   0        0        0     1563 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/bot.py
--rw-r--r--   0        0        0     1077 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/pyproject.toml
--rw-r--r--   0        0        0      613 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/src/plugins/{{cookiecutter.computed.ping_plugin_name}}.py
--rw-r--r--   0        0        0     4037 2024-03-05 15:57:30.206974 nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/utils.py
--rw-r--r--   0        0        0      713 2024-03-05 15:57:46.535041 nb_cli_plugin_bootstrap-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4040 1970-01-01 00:00:00.000000 nb_cli_plugin_bootstrap-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4182 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/const.py
+-rw-r--r--   0        0        0        0 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/handlers/__init__.py
+-rw-r--r--   0        0        0    13187 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/handlers/bootstrap.py
+-rw-r--r--   0        0        0     2275 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/handlers/pip_index.py
+-rw-r--r--   0        0        0      858 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/handlers/shell.py
+-rw-r--r--   0        0        0     6298 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/handlers/update_project.py
+-rw-r--r--   0        0        0     1954 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/plugin.py
+-rw-r--r--   0        0        0      722 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/cookiecutter.json
+-rw-r--r--   0        0        0      683 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      285 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      117 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/#run.sh
+-rw-r--r--   0        0        0       62 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/#shell.sh
+-rw-r--r--   0        0        0       71 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/#update.sh
+-rw-r--r--   0        0        0      105 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/#启动.bat
+-rw-r--r--   0        0        0       59 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/#更新所有插件.bat
+-rw-r--r--   0        0        0       44 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/#进入虚拟环境.bat
+-rw-r--r--   0        0        0     3199 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/.env.prod
+-rw-r--r--   0        0        0     1563 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/bot.py
+-rw-r--r--   0        0        0     1077 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/pyproject.toml
+-rw-r--r--   0        0        0      613 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/src/plugins/{{cookiecutter.computed.ping_plugin_name}}.py
+-rw-r--r--   0        0        0     5444 2024-04-06 16:23:28.409767 nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/utils.py
+-rw-r--r--   0        0        0      734 2024-04-06 16:23:40.961661 nb_cli_plugin_bootstrap-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4654 1970-01-01 00:00:00.000000 nb_cli_plugin_bootstrap-0.3.0/PKG-INFO
```

### Comparing `nb_cli_plugin_bootstrap-0.2.0/LICENSE` & `nb_cli_plugin_bootstrap-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_bootstrap-0.2.0/README.md` & `nb_cli_plugin_bootstrap-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -47,46 +47,64 @@
 
 ## 🎉 使用
 
 ### 创建一个更实用的 NoneBot2 初始项目
 
 ```shell
 nb bootstrap
-```
-
-或者
-
-```shell
 nb bs
 ```
 
 <details>
 <summary>效果图（点击展开）</summary>
 
 ![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/bootstrap.png)
 
 </details>
 
 ### 更新当前文件夹项目中的所有适配器和插件
 
 ```shell
 nb update-project
+nb up
 ```
 
-或者
+<details>
+<summary>效果图（点击展开）</summary>
+
+![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/update-project1.png)
+![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/update-project2.png)
+
+</details>
+
+### 快速修改全局 pip 的 PyPI 镜像源配置
 
 ```shell
-nb up
+nb pip-index
+nb pi
 ```
 
 <details>
 <summary>效果图（点击展开）</summary>
 
-![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/update-project1.png)
-![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/update-project2.png)
+![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/pip-index.png)
+
+</details>
+
+### 进入当前项目的虚拟环境
+
+```shell
+nb shell
+nb sh
+```
+
+<details>
+<summary>效果图（点击展开）</summary>
+
+![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/shell.png)
 
 </details>
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
@@ -103,14 +121,20 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.0
+
+- 添加 `nb pip-index` 与 `nb shell` 命令
+- 为部分指令新增 `-v` 选项用于输出更多信息
+- 微调项目模板
+
 ### 0.2.0
 
 - 适配 Pydantic V1 & V2
 - 可能再次修复了更新所有插件后统计归类不正确的问题
 
 ### 0.1.6
```

#### html2text {}

```diff
@@ -1,28 +1,35 @@
                             _[_N_o_n_e_B_o_t_C_l_i_P_l_u_g_i_n_L_o_g_o_]
                             [NoneBotCliPluginText]
  # NB-Cli-Plugin-Bootstrap _â¨ NoneBot2 æ´å®ç¨çåå§é¡¹ç®æ°å»ºå·¥å·
                       â¨_[python]_[_p_d_m_-_m_a_n_a_g_e_d_]_[_w_a_k_a_t_i_m_e_]
             _[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _1_ _O_r_ _2_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ```shell nb self install nb-cli-plugin-bootstrap ``` ## ð
 ä½¿ç¨ ### åå»ºä¸ä¸ªæ´å®ç¨ç NoneBot2 åå§é¡¹ç® ```shell nb bootstrap
-``` æè ```shell nb bs ``` ææå¾ï¼ç¹å»å±å¼ï¼ ![ææå¾](https://
+nb bs ``` ææå¾ï¼ç¹å»å±å¼ï¼ ![ææå¾](https://
 raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/bootstrap.png)
 ### æ´æ°å½åæä»¶å¤¹é¡¹ç®ä¸­çææééå¨åæä»¶ ```shell nb
-update-project ``` æè ```shell nb up ``` ææå¾ï¼ç¹å»å±å¼ï¼ !
+update-project nb up ``` ææå¾ï¼ç¹å»å±å¼ï¼ ![ææå¾](https://
+raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/update-
+project1.png) ![ææå¾](https://raw.githubusercontent.com/lgc-NB2Dev/readme/
+main/cli-bootstrap/update-project2.png) ### å¿«éä¿®æ¹å¨å± pip ç PyPI
+éåæºéç½® ```shell nb pip-index nb pi ``` ææå¾ï¼ç¹å»å±å¼ï¼ !
 [ææå¾](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-
-bootstrap/update-project1.png) ![ææå¾](https://raw.githubusercontent.com/
-lgc-NB2Dev/readme/main/cli-bootstrap/update-project2.png) ## ð èç³»
-QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
-[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+bootstrap/pip-index.png) ### è¿å¥å½åé¡¹ç®çèæç¯å¢ ```shell nb
+shell nb sh ``` ææå¾ï¼ç¹å»å±å¼ï¼ ![ææå¾](https://
+raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/shell.png) ##
+ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
+å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 -
+imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.3.0 - æ·»å  `nb pip-index` ä¸
+`nb shell` å½ä»¤ - ä¸ºé¨åæä»¤æ°å¢ `-v` éé¡¹ç¨äºè¾åºæ´å¤ä¿¡æ¯ -
+å¾®è°é¡¹ç®æ¨¡æ¿ ### 0.2.0 - éé Pydantic V1 & V2 -
 å¯è½åæ¬¡ä¿®å¤äºæ´æ°æææä»¶åç»è®¡å½ç±»ä¸æ­£ç¡®çé®é¢ ###
 0.1.6 - ä¿®å¤ç±äºä¸åçº¿æ¨ªçº¿ä¸ç»ä¸å¯¼è´çæ¾ç¤ºéè¯¯ ### 0.1.5 -
 æ´æ°é¡¹ç®çæ»ç»ä¼æ¾ç¤ºåæ´æ°åççæ¬å· -
 ç»æä»¤æ·»å äºå«å - æ°å¢éé¡¹ `-
 y`ï¼å¯ä»¥è·³è¿å¤§é¨åè¯¢é®ï¼ç´æ¥ä½¿ç¨é»è®¤å¼ - å¾®è°é¡¹ç®æ¨¡æ¿
 ### 0.1.4 - æ´æ°æææä»¶åå¦ææå¤±è´¥é¡¹ä¼è¯¢é®æ¯å¦éè¯ -
 æ°å¢é¨å pip å®è£éè¯¯åå åæ - éæé¨åé»è¾ -
```

### Comparing `nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/handlers/bootstrap.py` & `nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/handlers/bootstrap.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,36 @@
 import json
-import platform
 import shlex
 import subprocess
 import sys
 import traceback
 from pathlib import Path
 from typing import List
 
 import click
 from cookiecutter.main import cookiecutter
 from nb_cli.cli.commands.project import (
     ProjectContext,
     project_name_validator,
 )
 from nb_cli.cli.utils import CLI_DEFAULT_STYLE
-from nb_cli.compat import type_validate_python
 from nb_cli.config.parser import ConfigManager
+from nb_cli.consts import WINDOWS
 from nb_cli.handlers.adapter import list_adapters
 from nb_cli.handlers.plugin import list_builtin_plugins
 from nb_cli.handlers.process import create_process
 from nb_cli.handlers.venv import create_virtualenv
 from noneprompt import CheckboxPrompt, Choice, ConfirmPrompt, InputPrompt
-from noneprompt.prompts.list import ListPrompt
-from pydantic import AnyHttpUrl, BaseModel, IPvAnyAddress, ValidationError
 
-from ..utils import call_pip_no_output, call_pip_update_no_output
+from ..const import INPUT_QUESTION
+from ..utils import call_pip_update_simp, validate_ip_v_any_addr, wait
+from .pip_index import pip_index_handler
 
 TEMPLATES_DIR = Path(__file__).parent.parent / "templates"
 BOOTSTRAP_TEMPLATE_DIR = TEMPLATES_DIR / "bootstrap"
-IS_WINDOWS = "Windows" in platform.system()
-INPUT_QUESTION = "请输入 > "
-
-PyPIMirrorCustom = type("PyPIMirrorCustom", (), {})
-PYPI_MIRRORS = (
-    ("清华大学", "https://pypi.tuna.tsinghua.edu.cn/simple"),
-    ("中国科学技术大学", "https://pypi.mirrors.ustc.edu.cn/simple"),
-    ("阿里云", "https://mirrors.aliyun.com/pypi/simple/"),
-    ("豆瓣", "https://pypi.douban.com/simple/"),
-    ("自定义", PyPIMirrorCustom()),
-    ("不使用镜像源", None),
-)
-
-
-def validate_ip_v_any_addr(addr: str) -> bool:
-    class ValidateModel(BaseModel):
-        addr: IPvAnyAddress
-
-    try:
-        type_validate_python(ValidateModel, {"addr": addr})
-    except ValidationError:
-        return False
-    return True
-
-
-def validate_http_url(url: str) -> bool:
-    class ValidateModel(BaseModel):
-        url: AnyHttpUrl
-
-    try:
-        type_validate_python(ValidateModel, {"url": url})
-    except ValidationError:
-        return False
-    return True
 
 
 def format_project_folder_name(project_name: str) -> str:
     return project_name.replace(" ", "-").lower()
 
 
 async def prompt_input_list(prompt: str, **kwargs) -> List[str]:
@@ -209,50 +174,28 @@
     context.variables["env_port"] = env_port
 
     use_run_script = yes or await ConfirmPrompt(
         "是否在项目目录中释出快捷启动脚本？",
         default_choice=True,
     ).prompt_async(style=CLI_DEFAULT_STYLE)
     context.variables["use_run_script"] = use_run_script
-    context.variables["is_windows"] = IS_WINDOWS
+    context.variables["is_windows"] = WINDOWS
 
     redirect_localstore = yes or await ConfirmPrompt(
         "是否将 localstore 插件的存储路径重定向到项目路径下以便于后续迁移 Bot？",
         default_choice=True,
     ).prompt_async(style=CLI_DEFAULT_STYLE)
     context.variables["redirect_localstore"] = redirect_localstore
 
     use_ping = yes or await ConfirmPrompt(
         "是否使用超级用户 Ping 指令回复插件？",
         default_choice=True,
     ).prompt_async(style=CLI_DEFAULT_STYLE)
     context.variables["use_ping"] = use_ping
 
-    has_onebot = "nonebot-adapter-onebot" in context.packages
-    if has_onebot:
-        install_gocqhttp = (
-            False
-            if yes
-            else await ConfirmPrompt(
-                "是否安装 gocqhttp 插件提供内置 GoCQHTTP 启动器？（不推荐）",
-                default_choice=False,
-            ).prompt_async(style=CLI_DEFAULT_STYLE)
-        )
-        if install_gocqhttp:
-            context.packages.append("nonebot-plugin-gocqhttp")
-            context.variables["plugins"].append("nonebot_plugin_gocqhttp")
-
-        install_guild_patch = yes or await ConfirmPrompt(
-            "是否安装 guild-patch 插件提供对 GoCQHTTP 的 QQ 频道支持？",
-            default_choice=True,
-        ).prompt_async(style=CLI_DEFAULT_STYLE)
-        if install_guild_patch:
-            context.packages.append("nonebot-plugin-guild-patch")
-            context.variables["plugins"].append("nonebot_plugin_guild_patch")
-
     install_logpile = yes or await ConfirmPrompt(
         "是否安装 logpile 插件提供日志记录到文件功能？",
         default_choice=True,
     ).prompt_async(style=CLI_DEFAULT_STYLE)
     context.variables["use_logpile"] = install_logpile
     if install_logpile:
         context.packages.append("nonebot-plugin-logpile")
@@ -270,88 +213,46 @@
         context.variables["use_web_ui"] = use_web_ui
     else:
         context.variables["use_web_ui"] = False
 
     context.variables["plugins"] = json.dumps(context.variables["plugins"])
 
 
-async def configure_web_ui():
+async def configure_web_ui(verbose: bool):
     click.secho("正在为 nb-cli 安装 webui 插件，请稍候", fg="yellow", bold=True)
-    proc = await call_pip_update_no_output(
+    proc = await call_pip_update_simp(
         ["nb-cli-plugin-webui"],
         python_path=sys.executable,
     )
-    if await proc.wait() != 0:
+    code, _, stderr = await wait(proc, verbose=verbose)
+    if code != 0:
         click.secho(
-            f"插件安装失败，请使用 `nb self update nb-cli-plugin-webui` 指令手动安装\n{proc.stderr}",
+            f"插件安装失败，请使用 `nb self update nb-cli-plugin-webui` 指令手动安装\n{stderr}",
             fg="red",
             bold=True,
             err=True,
         )
 
     click.secho("插件安装成功", fg="green", bold=True)
     # click.secho("接下来，让我们开始配置 webui 插件，请稍等", fg="yellow", bold=True)
     proc = await create_process(
         sys.executable,
         "-c",
         "import nb_cli_plugin_webui.app.config",
     )
-    await proc.wait()
-
-
-async def change_pip_mirror():
-    choice = await ListPrompt(
-        "请选择你想要使用的 PyPI 镜像源",
-        [
-            Choice(f"{name} > {url}" if isinstance(url, str) else name, url)
-            for name, url in PYPI_MIRRORS
-        ],
-    ).prompt_async(style=CLI_DEFAULT_STYLE)
-
-    selected = choice.data
-    if isinstance(selected, PyPIMirrorCustom):
-        click.secho("请输入 PyPI 源地址", bold=True)
-        selected_mirror = await InputPrompt(
-            INPUT_QUESTION,
-            validator=validate_http_url,
-            error_message="链接格式不正确！",
-        ).prompt_async(style=CLI_DEFAULT_STYLE)
-    else:
-        selected_mirror = selected
-
-    proc = await call_pip_no_output(["config", "get", "global.index-url"])
-    current_mirror = (
-        (await proc.stdout.read()).decode().strip()
-        if (await proc.wait() == 0) and proc.stdout
-        else None
-    )
-    if selected_mirror:
-        proc = await call_pip_no_output(
-            ["config", "set", "global.index-url", selected_mirror],
-        )
-    elif current_mirror:  # 设置过才执行清空
-        proc = await call_pip_no_output(
-            ["config", "unset", "global.index-url"],
-        )
-    else:
-        proc = None
-    code = await proc.wait() if proc else 0
-
-    if (not proc) or current_mirror == selected_mirror:
-        click.secho("PyPI 源配置未变", fg="yellow", bold=True)
-    elif code == 0:
-        click.secho("PyPI 源配置成功", fg="green", bold=True)
-    else:
-        err = (await proc.stderr.read()).decode() if proc.stderr else ""
-        click.secho(f"PyPI 源配置失败！\n{err}", fg="red", bold=True, err=True)
+    await wait(proc, verbose=verbose)
 
 
-async def post_project_render(context: ProjectContext, yes: bool = False) -> bool:
+async def post_project_render(
+    context: ProjectContext,
+    yes: bool = False,
+    verbose: bool = False,
+) -> bool:
     if context.variables["use_web_ui"]:
-        await configure_web_ui()
+        await configure_web_ui(verbose=verbose)
 
     use_venv = yes or await ConfirmPrompt(
         "是否新建虚拟环境？",
         default_choice=True,
     ).prompt_async(style=CLI_DEFAULT_STYLE)
     project_dir_name = context.variables["project_name"].replace(" ", "-").lower()
     project_dir = Path.cwd() / project_dir_name
@@ -374,15 +275,15 @@
         False
         if yes
         else await ConfirmPrompt(
             "是否需要修改或清除 pip 的 PyPI 镜像源配置？",
             default_choice=False,
         ).prompt_async(style=CLI_DEFAULT_STYLE)
     ):
-        await change_pip_mirror()
+        await pip_index_handler(verbose=verbose)
 
     manually_install_tip = "项目依赖已写入项目 pyproject.toml 中，请自行手动安装，或使用 pdm 等包管理器安装"
     if (not use_venv) or (
         not (
             yes
             or await ConfirmPrompt(
                 "是否立即安装项目依赖？",
@@ -391,23 +292,24 @@
         )
     ):
         click.secho(manually_install_tip, fg="green")
         return True
 
     click.secho("正在安装项目依赖", fg="yellow")
     config_manager = ConfigManager(working_dir=project_dir, use_venv=use_venv)
-    proc = await call_pip_update_no_output(
+    proc = await call_pip_update_simp(
         context.packages,
         python_path=config_manager.python_path,
     )
-    if await proc.wait() == 0:
+    code, _, stderr = await wait(proc, verbose=verbose)
+    if code == 0:
         click.secho("依赖安装成功", fg="green", bold=True)
     else:
         click.secho(
-            f"依赖安装失败，{manually_install_tip}\n{proc.stderr}",
+            f"依赖安装失败，{manually_install_tip}\n{stderr}",
             fg="red",
             bold=True,
             err=True,
         )
         return False
 
     if not yes:
@@ -432,22 +334,22 @@
                 err=True,
             )
             return False
 
     return True
 
 
-async def bootstrap_handler(*, yes: bool = False):
+async def bootstrap_handler(*, yes: bool = False, verbose: bool = False):
     context = ProjectContext()
     await prompt_bootstrap_context(context, yes=yes)
 
     nb_command_list = [sys.executable, "-m", "nb_cli"]
     context.variables["nb_command"] = (
         subprocess.list2cmdline(nb_command_list)
-        if IS_WINDOWS
+        if WINDOWS
         else " ".join(shlex.quote(x) for x in nb_command_list)
     )
     extra_context = {
         "nonebot": {
             **context.variables,
             "packages": json.dumps(context.packages),
         },
@@ -469,15 +371,15 @@
         return
     click.secho(
         f"成功新建项目 {context.variables['project_name']}",
         fg="green",
         bold=True,
     )
 
-    if await post_project_render(context, yes=yes):
+    if await post_project_render(context, yes=yes, verbose=verbose):
         click.secho("项目配置完毕，开始使用吧！", fg="green", bold=True)
     else:
         click.secho(
             "项目配置失败！你可能需要考虑手动进行后续配置，或重新创建一次项目",
             fg="red",
             bold=True,
             err=True,
```

### Comparing `nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/handlers/update_project.py` & `nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/handlers/update_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,27 +115,31 @@
         )
         info_li.append(f"{fail_title}\n{fail_plugins}")
 
     return "\n\n".join(info_li)
 
 
 # 不能一下子全传进去，否则可能导致依赖冲突
-async def update(packages: List[str], python_path: str) -> List[InstallInfoType]:
+async def update(
+    packages: List[str],
+    python_path: str,
+    verbose: bool = False,
+) -> List[InstallInfoType]:
     pkg_list_before = await list_all_packages(python_path)
     infos = []
     with click.progressbar(
         packages,
         show_eta=False,
         show_percent=True,
         show_pos=True,
         item_show_func=lambda x: (click.style(x, fg="green", bold=True) if x else None),
         bar_template=f"更新中 {click.style('%(info)s', fg='cyan')} [%(bar)s]",
     ) as pkgs_prog:
         for pkg in pkgs_prog:
-            info = await update_package(pkg, python_path)
+            info = await update_package(pkg, python_path, verbose=verbose)
             infos.append(info)
             if isinstance(info, FailInstallInfo):
                 click.secho(
                     f"\n更新 {pkg} 失败！可能原因：{info.reason}\n{info.stderr.rstrip()}",
                     fg="red",
                     err=True,
                 )
@@ -147,14 +151,15 @@
 
 
 @requires_project_root
 @requires_pip
 async def update_project_handler(
     *,
     yes: bool = False,
+    verbose: bool = False,
     python_path: Optional[str] = None,
     cwd: Optional[Path] = None,  # noqa: ARG001
 ):
     bot_config = get_nonebot_config()
     if python_path is None:
         python_path = await get_default_python()
 
@@ -172,15 +177,15 @@
             "一键更新所有适配器和插件有可能会导致它们之间不兼容导致报错，请问您是否真的要继续？",
             default_choice=True,
         ).prompt_async(style=CLI_DEFAULT_STYLE)
     ):
         return
 
     while True:
-        infos = await update(pkgs, python_path)
+        infos = await update(pkgs, python_path, verbose=verbose)
         failed_infos = [x for x in infos if isinstance(x, FailInstallInfo)]
         if (not failed_infos) or (
             not (
                 yes
                 or await ConfirmPrompt(
                     "部分包安装失败，是否重试？",
                     default_choice=True,
```

### Comparing `nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/cookiecutter.json` & `nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/hooks/post_gen_project.py` & `nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/.env.prod` & `nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/.env.prod`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/bot.py` & `nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/bot.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/pyproject.toml` & `nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/src/plugins/{{cookiecutter.computed.ping_plugin_name}}.py` & `nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/templates/bootstrap/{{cookiecutter.nonebot.folder_name}}/src/plugins/{{cookiecutter.computed.ping_plugin_name}}.py`

 * *Files identical despite different names*

### Comparing `nb_cli_plugin_bootstrap-0.2.0/nb_cli_plugin_bootstrap/utils.py` & `nb_cli_plugin_bootstrap-0.3.0/nb_cli_plugin_bootstrap/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import asyncio
 import json
 import locale
+import sys
 from asyncio.subprocess import Process
-from typing import Dict, List, Optional, Union
+from io import StringIO
+from typing import Dict, List, Optional, TextIO, Tuple, Union
 from typing_extensions import TypeAlias
 
+from nb_cli.compat import type_validate_python
 from nb_cli.handlers.pip import call_pip
+from pydantic import AnyHttpUrl, BaseModel, IPvAnyAddress, ValidationError
 
 InstallInfoType: TypeAlias = Union["SuccessInstallInfo", "FailInstallInfo"]
 
 ENC = locale.getpreferredencoding()
 
 
 class SuccessInstallInfo:
@@ -66,57 +70,113 @@
 def decode(s: bytes) -> str:
     try:
         return s.decode()
     except UnicodeDecodeError:
         return s.decode(ENC, errors="replace")
 
 
-async def call_pip_no_output(
+async def call_pip_simp(
     pip_args: List[str],
     python_path: Optional[str] = None,
 ) -> Process:
     return await call_pip(
         pip_args,
         python_path=python_path,
         stdin=asyncio.subprocess.DEVNULL,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
 
 
-async def call_pip_update_no_output(
+async def call_pip_update_simp(
     pip_args: List[str],
     python_path: Optional[str] = None,
 ) -> Process:
-    return await call_pip_no_output(
+    return await call_pip_simp(
         ["install", "--upgrade", *pip_args],
         python_path=python_path,
     )
 
 
+async def read_stream(
+    stream: Optional[asyncio.StreamReader],
+    outer: Optional[TextIO] = None,
+) -> str:
+    if not stream:
+        return ""
+
+    cached_io = StringIO()
+    async for data in stream:
+        data_str = decode(data)
+        cached_io.write(data_str)
+        if outer:
+            outer.write(data_str)
+
+    return cached_io.getvalue()
+
+
+async def wait(
+    proc: asyncio.subprocess.Process,
+    verbose: bool = False,
+) -> Tuple[int, str, str]:
+    if verbose:
+        stdout, stderr = await asyncio.gather(
+            read_stream(proc.stdout, sys.stdout),
+            read_stream(proc.stderr, sys.stderr),
+        )
+    else:
+        stdout_b, stderr_b = await proc.communicate()
+        stdout = decode(stdout_b)
+        stderr = decode(stderr_b)
+    return (await proc.wait(), stdout, stderr)
+
+
 def normalize_pkg_name(name: str) -> str:
     return name.replace("_", "-").lower()
 
 
 async def list_all_packages(python_path: Optional[str] = None) -> Dict[str, str]:
-    proc = await call_pip_no_output(["list", "--format=json"], python_path=python_path)
+    proc = await call_pip_simp(["list", "--format=json"], python_path=python_path)
     return_code = await proc.wait()
     if not return_code == 0:
         raise RuntimeError("Failed to execute command `pip list`")
     assert proc.stdout
     stdout = decode(await proc.stdout.read())
     return {normalize_pkg_name(x["name"]): x["version"] for x in json.loads(stdout)}
 
 
 async def update_package(
     pkg: str,
     python_path: Optional[str] = None,
+    verbose: bool = False,
 ) -> InstallInfoType:
-    proc = await call_pip_update_no_output([pkg], python_path=python_path)
-    return_code = await proc.wait()
-    stdout = decode(await proc.stdout.read()) if proc.stdout else ""
-    stderr = decode(await proc.stderr.read()) if proc.stderr else ""
+    if verbose:
+        print()
+    proc = await call_pip_update_simp([pkg], python_path=python_path)
+    return_code, stdout, stderr = await wait(proc, verbose=verbose)
     return (
         SuccessInstallInfo(pkg, stdout, stderr)
         if return_code == 0
         else FailInstallInfo(pkg, stdout, stderr)
     )
+
+
+def validate_ip_v_any_addr(addr: str) -> bool:
+    class ValidateModel(BaseModel):
+        addr: IPvAnyAddress
+
+    try:
+        type_validate_python(ValidateModel, {"addr": addr})
+    except ValidationError:
+        return False
+    return True
+
+
+def validate_http_url(url: str) -> bool:
+    class ValidateModel(BaseModel):
+        url: AnyHttpUrl
+
+    try:
+        type_validate_python(ValidateModel, {"url": url})
+    except ValidationError:
+        return False
+    return True
```

### Comparing `nb_cli_plugin_bootstrap-0.2.0/pyproject.toml` & `nb_cli_plugin_bootstrap-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 dynamic = []
 description = "A nb-cli plugin for quickly create and bootstrap a NoneBot2 project."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nb-cli>=1.4.0",
+    "poetry>=1.8.2",
 ]
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
-version = "0.2.0"
+version = "0.3.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nb-cli-plugin-bootstrap"
```

### Comparing `nb_cli_plugin_bootstrap-0.2.0/PKG-INFO` & `nb_cli_plugin_bootstrap-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: nb-cli-plugin-bootstrap
-Version: 0.2.0
+Version: 0.3.0
 Summary: A nb-cli plugin for quickly create and bootstrap a NoneBot2 project.
 Home-page: https://github.com/lgc-NB2Dev/nb-cli-plugin-bootstrap
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nb-cli-plugin-bootstrap
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nb-cli>=1.4.0
+Requires-Dist: poetry>=1.8.2
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://cli.nonebot.dev/">
@@ -59,46 +60,64 @@
 
 ## 🎉 使用
 
 ### 创建一个更实用的 NoneBot2 初始项目
 
 ```shell
 nb bootstrap
-```
-
-或者
-
-```shell
 nb bs
 ```
 
 <details>
 <summary>效果图（点击展开）</summary>
 
 ![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/bootstrap.png)
 
 </details>
 
 ### 更新当前文件夹项目中的所有适配器和插件
 
 ```shell
 nb update-project
+nb up
 ```
 
-或者
+<details>
+<summary>效果图（点击展开）</summary>
+
+![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/update-project1.png)
+![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/update-project2.png)
+
+</details>
+
+### 快速修改全局 pip 的 PyPI 镜像源配置
 
 ```shell
-nb up
+nb pip-index
+nb pi
 ```
 
 <details>
 <summary>效果图（点击展开）</summary>
 
-![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/update-project1.png)
-![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/update-project2.png)
+![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/pip-index.png)
+
+</details>
+
+### 进入当前项目的虚拟环境
+
+```shell
+nb shell
+nb sh
+```
+
+<details>
+<summary>效果图（点击展开）</summary>
+
+![效果图](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/shell.png)
 
 </details>
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
@@ -115,14 +134,20 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.0
+
+- 添加 `nb pip-index` 与 `nb shell` 命令
+- 为部分指令新增 `-v` 选项用于输出更多信息
+- 微调项目模板
+
 ### 0.2.0
 
 - 适配 Pydantic V1 & V2
 - 可能再次修复了更新所有插件后统计归类不正确的问题
 
 ### 0.1.6
```

#### html2text {}

```diff
@@ -1,35 +1,42 @@
-Metadata-Version: 2.1 Name: nb-cli-plugin-bootstrap Version: 0.2.0 Summary: A
+Metadata-Version: 2.1 Name: nb-cli-plugin-bootstrap Version: 0.3.0 Summary: A
 nb-cli plugin for quickly create and bootstrap a NoneBot2 project. Home-page:
 https://github.com/lgc-NB2Dev/nb-cli-plugin-bootstrap Author-Email:
 student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/nb-
 cli-plugin-bootstrap Requires-Python: <4.0,>=3.9 Requires-Dist: nb-cli>=1.4.0
-Description-Content-Type: text/markdown
+Requires-Dist: poetry>=1.8.2 Description-Content-Type: text/markdown
                             _[_N_o_n_e_B_o_t_C_l_i_P_l_u_g_i_n_L_o_g_o_]
                             [NoneBotCliPluginText]
  # NB-Cli-Plugin-Bootstrap _â¨ NoneBot2 æ´å®ç¨çåå§é¡¹ç®æ°å»ºå·¥å·
                       â¨_[python]_[_p_d_m_-_m_a_n_a_g_e_d_]_[_w_a_k_a_t_i_m_e_]
             _[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _1_ _O_r_ _2_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ```shell nb self install nb-cli-plugin-bootstrap ``` ## ð
 ä½¿ç¨ ### åå»ºä¸ä¸ªæ´å®ç¨ç NoneBot2 åå§é¡¹ç® ```shell nb bootstrap
-``` æè ```shell nb bs ``` ææå¾ï¼ç¹å»å±å¼ï¼ ![ææå¾](https://
+nb bs ``` ææå¾ï¼ç¹å»å±å¼ï¼ ![ææå¾](https://
 raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/bootstrap.png)
 ### æ´æ°å½åæä»¶å¤¹é¡¹ç®ä¸­çææééå¨åæä»¶ ```shell nb
-update-project ``` æè ```shell nb up ``` ææå¾ï¼ç¹å»å±å¼ï¼ !
+update-project nb up ``` ææå¾ï¼ç¹å»å±å¼ï¼ ![ææå¾](https://
+raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/update-
+project1.png) ![ææå¾](https://raw.githubusercontent.com/lgc-NB2Dev/readme/
+main/cli-bootstrap/update-project2.png) ### å¿«éä¿®æ¹å¨å± pip ç PyPI
+éåæºéç½® ```shell nb pip-index nb pi ``` ææå¾ï¼ç¹å»å±å¼ï¼ !
 [ææå¾](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-
-bootstrap/update-project1.png) ![ææå¾](https://raw.githubusercontent.com/
-lgc-NB2Dev/readme/main/cli-bootstrap/update-project2.png) ## ð èç³»
-QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
-[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+bootstrap/pip-index.png) ### è¿å¥å½åé¡¹ç®çèæç¯å¢ ```shell nb
+shell nb sh ``` ææå¾ï¼ç¹å»å±å¼ï¼ ![ææå¾](https://
+raw.githubusercontent.com/lgc-NB2Dev/readme/main/cli-bootstrap/shell.png) ##
+ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
+å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 -
+imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.3.0 - æ·»å  `nb pip-index` ä¸
+`nb shell` å½ä»¤ - ä¸ºé¨åæä»¤æ°å¢ `-v` éé¡¹ç¨äºè¾åºæ´å¤ä¿¡æ¯ -
+å¾®è°é¡¹ç®æ¨¡æ¿ ### 0.2.0 - éé Pydantic V1 & V2 -
 å¯è½åæ¬¡ä¿®å¤äºæ´æ°æææä»¶åç»è®¡å½ç±»ä¸æ­£ç¡®çé®é¢ ###
 0.1.6 - ä¿®å¤ç±äºä¸åçº¿æ¨ªçº¿ä¸ç»ä¸å¯¼è´çæ¾ç¤ºéè¯¯ ### 0.1.5 -
 æ´æ°é¡¹ç®çæ»ç»ä¼æ¾ç¤ºåæ´æ°åççæ¬å· -
 ç»æä»¤æ·»å äºå«å - æ°å¢éé¡¹ `-
 y`ï¼å¯ä»¥è·³è¿å¤§é¨åè¯¢é®ï¼ç´æ¥ä½¿ç¨é»è®¤å¼ - å¾®è°é¡¹ç®æ¨¡æ¿
 ### 0.1.4 - æ´æ°æææä»¶åå¦ææå¤±è´¥é¡¹ä¼è¯¢é®æ¯å¦éè¯ -
 æ°å¢é¨å pip å®è£éè¯¯åå åæ - éæé¨åé»è¾ -
```

