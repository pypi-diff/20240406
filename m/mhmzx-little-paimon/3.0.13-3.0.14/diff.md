# Comparing `tmp/mhmzx_little_paimon-3.0.13.tar.gz` & `tmp/mhmzx_little_paimon-3.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mhmzx_little_paimon-3.0.13.tar", max compression
+gzip compressed data, was "mhmzx_little_paimon-3.0.14.tar", max compression
```

## Comparing `mhmzx_little_paimon-3.0.13.tar` & `mhmzx_little_paimon-3.0.14.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0    34523 2023-10-03 11:58:12.363188 mhmzx_little_paimon-3.0.13/LICENSE
--rw-r--r--   0        0        0     3118 2023-10-04 07:14:41.385648 mhmzx_little_paimon-3.0.13/LittlePaimon/__init__.py
--rw-r--r--   0        0        0      186 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.13/LittlePaimon/config/__init__.py
--rw-r--r--   0        0        0     1665 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.13/LittlePaimon/config/command/__init__.py
--rw-r--r--   0        0        0     1752 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.13/LittlePaimon/config/config/manage.py
--rw-r--r--   0        0        0     3423 2024-02-12 14:42:03.666780 mhmzx_little_paimon-3.0.13/LittlePaimon/config/config/model.py
--rw-r--r--   0        0        0    36556 2024-02-12 14:42:03.666780 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/alias.json
--rw-r--r--   0        0        0    35003 2024-01-05 08:01:44.338265 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/artifact.json
--rw-r--r--   0        0        0    25724 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/ban_word.txt
--rw-r--r--   0        0        0    57404 2024-02-12 14:42:03.666780 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/genshin_info.json
--rw-r--r--   0        0        0     1508 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/prop.json
--rw-r--r--   0        0        0    43083 2024-02-12 14:42:03.666780 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/role_skill.json
--rw-r--r--   0        0        0    33376 2024-02-12 14:42:03.666780 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/role_talent.json
--rw-r--r--   0        0        0  1377172 2024-02-12 14:42:03.666780 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/roles_data.json
--rw-r--r--   0        0        0    25217 2024-02-12 14:42:03.666780 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/score.json
--rw-r--r--   0        0        0      949 2023-10-03 14:13:02.126748 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/upheaval.json
--rw-r--r--   0        0        0    21997 2024-02-12 14:42:03.666780 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/weapon.json
--rw-r--r--   0        0        0     7628 2024-01-05 08:01:44.338265 mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/类型.json
--rw-r--r--   0        0        0     8927 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.13/LittlePaimon/config/plugin/manage.py
--rw-r--r--   0        0        0      795 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/config/plugin/model.py
--rw-r--r--   0        0        0     4161 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/database/__init__.py
--rw-r--r--   0        0        0      308 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/__init__.py
--rw-r--r--   0        0        0    11634 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/abyss_info.py
--rw-r--r--   0        0        0    20220 2023-12-07 15:12:48.876317 mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/character.py
--rw-r--r--   0        0        0     2602 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/cookie.py
--rw-r--r--   0        0        0     1234 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/genshin_voice.py
--rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/manage.py
--rw-r--r--   0        0        0      451 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/memory_db.py
--rw-r--r--   0        0        0      782 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/other.py
--rw-r--r--   0        0        0    12879 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/player_info.py
--rw-r--r--   0        0        0     3546 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/subscription.py
--rw-r--r--   0        0        0     4573 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/__init__.py
--rw-r--r--   0        0        0     6849 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/event.py
--rw-r--r--   0        0        0     2540 2024-02-12 14:42:03.666780 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/generate.py
--rw-r--r--   0        0        0     2466 2024-02-12 14:42:03.666780 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html
--rw-r--r--   0        0        0     6882 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/template/index.css
--rw-r--r--   0        0        0   315626 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/template/iview.css
--rw-r--r--   0        0        0     6346 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css
--rw-r--r--   0        0        0   158333 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg
--rw-r--r--   0        0        0     4436 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Voice/__init__.py
--rw-r--r--   0        0        0     2535 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Voice/draw.py
--rw-r--r--   0        0        0     5816 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Voice/handler.py
--rw-r--r--   0        0        0     3565 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Voice/resources.py
--rw-r--r--   0        0        0     3382 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/__init__.py
--rw-r--r--   0        0        0     3046 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/config.py
--rw-r--r--   0        0        0     6587 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/genshin_word.txt
--rw-r--r--   0        0        0    30915 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/handler.py
--rw-r--r--   0        0        0     3970 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/models.py
--rw-r--r--   0        0        0     9972 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/web_api.py
--rw-r--r--   0        0        0    23060 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/web_page.py
--rw-r--r--   0        0        0     1306 2024-02-12 14:42:03.666780 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Mihoyo_bbs/__init__.py
--rw-r--r--   0        0        0    10040 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/NoticeAndRequest/__init__.py
--rw-r--r--   0        0        0     1235 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/NoticeAndRequest/config.py
--rw-r--r--   0        0        0     3343 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/__init__.py
--rw-r--r--   0        0        0    16481 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py
--rw-r--r--   0        0        0    13495 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py
--rw-r--r--   0        0        0       28 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/youchuang/__init__.py
--rw-r--r--   0        0        0     1727 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py
--rw-r--r--   0        0        0     3552 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py
--rw-r--r--   0        0        0      991 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py
--rw-r--r--   0        0        0     8135 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Autobbs/__init__.py
--rw-r--r--   0        0        0    14974 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py
--rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Autobbs/draw.py
--rw-r--r--   0        0        0     8833 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py
--rw-r--r--   0        0        0    20499 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Bind/__init__.py
--rw-r--r--   0        0        0    11054 2023-12-07 13:48:58.774988 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Bind/get_cookie.py
--rw-r--r--   0        0        0     4387 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py
--rw-r--r--   0        0        0     1768 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_CloudGenshin/api.py
--rw-r--r--   0        0        0     3894 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py
--rw-r--r--   0        0        0     3147 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_DailyNote/__init__.py
--rw-r--r--   0        0        0     9780 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_DailyNote/draw.py
--rw-r--r--   0        0        0     7660 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_DailyNote/handler.py
--rw-r--r--   0        0        0    10565 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha/__init__.py
--rw-r--r--   0        0        0     1341 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha/data_handle.py
--rw-r--r--   0        0        0     7925 2023-11-29 06:20:17.596561 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha/data_source.py
--rw-r--r--   0        0        0     4364 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha/draw.py
--rw-r--r--   0        0        0     8177 2023-12-07 13:49:08.459066 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py
--rw-r--r--   0        0        0    10311 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py
--rw-r--r--   0        0        0    13248 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py
--rw-r--r--   0        0        0     3580 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha_Log/models.py
--rw-r--r--   0        0        0    15959 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/__init__.py
--rw-r--r--   0        0        0    11703 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/damage_cal.py
--rw-r--r--   0        0        0    65408 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/damage_model.py
--rw-r--r--   0        0        0    10845 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py
--rw-r--r--   0        0        0     7799 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/draw_character_card.py
--rw-r--r--   0        0        0    14100 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py
--rw-r--r--   0        0        0     9721 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/draw_player_card.py
--rw-r--r--   0        0        0     1502 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py
--rw-r--r--   0        0        0     3990 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_MonthInfo/draw.py
--rw-r--r--   0        0        0     1431 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_MonthInfo/handler.py
--rw-r--r--   0        0        0      123 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/Atlas/__init__.py
--rw-r--r--   0        0        0     2029 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py
--rw-r--r--   0        0        0       37 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/__init__.py
--rw-r--r--   0        0        0     3357 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py
--rw-r--r--   0        0        0     5089 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py
--rw-r--r--   0        0        0      209 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/models.py
--rw-r--r--   0        0        0    22279 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/__init__.py
--rw-r--r--   0        0        0     7572 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py
--rw-r--r--   0        0        0     8754 2023-11-29 04:10:49.880595 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/draw_map.py
--rw-r--r--   0        0        0      888 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py
--rw-r--r--   0        0        0      446 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/genshinmap/exc.py
--rw-r--r--   0        0        0     2600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py
--rw-r--r--   0        0        0     3573 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py
--rw-r--r--   0        0        0     4320 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py
--rw-r--r--   0        0        0     2902 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py
--rw-r--r--   0        0        0     1231 2023-11-02 02:35:17.358460 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py
--rw-r--r--   0        0        0     7228 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/bot_manager/__init__.py
--rw-r--r--   0        0        0     4615 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/news60s/__init__.py
--rw-r--r--   0        0        0     8537 2023-12-07 12:31:51.791454 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/plugin_manager/__init__.py
--rw-r--r--   0        0        0     5192 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/plugin_manager/draw_help.py
--rw-r--r--   0        0        0     1443 2024-02-12 14:42:03.670780 mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/tools/__init__.py
--rw-r--r--   0        0        0      607 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/__init__.py
--rw-r--r--   0        0        0     6214 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/alias.py
--rw-r--r--   0        0        0    18691 2023-12-07 15:12:48.876317 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/api.py
--rw-r--r--   0        0        0     3844 2024-02-12 14:42:03.670780 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/browser.py
--rw-r--r--   0        0        0     2695 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/files.py
--rw-r--r--   0        0        0     2420 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/filter.py
--rw-r--r--   0        0        0    19469 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/genshin.py
--rw-r--r--   0        0        0    22335 2023-11-29 04:12:29.325419 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/image.py
--rw-r--r--   0        0        0     1380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/logger.py
--rw-r--r--   0        0        0    14786 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/message.py
--rw-r--r--   0        0        0     2380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/path.py
--rw-r--r--   0        0        0     9531 2023-11-29 04:13:41.406015 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/requests.py
--rw-r--r--   0        0        0     1254 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/scheduler.py
--rw-r--r--   0        0        0     1600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/status.py
--rw-r--r--   0        0        0     5838 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/tool.py
--rw-r--r--   0        0        0     3809 2024-02-12 14:42:03.670780 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/typing.py
--rw-r--r--   0        0        0     4568 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/utils/update.py
--rw-r--r--   0        0        0     2576 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.13/LittlePaimon/web/__init__.py
--rw-r--r--   0        0        0      655 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/__init__.py
--rw-r--r--   0        0        0     4853 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/bot_info.py
--rw-r--r--   0        0        0     1807 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/command_alias.py
--rw-r--r--   0        0        0    15631 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/cookie.py
--rw-r--r--   0        0        0      791 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/login.py
--rw-r--r--   0        0        0     6463 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/plugin.py
--rw-r--r--   0        0        0     1974 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/status.py
--rw-r--r--   0        0        0     1081 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/utils.py
--rw-r--r--   0        0        0      112 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/__init__.py
--rw-r--r--   0        0        0     1651 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/bind_cookie.py
--rw-r--r--   0        0        0     3525 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/command_alias.py
--rw-r--r--   0        0        0    16990 2024-02-12 14:42:03.670780 mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/config_manage.py
--rw-r--r--   0        0        0      347 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/constants.py
--rw-r--r--   0        0        0     5482 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/home_page.py
--rw-r--r--   0        0        0     1903 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/login.py
--rw-r--r--   0        0        0     1816 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/main.py
--rw-r--r--   0        0        0     8089 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/plugin_manage.py
--rw-r--r--   0        0        0     6613 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/private_cookie.py
--rw-r--r--   0        0        0     3067 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/public_cookie.py
--rw-r--r--   0        0        0     1251 2024-02-12 14:45:19.920414 mhmzx_little_paimon-3.0.13/pyproject.toml
--rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 mhmzx_little_paimon-3.0.13/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-10-03 11:58:12.363188 mhmzx_little_paimon-3.0.14/LICENSE
+-rw-r--r--   0        0        0     3118 2023-10-04 07:14:41.385648 mhmzx_little_paimon-3.0.14/LittlePaimon/__init__.py
+-rw-r--r--   0        0        0      186 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/__init__.py
+-rw-r--r--   0        0        0     1665 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/command/__init__.py
+-rw-r--r--   0        0        0     1752 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/config/manage.py
+-rw-r--r--   0        0        0     3423 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/config/model.py
+-rw-r--r--   0        0        0    36975 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/alias.json
+-rw-r--r--   0        0        0    35003 2024-01-05 08:01:44.338265 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/artifact.json
+-rw-r--r--   0        0        0    25724 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/ban_word.txt
+-rw-r--r--   0        0        0    57661 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/genshin_info.json
+-rw-r--r--   0        0        0     1508 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/prop.json
+-rw-r--r--   0        0        0    43602 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/role_skill.json
+-rw-r--r--   0        0        0    33754 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/role_talent.json
+-rw-r--r--   0        0        0  1377251 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/roles_data.json
+-rw-r--r--   0        0        0    25277 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/score.json
+-rw-r--r--   0        0        0      949 2023-10-03 14:13:02.126748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/upheaval.json
+-rw-r--r--   0        0        0    22269 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/weapon.json
+-rw-r--r--   0        0        0     7720 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/类型.json
+-rw-r--r--   0        0        0     8927 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.14/LittlePaimon/config/plugin/manage.py
+-rw-r--r--   0        0        0      795 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/plugin/model.py
+-rw-r--r--   0        0        0     4161 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/__init__.py
+-rw-r--r--   0        0        0      308 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/__init__.py
+-rw-r--r--   0        0        0    11634 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/abyss_info.py
+-rw-r--r--   0        0        0    20220 2023-12-07 15:12:48.876317 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/character.py
+-rw-r--r--   0        0        0     2602 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/cookie.py
+-rw-r--r--   0        0        0     1234 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/genshin_voice.py
+-rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/manage.py
+-rw-r--r--   0        0        0      451 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/memory_db.py
+-rw-r--r--   0        0        0      782 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/other.py
+-rw-r--r--   0        0        0    12879 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/player_info.py
+-rw-r--r--   0        0        0     3546 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/subscription.py
+-rw-r--r--   0        0        0     4573 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/__init__.py
+-rw-r--r--   0        0        0     6849 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/event.py
+-rw-r--r--   0        0        0     2540 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/generate.py
+-rw-r--r--   0        0        0     2466 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html
+-rw-r--r--   0        0        0     6882 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/index.css
+-rw-r--r--   0        0        0   315626 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/iview.css
+-rw-r--r--   0        0        0     6346 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css
+-rw-r--r--   0        0        0   158333 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg
+-rw-r--r--   0        0        0     4436 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/__init__.py
+-rw-r--r--   0        0        0     2535 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/draw.py
+-rw-r--r--   0        0        0     5816 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/handler.py
+-rw-r--r--   0        0        0     3565 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/resources.py
+-rw-r--r--   0        0        0     3382 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/__init__.py
+-rw-r--r--   0        0        0     3046 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/config.py
+-rw-r--r--   0        0        0     6587 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/genshin_word.txt
+-rw-r--r--   0        0        0    30915 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/handler.py
+-rw-r--r--   0        0        0     3970 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/models.py
+-rw-r--r--   0        0        0     9972 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/web_api.py
+-rw-r--r--   0        0        0    23060 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/web_page.py
+-rw-r--r--   0        0        0     1306 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Mihoyo_bbs/__init__.py
+-rw-r--r--   0        0        0    10040 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/NoticeAndRequest/__init__.py
+-rw-r--r--   0        0        0     1235 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/NoticeAndRequest/config.py
+-rw-r--r--   0        0        0     3343 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/__init__.py
+-rw-r--r--   0        0        0    16481 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py
+-rw-r--r--   0        0        0    13495 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py
+-rw-r--r--   0        0        0       28 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/__init__.py
+-rw-r--r--   0        0        0     1727 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py
+-rw-r--r--   0        0        0     3552 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py
+-rw-r--r--   0        0        0      991 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py
+-rw-r--r--   0        0        0     8135 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/__init__.py
+-rw-r--r--   0        0        0    14974 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py
+-rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/draw.py
+-rw-r--r--   0        0        0     8833 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py
+-rw-r--r--   0        0        0    20499 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Bind/__init__.py
+-rw-r--r--   0        0        0    11054 2023-12-07 13:48:58.774988 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Bind/get_cookie.py
+-rw-r--r--   0        0        0     4387 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py
+-rw-r--r--   0        0        0     1768 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/api.py
+-rw-r--r--   0        0        0     3894 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py
+-rw-r--r--   0        0        0     3147 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/__init__.py
+-rw-r--r--   0        0        0     9780 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/draw.py
+-rw-r--r--   0        0        0     7660 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/handler.py
+-rw-r--r--   0        0        0    10565 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/__init__.py
+-rw-r--r--   0        0        0     1341 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/data_handle.py
+-rw-r--r--   0        0        0     7925 2023-11-29 06:20:17.596561 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/data_source.py
+-rw-r--r--   0        0        0     4364 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/draw.py
+-rw-r--r--   0        0        0     8177 2023-12-07 13:49:08.459066 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py
+-rw-r--r--   0        0        0    10500 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py
+-rw-r--r--   0        0        0    13429 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py
+-rw-r--r--   0        0        0     3852 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/models.py
+-rw-r--r--   0        0        0    15959 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/__init__.py
+-rw-r--r--   0        0        0    11703 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/damage_cal.py
+-rw-r--r--   0        0        0    65408 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/damage_model.py
+-rw-r--r--   0        0        0    10845 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py
+-rw-r--r--   0        0        0     7799 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_card.py
+-rw-r--r--   0        0        0    14100 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py
+-rw-r--r--   0        0        0     9721 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_player_card.py
+-rw-r--r--   0        0        0     1502 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py
+-rw-r--r--   0        0        0     3990 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/draw.py
+-rw-r--r--   0        0        0     1431 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/handler.py
+-rw-r--r--   0        0        0      123 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/Atlas/__init__.py
+-rw-r--r--   0        0        0     2029 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py
+-rw-r--r--   0        0        0       37 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/__init__.py
+-rw-r--r--   0        0        0     3357 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py
+-rw-r--r--   0        0        0     5089 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py
+-rw-r--r--   0        0        0      209 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/models.py
+-rw-r--r--   0        0        0    22279 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/__init__.py
+-rw-r--r--   0        0        0     7572 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py
+-rw-r--r--   0        0        0     8754 2023-11-29 04:10:49.880595 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/draw_map.py
+-rw-r--r--   0        0        0      888 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py
+-rw-r--r--   0        0        0      446 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/exc.py
+-rw-r--r--   0        0        0     2600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py
+-rw-r--r--   0        0        0     3573 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py
+-rw-r--r--   0        0        0     4320 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py
+-rw-r--r--   0        0        0     2902 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py
+-rw-r--r--   0        0        0     1231 2023-11-02 02:35:17.358460 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py
+-rw-r--r--   0        0        0     7228 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/bot_manager/__init__.py
+-rw-r--r--   0        0        0     4615 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/news60s/__init__.py
+-rw-r--r--   0        0        0     8537 2023-12-07 12:31:51.791454 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/plugin_manager/__init__.py
+-rw-r--r--   0        0        0     5192 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/plugin_manager/draw_help.py
+-rw-r--r--   0        0        0     1443 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/tools/__init__.py
+-rw-r--r--   0        0        0      607 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/__init__.py
+-rw-r--r--   0        0        0     6214 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/alias.py
+-rw-r--r--   0        0        0    18691 2023-12-07 15:12:48.876317 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/api.py
+-rw-r--r--   0        0        0     3844 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/browser.py
+-rw-r--r--   0        0        0     2695 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/files.py
+-rw-r--r--   0        0        0     2420 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/filter.py
+-rw-r--r--   0        0        0    19469 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/genshin.py
+-rw-r--r--   0        0        0    22406 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/image.py
+-rw-r--r--   0        0        0     1380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/logger.py
+-rw-r--r--   0        0        0    14786 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/message.py
+-rw-r--r--   0        0        0     2380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/path.py
+-rw-r--r--   0        0        0     9531 2023-11-29 04:13:41.406015 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/requests.py
+-rw-r--r--   0        0        0     1254 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/scheduler.py
+-rw-r--r--   0        0        0     1600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/status.py
+-rw-r--r--   0        0        0     5838 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/tool.py
+-rw-r--r--   0        0        0     3829 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/typing.py
+-rw-r--r--   0        0        0     4568 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/update.py
+-rw-r--r--   0        0        0     2576 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.14/LittlePaimon/web/__init__.py
+-rw-r--r--   0        0        0      655 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/__init__.py
+-rw-r--r--   0        0        0     4853 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/bot_info.py
+-rw-r--r--   0        0        0     1807 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/command_alias.py
+-rw-r--r--   0        0        0    15631 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/cookie.py
+-rw-r--r--   0        0        0      791 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/login.py
+-rw-r--r--   0        0        0     6463 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/plugin.py
+-rw-r--r--   0        0        0     1974 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/status.py
+-rw-r--r--   0        0        0     1081 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/utils.py
+-rw-r--r--   0        0        0      112 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/__init__.py
+-rw-r--r--   0        0        0     1651 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/bind_cookie.py
+-rw-r--r--   0        0        0     3525 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/command_alias.py
+-rw-r--r--   0        0        0    16990 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/config_manage.py
+-rw-r--r--   0        0        0      347 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/constants.py
+-rw-r--r--   0        0        0     5482 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/home_page.py
+-rw-r--r--   0        0        0     1903 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/login.py
+-rw-r--r--   0        0        0     1816 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/main.py
+-rw-r--r--   0        0        0     8089 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/plugin_manage.py
+-rw-r--r--   0        0        0     6613 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/private_cookie.py
+-rw-r--r--   0        0        0     3067 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/public_cookie.py
+-rw-r--r--   0        0        0     1251 2024-04-06 04:32:46.440414 mhmzx_little_paimon-3.0.14/pyproject.toml
+-rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 mhmzx_little_paimon-3.0.14/PKG-INFO
```

### Comparing `mhmzx_little_paimon-3.0.13/LICENSE` & `mhmzx_little_paimon-3.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/command/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/command/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/config/manage.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/config/manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/config/model.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/config/model.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/alias.json` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/alias.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9919735338375171%*

 * *Differences: {"'圣遗物'": "{'昔时之歌': ['昔时之歌', '昔时'], '回声之林夜话': ['回声之林夜话', '回声']}",*

 * * "'武器'": "{'有乐御簾切': ['有乐御簾切', '有乐', '御簾切', '千织专武'], '沙中伟贤的对答': ['沙中伟贤的对答', '沙中伟贤', '伟贤', '对答']}",*

 * * "'角色'": "{'10000094': ['千织']}"}*

```diff
@@ -666,14 +666,18 @@
             "\u751f\u547d"
         ],
         "\u534e\u9986\u68a6\u9192\u5f62\u9ab8\u8bb0": [
             "\u534e\u9986\u68a6\u9192\u5f62\u9ab8\u8bb0",
             "\u534e\u9986",
             "\u9632\u5fa1"
         ],
+        "\u56de\u58f0\u4e4b\u6797\u591c\u8bdd": [
+            "\u56de\u58f0\u4e4b\u6797\u591c\u8bdd",
+            "\u56de\u58f0"
+        ],
         "\u5947\u8ff9": [
             "\u5947\u8ff9"
         ],
         "\u5982\u96f7\u7684\u76db\u6012": [
             "\u5982\u96f7\u7684\u76db\u6012",
             "\u5982\u96f7"
         ],
@@ -700,14 +704,18 @@
         "\u6559\u5b98": [
             "\u6559\u5b98"
         ],
         "\u6614\u65e5\u5b97\u5ba4\u4e4b\u4eea": [
             "\u6614\u65e5\u5b97\u5ba4\u4e4b\u4eea",
             "\u5b97\u5ba4"
         ],
+        "\u6614\u65f6\u4e4b\u6b4c": [
+            "\u6614\u65f6\u4e4b\u6b4c",
+            "\u6614\u65f6"
+        ],
         "\u6765\u6b46\u4f59\u54cd": [
             "\u6765\u6b46\u4f59\u54cd",
             "\u666e\u653b",
             "\u4f59\u54cd"
         ],
         "\u67d3\u8840\u7684\u9a91\u58eb\u9053": [
             "\u67d3\u8840\u7684\u9a91\u58eb\u9053",
@@ -1127,14 +1135,20 @@
             "\u66da\u4e91\u5f13"
         ],
         "\u6700\u521d\u7684\u5927\u9b54\u672f": [
             "\u6700\u521d\u7684\u5927\u9b54\u672f",
             "\u6797\u5c3c\u4e13\u6b66",
             "\u5927\u9b54\u672f"
         ],
+        "\u6709\u4e50\u5fa1\u7c3e\u5207": [
+            "\u6709\u4e50\u5fa1\u7c3e\u5207",
+            "\u6709\u4e50",
+            "\u5fa1\u7c3e\u5207",
+            "\u5343\u7ec7\u4e13\u6b66"
+        ],
         "\u677e\u7c41\u54cd\u8d77\u4e4b\u65f6": [
             "\u677e\u7c41\u54cd\u8d77\u4e4b\u65f6",
             "\u677e\u7c41",
             "\u4e50\u56e2\u5927\u5251",
             "\u677e\u5251",
             "\u4f18\u83c8\u4e13\u6b66"
         ],
@@ -1150,14 +1164,20 @@
         "\u6c34\u4ed9\u5341\u5b57\u4e4b\u5251": [
             "\u6c34\u4ed9\u5341\u5b57\u4e4b\u5251",
             "\u6c34\u4ed9"
         ],
         "\u6c90\u6d74\u9f99\u8840\u7684\u5251": [
             "\u6c90\u6d74\u9f99\u8840\u7684\u5251"
         ],
+        "\u6c99\u4e2d\u4f1f\u8d24\u7684\u5bf9\u7b54": [
+            "\u6c99\u4e2d\u4f1f\u8d24\u7684\u5bf9\u7b54",
+            "\u6c99\u4e2d\u4f1f\u8d24",
+            "\u4f1f\u8d24",
+            "\u5bf9\u7b54"
+        ],
         "\u6ce2\u4e71\u6708\u767d\u7ecf\u6d25": [
             "\u6ce2\u4e71\u6708\u767d\u7ecf\u6d25",
             "\u6ce2\u4e71",
             "\u6708\u767d",
             "\u6708\u7ecf\u5251",
             "\u6ce2\u6ce2\u6d25",
             "\u795e\u91cc\u7eeb\u4eba\u4e13\u6b66"
@@ -2041,10 +2061,13 @@
             "\u5a1c\u7ef4\u5a05"
         ],
         "10000092": [
             "\u5609\u660e"
         ],
         "10000093": [
             "\u95f2\u4e91"
+        ],
+        "10000094": [
+            "\u5343\u7ec7"
         ]
     }
 }
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/artifact.json` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/artifact.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/ban_word.txt` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/ban_word.txt`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/genshin_info.json` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/genshin_info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9896907216494846%*

 * *Differences: {"'10000094'": "OrderedDict([('SkillOrder', [10941, 10942, 10945]), ('Skills', "*

 * *               "OrderedDict([('10941', 'Skill_A_01'), ('10942', 'Skill_S_Chiori_01'), ('10945', "*

 * *               "'Skill_E_Chiori_01')])), ('SideIconName', 'UI_AvatarIcon_Side_Chiori')])"}*

```diff
@@ -2536,9 +2536,22 @@
             10935
         ],
         "Skills": {
             "10931": "Skill_A_Catalyst_MD",
             "10932": "Skill_S_Liuyun_01",
             "10935": "Skill_E_Liuyun_01"
         }
+    },
+    "10000094": {
+        "SideIconName": "UI_AvatarIcon_Side_Chiori",
+        "SkillOrder": [
+            10941,
+            10942,
+            10945
+        ],
+        "Skills": {
+            "10941": "Skill_A_01",
+            "10942": "Skill_S_Chiori_01",
+            "10945": "Skill_E_Chiori_01"
+        }
     }
 }
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/prop.json` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/prop.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/role_skill.json` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/role_skill.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9926236044657097%*

 * *Differences: {"'Icon'": "{'20400': 'Btn_HideAndSeekV4_Seeker_S', '20401': 'Btn_HideAndSeekV4_Seeker_S', "*

 * *           "'20411': 'Btn_HideAndSeekV4_Seeker_A_02', '20421': 'Btn_HideAndSeekV4_Seeker_E_02', "*

 * *           "'20422': 'Btn_HideAndSeekV4_Seeker_E_01', '20510': 'Btn_HideAndSeekV4_Hider_A_01', "*

 * *           "'20520': 'Btn_HideAndSeekV4_Hider_E', '20523': 'Btn_HideAndSeekV4_Hider_A_02', "*

 * *           "'20524': 'Btn_HideAndSeekV4_Seeker_A_01', '10941': 'Skill_A_01', '10942': "*

 * *           "'Skill_S_Chiori_01', '10944': ' […]*

```diff
@@ -386,14 +386,18 @@
         "10931": "Skill_A_Catalyst_MD",
         "10932": "Skill_S_Liuyun_01",
         "10933": "Skill_S_Liuyun_02",
         "10934": "Skill_S_Liuyun_04",
         "10935": "Skill_E_Liuyun_01",
         "10936": "Skill_S_Liuyun_03",
         "10937": "Skill_S_Liuyun_05",
+        "10941": "Skill_A_01",
+        "10942": "Skill_S_Chiori_01",
+        "10944": "Skill_S_Chiori_03",
+        "10945": "Skill_E_Chiori_01",
         "11301": "Skill_A_02",
         "11302": "Skill_S_Ambor_01",
         "11305": "Skill_E_Beidou_01",
         "11371": "Skill_A_02",
         "11372": "Skill_S_Razor_01",
         "11373": "Skill_E_Razor_01",
         "11374": "Skill_A_02",
@@ -451,14 +455,16 @@
         "20067": "Skill_Diving_Octopus",
         "20070": "QuesteventSkillIcon_01",
         "20077": "Skill_LanV4PartyLion_01",
         "20080": "QuesteventSkillIcon_01",
         "20082": "",
         "20083": "Skill_LanV4PartyLion_01",
         "20084": "Skill_LanV4PartyLion_01",
+        "20093": "Btn_SlimeCannon_Fire_01",
+        "20094": "Btn_SlimeCannon_Fire_04",
         "20100": "Btn_HideAndSeek_Seeker_A_01",
         "20101": "Btn_HideAndSeek_Seeker_A_01",
         "20110": "Btn_HideAndSeek_Seeker_S_01",
         "20111": "Btn_HideAndSeek_Seeker_S_02",
         "20120": "Btn_HideAndSeek_Seeker_E_01",
         "20121": "Btn_HideAndSeek_Seeker_E_02",
         "20122": "Btn_HideAndSeek_Seeker_E_03",
@@ -495,32 +501,32 @@
         "20352": "Btn_Fishing_Bait",
         "20361": "Skill_E_Klee_01",
         "20362": "Skill_PoetryFestival_PitchPot_Icon01",
         "20363": "Skill_E_Klee_01",
         "20364": "Skill_E_BubbleGun_01",
         "20365": "Btn_Recon_Bait",
         "20366": "Btn_Recon_Bait",
-        "20400": "Btn_HideAndSeek_Seeker_A_01",
-        "20401": "Btn_HideAndSeek_Seeker_A_01",
+        "20400": "Btn_HideAndSeekV4_Seeker_S",
+        "20401": "Btn_HideAndSeekV4_Seeker_S",
         "20410": "Btn_HideAndSeek_Seeker_S_01",
-        "20411": "Btn_HideAndSeek_Seeker_S_02",
+        "20411": "Btn_HideAndSeekV4_Seeker_A_02",
         "20420": "Btn_HideAndSeek_Seeker_E_01",
-        "20421": "Btn_HideAndSeek_Seeker_E_02",
-        "20422": "Btn_HideAndSeek_Seeker_E_03",
+        "20421": "Btn_HideAndSeekV4_Seeker_E_02",
+        "20422": "Btn_HideAndSeekV4_Seeker_E_01",
         "20500": "Btn_HideAndSeek_Hider_A_01",
         "20501": "Btn_HideAndSeek_Hider_A_03",
-        "20510": "Btn_HideAndSeek_Hider_S_01",
+        "20510": "Btn_HideAndSeekV4_Hider_A_01",
         "20511": "Btn_HideAndSeek_Hider_S_02",
         "20512": "Btn_HideAndSeek_Hider_S_01_Borbid",
         "20513": "Btn_HideAndSeek_Hider_S_02_Borbid",
-        "20520": "Btn_HideAndSeek_Hider_E_01",
+        "20520": "Btn_HideAndSeekV4_Hider_E",
         "20521": "UI_Icon_Skill_Hunter_Net",
         "20522": "Btn_HideAndSeek_Hider_S_02",
-        "20523": "UI_Icon_Skill_Prey_Invisible_Bait",
-        "20524": "Btn_HideAndSeek_Seeker_S_01",
+        "20523": "Btn_HideAndSeekV4_Hider_A_02",
+        "20524": "Btn_HideAndSeekV4_Seeker_A_01",
         "20525": "Btn_HideAndSeek_Hider_A_01",
         "20526": "Btn_HideAndSeek_Hider_A_03",
         "20527": "Skill_CarpJump_02",
         "20528": "Skill_C_FairyGadgetSet",
         "20529": "Btn_Fishing_Exit",
         "20530": "Skill_CarpJump_01",
         "20531": "Btn_Fishing_Exit",
@@ -615,15 +621,16 @@
         "5086010": "Skill_A_Catalyst_MD",
         "5087010": "Skill_A_Catalyst_MD",
         "5088010": "Skill_A_Catalyst_MD",
         "5089010": "Skill_A_01",
         "5090010": "Skill_A_03",
         "5091010": "Skill_A_04",
         "5092010": "Skill_A_04",
-        "5093010": "Skill_A_Catalyst_MD"
+        "5093010": "Skill_A_Catalyst_MD",
+        "5094010": "Skill_A_01"
     },
     "Name": {
         "10001": "\u5355\u624b\u5251\u91cd\u653b\u51fb",
         "10002": "\u957f\u67aa\u91cd\u653b\u51fb",
         "10003": "\u6cd5\u5668\u91cd\u51fb",
         "10004": "\u53cc\u624b\u5251\u5355\u6b21\u91cd\u51fb",
         "10006": "\u84c4\u529b\u6280\u80fd\u6559\u5b66\u89e6\u53d1\u5668",
@@ -1008,14 +1015,18 @@
         "10931": "\u666e\u901a\u653b\u51fb\u00b7\u6e05\u98ce\u6563\u82b1\u8bcd",
         "10932": "\u671d\u8d77\u9e64\u4e91",
         "10933": "\u7559\u4e91\u5143\u7d20\u6218\u6280_\u7b2c\u4e8c\u8df3",
         "10934": "\u7559\u4e91\u5143\u7d20\u6218\u6280_\u9e64\u5f62\u8ffd\u51fb",
         "10935": "\u66ae\u96c6\u7af9\u661f",
         "10936": "\u7559\u4e91\u5143\u7d20\u6218\u6280_\u7b2c\u4e09\u8df3",
         "10937": "\u7559\u4e91\u547d6_\u5730\u9762\u7b2c\u4e00\u8df3",
+        "10941": "\u666e\u901a\u653b\u51fb\u00b7\u5fc3\u7ec7\u5200\u6d41",
+        "10942": "\u7fbd\u8896\u4e00\u89e6",
+        "10944": "\u5343\u7ec7\u4e8c\u6bb5E\u540e-\u6280\u80fd\u66ff\u6362",
+        "10945": "\u4e8c\u5200\u4e4b\u5f62\u00b7\u6bd4\u7ffc",
         "11301": "\u83f2\u8c22\u5c14\u666e\u653b",
         "11302": "\u83f2\u8c22\u5c14\u5c0f\u6280\u80fd",
         "11305": "\u83f2\u8c22\u5c14\u5145\u80fd\u6280",
         "11371": "Rx\u767d\u76d2\u6d4b\u8bd5\u666e\u653b",
         "11372": "Rx\u767d\u76d2\u6d4b\u8bd5\u6280\u80fd1",
         "11373": "Rx\u767d\u76d2\u6d4b\u8bd5\u6280\u80fd2",
         "11374": "Rx\u767d\u76d2\u8fdb\u5165\u7784\u51c6",
@@ -1073,14 +1084,16 @@
         "20067": "4.2 \u9646\u5730\u7ae0\u9c7c-\u55b7\u5c04\u80fd\u529b",
         "20070": "\u63a2\u67e5\u6280\u80fd",
         "20077": "4.4\u6d77\u706f\u8282-\u53d8\u8eab\u6280\u80fd-\u91d1\u5e01\u5173",
         "20080": "\u63a2\u67e5\u6280\u80fd",
         "20082": "4.2\u6c34\u4e0b\u5f39\u5c04",
         "20083": "4.4\u6d77\u706f\u8282-\u53d8\u8eab\u6280\u80fd-\u79ef\u5206\u5173",
         "20084": "4.4\u6d77\u706f\u8282-\u53d8\u8eab\u6280\u80fd-\u751f\u5b58\u5173",
+        "20093": "4.5\u53f2\u83b1\u59c6\u7403-\u5143\u7d20\u5f39",
+        "20094": "4.5\u53f2\u83b1\u59c6\u7403-\u7269\u7406\u8fde\u5c04",
         "20100": "\u6355\u83b7\uff01",
         "20101": "\u6355\u83b7\uff01",
         "20110": "\u795e\u79d8\u9884\u611f",
         "20111": "\u611f\u5e94\u5149\u73af",
         "20120": "\u72e9\u730e\u76f4\u89c9",
         "20121": "\u6d1e\u5bdf\u5168\u5c40",
         "20122": "\u7981\u9522\u8bc5\u5492",
@@ -1237,10 +1250,11 @@
         "5086010": "\u83b1\u6b27\u65af\u5229\u7a7a\u4e2d\u653b\u51fb",
         "5087010": "\u90a3\u7ef4\u83b1\u7279\u7a7a\u4e2d\u653b\u51fb",
         "5088010": "\u590f\u6d1b\u8482\u7a7a\u4e2d\u653b\u51fb",
         "5089010": "\u8299\u5b81\u5a1c\u7a7a\u4e2d\u653b\u51fb",
         "5090010": "\u590f\u6c83\u857e\u7a7a\u4e2d\u653b\u51fb",
         "5091010": "\u5a1c\u7ef4\u5a05\u7a7a\u4e2d\u653b\u51fb",
         "5092010": "\u5609\u660e\u7a7a\u4e2d\u653b\u51fb",
-        "5093010": "\u95f2\u4e91\u7a7a\u4e2d\u653b\u51fb"
+        "5093010": "\u95f2\u4e91\u7a7a\u4e2d\u653b\u51fb",
+        "5094010": "\u5343\u7ec7\u7a7a\u4e2d\u653b\u51fb"
     }
 }
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/role_talent.json` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/role_talent.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940476190476191%*

 * *Differences: {"'Icon'": "{'941': 'UI_Talent_S_Chiori_01', '942': 'UI_Talent_S_Chiori_03', '943': "*

 * *           "'UI_Talent_U_Chiori_01', '944': 'UI_Talent_S_Chiori_02', '945': "*

 * *           "'UI_Talent_U_Chiori_02', '946': 'UI_Talent_S_Chiori_04'}",*

 * * "'Name'": "{'941': '正绢六通', '942': '落染五色', '943': '缀锦四分', '944': '衣裁三礼', '945': '绫羽二重', '946': "*

 * *           "'万理一空'}"}*

```diff
@@ -492,14 +492,20 @@
         "931": "UI_Talent_S_Liuyun_01",
         "932": "UI_Talent_S_Liuyun_02",
         "933": "UI_Talent_U_Liuyun_02",
         "934": "UI_Talent_S_Liuyun_03",
         "935": "UI_Talent_U_Liuyun_01",
         "936": "UI_Talent_S_Liuyun_04",
         "94": "UI_Talent_S_PlayerRock_03",
+        "941": "UI_Talent_S_Chiori_01",
+        "942": "UI_Talent_S_Chiori_03",
+        "943": "UI_Talent_U_Chiori_01",
+        "944": "UI_Talent_S_Chiori_02",
+        "945": "UI_Talent_U_Chiori_02",
+        "946": "UI_Talent_S_Chiori_04",
         "95": "UI_Talent_U_PlayerRock_01",
         "96": "UI_Talent_S_PlayerRock_04"
     },
     "Name": {
         "101": "\u4e30\u7a70\u7684\u6625\u96f7",
         "102": "\u9707\u6012\u7684\u82cd\u96f7",
         "103": "\u8fde\u5ef6\u7684\u8fdc\u96f7",
@@ -992,11 +998,17 @@
         "931": "\u501f\u98ce\u6d17\u5c18\u7f18",
         "932": "\u9e64\u5533\u8fdc\u4eba\u95f4",
         "933": "\u9020\u5316\u6709\u661f\u6708",
         "934": "\u5965\u5999\u70f9\u9ecd\u73e0",
         "935": "\u65cb\u6b65\u971e\u851a\u4e0a",
         "936": "\u77e5\u662f\u7559\u4e91\u50ca",
         "94": "\u9669\u5cfb\u7684\u91cd\u5ca9",
+        "941": "\u6b63\u7ee2\u516d\u901a",
+        "942": "\u843d\u67d3\u4e94\u8272",
+        "943": "\u7f00\u9526\u56db\u5206",
+        "944": "\u8863\u88c1\u4e09\u793c",
+        "945": "\u7eeb\u7fbd\u4e8c\u91cd",
+        "946": "\u4e07\u7406\u4e00\u7a7a",
         "95": "\u5929\u5760\u4e4b\u5ca9",
         "96": "\u6c38\u4e16\u7684\u78d0\u5ca9"
     }
 }
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/roles_data.json` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/roles_data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'千织'": "OrderedDict([('region', '枫丹'), ('star', 5), ('element', '岩')])"}*

```diff
@@ -5274,14 +5274,19 @@
             "\u7483\u6708\u4e0e\u7a3b\u59bb\u4e2d\u6d41\u4f20\u7740\u4e00\u53e5\u77ed\u8bed\uff1a\u300c\u9ccd\u5316\u51a5\u6d77\uff0c\u5c3e\u70b9\u8fdc\u5c71\u300d\u3002\u6e14\u4eba\u4ece\u5cb8\u4e0a\u5b66\u6765\u8fd9\u53e5\uff0c\u7ffb\u6765\u8986\u53bb\u5730\u5531\u3002\u66f2\u5b50\u8d8a\u4f20\u8d8a\u8fdc\uff0c\u6210\u4e3a\u810d\u7099\u4eba\u53e3\u7684\u6e14\u6b4c\u3002\u6bcf\u5230\u6d77\u4e0a\u8d77\u96fe\uff0c\u6e14\u6c11\u4eec\u7684\u5c0f\u8239\u9690\u6ca1\u5728\u767d\u96fe\u91cc\uff0c\u6b4c\u58f0\u9065\u9065\u4f20\u6765\uff1a\u9ccd\u5316\u51a5\u6d77\uff0c\u5c3e\u70b9\u8fdc\u5c71\u2026\u8fd9\u9996\u6b4c\u4fbf\u662f\u5317\u6597\u7684\u6447\u7bee\u66f2\u3002\u5ca9\u738b\u5e1d\u541b\u795e\u5251\u65a9\u6d77\u602a\uff0c\u7483\u6708\u4eba\u5c06\u4e4b\u4f20\u4e3a\u7f8e\u8c08\u3002\u5e74\u5e7c\u7684\u5317\u6597\u7231\u542c\u795e\u8bdd\uff0c\u7761\u89c9\u4e5f\u60f3\u7740\uff1a\u603b\u6709\u4e00\u5929\u5f97\u89c1\u89c1\u8fd9\u6761\u5927\u9c7c\u3002\u4eca\u5929\uff0c\u5979\u5374\u7528\u53e6\u4e00\u79cd\u5fc3\u60c5\u5531\u8d77\u8fd9\u9996\u6b4c\u3002\u5168\u8239\u6d77\u5458\u8ddf\u7740\u54fc\u5531\uff0c\u626c\u5e06\u8d77\u822a\u3002\u6d77\u5c71\u5c31\u5728\u6d77\u4e2d\u3002\u5b83\u65e2\u50cf\u9c7c\u4e5f\u50cf\u9f99\uff0c\u5e9e\u5927\u5982\u5669\u68a6\uff0c\u529b\u5927\u5982\u795e\u7075\uff0c\u8f7b\u8f7b\u4e00\u51fb\u4fbf\u80fd\u6380\u8d77\u6570\u5341\u7c73\u9ad8\u7684\u5de8\u6d6a\u3002\u5728\u6d77\u4e0a\u640f\u547d\u7684\u4eba\uff0c\u603b\u4f1a\u4e0e\u6d77\u5c71\u76f8\u9047\u3002\u5317\u6597\u4ece\u4e5d\u5c81\u5c31\u60f3\u89c1\u5b83\uff0c\u76fc\u7740\u80fd\u5c06\u5b83\u7684\u5934\u9885\u4e00\u5200\u65a9\u4e0b\u3002\u5979\u66fe\u591a\u6b21\u6311\u6218\u6d77\u5c71\uff0c\u5747\u4ee5\u5931\u8d25\u544a\u7ec8\u3002\u4eca\u5929\u5374\u4e0d\u540c\uff0c\u5317\u6597\u80cc\u4e0a\u6700\u597d\u7684\u5927\u5251\uff0c\u5e26\u4e0a\u6700\u901a\u6c34\u6027\u7684\u6c34\u624b\uff0c\u76f4\u5954\u6d77\u5c71\u800c\u53bb\u3002\u77ed\u5175\u76f8\u63a5\uff0c\u4e00\u6218\u60ca\u96f7\u3002\u8fd9\u573a\u6218\u6597\u6301\u7eed\u4e86\u6574\u6574\u56db\u5929\u3002\u8239\u961f\u643a\u5e26\u5927\u70ae\u3001\u6e14\u67aa\uff0c\u8f85\u4ee5\u5f13\u7bad\u548c\u7ef3\u7d22\uff0c\u5168\u529b\u7275\u5236\u6d77\u5c71\u3002\u5317\u6597\u4e0e\u56db\u8db3\u88ab\u7f1a\u7684\u6d77\u5c71\u7f20\u6597\u6570\u4e2a\u65f6\u8fb0\uff0c\u76f4\u81f3\u5929\u9ed1\u4e5f\u6ca1\u80fd\u5206\u51fa\u80dc\u8d1f\u3002\u591c\u665a\u662f\u6d77\u5c71\u6700\u5371\u9669\u7684\u65f6\u523b\u3002\u4eba\u4eec\u63d0\u9632\u7740\u6d77\u5c71\u7684\u8fdb\u72af\uff0c\u6574\u591c\u4e0d\u6562\u5165\u7761\u3002\u5317\u6597\u7ad9\u5728\u8239\u5934\uff0c\u8046\u542c\u98ce\u58f0\u3002\u4e00\u51fb\uff0c\u53ea\u8981\u4e00\u51fb\u3002\u5979\u5728\u5bd2\u98ce\u4e2d\u4e00\u52a8\u4e0d\u52a8\u5730\u7b49\u5f85\u3002\u4e0d\u77e5\u8fc7\u53bb\u591a\u4e45\uff0c\u7c92\u7c73\u672a\u8fdb\u3001\u6ef4\u6c34\u672a\u6cbe\u7684\u5317\u6597\u7cbe\u51c6\u6355\u6349\u5230\u592a\u9633\u5347\u8d77\u5239\u90a3\uff0c\u6d77\u4e2d\u4f20\u6765\u7684\u6d6a\u82b1\u58f0\u3002\u8fd9\u4e00\u51fb\uff0c\u7834\u4e91\u65a9\u6708\uff0c\u5982\u5c71\u5982\u6d77\uff0c\u5c06\u9c7c\u9f99\u7684\u5934\u9885\u5f7b\u5e95\u780d\u65ad\uff01\u4f34\u968f\u6f2b\u5929\u60ca\u96f7\uff0c\u4e00\u9053\u7d2b\u7535\u81ea\u534a\u7a7a\u964d\u4e0b\uff0c\u51dd\u805a\u5728\u6d74\u8840\u7684\u5317\u6597\u9762\u524d\u3002\u5c60\u9f99\u8005\u5317\u6597\u7684\u300c\u795e\u4e4b\u773c\u300d\u81ea\u5929\u4e0a\u800c\u6765\uff0c\u6709\u7740\u96f7\u7535\u822c\u593a\u76ee\u7684\u7d2b\u5149\uff0c\u662f\u9f99\u8840\u4e5f\u65e0\u6cd5\u5339\u654c\u7684\u5b9d\u73e0\u3002\u8fd9\u9897\u795e\u7389\uff0c\u53ea\u5e94\u8d60\u7ed9\u5c71\u4e0e\u6d77\u7684\u5f81\u670d\u8005\u3002"
         ],
         "tag": "\u62a4\u76fe\u3001\u51cf\u6297\u3001\u6297\u6253\u65ad\u3001\u4f24\u5bb3\u51cf\u514d\u3001\u6e38\u6cf3\u6d88\u8017\u51cf\u5c11\u3001\u534f\u540c\u653b\u51fb\u3001\u5f39\u53cd\u3001\u81ea\u8eab\u4f24\u5bb3\u63d0\u5347",
         "title": "\u65e0\u5195\u7684\u9f99\u738b",
         "type": "\u5e38\u9a7bUP",
         "weapon": "\u53cc\u624b\u5251"
     },
+    "\u5343\u7ec7": {
+        "element": "\u5ca9",
+        "region": "\u67ab\u4e39",
+        "star": 5
+    },
     "\u5361\u7ef4": {
         "attribute": {
             "atk": {
                 "1": "",
                 "20": "",
                 "40": "",
                 "50": "",
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/score.json` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/score.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'Talent'": "{'千织': [0, 1]}"}*

```diff
@@ -804,14 +804,18 @@
             2,
             1
         ],
         "\u5317\u6597": [
             1,
             2
         ],
+        "\u5343\u7ec7": [
+            0,
+            1
+        ],
         "\u5361\u7ef4": [
             2,
             1
         ],
         "\u53ef\u8389": [
             1,
             2
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/upheaval.json` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/upheaval.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/weapon.json` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/weapon.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947532204371111%*

 * *Differences: {"'Icon'": "{'有乐御簾切': 'UI_EquipIcon_Sword_Needle', '沙中伟贤的对答': 'UI_EquipIcon_Pole_Caduceus'}",*

 * * "'Name'": "{'1818340435': '有乐御簾切', '2847771107': '沙中伟贤的对答'}",*

 * * "'Type'": "{'有乐御簾切': '单手剑', '沙中伟贤的对答': '长柄武器'}"}*

```diff
@@ -69,19 +69,21 @@
         "\u662d\u5fc3": "UI_EquipIcon_Catalyst_Truelens",
         "\u6697\u5df7\u730e\u624b": "UI_EquipIcon_Bow_Outlaw",
         "\u6697\u5df7\u7684\u9152\u4e0e\u8bd7": "UI_EquipIcon_Catalyst_Outlaw",
         "\u6697\u5df7\u95ea\u5149": "UI_EquipIcon_Sword_Outlaw",
         "\u6697\u94c1\u5251": "UI_EquipIcon_Sword_Darker",
         "\u66da\u4e91\u4e4b\u6708": "UI_EquipIcon_Bow_Maria",
         "\u6700\u521d\u7684\u5927\u9b54\u672f": "UI_EquipIcon_Bow_Pledge",
+        "\u6709\u4e50\u5fa1\u7c3e\u5207": "UI_EquipIcon_Sword_Needle",
         "\u677e\u7c41\u54cd\u8d77\u4e4b\u65f6": "UI_EquipIcon_Claymore_Widsith",
         "\u6842\u6728\u65a9\u957f\u6b63": "UI_EquipIcon_Claymore_Bakufu",
         "\u68ee\u6797\u738b\u5668": "UI_EquipIcon_Claymore_Arakalari",
         "\u6c34\u4ed9\u5341\u5b57\u4e4b\u5251": "UI_EquipIcon_Sword_Purewill",
         "\u6c90\u6d74\u9f99\u8840\u7684\u5251": "UI_EquipIcon_Claymore_Siegfry",
+        "\u6c99\u4e2d\u4f1f\u8d24\u7684\u5bf9\u7b54": "UI_EquipIcon_Pole_Caduceus",
         "\u6ce2\u4e71\u6708\u767d\u7ecf\u6d25": "UI_EquipIcon_Sword_Amenoma",
         "\u6d41\u6708\u9488": "UI_EquipIcon_Pole_Exotic",
         "\u6d41\u6d6a\u4e50\u7ae0": "UI_EquipIcon_Catalyst_Troupe",
         "\u6d41\u6d6a\u7684\u665a\u661f": "UI_EquipIcon_Catalyst_Pleroma",
         "\u6d4b\u8ddd\u89c4": "UI_EquipIcon_Bow_Mechanic",
         "\u6d6a\u5f71\u9614\u5251": "UI_EquipIcon_Claymore_Vorpal",
         "\u6d77\u6e0a\u7ec8\u66f2": "UI_EquipIcon_Sword_Vorpal",
@@ -219,14 +221,15 @@
         "1595734083": "(test)\u7a7f\u6a21\u6d4b\u8bd5",
         "1600275315": "\u6ce2\u4e71\u6708\u767d\u7ecf\u6d25",
         "160493219": "\u6697\u94c1\u5251",
         "1608953539": "\u9ece\u660e\u795e\u5251",
         "1675686363": "\u796d\u793c\u5927\u5251",
         "1773425155": "\u964d\u4e34\u4e4b\u5251",
         "1790067483": "\u8239\u575e\u957f\u5251",
+        "1818340435": "\u6709\u4e50\u5fa1\u7c3e\u5207",
         "1860795787": "\u66da\u4e91\u4e4b\u6708",
         "1890163363": "\u4e0d\u706d\u6708\u534e",
         "1901973075": "\u51ac\u6781\u767d\u661f",
         "1921306659": "\u7070\u6cb3\u6e21\u624b",
         "197755235": "\u8d2f\u8679\u4e4b\u69ca",
         "1990641987": "\u796d\u793c\u5251",
         "1990820123": "\u5929\u76ee\u5f71\u6253\u5200",
@@ -269,14 +272,15 @@
         "2749853923": "\u8150\u6b96\u4e4b\u5251",
         "2753539619": "\u96ea\u846c\u7684\u661f\u94f6",
         "275622963": "\u88c1\u53f6\u8403\u5149",
         "2792766467": "\u65e0\u5de5\u4e4b\u5251",
         "2796697027": "\u65b0\u624b\u957f\u67aa",
         "2832648187": "\u5b97\u5ba4\u957f\u5f13",
         "2834063555": "\u82c7\u6d77\u4fe1\u6807",
+        "2847771107": "\u6c99\u4e2d\u4f1f\u8d24\u7684\u5bf9\u7b54",
         "2918525947": "\u98de\u96f7\u4e4b\u5f26\u632f",
         "2935286715": "\u5b97\u5ba4\u730e\u67aa",
         "2947140987": "\u6697\u5df7\u95ea\u5149",
         "2949448555": "\u82cd\u53e4\u81ea\u7531\u4e4b\u8a93",
         "2958179435": "\u70c8\u9633\u4e4b\u55e3",
         "2963220587": "\u7fe1\u7389\u6cd5\u7403",
         "2988480723": "\u6700\u521d\u7684\u5927\u9b54\u672f",
@@ -453,19 +457,21 @@
         "\u662d\u5fc3": "\u6cd5\u5668",
         "\u6697\u5df7\u730e\u624b": "\u5f13",
         "\u6697\u5df7\u7684\u9152\u4e0e\u8bd7": "\u6cd5\u5668",
         "\u6697\u5df7\u95ea\u5149": "\u5355\u624b\u5251",
         "\u6697\u94c1\u5251": "\u5355\u624b\u5251",
         "\u66da\u4e91\u4e4b\u6708": "\u5f13",
         "\u6700\u521d\u7684\u5927\u9b54\u672f": "\u5f13",
+        "\u6709\u4e50\u5fa1\u7c3e\u5207": "\u5355\u624b\u5251",
         "\u677e\u7c41\u54cd\u8d77\u4e4b\u65f6": "\u53cc\u624b\u5251",
         "\u6842\u6728\u65a9\u957f\u6b63": "\u53cc\u624b\u5251",
         "\u68ee\u6797\u738b\u5668": "\u53cc\u624b\u5251",
         "\u6c34\u4ed9\u5341\u5b57\u4e4b\u5251": "\u5355\u624b\u5251",
         "\u6c90\u6d74\u9f99\u8840\u7684\u5251": "\u53cc\u624b\u5251",
+        "\u6c99\u4e2d\u4f1f\u8d24\u7684\u5bf9\u7b54": "\u957f\u67c4\u6b66\u5668",
         "\u6ce2\u4e71\u6708\u767d\u7ecf\u6d25": "\u5355\u624b\u5251",
         "\u6d41\u6708\u9488": "\u957f\u67c4\u6b66\u5668",
         "\u6d41\u6d6a\u4e50\u7ae0": "\u6cd5\u5668",
         "\u6d41\u6d6a\u7684\u665a\u661f": "\u6cd5\u5668",
         "\u6d4b\u8ddd\u89c4": "\u5f13",
         "\u6d6a\u5f71\u9614\u5251": "\u53cc\u624b\u5251",
         "\u6d77\u6e0a\u7ec8\u66f2": "\u5355\u624b\u5251",
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/data/类型.json` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/类型.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978532608695652%*

 * *Differences: {"'武器'": "{'单手剑': {insert: [(41, '有乐御簾切')]}, '长柄武器': {insert: [(29, '沙中伟贤的对答')]}}",*

 * * "'角色'": "{'武器类型': {'单手剑': {insert: [(22, '千织')]}}, '元素类型': {'岩': {insert: [(9, '千织')]}}}"}*

```diff
@@ -37,15 +37,16 @@
             "\u5723\u663e\u4e4b\u94a5",
             "\u88c1\u53f6\u8403\u5149",
             "\u72fc\u7259",
             "\u6d77\u6e0a\u7ec8\u66f2",
             "\u7070\u6cb3\u6e21\u624b",
             "\u8239\u575e\u957f\u5251",
             "\u6c34\u4ed9\u5341\u5b57\u4e4b\u5251",
-            "\u9759\u6c34\u6d41\u6d8c\u4e4b\u8f89"
+            "\u9759\u6c34\u6d41\u6d8c\u4e4b\u8f89",
+            "\u6709\u4e50\u5fa1\u7c3e\u5207"
         ],
         "\u53cc\u624b\u5251": [
             "\u8bad\u7ec3\u5927\u5251",
             "\u4f63\u5175\u91cd\u5251",
             "\u94c1\u5f71\u9614\u5251",
             "\u6c90\u6d74\u9f99\u8840\u7684\u5251",
             "\u767d\u94c1\u5927\u5251",
@@ -180,15 +181,16 @@
             "\u8d2f\u8679\u4e4b\u69ca",
             "\u548c\u749e\u9e22",
             "\u606f\u707e",
             "\u8599\u8349\u4e4b\u7a3b\u5149",
             "\u8d64\u6c99\u4e4b\u6756",
             "\u5ce1\u6e7e\u957f\u6b4c",
             "\u516c\u4e49\u7684\u916c\u62a5",
-            "\u52d8\u63a2\u94bb\u673a"
+            "\u52d8\u63a2\u94bb\u673a",
+            "\u6c99\u4e2d\u4f1f\u8d24\u7684\u5bf9\u7b54"
         ]
     },
     "\u89d2\u8272": {
         "\u5143\u7d20\u7c7b\u578b": {
             "\u51b0": [
                 "\u795e\u91cc\u7eeb\u534e",
                 "\u51ef\u4e9a",
@@ -211,15 +213,16 @@
                 "\u949f\u79bb",
                 "\u8bfa\u827e\u5c14",
                 "\u963f\u8d1d\u591a",
                 "\u4e94\u90ce",
                 "\u8352\u6cf7\u4e00\u6597",
                 "\u4e91\u5807",
                 "\u65c5\u884c\u8005\u5ca9",
-                "\u5a1c\u7ef4\u5a05"
+                "\u5a1c\u7ef4\u5a05",
+                "\u5343\u7ec7"
             ],
             "\u6c34": [
                 "\u82ad\u82ad\u62c9",
                 "\u884c\u79cb",
                 "\u8fbe\u8fbe\u5229\u4e9a",
                 "\u83ab\u5a1c",
                 "\u73ca\u745a\u5bab\u5fc3\u6d77",
@@ -304,15 +307,16 @@
                 "\u65c5\u884c\u8005\u98ce",
                 "\u65c5\u884c\u8005\u5ca9",
                 "\u65c5\u884c\u8005\u96f7",
                 "\u65c5\u884c\u8005\u8349",
                 "\u65c5\u884c\u8005\u6c34",
                 "\u7eee\u826f\u826f",
                 "\u7433\u59ae\u7279",
-                "\u8299\u5b81\u5a1c"
+                "\u8299\u5b81\u5a1c",
+                "\u5343\u7ec7"
             ],
             "\u53cc\u624b\u5251": [
                 "\u8fea\u5362\u514b",
                 "\u96f7\u6cfd",
                 "\u5317\u6597",
                 "\u8bfa\u827e\u5c14",
                 "\u91cd\u4e91",
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/plugin/manage.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/plugin/manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/config/plugin/model.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/config/plugin/model.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/database/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/abyss_info.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/abyss_info.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/character.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/character.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/cookie.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/genshin_voice.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/genshin_voice.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/manage.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/other.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/other.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/player_info.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/player_info.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/database/models/subscription.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/subscription.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/event.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/event.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/generate.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/generate.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/template/index.css` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/index.css`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/template/iview.css` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/iview.css`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Voice/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Voice/draw.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Voice/handler.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Genshin_Voice/resources.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/resources.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/config.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/config.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/genshin_word.txt` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/genshin_word.txt`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/handler.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/models.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/models.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/web_api.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/web_api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Learning_Chat/web_page.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/web_page.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Mihoyo_bbs/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Mihoyo_bbs/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/NoticeAndRequest/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/NoticeAndRequest/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/NoticeAndRequest/config.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/NoticeAndRequest/config.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Autobbs/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Autobbs/draw.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Bind/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Bind/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Bind/get_cookie.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Bind/get_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_CloudGenshin/api.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_DailyNote/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_DailyNote/draw.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_DailyNote/handler.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha/data_handle.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/data_handle.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha/data_source.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/data_source.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha/draw.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,18 @@
 
     :param user_id: 用户id
     :param uid: 原神uid
     :return: 抽卡记录数据
     """
     file_path = GACHA_LOG / f'gacha_log-{user_id}-{uid}.json'
     if file_path.exists():
-        return GachaLogInfo.parse_obj(load_json(file_path)), True
+        old_gacha_info = load_json(file_path)
+        if "集录祈愿" not in old_gacha_info["item_list"]:
+            old_gacha_info["item_list"]["集录祈愿"] = []
+        return GachaLogInfo.parse_obj(old_gacha_info), True
     else:
         return GachaLogInfo(user_id=user_id,
                             uid=uid,
                             update_time=datetime.datetime.now()), False
 
 
 def save_gacha_log_info(user_id: str, uid: str, info: GachaLogInfo):
@@ -130,14 +133,15 @@
     await LastQuery.update_last_query(user_id, uid)
     new_num = 0
     type_new_num = {
         '角色祈愿': 0,
         '武器祈愿': 0,
         '常驻祈愿': 0,
         '新手祈愿': 0,
+        '集录祈愿': 0
     }
     server_id = 'cn_qd01' if uid[0] == '5' else 'cn_gf01'
     authkey, state, cookie_info = await get_authkey_by_stoken(user_id, uid)
     if not state:
         return authkey
     gacha_log, _ = load_history_info(user_id, uid)
     params = PARAMS.copy()
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from LittlePaimon.utils.image import PMImage, get_qq_avatar, font_manager as fm, load_image
 from LittlePaimon.utils.message import MessageBuild
 from LittlePaimon.utils.path import RESOURCE_BASE_PATH
 from .models import GachaLogInfo, FiveStarItem, FourStarItem
 
 avatar_point = [69, 156, 259, 358, 456, 558, 645, 746, 840, 945]
 line_point = [88, 182, 282, 378, 477, 574, 673, 769, 864, 967]
-bar_color = [('#b6d6f2', '#3d6e99'), ('#c8b6f2', '#593d99'), ('#abede0', '#3a9382')]
+bar_color = [('#b6d6f2', '#3d6e99'), ('#c8b6f2', '#593d99'), ('#abede0', '#3a9382'), ("#e3d809", "#646C04")]
 name_level_color = [('#f6b9c9', '#a90d35'), ('#f2cab9', '#ff6f30'), ('#b9d8f2', '#157eaa'), ('#dedede', '#707070')]
 small_avatar_cache = {}
 """
     角色  武器
 欧 50以下 45以下
 吉 50-60 45-55
 中 60-70 55-65
@@ -157,22 +157,22 @@
     await img.to_circle('circle')
     await bg.paste(img, (34, 26))
     await bg.text(info.name, (0, bg.width), 163, fm.get('hywh', 24), '#221a33', 'center')
     await bg.text(str(info.num['角色祈愿']), (4, 64), 209, fm.get('bahnschrift_regular', 36, 'Bold'), '#3d6e99',
                   'center')
     await bg.text(str(info.num['武器祈愿']), (65, 125), 209, fm.get('bahnschrift_regular', 36, 'Bold'), '#593d99',
                   'center')
-    await bg.text(str(info.num['常驻祈愿'] + info.num['新手祈愿']), (126, 186), 209, fm.get('bahnschrift_regular', 36, 'Bold'),
+    await bg.text(str(info.num['常驻祈愿'] + info.num['新手祈愿'] + info.num['集录祈愿']), (126, 186), 209, fm.get('bahnschrift_regular', 36, 'Bold'),
                   '#3a9381',
                   'center')
     return bg
 
 
 async def draw_four_star_detail(data: List[FourStarItem]):
-    data.sort(key=lambda x: x.num['角色祈愿'] + x.num['武器祈愿'] + x.num['常驻祈愿'] + x.num['新手祈愿'], reverse=True)
+    data.sort(key=lambda x: x.num['角色祈愿'] + x.num['武器祈愿'] + x.num['常驻祈愿'] + x.num['新手祈愿'] + x.num['集录祈愿'], reverse=True)
     bar = await load_image(RESOURCE_BASE_PATH / 'gacha_log' / 'four_star_bar.png')
     total_height = 105 + 260 * math.ceil(len(data) / 5)
     bg = PMImage(size=(1008, total_height), mode='RGBA', color=(255, 255, 255, 0))
     await bg.paste(bar, (0, 0))
     await asyncio.gather(*[bg.paste(await draw_four_star(data[i]), (i % 5 * 204, 105 + i // 5 * 260)) for i in range(len(data))])
     return bg
 
@@ -217,16 +217,17 @@
     lucky = '欧' if lucky_num <= 50 else '吉' if lucky_num <= 60 else '中' if lucky_num <= 70 else '非'
     await img.paste(await load_image(RESOURCE_BASE_PATH / 'gacha_log' / f'{lucky}{random.randint(1, 3)}.png'), (788, 271))
     four_star_detail = await draw_four_star_detail(list(data4.values()))
     if total_five_star_count:
         chara_pool_per = round(len(data5['角色祈愿']) / total_five_star_count * 100, 1)
         weapon_pool_per = round(len(data5['武器祈愿']) / total_five_star_count * 100, 1)
         new_pool_per = round((len(data5['常驻祈愿']) + len(data5['新手祈愿'])) / total_five_star_count * 100, 1)
+        jilu_pool_per = round(len(data5['集录祈愿']) / total_five_star_count * 100, 1)
         now_used_width = 56
-        pers = [chara_pool_per, weapon_pool_per, new_pool_per]
+        pers = [chara_pool_per, weapon_pool_per, new_pool_per, jilu_pool_per]
         i = 0
         for per in pers:
             if per >= 3:
                 await img.draw_rectangle((now_used_width, 399, now_used_width + int(per / 100 * 967), 446),
                                          bar_color[i][0])
                 if per >= 10:
                     await img.text(f'{per}%', now_used_width + 18, 410, fm.get('bahnschrift_regular', 30, 'Bold'),
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Gacha_Log/models.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 from typing import List, Dict, Tuple, Optional
 
 from pydantic import BaseModel
 
 from LittlePaimon.utils.alias import get_chara_icon, get_weapon_icon
 
-GACHA_TYPE_LIST = {'100': '新手祈愿', '200': '常驻祈愿', '302': '武器祈愿', '301': '角色祈愿', '400': '角色祈愿'}
+GACHA_TYPE_LIST = {'100': '新手祈愿', '200': '常驻祈愿', '302': '武器祈愿', '301': '角色祈愿', '400': '角色祈愿', '500': '集录祈愿'}
 
 
 class FiveStarItem(BaseModel):
     name: str
     icon: Optional[str]
     count: int
     type: str
@@ -19,15 +19,16 @@
     name: str
     icon: Optional[str]
     type: str
     num: Dict[str, int] = {
         '角色祈愿': 0,
         '武器祈愿': 0,
         '常驻祈愿': 0,
-        '新手祈愿': 0}
+        '新手祈愿': 0,
+        '集录祈愿': 0}
 
 
 class GachaItem(BaseModel):
     id: str
     name: str
     gacha_type: str
     item_type: str
@@ -40,30 +41,33 @@
     uid: str
     update_time: datetime.datetime
     item_list: Dict[str, List[GachaItem]] = {
         '角色祈愿': [],
         '武器祈愿': [],
         '常驻祈愿': [],
         '新手祈愿': [],
+        '集录祈愿': []
     }
 
     def get_record_time(self) -> Dict[str, Tuple[datetime.datetime, datetime.datetime]]:
         return {
             '角色祈愿': (self.item_list['角色祈愿'][0].time, self.item_list['角色祈愿'][-1].time) if self.item_list['角色祈愿'] else (None, None),
             '武器祈愿': (self.item_list['武器祈愿'][0].time, self.item_list['武器祈愿'][-1].time) if self.item_list['武器祈愿'] else (None, None),
             '常驻祈愿': (self.item_list['常驻祈愿'][0].time, self.item_list['常驻祈愿'][-1].time) if self.item_list['常驻祈愿'] else (None, None),
-            '新手祈愿': (self.item_list['新手祈愿'][0].time, self.item_list['新手祈愿'][-1].time) if self.item_list['新手祈愿'] else (None, None)
+            '新手祈愿': (self.item_list['新手祈愿'][0].time, self.item_list['新手祈愿'][-1].time) if self.item_list['新手祈愿'] else (None, None),
+            '集录祈愿': (self.item_list['集录祈愿'][0].time, self.item_list['集录祈愿'][-1].time) if self.item_list['集录祈愿'] else (None, None),
         }
 
     def get_statistics(self) -> Tuple[Dict[str, List[FiveStarItem]], Dict[str, FourStarItem],  Dict[str, int]]:
         gacha_data_five: Dict[str, List[FiveStarItem]] = {
             '角色祈愿': [],
             '武器祈愿': [],
             '常驻祈愿': [],
             '新手祈愿': [],
+            '集录祈愿': []
         }
         gacha_data_four: Dict[str, FourStarItem] = {}
         gacha_not_out: Dict[str, int] = {}
         for pool_name, item_list in self.item_list.items():
             count_now = 0
             for item in item_list:
                 if item.rank_type == '5':
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/damage_cal.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/damage_cal.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/damage_model.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/damage_model.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/draw_character_card.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_card.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Info/draw_player_card.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_player_card.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_MonthInfo/draw.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_MonthInfo/handler.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/draw_map.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/draw_map.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/bot_manager/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/bot_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/news60s/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/news60s/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/plugin_manager/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/plugin_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/plugin_manager/draw_help.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/plugin_manager/draw_help.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/plugins/tools/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/alias.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/alias.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/api.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/browser.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/browser.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/files.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/files.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/filter.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/filter.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/genshin.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/genshin.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/image.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
     @run_sync
     def text_box(self,
                  text: str,
                  width: Tuple[int, int],
                  height: Tuple[int, int],
                  font: ImageFont.ImageFont,
                  color: Union[str, Tuple[int, int, int, int]] = 'white'):
-        text_height = self.draw.textsize(text, font=font)[1]
+        text_height = self.draw.textbbox((0, 0), text = text, font=font)[3] - self.draw.textbbox((0, 0), text = text, font=font)[1]
         width_now = width[0]
         height_now = height[0]
         for c in text:
             if c in ['.', '。'] and width_now == width[0] and c == text[-1]:
                 continue
             if c == '^':
                 width_now = width[0]
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/logger.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/message.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/message.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/path.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/path.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/requests.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/requests.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/scheduler.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/status.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/status.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/tool.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/tool.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/typing.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 CHARACTERS = ['神里绫华', '琴', '丽莎', '芭芭拉', '凯亚', '迪卢克', '雷泽', '安柏', '温迪', '香菱', '北斗', '行秋',
               '魈', '凝光', '可莉', '钟离',
               '菲谢尔', '班尼特', '达达利亚', '诺艾尔', '七七', '重云', '甘雨', '阿贝多', '迪奥娜', '莫娜', '刻晴',
               '砂糖', '辛焱', '罗莎莉亚', '胡桃',
               '枫原万叶', '烟绯', '宵宫', '托马', '优菈', '雷电将军', '早柚', '珊瑚宫心海', '五郎', '九条裟罗',
               '荒泷一斗', '八重神子', '夜兰', '埃洛伊',
               '申鹤', '云堇', '久岐忍', '神里绫人', '鹿野院平藏', '提纳里', '柯莱', '多莉', '赛诺', '坎蒂丝', '妮露',
-              '纳西妲', '莱依拉', '流浪者', '珐露珊', '艾尔海森', '瑶瑶', '迪希雅', '米卡', '白术', '卡维', '绮良良', '琳妮特', '林尼', '菲米尼', '莱欧斯利', '那维莱特', '夏洛蒂', '芙宁娜', '夏沃蕾', '娜维娅', '嘉明', '闲云']
+              '纳西妲', '莱依拉', '流浪者', '珐露珊', '艾尔海森', '瑶瑶', '迪希雅', '米卡', '白术', '卡维', '绮良良', '琳妮特', '林尼', '菲米尼', '莱欧斯利', '那维莱特', '夏洛蒂', '芙宁娜', '夏沃蕾', '娜维娅', '嘉明', '闲云', '千织']
 """全角色"""
 MALE_CHARACTERS = ['凯亚', '迪卢克', '钟离', '达达利亚', '托马', '荒泷一斗', '神里绫人', '艾尔海森', '白术', '卡维', '莱欧斯利', '那维莱特']
 """成男角色"""
 FEMALE_CHARACTERS = ['琴', '丽莎', '北斗', '凝光', '罗莎莉亚', '优菈', '雷电将军', '九条裟罗', '八重神子', '夜兰',
                      '申鹤', '坎蒂丝', '迪希雅', '闲云']
 """成女角色"""
 GIRL_CHARACTERS = ['神里绫华', '芭芭拉', '安柏', '香菱', '菲谢尔', '诺艾尔', '甘雨', '莫娜', '刻晴', '砂糖', '辛焱',
-                   '胡桃', '烟绯', '宵宫', '珊瑚宫心海', '埃洛伊', '云堇', '久岐忍', '柯莱', '妮露', '莱依拉', '珐露珊', '绮良良', '琳妮特', '夏洛蒂', '芙宁娜', '夏沃蕾', '娜维娅']
+                   '胡桃', '烟绯', '宵宫', '珊瑚宫心海', '埃洛伊', '云堇', '久岐忍', '柯莱', '妮露', '莱依拉', '珐露珊', '绮良良', '琳妮特', '夏洛蒂', '芙宁娜', '夏沃蕾', '娜维娅', '千织']
 """少女角色"""
 BOY_CHARACTERS = ['雷泽', '温迪', '行秋', '魈', '班尼特', '重云', '阿贝多', '枫原万叶', '五郎', '鹿野院平藏', '提纳里',
                   '赛诺', '流浪者', '米卡', '林尼', '菲米尼', '嘉明']
 """少男角色"""
 LOLI_CHARACTERS = ['七七', '可莉', '迪奥娜', '早柚', '多莉', '纳西妲', '瑶瑶']
 """萝莉"""
```

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/utils/update.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/update.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/__init__.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/bot_info.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/bot_info.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/command_alias.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/command_alias.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/cookie.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/login.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/login.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/plugin.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/plugin.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/status.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/status.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/api/utils.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/utils.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/bind_cookie.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/bind_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/command_alias.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/command_alias.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/config_manage.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/config_manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/home_page.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/home_page.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/login.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/login.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/main.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/main.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/plugin_manage.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/plugin_manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/private_cookie.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/private_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/LittlePaimon/web/pages/public_cookie.py` & `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/public_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.13/pyproject.toml` & `mhmzx_little_paimon-3.0.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mhmzx-little-paimon"
-version = "3.0.13"
+version = "3.0.14"
 description = "（非官方）小派蒙！原神qq群机器人，基于NoneBot2的UID查询、抽卡导出分析、模拟抽卡、实时便签、札记等多功能小助手。"
 authors = ["Madray Haven <sgpublic2002@gmail.com>"]
 license = "AGPL"
 packages = [
     { include = "LittlePaimon" },
 ]
```

### Comparing `mhmzx_little_paimon-3.0.13/PKG-INFO` & `mhmzx_little_paimon-3.0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mhmzx-little-paimon
-Version: 3.0.13
+Version: 3.0.14
 Summary: （非官方）小派蒙！原神qq群机器人，基于NoneBot2的UID查询、抽卡导出分析、模拟抽卡、实时便签、札记等多功能小助手。
 License: AGPL
 Author: Madray Haven
 Author-email: sgpublic2002@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

