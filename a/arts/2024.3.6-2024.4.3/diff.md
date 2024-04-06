# Comparing `tmp/arts-2024.3.6.tar.gz` & `tmp/arts-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arts-2024.3.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "arts-2024.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `arts-2024.3.6.tar` & `arts-2024.4.3.tar`

### file list

```diff
@@ -1,222 +1,231 @@
--rw-r--r--   0        0        0     2175 2023-12-20 10:09:43.709218 arts-2024.3.6/.gitignore
--rw-r--r--   0        0        0      724 2024-02-16 09:23:52.390153 arts-2024.3.6/README.md
--rw-r--r--   0        0        0      317 2024-02-22 12:02:36.224046 arts-2024.3.6/arts/CoolMemory-English/Copyright
--rw-r--r--   0        0        0    10295 2024-03-04 05:19:20.063253 arts-2024.3.6/arts/CoolMemory-English/README.md
--rw-r--r--   0        0        0      110 2024-03-06 00:07:28.301653 arts-2024.3.6/arts/CoolMemory-English/art.json
--rw-r--r--   0        0        0      393 2023-12-10 08:00:44.000000 arts-2024.3.6/arts/CoolMemory-English/licenses/README.md
--rw-r--r--   0        0        0     1586 2023-12-10 08:00:44.000000 arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE
--rw-r--r--   0        0        0    11550 2023-12-10 08:00:44.000000 arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE
--rw-r--r--   0        0        0    32825 2023-12-10 08:00:44.000000 arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/Python/LICENSE
--rw-r--r--   0        0        0     2987 2023-12-10 08:00:44.000000 arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE
--rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE
--rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE
--rw-r--r--   0        0        0        0 2024-02-22 15:47:26.927352 arts-2024.3.6/arts/__init__.py
--rw-r--r--   0        0        0     3088 2023-09-24 08:08:30.000000 arts-2024.3.6/arts/articles/010-赚钱宝典/010-财富的本质/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:01:11.532367 arts-2024.3.6/arts/articles/010-赚钱宝典/010-财富的本质/art.json
--rw-r--r--   0        0        0     1681 2023-12-20 10:09:07.827303 arts-2024.3.6/arts/articles/010-赚钱宝典/020-商业价值/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:01:11.533332 arts-2024.3.6/arts/articles/010-赚钱宝典/020-商业价值/art.json
--rw-r--r--   0        0        0     3552 2023-12-22 07:27:54.636897 arts-2024.3.6/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md
--rw-r--r--   0        0        0       44 2023-12-22 07:26:00.584312 arts-2024.3.6/arts/articles/010-赚钱宝典/030-财富稳定型社会/art.json
--rw-r--r--   0        0        0     1812 2024-01-02 20:05:02.520382 arts-2024.3.6/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md
--rw-r--r--   0        0        0       44 2024-01-02 20:46:41.567445 arts-2024.3.6/arts/articles/075-追英赶美/300-产业升级与失业潮/art.json
--rw-r--r--   0        0        0     1253 2024-01-18 01:49:14.297346 arts-2024.3.6/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md
--rw-r--r--   0        0        0       44 2024-01-02 20:47:04.916014 arts-2024.3.6/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/art.json
--rw-r--r--   0        0        0     1559 2023-11-15 13:45:10.000000 arts-2024.3.6/arts/articles/150-小民参政/300-广义的民主/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:02:18.547561 arts-2024.3.6/arts/articles/150-小民参政/300-广义的民主/art.json
--rw-r--r--   0        0        0     1499 2023-10-24 11:49:00.000000 arts-2024.3.6/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:02:18.545561 arts-2024.3.6/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/art.json
--rw-r--r--   0        0        0     1450 2023-11-05 04:22:04.000000 arts-2024.3.6/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.648073 arts-2024.3.6/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/art.json
--rw-r--r--   0        0        0     3278 2024-02-25 10:11:51.363950 arts-2024.3.6/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.644190 arts-2024.3.6/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/art.json
--rw-r--r--   0        0        0     1456 2023-12-28 00:10:08.901209 arts-2024.3.6/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.645220 arts-2024.3.6/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/art.json
--rw-r--r--   0        0        0     1135 2024-03-04 05:13:36.283230 arts-2024.3.6/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.647184 arts-2024.3.6/arts/articles/300-批判那些伪文艺/800-务实与务虚/art.json
--rw-r--r--   0        0        0     2095 2024-01-18 01:48:33.751985 arts-2024.3.6/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.900873 arts-2024.3.6/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/art.json
--rw-r--r--   0        0        0     1668 2023-11-05 03:35:50.000000 arts-2024.3.6/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.909872 arts-2024.3.6/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/art.json
--rw-r--r--   0        0        0     1669 2023-11-15 13:41:24.000000 arts-2024.3.6/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.903896 arts-2024.3.6/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/art.json
--rw-r--r--   0        0        0     1906 2023-12-27 20:37:35.730568 arts-2024.3.6/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.899872 arts-2024.3.6/arts/articles/450-万象思考/200-人工智能会不会统治人类？/art.json
--rw-r--r--   0        0        0     1154 2023-11-05 02:49:06.000000 arts-2024.3.6/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.907909 arts-2024.3.6/arts/articles/450-万象思考/250-忒修斯之船悖论/art.json
--rw-r--r--   0        0        0     3155 2023-12-27 20:37:10.901781 arts-2024.3.6/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md
--rw-r--r--   0        0        0       44 2024-01-05 13:23:02.578368 arts-2024.3.6/arts/articles/450-万象思考/300-有无相生，难易相成的启发/art.json
--rw-r--r--   0        0        0     1354 2023-11-05 03:42:52.000000 arts-2024.3.6/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md
--rw-r--r--   0        0        0       44 2024-01-05 13:30:30.884939 arts-2024.3.6/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/art.json
--rw-r--r--   0        0        0     1123 2023-09-10 18:11:18.000000 arts-2024.3.6/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.906885 arts-2024.3.6/arts/articles/450-万象思考/500-人们为什么希望拥有后代/art.json
--rw-r--r--   0        0        0      708 2023-12-27 20:36:45.425482 arts-2024.3.6/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.904897 arts-2024.3.6/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/art.json
--rw-r--r--   0        0        0     5024 2023-11-15 13:32:28.000000 arts-2024.3.6/arts/articles/450-万象思考/700-堕胎自由权/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.901873 arts-2024.3.6/arts/articles/450-万象思考/700-堕胎自由权/art.json
--rw-r--r--   0        0        0     3701 2023-11-15 13:30:02.000000 arts-2024.3.6/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.910899 arts-2024.3.6/arts/articles/450-万象思考/800-人人平等是个伪概念/art.json
--rw-r--r--   0        0        0     3385 2023-12-27 20:36:19.402593 arts-2024.3.6/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.414383 arts-2024.3.6/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/art.json
--rw-r--r--   0        0        0     2466 2024-02-25 10:07:00.576902 arts-2024.3.6/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.399805 arts-2024.3.6/arts/articles/600-时空猜想/400-我们可能处在人造世界/art.json
--rw-r--r--   0        0        0     3007 2023-11-04 19:08:36.000000 arts-2024.3.6/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.412423 arts-2024.3.6/arts/articles/600-时空猜想/600-占卜真的存在吗？/art.json
--rw-r--r--   0        0        0     2630 2023-11-04 19:15:30.000000 arts-2024.3.6/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.411378 arts-2024.3.6/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/art.json
--rw-r--r--   0        0        0     2038 2023-12-28 02:10:43.748193 arts-2024.3.6/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md
--rw-r--r--   0        0        0       44 2023-12-28 02:02:17.049897 arts-2024.3.6/arts/articles/700-论时事/300-那些年，我们经历过的历史/art.json
--rw-r--r--   0        0        0     1742 2024-01-13 20:46:22.292355 arts-2024.3.6/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:35.958057 arts-2024.3.6/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/art.json
--rw-r--r--   0        0        0     7343 2023-06-23 06:29:18.000000 arts-2024.3.6/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:05:12.312457 arts-2024.3.6/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/art.json
--rw-r--r--   0        0        0     1652 2023-06-23 06:48:36.000000 arts-2024.3.6/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:05:34.053435 arts-2024.3.6/arts/articles/800-小说/600-一念天堂/050-被绑架/art.json
--rw-r--r--   0        0        0       26 2023-12-20 07:52:46.818615 arts-2024.3.6/arts/cooltypes/Coolstr/__init__.py
--rw-r--r--   0        0        0     1092 2024-02-25 05:38:12.586187 arts-2024.3.6/arts/cooltypes/Coolstr/_core.py
--rw-r--r--   0        0        0     3317 2024-02-24 16:44:27.960191 arts-2024.3.6/arts/cooltypes/Cooltime/README.md
--rw-r--r--   0        0        0       27 2023-12-20 07:55:46.771625 arts-2024.3.6/arts/cooltypes/Cooltime/__init__.py
--rw-r--r--   0        0        0       44 2024-02-22 10:39:05.460423 arts-2024.3.6/arts/cooltypes/Cooltime/_art.json
--rw-r--r--   0        0        0     3691 2024-02-24 16:55:03.249175 arts-2024.3.6/arts/cooltypes/Cooltime/_core.py
--rw-r--r--   0        0        0    11283 2024-02-22 12:02:36.224046 arts-2024.3.6/arts/cooltypes/LICENSE
--rw-r--r--   0        0        0      474 2024-02-24 16:35:52.576679 arts-2024.3.6/arts/cooltypes/__init__.py
--rw-r--r--   0        0        0     1543 2024-02-23 04:50:51.702716 arts-2024.3.6/arts/cooltypes/envname/README.md
--rw-r--r--   0        0        0       62 2024-02-23 04:28:30.402332 arts-2024.3.6/arts/cooltypes/envname/__init__.py
--rw-r--r--   0        0        0      409 2024-02-23 04:27:58.084752 arts-2024.3.6/arts/cooltypes/envname/_core.py
--rw-r--r--   0        0        0      865 2024-02-23 04:12:59.530774 arts-2024.3.6/arts/cooltypes/moduledb/README.md
--rw-r--r--   0        0        0       32 2024-02-23 04:03:44.487797 arts-2024.3.6/arts/cooltypes/moduledb/__init__.py
--rw-r--r--   0        0        0     3717 2024-02-23 04:15:35.883622 arts-2024.3.6/arts/cooltypes/moduledb/_core.py
--rw-r--r--   0        0        0     5793 2024-02-22 13:11:46.788704 arts-2024.3.6/arts/cooltypes/rstyleslice/README.md
--rw-r--r--   0        0        0       25 2023-07-13 08:31:54.000000 arts-2024.3.6/arts/cooltypes/rstyleslice/__init__.py
--rw-r--r--   0        0        0     2801 2023-11-10 18:12:44.000000 arts-2024.3.6/arts/cooltypes/rstyleslice/_core.py
--rw-r--r--   0        0        0      345 2024-02-24 06:36:31.328590 arts-2024.3.6/arts/cooltypes/vtype/__init__.py
--rw-r--r--   0        0        0    14555 2024-02-25 03:45:53.369925 arts-2024.3.6/arts/cooltypes/vtype/_core.py
--rw-r--r--   0        0        0      188 2024-02-24 09:59:49.203886 arts-2024.3.6/arts/cooltypes/设计.md
--rw-r--r--   0        0        0    58890 2024-03-06 01:05:42.992260 arts-2024.3.6/arts/index.html
--rw-r--r--   0        0        0       44 2024-01-16 13:04:45.523107 arts-2024.3.6/arts/life/2018/莆田学院·毕业生留影/art.json
--rw-r--r--   0        0        0      830 2024-02-12 15:02:22.123647 arts-2024.3.6/arts/life/2018/莆田学院·毕业生留影/index.html
--rw-r--r--   0        0        0       44 2024-01-17 04:28:07.076300 arts-2024.3.6/arts/life/2019/苏州市虎丘山/art.json
--rw-r--r--   0        0        0     1235 2024-01-30 04:02:53.678647 arts-2024.3.6/arts/life/2019/苏州市虎丘山/index.html
--rw-r--r--   0        0        0       44 2024-01-17 03:40:13.294365 arts-2024.3.6/arts/life/2022/泉州市丰泽区·雨后街道/art.json
--rw-r--r--   0        0        0      963 2024-01-17 23:21:51.767082 arts-2024.3.6/arts/life/2022/泉州市丰泽区·雨后街道/index.html
--rw-r--r--   0        0        0       44 2024-01-30 05:00:40.402244 arts-2024.3.6/arts/life/2023/更换微信账号了/art.json
--rw-r--r--   0        0        0      832 2024-02-12 15:02:47.979648 arts-2024.3.6/arts/life/2023/更换微信账号了/index.html
--rw-r--r--   0        0        0    11276 2024-02-22 12:02:36.224046 arts-2024.3.6/arts/miumapp/LICENSE
--rw-r--r--   0        0        0     5763 2024-02-25 09:30:59.717634 arts-2024.3.6/arts/miumapp/README.md
--rw-r--r--   0        0        0       36 2024-02-12 15:08:38.569224 arts-2024.3.6/arts/miumapp/__init__.py
--rw-r--r--   0        0        0     8609 2024-03-03 08:49:44.726292 arts-2024.3.6/arts/miumapp/_core.py
--rw-r--r--   0        0        0      111 2024-03-05 23:26:53.659150 arts-2024.3.6/arts/miumapp/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.3.6/arts/miumapp/licenses/README.md
--rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.3.6/arts/miumapp/licenses/pyppeteer/LICENSE
--rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.3.6/arts/miumapp/licenses/tornado/LICENSE
--rw-r--r--   0        0        0       48 2024-02-12 15:15:42.556195 arts-2024.3.6/arts/miumapp/miumapp/__init__.py
--rw-r--r--   0        0        0     4657 2024-02-22 17:30:50.375647 arts-2024.3.6/arts/miumapp/miumapp/demo.html
--rw-r--r--   0        0        0     1241 2024-02-23 06:04:01.387180 arts-2024.3.6/arts/miumapp/miumapp/demo.py
--rw-r--r--   0        0        0      643 2024-03-06 00:09:18.507101 arts-2024.3.6/arts/miumapp/pyproject.toml
--rw-r--r--   0        0        0    11273 2024-03-02 20:20:55.781363 arts-2024.3.6/arts/oodb/LICENSE
--rw-r--r--   0        0        0    22163 2024-03-05 23:53:00.934606 arts-2024.3.6/arts/oodb/README.md
--rw-r--r--   0        0        0       44 2024-03-06 00:36:04.879589 arts-2024.3.6/arts/oodb/__init__.py
--rw-r--r--   0        0        0    19027 2024-03-06 00:36:04.879589 arts-2024.3.6/arts/oodb/_core.py
--rw-r--r--   0        0        0       99 2024-03-06 01:01:05.433633 arts-2024.3.6/arts/oodb/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.3.6/arts/oodb/licenses/README.md
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.3.6/arts/oodb/licenses/pymongo/LICENSE
--rw-r--r--   0        0        0       53 2024-03-06 00:36:04.879589 arts-2024.3.6/arts/oodb/oodb.py
--rw-r--r--   0        0        0      624 2024-03-06 00:12:56.663134 arts-2024.3.6/arts/oodb/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-03-03 07:09:08.518004 arts-2024.3.6/arts/oomongo/LICENSE
--rw-r--r--   0        0        0    17250 2024-03-05 13:21:42.573762 arts-2024.3.6/arts/oomongo/README.md
--rw-r--r--   0        0        0       49 2024-03-05 08:01:41.054010 arts-2024.3.6/arts/oomongo/__init__.py
--rw-r--r--   0        0        0    27613 2024-03-06 00:34:47.221863 arts-2024.3.6/arts/oomongo/_core.py
--rw-r--r--   0        0        0       92 2024-03-06 00:50:10.273786 arts-2024.3.6/arts/oomongo/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.3.6/arts/oomongo/licenses/README.md
--rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 arts-2024.3.6/arts/oomongo/licenses/motor/LICENSE
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.3.6/arts/oomongo/licenses/pymongo/LICENSE
--rw-r--r--   0        0        0       61 2024-03-05 08:01:41.059008 arts-2024.3.6/arts/oomongo/oomongo.py
--rw-r--r--   0        0        0      563 2024-03-06 00:09:25.377118 arts-2024.3.6/arts/oomongo/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-03-03 07:10:17.933453 arts-2024.3.6/arts/oomysql/LICENSE
--rw-r--r--   0        0        0    16980 2024-03-05 13:19:03.747040 arts-2024.3.6/arts/oomysql/README.md
--rw-r--r--   0        0        0       45 2024-03-05 08:02:05.322948 arts-2024.3.6/arts/oomysql/__init__.py
--rw-r--r--   0        0        0    35279 2024-03-06 00:34:05.340548 arts-2024.3.6/arts/oomysql/_core.py
--rw-r--r--   0        0        0       90 2024-03-06 00:10:16.490984 arts-2024.3.6/arts/oomysql/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.3.6/arts/oomysql/licenses/README.md
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:56.000000 arts-2024.3.6/arts/oomysql/licenses/aiomysql/LICENSE
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 arts-2024.3.6/arts/oomysql/licenses/pymysql/LICENSE
--rw-r--r--   0        0        0       57 2024-03-05 08:02:05.335929 arts-2024.3.6/arts/oomysql/oomysql.py
--rw-r--r--   0        0        0      641 2024-03-06 00:09:38.203916 arts-2024.3.6/arts/oomysql/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 arts-2024.3.6/arts/openai2/LICENSE
--rw-r--r--   0        0        0    13972 2024-03-01 12:35:49.672946 arts-2024.3.6/arts/openai2/README.md
--rw-r--r--   0        0        0      167 2023-12-19 12:18:48.792856 arts-2024.3.6/arts/openai2/__init__.py
--rw-r--r--   0        0        0     6923 2023-11-15 22:45:46.000000 arts-2024.3.6/arts/openai2/_core/GroupChat.py
--rw-r--r--   0        0        0     9258 2023-12-17 18:34:22.000000 arts-2024.3.6/arts/openai2/_core/chat.py
--rw-r--r--   0        0        0     2279 2024-02-23 04:06:51.826269 arts-2024.3.6/arts/openai2/_core/chat_in_cmd.py
--rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 arts-2024.3.6/arts/openai2/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.3.6/arts/openai2/licenses/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 arts-2024.3.6/arts/openai2/licenses/openai/LICENSE
--rw-r--r--   0        0        0      203 2024-03-03 10:11:45.701543 arts-2024.3.6/arts/openai2/openai2.py
--rw-r--r--   0        0        0      801 2024-03-06 00:09:43.494818 arts-2024.3.6/arts/openai2/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.3.6/arts/skybox/Copyright
--rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 arts-2024.3.6/arts/skybox/README.md
--rw-r--r--   0        0        0      320 2024-03-06 00:10:09.097613 arts-2024.3.6/arts/skybox/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.3.6/arts/skybox/skybox/Copyright
--rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 arts-2024.3.6/arts/skybox/skybox/__init__.py
--rw-r--r--   0        0        0     9850 2024-02-25 04:56:08.117767 arts-2024.3.6/arts/skybox/skybox/files_hashes
--rw-r--r--   0        0        0       44 2023-12-19 10:10:36.391618 arts-2024.3.6/arts/thoughts/2022/现代工人的螺丝钉处境/art.json
--rw-r--r--   0        0        0     1374 2024-01-16 22:36:30.326371 arts-2024.3.6/arts/thoughts/2022/现代工人的螺丝钉处境/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.542208 arts-2024.3.6/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/art.json
--rw-r--r--   0        0        0     1346 2024-01-30 04:04:01.359662 arts-2024.3.6/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.562268 arts-2024.3.6/arts/thoughts/2023/专利是个公平的赛道/art.json
--rw-r--r--   0        0        0      941 2024-01-17 23:21:51.767082 arts-2024.3.6/arts/thoughts/2023/专利是个公平的赛道/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.547209 arts-2024.3.6/arts/thoughts/2023/事情的真实性是由度的/art.json
--rw-r--r--   0        0        0     1001 2024-01-16 22:36:30.329386 arts-2024.3.6/arts/thoughts/2023/事情的真实性是由度的/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.556244 arts-2024.3.6/arts/thoughts/2023/人无法摆脱兽性/art.json
--rw-r--r--   0        0        0     1659 2024-01-16 22:36:30.330406 arts-2024.3.6/arts/thoughts/2023/人无法摆脱兽性/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.551211 arts-2024.3.6/arts/thoughts/2023/什么是极端？/art.json
--rw-r--r--   0        0        0      884 2024-01-16 22:36:30.330406 arts-2024.3.6/arts/thoughts/2023/什么是极端？/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.541243 arts-2024.3.6/arts/thoughts/2023/保护好人/art.json
--rw-r--r--   0        0        0      802 2024-01-16 22:36:30.331373 arts-2024.3.6/arts/thoughts/2023/保护好人/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.554209 arts-2024.3.6/arts/thoughts/2023/只筛选，不教化/art.json
--rw-r--r--   0        0        0      853 2024-01-16 22:36:30.331373 arts-2024.3.6/arts/thoughts/2023/只筛选，不教化/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.549209 arts-2024.3.6/arts/thoughts/2023/喊高考加油是刷存在感/art.json
--rw-r--r--   0        0        0     1047 2024-01-16 22:36:30.332406 arts-2024.3.6/arts/thoughts/2023/喊高考加油是刷存在感/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.552210 arts-2024.3.6/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/art.json
--rw-r--r--   0        0        0     1630 2024-01-16 22:36:30.333372 arts-2024.3.6/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.553243 arts-2024.3.6/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/art.json
--rw-r--r--   0        0        0     2475 2024-01-30 04:03:34.796607 arts-2024.3.6/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.561243 arts-2024.3.6/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/art.json
--rw-r--r--   0        0        0      833 2024-01-18 01:51:26.994040 arts-2024.3.6/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.545246 arts-2024.3.6/arts/thoughts/2023/想去国外了解自己/art.json
--rw-r--r--   0        0        0      966 2024-01-16 22:36:30.335371 arts-2024.3.6/arts/thoughts/2023/想去国外了解自己/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.548245 arts-2024.3.6/arts/thoughts/2023/现代化的分工合作机制/art.json
--rw-r--r--   0        0        0     1668 2024-01-16 22:36:30.335371 arts-2024.3.6/arts/thoughts/2023/现代化的分工合作机制/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.544210 arts-2024.3.6/arts/thoughts/2023/用理性处理简单的事情/art.json
--rw-r--r--   0        0        0     1587 2024-01-16 22:36:30.336371 arts-2024.3.6/arts/thoughts/2023/用理性处理简单的事情/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.557226 arts-2024.3.6/arts/thoughts/2023/真正的问题无法通过花招解决/art.json
--rw-r--r--   0        0        0      977 2024-01-16 22:36:30.336371 arts-2024.3.6/arts/thoughts/2023/真正的问题无法通过花招解决/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.560208 arts-2024.3.6/arts/thoughts/2023/艺术本天成，媒介偶显之/art.json
--rw-r--r--   0        0        0      629 2024-01-16 22:36:30.337410 arts-2024.3.6/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.558244 arts-2024.3.6/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/art.json
--rw-r--r--   0        0        0     1168 2024-01-16 22:36:30.338372 arts-2024.3.6/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html
--rw-r--r--   0        0        0       44 2024-01-13 21:13:40.122707 arts-2024.3.6/arts/thoughts/2024/不要害怕犯错/art.json
--rw-r--r--   0        0        0      698 2024-01-16 22:36:30.339373 arts-2024.3.6/arts/thoughts/2024/不要害怕犯错/index.html
--rw-r--r--   0        0        0       44 2024-01-01 14:23:12.130009 arts-2024.3.6/arts/thoughts/2024/新年题诗/art.json
--rw-r--r--   0        0        0     1152 2024-01-18 06:19:08.705581 arts-2024.3.6/arts/thoughts/2024/新年题诗/index.html
--rw-r--r--   0        0        0       44 2024-01-03 04:10:15.709103 arts-2024.3.6/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/art.json
--rw-r--r--   0        0        0     1270 2024-01-16 22:36:30.341372 arts-2024.3.6/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html
--rw-r--r--   0        0        0       44 2024-01-30 04:08:51.850343 arts-2024.3.6/arts/thoughts/2024/萝莉岛事件引发的信任危机/art.json
--rw-r--r--   0        0        0     1077 2024-01-30 04:15:45.681734 arts-2024.3.6/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html
--rw-r--r--   0        0        0       44 2024-01-18 06:20:18.873404 arts-2024.3.6/arts/thoughts/2024/霍金去萝莉岛干嘛了/art.json
--rw-r--r--   0        0        0     1174 2024-01-18 06:24:05.339876 arts-2024.3.6/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html
--rw-r--r--   0        0        0      103 2024-03-03 07:12:46.987154 arts-2024.3.6/arts/tutorials/150-操作MySQL/art.json
--rw-r--r--   0        0        0      103 2024-03-06 00:50:30.486267 arts-2024.3.6/arts/tutorials/225-操作MongoDB/art.json
--rw-r--r--   0        0        0      146 2024-02-25 14:11:14.480558 arts-2024.3.6/arts/tutorials/300-开发桌面GUI应用/art.json
--rw-r--r--   0        0        0      103 2024-02-18 14:43:25.042841 arts-2024.3.6/arts/tutorials/450-对接ChatGPT/art.json
--rw-r--r--   0        0        0      114 2024-02-22 11:01:39.896717 arts-2024.3.6/arts/tutorials/525-时间模块/art.json
--rw-r--r--   0        0        0      100 2024-03-06 01:01:25.689741 arts-2024.3.6/arts/tutorials/562-面向对象数据库/art.json
--rw-r--r--   0        0        0     3415 2023-12-20 10:09:07.822297 arts-2024.3.6/arts/tutorials/600-用37行代码实现AI五子棋/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:14:03.255370 arts-2024.3.6/arts/tutorials/600-用37行代码实现AI五子棋/art.json
--rw-r--r--   0        0        0     8070 2024-02-25 05:45:21.624081 arts-2024.3.6/arts/tutorials/750-正则表达式/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:13:55.412792 arts-2024.3.6/arts/tutorials/750-正则表达式/art.json
--rw-r--r--   0        0        0       44 2024-01-30 03:46:52.790397 arts-2024.3.6/arts/videos/200-秦时明月[项羽]·谪居/art.json
--rw-r--r--   0        0        0       44 2023-12-19 10:07:05.944886 arts-2024.3.6/arts/videos/400-李连杰[霍元甲]·兰亭序/art.json
--rw-r--r--   0        0        0       44 2023-12-19 10:07:05.933448 arts-2024.3.6/arts/videos/600-楚门的世界·五月雨/art.json
--rw-r--r--   0        0        0       44 2024-01-05 13:31:13.729378 arts-2024.3.6/arts/videos/800-AI是这样画包拯的/art.json
--rw-r--r--   0        0        0      524 2024-03-06 00:09:06.366469 arts-2024.3.6/pyproject.toml
--rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 arts-2024.3.6/PKG-INFO
+-rw-r--r--   0        0        0     2175 2023-12-20 10:09:43.709218 arts-2024.4.3/.gitignore
+-rw-r--r--   0        0        0       46 2024-03-10 10:13:06.948005 arts-2024.4.3/README.md
+-rw-r--r--   0        0        0      317 2024-02-22 12:02:36.224046 arts-2024.4.3/arts/CoolMemory-English/Copyright
+-rw-r--r--   0        0        0    10294 2024-03-31 09:22:44.234618 arts-2024.4.3/arts/CoolMemory-English/README.md
+-rw-r--r--   0        0        0      110 2024-03-06 00:07:28.301653 arts-2024.4.3/arts/CoolMemory-English/art.json
+-rw-r--r--   0        0        0      393 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/README.md
+-rw-r--r--   0        0        0     1586 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE
+-rw-r--r--   0        0        0    11550 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE
+-rw-r--r--   0        0        0    32825 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Python/LICENSE
+-rw-r--r--   0        0        0     2987 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE
+-rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE
+-rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE
+-rw-r--r--   0        0        0      106 2024-03-31 10:18:29.252509 arts-2024.4.3/arts/WeChat-Art-Museum/art.json
+-rw-r--r--   0        0        0    52542 2024-04-03 06:13:33.904082 arts-2024.4.3/arts/WeChat-Art-Museum/index.html
+-rw-r--r--   0        0        0        0 2024-02-22 15:47:26.927352 arts-2024.4.3/arts/__init__.py
+-rw-r--r--   0        0        0     3088 2023-09-24 08:08:30.000000 arts-2024.4.3/arts/articles/010-赚钱宝典/010-财富的本质/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:01:11.532367 arts-2024.4.3/arts/articles/010-赚钱宝典/010-财富的本质/art.json
+-rw-r--r--   0        0        0     1681 2023-12-20 10:09:07.827303 arts-2024.4.3/arts/articles/010-赚钱宝典/020-商业价值/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:01:11.533332 arts-2024.4.3/arts/articles/010-赚钱宝典/020-商业价值/art.json
+-rw-r--r--   0        0        0     3552 2023-12-22 07:27:54.636897 arts-2024.4.3/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md
+-rw-r--r--   0        0        0       44 2023-12-22 07:26:00.584312 arts-2024.4.3/arts/articles/010-赚钱宝典/030-财富稳定型社会/art.json
+-rw-r--r--   0        0        0     1812 2024-01-02 20:05:02.520382 arts-2024.4.3/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md
+-rw-r--r--   0        0        0       44 2024-01-02 20:46:41.567445 arts-2024.4.3/arts/articles/075-追英赶美/300-产业升级与失业潮/art.json
+-rw-r--r--   0        0        0     1253 2024-01-18 01:49:14.297346 arts-2024.4.3/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md
+-rw-r--r--   0        0        0       44 2024-01-02 20:47:04.916014 arts-2024.4.3/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/art.json
+-rw-r--r--   0        0        0     1559 2023-11-15 13:45:10.000000 arts-2024.4.3/arts/articles/150-小民参政/300-广义的民主/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:02:18.547561 arts-2024.4.3/arts/articles/150-小民参政/300-广义的民主/art.json
+-rw-r--r--   0        0        0     1499 2023-10-24 11:49:00.000000 arts-2024.4.3/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:02:18.545561 arts-2024.4.3/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/art.json
+-rw-r--r--   0        0        0     1450 2023-11-05 04:22:04.000000 arts-2024.4.3/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.648073 arts-2024.4.3/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/art.json
+-rw-r--r--   0        0        0     3278 2024-02-25 10:11:51.363950 arts-2024.4.3/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.644190 arts-2024.4.3/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/art.json
+-rw-r--r--   0        0        0     1265 2024-03-28 16:30:38.111960 arts-2024.4.3/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.645220 arts-2024.4.3/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/art.json
+-rw-r--r--   0        0        0     1135 2024-03-04 05:13:36.283230 arts-2024.4.3/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.647184 arts-2024.4.3/arts/articles/300-批判那些伪文艺/800-务实与务虚/art.json
+-rw-r--r--   0        0        0     2095 2024-01-18 01:48:33.751985 arts-2024.4.3/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.900873 arts-2024.4.3/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/art.json
+-rw-r--r--   0        0        0     1668 2023-11-05 03:35:50.000000 arts-2024.4.3/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.909872 arts-2024.4.3/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/art.json
+-rw-r--r--   0        0        0     1669 2023-11-15 13:41:24.000000 arts-2024.4.3/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.903896 arts-2024.4.3/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/art.json
+-rw-r--r--   0        0        0     1906 2023-12-27 20:37:35.730568 arts-2024.4.3/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.899872 arts-2024.4.3/arts/articles/450-万象思考/200-人工智能会不会统治人类？/art.json
+-rw-r--r--   0        0        0     1154 2023-11-05 02:49:06.000000 arts-2024.4.3/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.907909 arts-2024.4.3/arts/articles/450-万象思考/250-忒修斯之船悖论/art.json
+-rw-r--r--   0        0        0     3155 2023-12-27 20:37:10.901781 arts-2024.4.3/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md
+-rw-r--r--   0        0        0       44 2024-01-05 13:23:02.578368 arts-2024.4.3/arts/articles/450-万象思考/300-有无相生，难易相成的启发/art.json
+-rw-r--r--   0        0        0     1354 2023-11-05 03:42:52.000000 arts-2024.4.3/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md
+-rw-r--r--   0        0        0       44 2024-01-05 13:30:30.884939 arts-2024.4.3/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/art.json
+-rw-r--r--   0        0        0     1123 2023-09-10 18:11:18.000000 arts-2024.4.3/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.906885 arts-2024.4.3/arts/articles/450-万象思考/500-人们为什么希望拥有后代/art.json
+-rw-r--r--   0        0        0      708 2023-12-27 20:36:45.425482 arts-2024.4.3/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.904897 arts-2024.4.3/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/art.json
+-rw-r--r--   0        0        0     5024 2023-11-15 13:32:28.000000 arts-2024.4.3/arts/articles/450-万象思考/700-堕胎自由权/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.901873 arts-2024.4.3/arts/articles/450-万象思考/700-堕胎自由权/art.json
+-rw-r--r--   0        0        0     3701 2023-11-15 13:30:02.000000 arts-2024.4.3/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.910899 arts-2024.4.3/arts/articles/450-万象思考/800-人人平等是个伪概念/art.json
+-rw-r--r--   0        0        0     3385 2023-12-27 20:36:19.402593 arts-2024.4.3/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.414383 arts-2024.4.3/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/art.json
+-rw-r--r--   0        0        0     2466 2024-02-25 10:07:00.576902 arts-2024.4.3/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.399805 arts-2024.4.3/arts/articles/600-时空猜想/400-我们可能处在人造世界/art.json
+-rw-r--r--   0        0        0     3007 2023-11-04 19:08:36.000000 arts-2024.4.3/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.412423 arts-2024.4.3/arts/articles/600-时空猜想/600-占卜真的存在吗？/art.json
+-rw-r--r--   0        0        0     2630 2023-11-04 19:15:30.000000 arts-2024.4.3/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.411378 arts-2024.4.3/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/art.json
+-rw-r--r--   0        0        0     2038 2023-12-28 02:10:43.748193 arts-2024.4.3/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md
+-rw-r--r--   0        0        0       44 2023-12-28 02:02:17.049897 arts-2024.4.3/arts/articles/700-论时事/300-那些年，我们经历过的历史/art.json
+-rw-r--r--   0        0        0     1742 2024-01-13 20:46:22.292355 arts-2024.4.3/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:35.958057 arts-2024.4.3/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/art.json
+-rw-r--r--   0        0        0     7343 2023-06-23 06:29:18.000000 arts-2024.4.3/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:05:12.312457 arts-2024.4.3/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/art.json
+-rw-r--r--   0        0        0     1652 2023-06-23 06:48:36.000000 arts-2024.4.3/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:05:34.053435 arts-2024.4.3/arts/articles/800-小说/600-一念天堂/050-被绑架/art.json
+-rw-r--r--   0        0        0    11283 2024-02-22 12:02:36.224046 arts-2024.4.3/arts/cooltypes/LICENSE
+-rw-r--r--   0        0        0      293 2024-03-22 15:18:30.564599 arts-2024.4.3/arts/cooltypes/__init__.py
+-rw-r--r--   0        0        0     1542 2024-03-31 09:40:29.228723 arts-2024.4.3/arts/cooltypes/envname/README.md
+-rw-r--r--   0        0        0       62 2024-02-23 04:28:30.402332 arts-2024.4.3/arts/cooltypes/envname/__init__.py
+-rw-r--r--   0        0        0      409 2024-02-23 04:27:58.084752 arts-2024.4.3/arts/cooltypes/envname/_core.py
+-rw-r--r--   0        0        0      865 2024-02-23 04:12:59.530774 arts-2024.4.3/arts/cooltypes/moduledb/README.md
+-rw-r--r--   0        0        0       32 2024-02-23 04:03:44.487797 arts-2024.4.3/arts/cooltypes/moduledb/__init__.py
+-rw-r--r--   0        0        0     3717 2024-02-23 04:15:35.883622 arts-2024.4.3/arts/cooltypes/moduledb/_core.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:20:36.445694 arts-2024.4.3/arts/cooltypes/modules/coolstr/__init__.py
+-rw-r--r--   0        0        0     2181 2024-03-22 15:28:12.579126 arts-2024.4.3/arts/cooltypes/modules/coolstr/_core.py
+-rw-r--r--   0        0        0     3316 2024-03-31 09:40:29.228723 arts-2024.4.3/arts/cooltypes/modules/cooltime/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 20:20:55.541076 arts-2024.4.3/arts/cooltypes/modules/cooltime/__init__.py
+-rw-r--r--   0        0        0       44 2024-02-22 10:39:05.460423 arts-2024.4.3/arts/cooltypes/modules/cooltime/_art.json
+-rw-r--r--   0        0        0     3665 2024-03-22 15:09:31.411034 arts-2024.4.3/arts/cooltypes/modules/cooltime/_core.py
+-rw-r--r--   0        0        0     5793 2024-03-22 15:12:37.868753 arts-2024.4.3/arts/cooltypes/modules/rslice/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 20:26:19.316480 arts-2024.4.3/arts/cooltypes/modules/rslice/__init__.py
+-rw-r--r--   0        0        0     2801 2024-03-22 15:12:37.864736 arts-2024.4.3/arts/cooltypes/modules/rslice/_core.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:22:01.981114 arts-2024.4.3/arts/cooltypes/modules/vtype/__init__.py
+-rw-r--r--   0        0        0    10008 2024-03-22 15:22:10.216978 arts-2024.4.3/arts/cooltypes/modules/vtype/_core.py
+-rw-r--r--   0        0        0      238 2024-03-22 14:31:42.101320 arts-2024.4.3/arts/cooltypes/设计.md
+-rw-r--r--   0        0        0    60426 2024-04-03 06:13:25.657966 arts-2024.4.3/arts/index.html
+-rw-r--r--   0        0        0       44 2024-01-16 13:04:45.523107 arts-2024.4.3/arts/life/2018/莆田学院·毕业生留影/art.json
+-rw-r--r--   0        0        0      830 2024-02-12 15:02:22.123647 arts-2024.4.3/arts/life/2018/莆田学院·毕业生留影/index.html
+-rw-r--r--   0        0        0       44 2024-01-17 04:28:07.076300 arts-2024.4.3/arts/life/2019/苏州市虎丘山/art.json
+-rw-r--r--   0        0        0     1233 2024-03-24 16:39:19.059155 arts-2024.4.3/arts/life/2019/苏州市虎丘山/index.html
+-rw-r--r--   0        0        0       44 2024-01-17 03:40:13.294365 arts-2024.4.3/arts/life/2022/泉州市丰泽区·雨后街道/art.json
+-rw-r--r--   0        0        0      969 2024-03-24 16:39:36.018072 arts-2024.4.3/arts/life/2022/泉州市丰泽区·雨后街道/index.html
+-rw-r--r--   0        0        0       44 2024-01-30 05:00:40.402244 arts-2024.4.3/arts/life/2023/更换微信账号了/art.json
+-rw-r--r--   0        0        0      898 2024-04-03 03:17:39.386427 arts-2024.4.3/arts/life/2023/更换微信账号了/index.html
+-rw-r--r--   0        0        0       44 2024-03-24 16:41:15.708702 arts-2024.4.3/arts/life/2024/泉州市承天禅寺/art.json
+-rw-r--r--   0        0        0     1133 2024-03-25 03:52:07.749983 arts-2024.4.3/arts/life/2024/泉州市承天禅寺/index.html
+-rw-r--r--   0        0        0    11276 2024-02-22 12:02:36.224046 arts-2024.4.3/arts/miumapp/LICENSE
+-rw-r--r--   0        0        0     5762 2024-03-31 09:40:29.228723 arts-2024.4.3/arts/miumapp/README.md
+-rw-r--r--   0        0        0       36 2024-02-12 15:08:38.569224 arts-2024.4.3/arts/miumapp/__init__.py
+-rw-r--r--   0        0        0     7747 2024-03-25 04:09:08.267200 arts-2024.4.3/arts/miumapp/_core.py
+-rw-r--r--   0        0        0      111 2024-03-05 23:26:53.659150 arts-2024.4.3/arts/miumapp/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3/arts/miumapp/licenses/README.md
+-rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/miumapp/licenses/pyppeteer/LICENSE
+-rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.3/arts/miumapp/licenses/tornado/LICENSE
+-rw-r--r--   0        0        0       48 2024-02-12 15:15:42.556195 arts-2024.4.3/arts/miumapp/miumapp/__init__.py
+-rw-r--r--   0        0        0     4657 2024-02-22 17:30:50.375647 arts-2024.4.3/arts/miumapp/miumapp/demo.html
+-rw-r--r--   0        0        0     1241 2024-03-25 04:09:36.827762 arts-2024.4.3/arts/miumapp/miumapp/demo.py
+-rw-r--r--   0        0        0      645 2024-03-12 12:18:10.837369 arts-2024.4.3/arts/miumapp/pyproject.toml
+-rw-r--r--   0        0        0    11273 2024-03-02 20:20:55.781363 arts-2024.4.3/arts/oodb/LICENSE
+-rw-r--r--   0        0        0    22563 2024-03-31 09:40:29.216952 arts-2024.4.3/arts/oodb/README.md
+-rw-r--r--   0        0        0       44 2024-03-06 00:36:04.879589 arts-2024.4.3/arts/oodb/__init__.py
+-rw-r--r--   0        0        0    19029 2024-03-06 09:46:30.072966 arts-2024.4.3/arts/oodb/_core.py
+-rw-r--r--   0        0        0       99 2024-03-06 01:01:05.433633 arts-2024.4.3/arts/oodb/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3/arts/oodb/licenses/README.md
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.3/arts/oodb/licenses/pymongo/LICENSE
+-rw-r--r--   0        0        0       53 2024-03-06 00:36:04.879589 arts-2024.4.3/arts/oodb/oodb.py
+-rw-r--r--   0        0        0      626 2024-03-06 09:57:01.274330 arts-2024.4.3/arts/oodb/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-03-03 07:09:08.518004 arts-2024.4.3/arts/oomongo/LICENSE
+-rw-r--r--   0        0        0    17439 2024-03-31 09:40:29.227707 arts-2024.4.3/arts/oomongo/README.md
+-rw-r--r--   0        0        0       49 2024-03-05 08:01:41.054010 arts-2024.4.3/arts/oomongo/__init__.py
+-rw-r--r--   0        0        0    27613 2024-03-06 00:34:47.221863 arts-2024.4.3/arts/oomongo/_core.py
+-rw-r--r--   0        0        0       92 2024-03-06 00:50:10.273786 arts-2024.4.3/arts/oomongo/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3/arts/oomongo/licenses/README.md
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 arts-2024.4.3/arts/oomongo/licenses/motor/LICENSE
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.3/arts/oomongo/licenses/pymongo/LICENSE
+-rw-r--r--   0        0        0       61 2024-03-05 08:01:41.059008 arts-2024.4.3/arts/oomongo/oomongo.py
+-rw-r--r--   0        0        0      563 2024-03-06 00:09:25.377118 arts-2024.4.3/arts/oomongo/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-03-03 07:10:17.933453 arts-2024.4.3/arts/oomysql/LICENSE
+-rw-r--r--   0        0        0    17139 2024-03-31 09:40:29.228723 arts-2024.4.3/arts/oomysql/README.md
+-rw-r--r--   0        0        0       45 2024-03-05 08:02:05.322948 arts-2024.4.3/arts/oomysql/__init__.py
+-rw-r--r--   0        0        0    35301 2024-03-24 00:57:24.021318 arts-2024.4.3/arts/oomysql/_core.py
+-rw-r--r--   0        0        0       90 2024-03-06 00:10:16.490984 arts-2024.4.3/arts/oomysql/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3/arts/oomysql/licenses/README.md
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:56.000000 arts-2024.4.3/arts/oomysql/licenses/aiomysql/LICENSE
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 arts-2024.4.3/arts/oomysql/licenses/pymysql/LICENSE
+-rw-r--r--   0        0        0       57 2024-03-05 08:02:05.335929 arts-2024.4.3/arts/oomysql/oomysql.py
+-rw-r--r--   0        0        0      641 2024-03-06 00:09:38.203916 arts-2024.4.3/arts/oomysql/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 arts-2024.4.3/arts/openai2/LICENSE
+-rw-r--r--   0        0        0    13971 2024-03-31 09:40:29.216952 arts-2024.4.3/arts/openai2/README.md
+-rw-r--r--   0        0        0      167 2023-12-19 12:18:48.792856 arts-2024.4.3/arts/openai2/__init__.py
+-rw-r--r--   0        0        0     6923 2023-11-15 22:45:46.000000 arts-2024.4.3/arts/openai2/_core/GroupChat.py
+-rw-r--r--   0        0        0     9258 2023-12-17 18:34:22.000000 arts-2024.4.3/arts/openai2/_core/chat.py
+-rw-r--r--   0        0        0     2279 2024-02-23 04:06:51.826269 arts-2024.4.3/arts/openai2/_core/chat_in_cmd.py
+-rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 arts-2024.4.3/arts/openai2/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.3/arts/openai2/licenses/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 arts-2024.4.3/arts/openai2/licenses/openai/LICENSE
+-rw-r--r--   0        0        0      203 2024-03-03 10:11:45.701543 arts-2024.4.3/arts/openai2/openai2.py
+-rw-r--r--   0        0        0      801 2024-03-06 00:09:43.494818 arts-2024.4.3/arts/openai2/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.3/arts/skybox/Copyright
+-rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 arts-2024.4.3/arts/skybox/README.md
+-rw-r--r--   0        0        0      321 2024-03-31 11:04:55.600521 arts-2024.4.3/arts/skybox/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.3/arts/skybox/skybox/Copyright
+-rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 arts-2024.4.3/arts/skybox/skybox/__init__.py
+-rw-r--r--   0        0        0    12001 2024-04-01 02:53:11.002626 arts-2024.4.3/arts/skybox/skybox/files_hashes
+-rw-r--r--   0        0        0       44 2023-12-19 10:10:36.391618 arts-2024.4.3/arts/thoughts/2022/现代工人的螺丝钉处境/art.json
+-rw-r--r--   0        0        0     1374 2024-01-16 22:36:30.326371 arts-2024.4.3/arts/thoughts/2022/现代工人的螺丝钉处境/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.542208 arts-2024.4.3/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/art.json
+-rw-r--r--   0        0        0     1346 2024-01-30 04:04:01.359662 arts-2024.4.3/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.562268 arts-2024.4.3/arts/thoughts/2023/专利是个公平的赛道/art.json
+-rw-r--r--   0        0        0     1340 2024-03-27 02:41:37.370555 arts-2024.4.3/arts/thoughts/2023/专利是个公平的赛道/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.547209 arts-2024.4.3/arts/thoughts/2023/事情的真实性是由度的/art.json
+-rw-r--r--   0        0        0     1001 2024-01-16 22:36:30.329386 arts-2024.4.3/arts/thoughts/2023/事情的真实性是由度的/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.556244 arts-2024.4.3/arts/thoughts/2023/人无法摆脱兽性/art.json
+-rw-r--r--   0        0        0     1659 2024-01-16 22:36:30.330406 arts-2024.4.3/arts/thoughts/2023/人无法摆脱兽性/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.551211 arts-2024.4.3/arts/thoughts/2023/什么是极端？/art.json
+-rw-r--r--   0        0        0      884 2024-01-16 22:36:30.330406 arts-2024.4.3/arts/thoughts/2023/什么是极端？/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.541243 arts-2024.4.3/arts/thoughts/2023/保护好人/art.json
+-rw-r--r--   0        0        0      802 2024-01-16 22:36:30.331373 arts-2024.4.3/arts/thoughts/2023/保护好人/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.554209 arts-2024.4.3/arts/thoughts/2023/只筛选，不教化/art.json
+-rw-r--r--   0        0        0      853 2024-01-16 22:36:30.331373 arts-2024.4.3/arts/thoughts/2023/只筛选，不教化/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.549209 arts-2024.4.3/arts/thoughts/2023/喊高考加油是刷存在感/art.json
+-rw-r--r--   0        0        0     1047 2024-01-16 22:36:30.332406 arts-2024.4.3/arts/thoughts/2023/喊高考加油是刷存在感/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.552210 arts-2024.4.3/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/art.json
+-rw-r--r--   0        0        0     1630 2024-01-16 22:36:30.333372 arts-2024.4.3/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.553243 arts-2024.4.3/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/art.json
+-rw-r--r--   0        0        0     2475 2024-01-30 04:03:34.796607 arts-2024.4.3/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.561243 arts-2024.4.3/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/art.json
+-rw-r--r--   0        0        0      833 2024-01-18 01:51:26.994040 arts-2024.4.3/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.545246 arts-2024.4.3/arts/thoughts/2023/想去国外了解自己/art.json
+-rw-r--r--   0        0        0      966 2024-01-16 22:36:30.335371 arts-2024.4.3/arts/thoughts/2023/想去国外了解自己/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.548245 arts-2024.4.3/arts/thoughts/2023/现代化的分工合作机制/art.json
+-rw-r--r--   0        0        0     1668 2024-01-16 22:36:30.335371 arts-2024.4.3/arts/thoughts/2023/现代化的分工合作机制/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.544210 arts-2024.4.3/arts/thoughts/2023/用理性处理简单的事情/art.json
+-rw-r--r--   0        0        0     1587 2024-01-16 22:36:30.336371 arts-2024.4.3/arts/thoughts/2023/用理性处理简单的事情/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.557226 arts-2024.4.3/arts/thoughts/2023/真正的问题无法通过花招解决/art.json
+-rw-r--r--   0        0        0      977 2024-01-16 22:36:30.336371 arts-2024.4.3/arts/thoughts/2023/真正的问题无法通过花招解决/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.560208 arts-2024.4.3/arts/thoughts/2023/艺术本天成，媒介偶显之/art.json
+-rw-r--r--   0        0        0      629 2024-01-16 22:36:30.337410 arts-2024.4.3/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.558244 arts-2024.4.3/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/art.json
+-rw-r--r--   0        0        0     1168 2024-01-16 22:36:30.338372 arts-2024.4.3/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html
+-rw-r--r--   0        0        0       44 2024-01-13 21:13:40.122707 arts-2024.4.3/arts/thoughts/2024/不要害怕犯错/art.json
+-rw-r--r--   0        0        0      698 2024-01-16 22:36:30.339373 arts-2024.4.3/arts/thoughts/2024/不要害怕犯错/index.html
+-rw-r--r--   0        0        0       44 2024-04-03 04:23:50.480393 arts-2024.4.3/arts/thoughts/2024/做有趣的事情/art.json
+-rw-r--r--   0        0        0     2071 2024-04-03 05:42:46.206515 arts-2024.4.3/arts/thoughts/2024/做有趣的事情/index.html
+-rw-r--r--   0        0        0       44 2024-01-01 14:23:12.130009 arts-2024.4.3/arts/thoughts/2024/新年题诗/art.json
+-rw-r--r--   0        0        0     1152 2024-01-18 06:19:08.705581 arts-2024.4.3/arts/thoughts/2024/新年题诗/index.html
+-rw-r--r--   0        0        0       44 2024-01-03 04:10:15.709103 arts-2024.4.3/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/art.json
+-rw-r--r--   0        0        0     1270 2024-01-16 22:36:30.341372 arts-2024.4.3/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html
+-rw-r--r--   0        0        0       44 2024-03-24 15:35:39.622105 arts-2024.4.3/arts/thoughts/2024/编程语言的进化/art.json
+-rw-r--r--   0        0        0     1022 2024-03-24 16:22:12.389078 arts-2024.4.3/arts/thoughts/2024/编程语言的进化/example.html
+-rw-r--r--   0        0        0     1520 2024-03-25 03:53:51.266590 arts-2024.4.3/arts/thoughts/2024/编程语言的进化/index.html
+-rw-r--r--   0        0        0       44 2024-01-30 04:08:51.850343 arts-2024.4.3/arts/thoughts/2024/萝莉岛事件引发的信任危机/art.json
+-rw-r--r--   0        0        0     1077 2024-01-30 04:15:45.681734 arts-2024.4.3/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html
+-rw-r--r--   0        0        0       44 2024-01-18 06:20:18.873404 arts-2024.4.3/arts/thoughts/2024/霍金去萝莉岛干嘛了/art.json
+-rw-r--r--   0        0        0     1174 2024-01-18 06:24:05.339876 arts-2024.4.3/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html
+-rw-r--r--   0        0        0      103 2024-03-03 07:12:46.987154 arts-2024.4.3/arts/tutorials/150-操作MySQL/art.json
+-rw-r--r--   0        0        0      103 2024-03-06 00:50:30.486267 arts-2024.4.3/arts/tutorials/225-操作MongoDB/art.json
+-rw-r--r--   0        0        0      146 2024-02-25 14:11:14.480558 arts-2024.4.3/arts/tutorials/300-开发桌面GUI应用/art.json
+-rw-r--r--   0        0        0      103 2024-02-18 14:43:25.042841 arts-2024.4.3/arts/tutorials/450-对接ChatGPT/art.json
+-rw-r--r--   0        0        0      122 2024-03-22 15:10:08.573597 arts-2024.4.3/arts/tutorials/525-时间模块/art.json
+-rw-r--r--   0        0        0      100 2024-03-06 01:01:25.689741 arts-2024.4.3/arts/tutorials/562-面向对象数据库/art.json
+-rw-r--r--   0        0        0     3415 2023-12-20 10:09:07.822297 arts-2024.4.3/arts/tutorials/600-用37行代码实现AI五子棋/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:14:03.255370 arts-2024.4.3/arts/tutorials/600-用37行代码实现AI五子棋/art.json
+-rw-r--r--   0        0        0     8070 2024-02-25 05:45:21.624081 arts-2024.4.3/arts/tutorials/750-正则表达式/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:13:55.412792 arts-2024.4.3/arts/tutorials/750-正则表达式/art.json
+-rw-r--r--   0        0        0       44 2024-01-30 03:46:52.790397 arts-2024.4.3/arts/videos/200-秦时明月[项羽]·谪居/art.json
+-rw-r--r--   0        0        0       44 2023-12-19 10:07:05.944886 arts-2024.4.3/arts/videos/400-李连杰[霍元甲]·兰亭序/art.json
+-rw-r--r--   0        0        0       44 2023-12-19 10:07:05.933448 arts-2024.4.3/arts/videos/600-楚门的世界·五月雨/art.json
+-rw-r--r--   0        0        0       44 2024-01-05 13:31:13.729378 arts-2024.4.3/arts/videos/800-AI是这样画包拯的/art.json
+-rw-r--r--   0        0        0      524 2024-04-03 06:13:45.949704 arts-2024.4.3/pyproject.toml
+-rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 arts-2024.4.3/PKG-INFO
```

### Comparing `arts-2024.3.6/.gitignore` & `arts-2024.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/CoolMemory-English/README.md` & `arts-2024.4.3/arts/CoolMemory-English/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 当前版本：v1.0
 
 # 作者
 
 [江南雨上](mailto:lcctoor@outlook.com)
 
-[主页](https://lcctoor.github.io/arts/) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com)
+[主页](https://lcctoor.github.io/arts) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com)
 
 # 下载地址
 
 * [OneDrive](https://1drv.ms/f/s!AvKC1LvuVvx_gVZttKv6md5tgnOB) / Release / CoolMemory-English / v1.0 -binary -20231211.zip
 * [百度网盘](https://pan.baidu.com/s/1FaAz83Ima2uNE_I6Q9TDQg?pwd=nqt8)（提取码：nqt8） / Release / CoolMemory-English / v1.0 -binary -20231211.zip
 
 # 理论基础
```

### Comparing `arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/Python/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/Python/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE` & `arts-2024.4.3/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/010-赚钱宝典/010-财富的本质/README.md` & `arts-2024.4.3/arts/articles/010-赚钱宝典/010-财富的本质/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/010-赚钱宝典/020-商业价值/README.md` & `arts-2024.4.3/arts/articles/010-赚钱宝典/020-商业价值/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md` & `arts-2024.4.3/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md` & `arts-2024.4.3/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md` & `arts-2024.4.3/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/150-小民参政/300-广义的民主/README.md` & `arts-2024.4.3/arts/articles/150-小民参政/300-广义的民主/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md` & `arts-2024.4.3/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md` & `arts-2024.4.3/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md` & `arts-2024.4.3/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md` & `arts-2024.4.3/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-在今年国庆节的前一天，我的微信账号被人恶意举报导致封号，迫不得已更换了微信账号，这给我造成了很大的麻烦。对方竟然如此偏激和凶残，这引发我思考了一个经久的话题 —— 未经他人苦，莫劝他人善。
+经常有人说：未经他人苦，莫劝他人善。那么，这句话有道理吗？
 
 # 未经他人苦，莫劝他人善？
 
 我们需要区分这里的“善”具体指什么。
 
 如果这里的“善”指高尚的道德，如：助人为乐、舍己为人，那么我们自然没资格要求一个没被爱过的人去爱别人。
```

### Comparing `arts-2024.3.6/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md` & `arts-2024.4.3/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/450-万象思考/700-堕胎自由权/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/700-堕胎自由权/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md` & `arts-2024.4.3/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md` & `arts-2024.4.3/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md` & `arts-2024.4.3/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md` & `arts-2024.4.3/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md` & `arts-2024.4.3/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md` & `arts-2024.4.3/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md` & `arts-2024.4.3/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md` & `arts-2024.4.3/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md` & `arts-2024.4.3/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/cooltypes/Cooltime/README.md` & `arts-2024.4.3/arts/cooltypes/modules/cooltime/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,55 +2,55 @@
 
 一个优雅的时间模块。
 
 # 作者
 
 [江南雨上](mailto:lcctoor@outlook.com)
 
-[主页](https://lcctoor.github.io/arts/) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
+[主页](https://lcctoor.github.io/arts) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
+你可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
 
 # 安装
 
 ```
 pip install arts
 ```
 
 # 教程
 
 ## 导入
 
 ```python
-from arts.cooltypes import cooltime
+from arts.cooltypes import Cooltime
 ```
 
 ## 创建时间
 
 ```python
-t1 = cooltime()                                   # 创建1个当前时间
-t2 = cooltime.random()                            # 创建1个随机时间
-t3 = cooltime(1687271066.000028)                  # 从时间戳创建, 高精度
-t4 = cooltime(1687271066)                         # 从时间戳创建, 精确到秒
-t5 = cooltime(t3)                                 # 从 cooltime 创建
-t6 = cooltime('2023-06-20 22:24:26.000028')       # 从字符串创建, 高精度
-t7 = cooltime('2023-06-20 22:24:26')              # 从字符串创建, 精确到秒
-t8 = cooltime('2023-06-20 22:24')                 # 从字符串创建, 精确到分
-t9 = cooltime('2023-06-20 22')                    # 从字符串创建, 精确到时
-t10 = cooltime('2023-06-20')                      # 从字符串创建, 精确到日
-t11 = cooltime([2023, 6, 20, 22, 24, 26.000028])  # 从其它类型创建, 如: list、tuple、datetime、time.localtime ……
+t1 = Cooltime()                                   # 创建1个当前时间
+t2 = Cooltime.random()                            # 创建1个随机时间
+t3 = Cooltime(1687271066.000028)                  # 从时间戳创建, 高精度
+t4 = Cooltime(1687271066)                         # 从时间戳创建, 精确到秒
+t5 = Cooltime(t3)                                 # 从 Cooltime 创建
+t6 = Cooltime('2023-06-20 22:24:26.000028')       # 从字符串创建, 高精度
+t7 = Cooltime('2023-06-20 22:24:26')              # 从字符串创建, 精确到秒
+t8 = Cooltime('2023-06-20 22:24')                 # 从字符串创建, 精确到分
+t9 = Cooltime('2023-06-20 22')                    # 从字符串创建, 精确到时
+t10 = Cooltime('2023-06-20')                      # 从字符串创建, 精确到日
+t11 = Cooltime([2023, 6, 20, 22, 24, 26.000028])  # 从其它类型创建, 如: list、tuple、datetime、time.localtime ……
 ```
 
 注：
 
 1、从字符串创建时，字符串的格式可任意，比如 `2023/06/20/22/24/26.000028` 、`2023_06_20_22_24_26.000028` 、`2023.06+20-22:24#26.000028` 。
 
-2、从【时间戳、cooltime、字符串】以外的其它类型创建时，创建器会先执行 `str(obj)` 将对象转化成字符串，然后按处理字符串的方式创建。
+2、从【时间戳、Cooltime、字符串】以外的其它类型创建时，创建器会先执行 `str(obj)` 将对象转化成字符串，然后按处理字符串的方式创建。
 
 ## 转化为其它类型
 
 ```python
 t.date                            # '2023-06-20'
 t.time                            # '22:24:26.000028'
 t.datetime                        # '2023-06-20 22:24:26.000028'
@@ -85,15 +85,15 @@
 assert t4 <= t7
 assert t10 <= t9 <= t8 <= t7 <= t6
 ```
 
 ## 增量操作
 
 ```python
-B = cooltime('2023-06-20 22:24:26')
+B = Cooltime('2023-06-20 22:24:26')
 A = B.shift_copy(-3)  # 减3秒
 C = B.shift_copy(3)   # 加3秒
 print(A)              # '2023-06-20 22:24:23'
 print(B)              # '2023-06-20 22:24:26'
 print(C)              # '2023-06-20 22:24:29'
 print(A < B < C)      # True
 ```
```

### Comparing `arts-2024.3.6/arts/cooltypes/Cooltime/_core.py` & `arts-2024.4.3/arts/cooltypes/modules/cooltime/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import re
 from random import uniform
 from datetime import datetime as DT2
 from datetime import timedelta
-from typing import Union
 
 
 def parse_add(seconds=0, minutes=0, hours=0, days=0, weeks=0):
     return timedelta(seconds=seconds, minutes=minutes, hours=hours, days=days, weeks=weeks)
 
-def parse_time(datetime: Union[int, float, 'cooltime']=None) -> DT2:
+def parse_time(datetime: 'int|float|str|Cooltime|None'=None) -> DT2:
     typ = type(datetime)
     if typ in (int, float):  # 从时间戳生成
         return DT2.fromtimestamp(datetime)
     elif not datetime:  # 生成当前时区的当前时间
         return DT2.now()
-    elif isinstance(datetime, cooltime):  # 从自身类型生成
+    elif isinstance(datetime, Cooltime):  # 从自身类型生成
         return datetime._datetime
     else:  # 从字符串生成
         datetime = re.split(r'[^\d]+', re.sub(r'^[^\d]+', '', str(datetime)), 5)
         if len(datetime) == 6:
             if second := re.findall(r'(\d+)\.?(\d{0,6})', datetime.pop()):  # microsecond must be in 0..999999
                 datetime += second[0]
         return DT2(*[int(x) for x in datetime if x])
 
-class cooltime():
+class Cooltime():
 
-    def __init__(self, _datetime: Union[int, float, 'cooltime']=None):
+    def __init__(self, _datetime: 'int|float|str|Cooltime|None'=None):
         self._datetime = parse_time(_datetime)
 
     @property
     def year(self): return self._datetime.year
     
     @property
     def month(self): return self._datetime.month
@@ -46,27 +45,27 @@
     @property
     def second(self): return float(re.findall(r'[\d.]+$', str(self._datetime))[0])
 
     @staticmethod
     def random(start=None, end=None):
         if type(start) not in (int, float) and not start: start = 63043200  # 北京时间1972-01-01
         if type(end) not in (int, float) and not end: end = 2114352000  # 北京时间2037-01-01
-        return cooltime(uniform(float(cooltime(start)), float(cooltime(end))))
+        return Cooltime(uniform(float(Cooltime(start)), float(Cooltime(end))))
 
     def __eq__(self, _datetime): return self._datetime == parse_time(_datetime)
     def __ne__(self, _datetime): return self._datetime != parse_time(_datetime)
     def __lt__(self, _datetime): return self._datetime < parse_time(_datetime)
     def __le__(self, _datetime): return self._datetime <= parse_time(_datetime)
     def __ge__(self, _datetime): return self._datetime >= parse_time(_datetime)
     def __gt__(self, _datetime): return self._datetime >= parse_time(_datetime)
 
     def __float__(self): return self._datetime.timestamp()  # 1687271066.000028
     def __int__(self): return int(float(self))  # 1687271066
     def __str__(self): return self.datetime
-    def __repr__(self): return f"arts.cooltime<{self._datetime}>"  # arts.cooltime<2023-06-20 22:24:26.000028>
+    def __repr__(self): return f"arts.Cooltime<{self._datetime}>"  # arts.Cooltime<2023-06-20 22:24:26.000028>
 
     @property
     def datetime(self): return str(self._datetime)  # 2023-06-20 22:24:26.000028
 
     @property
     def floor_datetime(self): return self.datetime[:19]  # 2023-06-20 22:24:26
 
@@ -79,11 +78,11 @@
     @property
     def floor_time(self): return self.time[:8]  # 22:24:26
     
     def shift(self, seconds=0, minutes=0, hours=0, days=0, weeks=0):
         self._datetime += parse_add(seconds=seconds, minutes=minutes, hours=hours, days=days, weeks=weeks)
     
     def shift_copy(self, seconds=0, minutes=0, hours=0, days=0, weeks=0):
-        return cooltime(self._datetime + parse_add(seconds=seconds, minutes=minutes, hours=hours, days=days, weeks=weeks))
+        return Cooltime(self._datetime + parse_add(seconds=seconds, minutes=minutes, hours=hours, days=days, weeks=weeks))
     
     def strftime(self, fmt=r"%Y-%m-%d %H:%M:%S"):
         return self._datetime.strftime(fmt)
```

### Comparing `arts-2024.3.6/arts/cooltypes/LICENSE` & `arts-2024.4.3/arts/cooltypes/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/cooltypes/envname/README.md` & `arts-2024.4.3/arts/cooltypes/envname/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 有时候，对于某些功能，我们也许希望在不同的环境上采用不同的方案。以访问数据库为例：当程序在外网运行时，须通过数据库公网 ip 访问；而当程序在内网运行时，为了提高性能，我们可以通过数据库内网 ip 访问。
 
 # 作者
 
 [江南雨上](mailto:lcctoor@outlook.com)
 
-[主页](https://lcctoor.github.io/arts/) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
+[主页](https://lcctoor.github.io/arts) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
+你可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
 
 # 安装
 
 ```
 pip install arts
 ```
```

### Comparing `arts-2024.3.6/arts/cooltypes/moduledb/README.md` & `arts-2024.4.3/arts/cooltypes/moduledb/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/cooltypes/moduledb/_core.py` & `arts-2024.4.3/arts/cooltypes/moduledb/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/cooltypes/rstyleslice/README.md` & `arts-2024.4.3/arts/cooltypes/modules/rslice/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 项目描述
 
 一个符合直觉的索引和切片语法。
 
-|                                        | **Python**                                                           | rslice                                                                     |
+|                                        | **Python**                                                           | Rslice                                                                     |
 | -------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
 | **索引**                         | 从 0 开始（0 表示第 1 个元素）<br /><br />-1 表示倒数第 1 个元素（相同点） | 从 1 开始（1 表示第 1 个元素）<br /><br />-1 表示倒数第 1 个元素（相同点） |
 | **切片**                         | 左闭右开区间，例如：<br />[3: 5] 表示提取第 4、5 这 2 个元素               | 双闭区间，例如：<br />[3: 5] 表示提取第 3、4、5 这 3 个元素                |
 | **从右往**<br />**左切片** | step（步长）为负值，例如：<br />[9: 1: -1] 表示提取第 9~3 这 7 个元素      | step（步长）始终为正值，例如：<br />[9: 1: 1] 表示提取第 9~1 这 9 个元素   |
 
 切片格式为  [start: stop: step]  ，start 表示从哪条开始，stop 表示到哪条停止，step 表示步长。当  step>=2  时表示间隔式切片。
 
@@ -15,21 +15,21 @@
 ```
 pip install arts
 ```
 
 # 导入
 
 ```python
-from arts.cooltypes import rslice
+from arts.cooltypes import Rslice
 ```
 
 # 创建R风格容器
 
 ```python
-obj = rslice([1,2,3,4,5,6,7,8,9])
+obj = Rslice([1,2,3,4,5,6,7,8,9])
 ```
 
 Python中任何可以索引和切片的对象（如list、str、tuple）都可以转化成R风格容器。
 
 # 切片语法
 
 切片格式为  [start: stop: step]  ，start表示从哪条开始，stop表示到哪条停止，step表示步长。
@@ -124,15 +124,15 @@
 | obj[ 8: 2: 3 ]   | [8, 5, 2]         |
 | obj[ -2: 2: 3 ]  | [8, 5, 2]         |
 | obj[ -2: -8: 3 ] | [8, 5, 2]         |
 
 # 切片赋值
 
 ```python
-obj = rslice([111, 2, 3, 44, 55, 7, 8, 9])
+obj = Rslice([111, 2, 3, 44, 55, 7, 8, 9])
 
 obj[4:6] = []
 obj[:]
 # >>> [111, 2, 3, 8, 9]
 
 obj[4:] = [1, 2, 3, 4, 5]
 obj[:]
```

### Comparing `arts-2024.3.6/arts/cooltypes/rstyleslice/_core.py` & `arts-2024.4.3/arts/cooltypes/modules/rslice/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union
 
 
-class rslice:
+class Rslice:
     def __init__(self, core: Union[list, tuple, str]): self.core = core
     
     def __len__(self): return len(self.core)
 
     def __getitem__(self, key):
         core = self.core
         if isinstance(key, int):
```

### Comparing `arts-2024.3.6/arts/index.html` & `arts-2024.4.3/arts/index.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,146 +1,268 @@
 <!DOCTYPE html>
-<html class='ch_230'><head><title>江南雨上</title><meta content="FFA2094263C9178678410FC784304549" name="msvalidate.01"><meta content="UNx53G5kjiaAzNZavgTE604GQpveJ6pEtTPi3IMDfPg" name="google-site-verification"><style>
-* {vertical-align:middle; padding:0; outline:none; margin:0; font-family:'Chinese Quote', 'Segoe UI', Roboto, RobotoNum, 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'Helvetica Neue', Helvetica, Arial, sans-serif; box-sizing:border-box;}
-.ch_230 {position:relative; background-color:white;}
-.ch_251 {width:100vw; position:relative; padding:0.5rem 0 0 0; height:100vh; grid-auto-rows:3rem 1fr; display:inline-grid; border-width:0; border-radius:0; background-color:white;}
-.ch_252 {z-index:200; white-space:nowrap; scrollbar-width:none; overflow:auto; margin:0 1.25rem; justify-content:space-between; background-color:white; -ms-overflow-style:none;}
-.ch_238 {display:none;}
-.ch_254 {position:relative; padding:0.618em 1em 0.618em 1em; justify-items:center; font-size:1rem; display:inline-grid; border-width:0; border-radius:0; align-items:center;}
-#ch_8+.ch_256 {border-radius:3em; background-color:rgba(225, 172, 12, 0.744);}
-.ch_257 {top:0; right:0; position:absolute; height:2.5rem;}
-.ch_259 {padding:0; overflow:auto; display:none;}
-#ch_9+.ch_260 {display:block;}
-.ch_261 {z-index:100; width:100%; position:relative; min-height:calc(100vh - 3rem - 3rem); justify-items:center; display:inline-grid; border-width:0; border-radius:0; align-items:center; align-content:start;}
-.ch_235 {position:relative; justify-items:center; display:inline-grid; border-width:0; border-radius:0; align-items:center;}
-.ch_280 {width:100%; position:relative; padding:0 1.25rem; overflow-x:auto; margin:0.5rem 0; justify-items:center; justify-content:flex-start; grid-auto-flow:column; font-weight:500; font-size:1.5rem; display:inline-grid; color:rgb(225, 172, 12); border-width:0; border-radius:0; align-items:center;}
-.ch_265 {width:100%; row-gap:1.5rem; position:relative; overflow-x:auto; justify-items:center; justify-content:center; grid-template-columns:repeat(auto-fill, 15rem); display:inline-grid; column-gap:1.5rem; border-width:0; border-radius:0; align-items:center;}
-.ch_266 {width:15rem; text-decoration:none; position:relative; overflow-y:auto; justify-items:center; height:9.27rem; grid-template-rows:1fr auto; grid-auto-flow:row; display:inline-grid; color:black; border-width:0; border-radius:0; background-size:cover; background-color:rgb(255, 237, 195); align-items:center;}
-.ch_269 {width:100%; text-align:center; position:relative; overflow-x:auto; line-height:1.5; letter-spacing:0.075em; justify-items:center; height:100%; grid-auto-flow:column; font-size:1.1rem; display:inline-grid; border-width:0; border-radius:0; align-items:center;}
-.ch_271 {width:100%; position:relative; padding:0 0.25rem 0.25rem 0.25rem; overflow-x:auto; justify-items:end; grid-auto-flow:column; display:inline-grid; color:green; border-width:0; border-radius:0; align-items:end;}
-.ch_270 {width:100%; text-shadow:black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em; text-align:center; position:relative; overflow-x:auto; line-height:1.5; letter-spacing:0.075em; justify-items:center; height:100%; grid-auto-flow:column; font-weight:600; font-size:1.2rem; display:inline-grid; color:white; border-width:0; border-radius:0; align-items:center; -webkit-font-smoothing:antialiased;}
-.ch_281 {width:100%; position:relative; justify-items:center; display:inline-grid; border-width:0; border-radius:0; align-items:center;}
-.ch_262 {margin:1em 0; font-weight:500; font-size:1.5rem; color:rgb(225, 172, 12);}
-.ch_275 {row-gap:0.5rem; position:relative; justify-items:center; grid-template-rows:auto auto; grid-auto-flow:column; font-weight:500; font-size:1.1rem; display:inline-grid; column-gap:4rem; border-width:0; border-radius:0; align-items:center; align-content:center;}
-body[longaxis='y'] .ch_276 {width:100%; position:relative; overflow-x:auto; justify-items:center; grid-auto-flow:row; display:inline-grid; border-width:0; border-radius:0; align-items:center;}
-.ch_277 {position:relative; justify-items:center; display:inline-grid; border-width:0; border-radius:0; align-self:end; align-items:center;}
-body[longaxis='y'] .ch_278 {width:100%; position:relative; padding:1.5em 0 0 0; overflow-x:auto; justify-items:center; grid-auto-flow:column; display:inline-grid; color:rgb(225, 172, 12); border-width:0; border-radius:0; align-items:center;}
-.ch_279 {position:relative; justify-items:center; display:inline-grid; border-width:0; border-radius:0; align-self:start; align-items:center;}
-.ch_246 {text-decoration:none; padding:0 0.25em; color:#000000;}
-.ch_250 {vertical-align:middle;}
-.ch_248:visited {text-decoration:none; padding:0 0.25em; color:#000000;}
-.ch_255:hover {border-radius:3em; background-color:rgba(225, 172, 12, 0.24);}
-.ch_267:hover::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.3);}
-.ch_247:hover {text-decoration:underline; padding:0 0.25em; color:#1479d7;}
-.ch_268:active::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.5);}
-.ch_253::-webkit-scrollbar {display:none;}
-body[longaxis='y'] .ch_258 {display:none;}</style><meta charset="utf-8"><meta content="width=device-width, initial-scale=1.0" name="viewport"></head><body class='ch_251'><div class='ch_252 ch_253' onwheel="coolhtml.ch_284()" id="ch_137"><span class='ch_238' id="ch_8"></span><div class='ch_254 ch_255 ch_256' onclick="coolhtml.ch_285()" id="ch_120">动态</div><div class='ch_254 ch_255 ch_256' onclick="coolhtml.ch_286()" id="ch_123">视频</div><div class='ch_254 ch_255 ch_256' onclick="coolhtml.ch_287()" id="ch_125">文章</div><div class='ch_254 ch_255 ch_256' onclick="coolhtml.ch_288()" id="ch_127">想法</div><div class='ch_254 ch_255 ch_256' onclick="coolhtml.ch_289()" id="ch_129">软件</div><div class='ch_254 ch_255 ch_256' onclick="coolhtml.ch_290()" id="ch_131">Python教程</div><div class='ch_254 ch_255 ch_256' onclick="coolhtml.ch_291()" id="ch_133">生活</div><div class='ch_254 ch_255 ch_256' onclick="coolhtml.ch_292()" id="ch_135">自述</div><audio class='ch_257 ch_258' controls="" id="bgmusic"><source media="all" src="C:\\bpath\\standard\\vscode projects\\arts - static\\01\\ArtsBGM.ogg" type="audio/ogg"></audio></div><span class='ch_238' id="ch_9"></span><div class='ch_260 ch_259' id="ch_141"><div class='ch_261'><div class='ch_280'>2024-03-06</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="oodb/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>oodb<br/>（面向对象数据库）</div><div class='ch_271'>2024-03-06</div></a><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/oodb" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>面向对象数据库</div><div class='ch_271'>2024-03-06</div></a></div><div class='ch_280'>2024-02-13</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="miumapp/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_271'>2024-02-13</div></a><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/miumapp" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>开发跨平台GUI应用</div><div class='ch_271'>2024-02-13</div></a></div><div class='ch_280'>2024-01-30</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="videos/200-秦时明月[项羽]·谪居/README.mp4" onclick="bgmusic.pause()" target="_blank" style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_270'>秦时明月[项羽]·谪居</div><div class='ch_271'>2024-01-30</div></a></div><div class='ch_280'>2024-01-25</div><iframe class='ch_281' onload="coolhtml.ch_293()" id="ch_13" loading="lazy" src="thoughts/2024/萝莉岛事件引发的信任危机/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2024-01-13</div><iframe class='ch_281' onload="coolhtml.ch_294()" id="ch_17" loading="lazy" src="thoughts/2024/不要害怕犯错/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2024-01-09</div><iframe class='ch_281' onload="coolhtml.ch_295()" id="ch_21" loading="lazy" src="thoughts/2024/霍金去萝莉岛干嘛了/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2024-01-03</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/075-追英赶美/300-产业升级与失业潮/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_270'>产业升级与失业潮</div><div class='ch_271'>2024-01-03</div></a><a class='ch_268 ch_266 ch_267' href="articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_271'>2024-01-03</div></a></div><iframe class='ch_281' onload="coolhtml.ch_296()" id="ch_25" loading="lazy" src="thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2024-01-01</div><iframe class='ch_281' onload="coolhtml.ch_297()" id="ch_29" loading="lazy" src="thoughts/2024/新年题诗/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-12-28</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/700-论时事/300-那些年，我们经历过的历史/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>那些年，我们经历过的历史</div><div class='ch_271'>2023-12-28</div></a></div><div class='ch_280'>2023-12-22</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/010-赚钱宝典/030-财富稳定型社会/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>财富稳定型社会</div><div class='ch_271'>2023-12-22</div></a></div><div class='ch_280'>2023-12-11</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="CoolMemory-English/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_271'>2023-12-11</div></a></div><div class='ch_280'>2023-11-12</div><iframe class='ch_281' onload="coolhtml.ch_298()" id="ch_33" loading="lazy" src="thoughts/2023/只筛选，不教化/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-11-02</div><iframe class='ch_281' onload="coolhtml.ch_299()" id="ch_37" loading="lazy" src="thoughts/2023/现代化的分工合作机制/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-10-24</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>年轻人不结婚是文明的进步</div><div class='ch_271'>2023-10-24</div></a></div><div class='ch_280'>2023-10-09</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>未经他人苦，莫劝他人善？</div><div class='ch_271'>2023-10-09</div></a></div><div class='ch_280'>2023-10-06</div><iframe class='ch_281' onload="coolhtml.ch_300()" id="ch_105" loading="lazy" src="life/2023/更换微信账号了/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-09-22</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/010-赚钱宝典/020-商业价值/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>商业价值</div><div class='ch_271'>2023-09-22</div></a></div><div class='ch_280'>2023-09-20</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/010-赚钱宝典/010-财富的本质/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>财富的本质</div><div class='ch_271'>2023-09-20</div></a></div><div class='ch_280'>2023-09-15</div><iframe class='ch_281' onload="coolhtml.ch_301()" id="ch_41" loading="lazy" src="thoughts/2023/宣扬出来的宽容是恶的代名词/index.html"></iframe><hr style="width:100%;"><iframe class='ch_281' onload="coolhtml.ch_302()" id="ch_45" loading="lazy" src="thoughts/2023/什么是极端？/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-09-08</div><iframe class='ch_281' onload="coolhtml.ch_303()" id="ch_49" loading="lazy" src="thoughts/2023/专利是个公平的赛道/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-08-18</div><iframe class='ch_281' onload="coolhtml.ch_304()" id="ch_53" loading="lazy" src="thoughts/2023/真正的问题无法通过花招解决/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-08-17</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/500-人们为什么希望拥有后代/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>人们为什么希望拥有后代</div><div class='ch_271'>2023-08-17</div></a></div><div class='ch_280'>2023-08-06</div><iframe class='ch_281' onload="coolhtml.ch_305()" id="ch_57" loading="lazy" src="thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-30</div><iframe class='ch_281' onload="coolhtml.ch_306()" id="ch_61" loading="lazy" src="thoughts/2023/艺术本天成，媒介偶显之/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-20</div><iframe class='ch_281' onload="coolhtml.ch_307()" id="ch_65" loading="lazy" src="thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-19</div><iframe class='ch_281' onload="coolhtml.ch_308()" id="ch_69" loading="lazy" src="thoughts/2023/ChatGPT动了学阀的蛋糕/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-11</div><iframe class='ch_281' onload="coolhtml.ch_309()" id="ch_73" loading="lazy" src="thoughts/2023/想去国外了解自己/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-10</div><iframe class='ch_281' onload="coolhtml.ch_310()" id="ch_77" loading="lazy" src="thoughts/2023/人无法摆脱兽性/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-09</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>一元官司有意义吗？</div><div class='ch_271'>2023-07-09</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_271'>2023-07-09</div></a></div><div class='ch_280'>2023-07-06</div><iframe class='ch_281' onload="coolhtml.ch_311()" id="ch_81" loading="lazy" src="thoughts/2023/保护好人/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-04</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>心理学中个案研究有意义吗？</div><div class='ch_271'>2023-07-04</div></a></div><div class='ch_280'>2023-07-01</div><iframe class='ch_281' onload="coolhtml.ch_312()" id="ch_85" loading="lazy" src="thoughts/2023/用理性处理简单的事情/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-06-25</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/cooltypes/Cooltime" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>时间模块</div><div class='ch_271'>2023-06-25</div></a></div><div class='ch_280'>2023-06-19</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="tutorials/750-正则表达式/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>正则表达式</div><div class='ch_271'>2023-06-19</div></a></div><div class='ch_280'>2023-06-18</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_270'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_271'>2023-06-18</div></a></div><div class='ch_280'>2023-06-09</div><iframe class='ch_281' onload="coolhtml.ch_313()" id="ch_89" loading="lazy" src="thoughts/2023/事情的真实性是由度的/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-06-07</div><iframe class='ch_281' onload="coolhtml.ch_314()" id="ch_93" loading="lazy" src="thoughts/2023/喊高考加油是刷存在感/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-05-26</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>万物为什么会遵循着物理定律？</div><div class='ch_271'>2023-05-26</div></a></div><div class='ch_280'>2023-05-13</div><iframe class='ch_281' onload="coolhtml.ch_315()" id="ch_97" loading="lazy" src="thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-03-07</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="openai2/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>openai2<br/>（openai接口封装）</div><div class='ch_271'>2023-03-07</div></a><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/openai2" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>对接ChatGPT</div><div class='ch_271'>2023-03-07</div></a></div><div class='ch_280'>2023-03-06</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>ChatGPT已经有自我意识了</div><div class='ch_271'>2023-03-06</div></a></div><div class='ch_280'>2022-12-31</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/300-批判那些伪文艺/800-务实与务虚/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>务实与务虚</div><div class='ch_271'>2022-12-31</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/800-人人平等是个伪概念/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>人人平等是个伪概念</div><div class='ch_271'>2022-12-31</div></a></div><div class='ch_280'>2022-12-25</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/200-人工智能会不会统治人类？/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_270'>人工智能会不会统治人类？</div><div class='ch_271'>2022-12-25</div></a></div><div class='ch_280'>2022-12-16</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/150-小民参政/300-广义的民主/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_270'>广义的民主</div><div class='ch_271'>2022-12-16</div></a></div><div class='ch_280'>2022-11-25</div><iframe class='ch_281' onload="coolhtml.ch_316()" id="ch_109" loading="lazy" src="life/2022/泉州市丰泽区·雨后街道/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2022-09-27</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="videos/400-李连杰[霍元甲]·兰亭序/README.mp4" onclick="bgmusic.pause()" target="_blank" style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_270'>李连杰[霍元甲]·兰亭序</div><div class='ch_271'>2022-09-27</div></a></div><div class='ch_280'>2022-09-21</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/700-堕胎自由权/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>堕胎自由权</div><div class='ch_271'>2022-09-21</div></a></div><div class='ch_280'>2022-09-08</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="videos/600-楚门的世界·五月雨/README.mp4" onclick="bgmusic.pause()" target="_blank" style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_270'>楚门的世界·五月雨</div><div class='ch_271'>2022-09-08</div></a></div><div class='ch_280'>2022-08-12</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/800-小说/600-一念天堂/050-被绑架/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>被绑架</div><div class='ch_271'>2022-08-12</div></a></div><div class='ch_280'>2022-08-01</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/100-怎么理解「迷信科学」？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>怎么理解「迷信科学」？</div><div class='ch_271'>2022-08-01</div></a></div><div class='ch_280'>2022-06-15</div><iframe class='ch_281' onload="coolhtml.ch_317()" id="ch_101" loading="lazy" src="thoughts/2022/现代工人的螺丝钉处境/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2021-07-28</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="videos/800-AI是这样画包拯的/README.mp4" onclick="bgmusic.pause()" target="_blank" style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_270'>AI是这样画包拯的</div><div class='ch_271'>2021-07-28</div></a></div><div class='ch_280'>2021-06-11</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>“自由意志”其实是“随机意志”</div><div class='ch_271'>2021-06-11</div></a></div><div class='ch_280'>2021-06-10</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/300-有无相生，难易相成的启发/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>有无相生，难易相成的启发</div><div class='ch_271'>2021-06-10</div></a></div><div class='ch_280'>2021-06-09</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/600-时空猜想/600-占卜真的存在吗？/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_270'>占卜真的存在吗？</div><div class='ch_271'>2021-06-09</div></a></div><div class='ch_280'>2021-06-07</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/600-时空猜想/400-我们可能处在人造世界/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>我们可能处在人造世界</div><div class='ch_271'>2021-06-07</div></a></div><div class='ch_280'>2021-06-06</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="oomongo/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>oomongo<br/>（MongoDB ODM）</div><div class='ch_271'>2021-06-06</div></a><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/oomongo" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>操作MongoDB</div><div class='ch_271'>2021-06-06</div></a><a class='ch_268 ch_266 ch_267' href="oomysql/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>oomysql<br/>（MySQL ORM）</div><div class='ch_271'>2021-06-06</div></a><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/oomysql" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>操作MySQL</div><div class='ch_271'>2021-06-06</div></a></div><div class='ch_280'>2021-06-05</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/600-时空猜想/200-轮回转世真的存在吗？/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_270'>轮回转世真的存在吗？</div><div class='ch_271'>2021-06-05</div></a></div><div class='ch_280'>2021-06-03</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_270'>唯有变化是不变的？</div><div class='ch_271'>2021-06-03</div></a></div><div class='ch_280'>2021-06-01</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/250-忒修斯之船悖论/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>忒修斯之船悖论</div><div class='ch_271'>2021-06-01</div></a></div><div class='ch_280'>2020-12-31</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>燕山宝藏 第1章</div><div class='ch_271'>2020-12-31</div></a></div><div class='ch_280'>2019-08-05</div><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="tutorials/600-用37行代码实现AI五子棋/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>用37行代码实现AI五子棋</div><div class='ch_271'>2019-08-05</div></a></div><div class='ch_280'>2019-05-01</div><iframe class='ch_281' onload="coolhtml.ch_318()" id="ch_113" loading="lazy" src="life/2019/苏州市虎丘山/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2018-05-28</div><iframe class='ch_281' onload="coolhtml.ch_319()" id="ch_117" loading="lazy" src="life/2018/莆田学院·毕业生留影/index.html"></iframe><hr style="width:100%;"></div><div class='ch_235' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; font-weight:500;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_260 ch_259' id="ch_143"><div class='ch_261'><h3 class='ch_262'>videos</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="videos/200-秦时明月[项羽]·谪居/README.mp4" onclick="bgmusic.pause()" target="_blank" style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_270'>秦时明月[项羽]·谪居</div><div class='ch_271'>2024-01-30</div></a><a class='ch_268 ch_266 ch_267' href="videos/400-李连杰[霍元甲]·兰亭序/README.mp4" onclick="bgmusic.pause()" target="_blank" style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_270'>李连杰[霍元甲]·兰亭序</div><div class='ch_271'>2022-09-27</div></a><a class='ch_268 ch_266 ch_267' href="videos/600-楚门的世界·五月雨/README.mp4" onclick="bgmusic.pause()" target="_blank" style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_270'>楚门的世界·五月雨</div><div class='ch_271'>2022-09-08</div></a><a class='ch_268 ch_266 ch_267' href="videos/800-AI是这样画包拯的/README.mp4" onclick="bgmusic.pause()" target="_blank" style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_270'>AI是这样画包拯的</div><div class='ch_271'>2021-07-28</div></a></div></div><div class='ch_235' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; font-weight:500;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_260 ch_259' id="ch_145"><div class='ch_261'><h3 class='ch_262'>赚钱宝典</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/010-赚钱宝典/010-财富的本质/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>财富的本质</div><div class='ch_271'>2023-09-20</div></a><a class='ch_268 ch_266 ch_267' href="articles/010-赚钱宝典/020-商业价值/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>商业价值</div><div class='ch_271'>2023-09-22</div></a><a class='ch_268 ch_266 ch_267' href="articles/010-赚钱宝典/030-财富稳定型社会/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>财富稳定型社会</div><div class='ch_271'>2023-12-22</div></a></div><h3 class='ch_262'>追英赶美</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/075-追英赶美/300-产业升级与失业潮/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_270'>产业升级与失业潮</div><div class='ch_271'>2024-01-03</div></a><a class='ch_268 ch_266 ch_267' href="articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_271'>2024-01-03</div></a></div><h3 class='ch_262'>小民参政</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/150-小民参政/300-广义的民主/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_270'>广义的民主</div><div class='ch_271'>2022-12-16</div></a><a class='ch_268 ch_266 ch_267' href="articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>年轻人不结婚是文明的进步</div><div class='ch_271'>2023-10-24</div></a></div><h3 class='ch_262'>批判那些伪文艺</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>一元官司有意义吗？</div><div class='ch_271'>2023-07-09</div></a><a class='ch_268 ch_266 ch_267' href="articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_270'>唯有变化是不变的？</div><div class='ch_271'>2021-06-03</div></a><a class='ch_268 ch_266 ch_267' href="articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>未经他人苦，莫劝他人善？</div><div class='ch_271'>2023-10-09</div></a><a class='ch_268 ch_266 ch_267' href="articles/300-批判那些伪文艺/800-务实与务虚/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>务实与务虚</div><div class='ch_271'>2022-12-31</div></a></div><h3 class='ch_262'>万象思考</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>ChatGPT已经有自我意识了</div><div class='ch_271'>2023-03-06</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/100-怎么理解「迷信科学」？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>怎么理解「迷信科学」？</div><div class='ch_271'>2022-08-01</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>心理学中个案研究有意义吗？</div><div class='ch_271'>2023-07-04</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/200-人工智能会不会统治人类？/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_270'>人工智能会不会统治人类？</div><div class='ch_271'>2022-12-25</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/250-忒修斯之船悖论/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>忒修斯之船悖论</div><div class='ch_271'>2021-06-01</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/300-有无相生，难易相成的启发/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>有无相生，难易相成的启发</div><div class='ch_271'>2021-06-10</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_271'>2023-07-09</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/500-人们为什么希望拥有后代/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>人们为什么希望拥有后代</div><div class='ch_271'>2023-08-17</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>万物为什么会遵循着物理定律？</div><div class='ch_271'>2023-05-26</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/700-堕胎自由权/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>堕胎自由权</div><div class='ch_271'>2022-09-21</div></a><a class='ch_268 ch_266 ch_267' href="articles/450-万象思考/800-人人平等是个伪概念/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>人人平等是个伪概念</div><div class='ch_271'>2022-12-31</div></a></div><h3 class='ch_262'>时空猜想</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/600-时空猜想/200-轮回转世真的存在吗？/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_270'>轮回转世真的存在吗？</div><div class='ch_271'>2021-06-05</div></a><a class='ch_268 ch_266 ch_267' href="articles/600-时空猜想/400-我们可能处在人造世界/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>我们可能处在人造世界</div><div class='ch_271'>2021-06-07</div></a><a class='ch_268 ch_266 ch_267' href="articles/600-时空猜想/600-占卜真的存在吗？/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_270'>占卜真的存在吗？</div><div class='ch_271'>2021-06-09</div></a><a class='ch_268 ch_266 ch_267' href="articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>“自由意志”其实是“随机意志”</div><div class='ch_271'>2021-06-11</div></a></div><h3 class='ch_262'>论时事</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/700-论时事/300-那些年，我们经历过的历史/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>那些年，我们经历过的历史</div><div class='ch_271'>2023-12-28</div></a><a class='ch_268 ch_266 ch_267' href="articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md" onclick="bgmusic.pause()" target="_blank" style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_270'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_271'>2023-06-18</div></a></div><h3 class='ch_262'>小说 / 陆小凤新传</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>燕山宝藏 第1章</div><div class='ch_271'>2020-12-31</div></a></div><h3 class='ch_262'>小说 / 一念天堂</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="articles/800-小说/600-一念天堂/050-被绑架/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>被绑架</div><div class='ch_271'>2022-08-12</div></a></div></div><div class='ch_235' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; font-weight:500;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_260 ch_259' id="ch_147"><div class='ch_261'><div class='ch_280'>2024-01-25</div><iframe class='ch_281' onload="coolhtml.ch_320()" id="ch_10" loading="lazy" src="thoughts/2024/萝莉岛事件引发的信任危机/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2024-01-13</div><iframe class='ch_281' onload="coolhtml.ch_321()" id="ch_15" loading="lazy" src="thoughts/2024/不要害怕犯错/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2024-01-09</div><iframe class='ch_281' onload="coolhtml.ch_322()" id="ch_19" loading="lazy" src="thoughts/2024/霍金去萝莉岛干嘛了/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2024-01-03</div><iframe class='ch_281' onload="coolhtml.ch_323()" id="ch_23" loading="lazy" src="thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2024-01-01</div><iframe class='ch_281' onload="coolhtml.ch_324()" id="ch_27" loading="lazy" src="thoughts/2024/新年题诗/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-11-12</div><iframe class='ch_281' onload="coolhtml.ch_325()" id="ch_31" loading="lazy" src="thoughts/2023/只筛选，不教化/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-11-02</div><iframe class='ch_281' onload="coolhtml.ch_326()" id="ch_35" loading="lazy" src="thoughts/2023/现代化的分工合作机制/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-09-15</div><iframe class='ch_281' onload="coolhtml.ch_327()" id="ch_39" loading="lazy" src="thoughts/2023/宣扬出来的宽容是恶的代名词/index.html"></iframe><hr style="width:100%;"><iframe class='ch_281' onload="coolhtml.ch_328()" id="ch_43" loading="lazy" src="thoughts/2023/什么是极端？/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-09-08</div><iframe class='ch_281' onload="coolhtml.ch_329()" id="ch_47" loading="lazy" src="thoughts/2023/专利是个公平的赛道/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-08-18</div><iframe class='ch_281' onload="coolhtml.ch_330()" id="ch_51" loading="lazy" src="thoughts/2023/真正的问题无法通过花招解决/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-08-06</div><iframe class='ch_281' onload="coolhtml.ch_331()" id="ch_55" loading="lazy" src="thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-30</div><iframe class='ch_281' onload="coolhtml.ch_332()" id="ch_59" loading="lazy" src="thoughts/2023/艺术本天成，媒介偶显之/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-20</div><iframe class='ch_281' onload="coolhtml.ch_333()" id="ch_63" loading="lazy" src="thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-19</div><iframe class='ch_281' onload="coolhtml.ch_334()" id="ch_67" loading="lazy" src="thoughts/2023/ChatGPT动了学阀的蛋糕/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-11</div><iframe class='ch_281' onload="coolhtml.ch_335()" id="ch_71" loading="lazy" src="thoughts/2023/想去国外了解自己/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-10</div><iframe class='ch_281' onload="coolhtml.ch_336()" id="ch_75" loading="lazy" src="thoughts/2023/人无法摆脱兽性/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-06</div><iframe class='ch_281' onload="coolhtml.ch_337()" id="ch_79" loading="lazy" src="thoughts/2023/保护好人/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-07-01</div><iframe class='ch_281' onload="coolhtml.ch_338()" id="ch_83" loading="lazy" src="thoughts/2023/用理性处理简单的事情/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-06-09</div><iframe class='ch_281' onload="coolhtml.ch_339()" id="ch_87" loading="lazy" src="thoughts/2023/事情的真实性是由度的/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-06-07</div><iframe class='ch_281' onload="coolhtml.ch_340()" id="ch_91" loading="lazy" src="thoughts/2023/喊高考加油是刷存在感/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2023-05-13</div><iframe class='ch_281' onload="coolhtml.ch_341()" id="ch_95" loading="lazy" src="thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2022-06-15</div><iframe class='ch_281' onload="coolhtml.ch_342()" id="ch_99" loading="lazy" src="thoughts/2022/现代工人的螺丝钉处境/index.html"></iframe><hr style="width:100%;"></div><div class='ch_235' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; font-weight:500;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_260 ch_259' id="ch_149"><div class='ch_261'><h3 class='ch_262'>software</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="CoolMemory-English/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_271'>2023-12-11</div></a><a class='ch_268 ch_266 ch_267' href="miumapp/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_271'>2024-02-13</div></a><a class='ch_268 ch_266 ch_267' href="oodb/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>oodb<br/>（面向对象数据库）</div><div class='ch_271'>2024-03-06</div></a><a class='ch_268 ch_266 ch_267' href="oomongo/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>oomongo<br/>（MongoDB ODM）</div><div class='ch_271'>2021-06-06</div></a><a class='ch_268 ch_266 ch_267' href="oomysql/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>oomysql<br/>（MySQL ORM）</div><div class='ch_271'>2021-06-06</div></a><a class='ch_268 ch_266 ch_267' href="openai2/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>openai2<br/>（openai接口封装）</div><div class='ch_271'>2023-03-07</div></a></div></div><div class='ch_235' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; font-weight:500;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_260 ch_259' id="ch_153"><div class='ch_261'><div class='ch_280'>2023-10-06</div><iframe class='ch_281' onload="coolhtml.ch_343()" id="ch_103" loading="lazy" src="life/2023/更换微信账号了/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2022-11-25</div><iframe class='ch_281' onload="coolhtml.ch_344()" id="ch_107" loading="lazy" src="life/2022/泉州市丰泽区·雨后街道/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2019-05-01</div><iframe class='ch_281' onload="coolhtml.ch_345()" id="ch_111" loading="lazy" src="life/2019/苏州市虎丘山/index.html"></iframe><hr style="width:100%;"><div class='ch_280'>2018-05-28</div><iframe class='ch_281' onload="coolhtml.ch_346()" id="ch_115" loading="lazy" src="life/2018/莆田学院·毕业生留影/index.html"></iframe><hr style="width:100%;"></div><div class='ch_235' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; font-weight:500;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_260 ch_259' id="ch_151"><div class='ch_261'><h3 class='ch_262'>tutorials</h3><div class='ch_265'><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/oomysql" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>操作MySQL</div><div class='ch_271'>2021-06-06</div></a><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/oomongo" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>操作MongoDB</div><div class='ch_271'>2021-06-06</div></a><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/miumapp" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>开发跨平台GUI应用</div><div class='ch_271'>2024-02-13</div></a><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/openai2" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>对接ChatGPT</div><div class='ch_271'>2023-03-07</div></a><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/cooltypes/Cooltime" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>时间模块</div><div class='ch_271'>2023-06-25</div></a><a class='ch_268 ch_266 ch_267' href="https://lcctoor.github.io/arts/arts/oodb" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>面向对象数据库</div><div class='ch_271'>2024-03-06</div></a><a class='ch_268 ch_266 ch_267' href="tutorials/600-用37行代码实现AI五子棋/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>用37行代码实现AI五子棋</div><div class='ch_271'>2019-08-05</div></a><a class='ch_268 ch_266 ch_267' href="tutorials/750-正则表达式/README.md" onclick="bgmusic.pause()" target="_blank"><div class='ch_269'>正则表达式</div><div class='ch_271'>2023-06-19</div></a></div></div><div class='ch_235' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; font-weight:500;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_260 ch_259' id="ch_155"><div class='ch_261' style="align-content:stretch;"><div class='ch_276 ch_275'><div class='ch_278 ch_277'>邮箱</div><div class='ch_279'><a class='ch_247 ch_246 ch_248' href="mailto:lcctoor@outlook.com">lcctoor@outlook.com</a></div><div class='ch_278 ch_277'>微信</div><div class='ch_279'><img class='ch_250' src="./ip_static/WeChatQRC.jpg" style="max-width:15rem; height:auto;"></div><div class='ch_278 ch_277'>捐赠</div><div class='ch_279'><img class='ch_250' src="./ip_static/DonationQRC-0rmb.jpg" style="max-width:15rem; height:auto;"></div></div></div><div class='ch_235' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; font-weight:500;">Copyright 2018-2024 lcctoor@outlook.com</div></div><script>bgmusic = document.getElementById("bgmusic"); bgmusic.play()</script><script>
-const coolhtml = {}
-coolhtml.ch_1 = window.innerWidth > window.innerHeight
-coolhtml.ch_2 = 
-        (ele, prop, value) => {
-            ele.setAttribute(prop, value)
-            ele[prop] = value
-        }
-    
-coolhtml.ch_3 = document.body
-{
-        if (coolhtml.ch_1) {  coolhtml.ch_2(coolhtml.ch_3, 'longaxis', 'x')  }
-        else {  coolhtml.ch_2(coolhtml.ch_3, 'longaxis', 'y')  }
-    }
-coolhtml.ch_138 = document.getElementById("ch_137")
-coolhtml.ch_139 = 
-        (ele, addpx, subpx) => {
-            if (event.deltaY > 0) {ele.scrollLeft += addpx}
-            else {ele.scrollLeft -= subpx}
-            event.preventDefault()  // 阻止默认的垂直滚动
-        }
-    
-coolhtml.ch_119 = document.getElementById("ch_8")
-coolhtml.ch_121 = document.getElementById("ch_120")
-coolhtml.ch_124 = document.getElementById("ch_123")
-coolhtml.ch_126 = document.getElementById("ch_125")
-coolhtml.ch_128 = document.getElementById("ch_127")
-coolhtml.ch_130 = document.getElementById("ch_129")
-coolhtml.ch_132 = document.getElementById("ch_131")
-coolhtml.ch_134 = document.getElementById("ch_133")
-coolhtml.ch_136 = document.getElementById("ch_135")
-coolhtml.ch_140 = document.getElementById("ch_9")
-coolhtml.ch_142 = document.getElementById("ch_141")
-coolhtml.ch_144 = document.getElementById("ch_143")
-coolhtml.ch_146 = document.getElementById("ch_145")
-coolhtml.ch_148 = document.getElementById("ch_147")
-coolhtml.ch_150 = document.getElementById("ch_149")
-coolhtml.ch_152 = document.getElementById("ch_151")
-coolhtml.ch_154 = document.getElementById("ch_153")
-coolhtml.ch_156 = document.getElementById("ch_155")
-coolhtml.ch_122 = (a, b) => {b.parentElement.insertBefore(a, b)}
-coolhtml.ch_11 = document.getElementById("ch_10")
-coolhtml.ch_14 = document.getElementById("ch_13")
-coolhtml.ch_16 = document.getElementById("ch_15")
-coolhtml.ch_18 = document.getElementById("ch_17")
-coolhtml.ch_20 = document.getElementById("ch_19")
-coolhtml.ch_22 = document.getElementById("ch_21")
-coolhtml.ch_24 = document.getElementById("ch_23")
-coolhtml.ch_26 = document.getElementById("ch_25")
-coolhtml.ch_28 = document.getElementById("ch_27")
-coolhtml.ch_30 = document.getElementById("ch_29")
-coolhtml.ch_32 = document.getElementById("ch_31")
-coolhtml.ch_34 = document.getElementById("ch_33")
-coolhtml.ch_36 = document.getElementById("ch_35")
-coolhtml.ch_38 = document.getElementById("ch_37")
-coolhtml.ch_40 = document.getElementById("ch_39")
-coolhtml.ch_42 = document.getElementById("ch_41")
-coolhtml.ch_44 = document.getElementById("ch_43")
-coolhtml.ch_46 = document.getElementById("ch_45")
-coolhtml.ch_48 = document.getElementById("ch_47")
-coolhtml.ch_50 = document.getElementById("ch_49")
-coolhtml.ch_52 = document.getElementById("ch_51")
-coolhtml.ch_54 = document.getElementById("ch_53")
-coolhtml.ch_56 = document.getElementById("ch_55")
-coolhtml.ch_58 = document.getElementById("ch_57")
-coolhtml.ch_60 = document.getElementById("ch_59")
-coolhtml.ch_62 = document.getElementById("ch_61")
-coolhtml.ch_64 = document.getElementById("ch_63")
-coolhtml.ch_66 = document.getElementById("ch_65")
-coolhtml.ch_68 = document.getElementById("ch_67")
-coolhtml.ch_70 = document.getElementById("ch_69")
-coolhtml.ch_72 = document.getElementById("ch_71")
-coolhtml.ch_74 = document.getElementById("ch_73")
-coolhtml.ch_76 = document.getElementById("ch_75")
-coolhtml.ch_78 = document.getElementById("ch_77")
-coolhtml.ch_80 = document.getElementById("ch_79")
-coolhtml.ch_82 = document.getElementById("ch_81")
-coolhtml.ch_84 = document.getElementById("ch_83")
-coolhtml.ch_86 = document.getElementById("ch_85")
-coolhtml.ch_88 = document.getElementById("ch_87")
-coolhtml.ch_90 = document.getElementById("ch_89")
-coolhtml.ch_92 = document.getElementById("ch_91")
-coolhtml.ch_94 = document.getElementById("ch_93")
-coolhtml.ch_96 = document.getElementById("ch_95")
-coolhtml.ch_98 = document.getElementById("ch_97")
-coolhtml.ch_100 = document.getElementById("ch_99")
-coolhtml.ch_102 = document.getElementById("ch_101")
-coolhtml.ch_104 = document.getElementById("ch_103")
-coolhtml.ch_106 = document.getElementById("ch_105")
-coolhtml.ch_108 = document.getElementById("ch_107")
-coolhtml.ch_110 = document.getElementById("ch_109")
-coolhtml.ch_112 = document.getElementById("ch_111")
-coolhtml.ch_114 = document.getElementById("ch_113")
-coolhtml.ch_116 = document.getElementById("ch_115")
-coolhtml.ch_118 = document.getElementById("ch_117")
-coolhtml.ch_12 = 
-        (iframe) => {
+<html class='ch_151 ch_152'><head>
+<title id='ch_146'>江南雨上</title><meta name='msvalidate.01' content='FFA2094263C9178678410FC784304549'><meta name='google-site-verification' content='UNx53G5kjiaAzNZavgTE604GQpveJ6pEtTPi3IMDfPg'><meta charset='utf-8'><meta name='viewport' content='width=device-width, initial-scale=1.0'>
+<style>
+    * {vertical-align:middle; text-decoration:none; position:relative; padding:0; overflow:auto; outline:none; margin:0; font-family:'Chinese Quote', 'Segoe UI', Roboto, RobotoNum, 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'Helvetica Neue', Helvetica, Arial, sans-serif; box-sizing:border-box; border-width:0; border-style:solid;}
+    .ch_152 {width:100vw; height:100vh; display:block; background-color:white;}
+    .ch_180 {display:inline-block; align-self:end;}
+    .ch_181 {display:inline-block; align-self:start;}
+    .ch_153 {width:100%; padding:0.5rem 0 0 0; height:100%; grid-auto-rows:3rem 1fr; display:inline-grid; background-color:white;}
+    .ch_164 {z-index:100; width:100%; min-height:calc(100vh - 3rem - 3.1rem); display:inline-grid; align-content:start;}
+    .ch_165 {padding:0 1.25rem; margin:0.5rem 0; justify-content:flex-start; font-weight:500; font-size:1.5rem; display:inline-grid; color:rgb(225, 172, 12);}
+    .ch_166 {width:100%; display:inline-grid;}
+    .ch_170 {width:15rem; text-decoration:none; height:9.27rem; grid-template-rows:1fr auto; display:inline-grid; color:black; background-size:cover; background-color:rgb(255, 237, 195);}
+    .ch_172 {width:100%; text-align:center; line-height:1.5; letter-spacing:0.075em; height:100%; font-size:1.1rem; display:inline-grid; align-items:center;}
+    .ch_173 {padding:0 0.25rem 0.25rem 0.25rem; justify-items:end; display:inline-grid; color:green; align-items:end;}
+    .ch_174 {width:100%; text-shadow:black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em; text-align:center; line-height:1.5; letter-spacing:0.075em; height:100%; font-weight:600; font-size:1.2rem; display:inline-grid; color:white; align-items:center; -webkit-font-smoothing:antialiased;}
+    .ch_175 {display:inline-grid;}
+    .ch_177 {row-gap:0.5rem; justify-items:center; justify-content:center; grid-template-rows:auto auto; grid-auto-flow:column; font-weight:500; font-size:1.1rem; display:inline-grid; column-gap:4rem; align-content:center;}
+    body[is_x_screen='False'] .ch_178 {grid-auto-flow:row; display:inline-grid;}
+    body[is_x_screen='False'] .ch_179 {padding:1.5em 0 0 0; display:inline-grid; color:rgb(225, 172, 12);}
+    .ch_155 {z-index:200; white-space:nowrap; scrollbar-width:none; overflow:auto; max-width:100%; margin:0 1.25rem; justify-content:space-between; display:inline-block; background-color:white; -ms-overflow-style:none;}
+    .ch_154::-webkit-scrollbar {display:none;}
+    .ch_168 {row-gap:1.5rem; justify-content:center; grid-template-columns:repeat(auto-fill, 15rem); display:inline-grid; column-gap:1.5rem;}
+    .ch_158 {padding:0.618em 1em 0.618em 1em; font-size:1rem; border-radius:3em; background-color:transparent;}
+    body[is_x_screen='True'] .ch_157:not([is_current_nav="True"]):hover {background-color:rgba(247, 215, 114, 0.45);}
+    .ch_156[is_current_nav="True"] {background-color:rgba(247, 215, 114, 1);}
+    .ch_159 {white-space:nowrap; scrollbar-width:none; overflow-x:auto; display:inline-block; -ms-overflow-style:none;}
+    .ch_162:not(.ch_exec_smooth_to_scrollLeft) {scroll-snap-type:x mandatory;}
+    .ch_161::-webkit-scrollbar {display:none;}
+    .ch_160 > * {white-space:normal;}
+    .ch_163 {width:100%; scroll-snap-align:start; padding:0; overflow:auto; margin:0; height:100%; flex-wrap:wrap; display:inline-flex;}
+    .ch_185 {vertical-align:middle;}
+    .ch_182 {vertical-align:baseline; display:inline-block; color:rgba(0, 89, 255, 0.758);}
+    .ch_184:hover {color:rgb(0, 55, 255);}
+    .ch_183:visited {color:rgba(0, 89, 255, 0.758);}
+    .ch_167 {border-width:0.02rem; border-color:rgb(205, 205, 205);}
+    .ch_176 {margin:1em 0; justify-self:center; font-weight:500; font-size:1.5rem; color:rgb(225, 172, 12);}
+    .ch_169:hover::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.3);}
+    .ch_171:active::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.5);}
+</style></head>
+<body class='ch_153'>
+<script>const ch = {}
+</script><div class='ch_154 ch_155' id='ch_127'><button class='ch_156 ch_157 is_nav ch_158' is_current_nav='True'>动态</button><button class='ch_156 ch_157 is_nav ch_158'>视频</button><button class='ch_156 ch_157 is_nav ch_158'>文章</button><button class='ch_156 ch_157 is_nav ch_158'>想法</button><button class='ch_156 ch_157 is_nav ch_158'>软件</button><button class='ch_156 ch_157 is_nav ch_158'>Python教程</button><button class='ch_156 ch_157 is_nav ch_158'>生活</button><button class='ch_156 ch_157 is_nav ch_158'>自述</button></div><div class='ch_159 ch_160 ch_161 ch_162' id='ch_140'><div class='ch_163'><div class='ch_164'><div class='ch_165'>2024-04-03</div><iframe class='ch_166' src='thoughts/2024/做有趣的事情/index.html' loading='lazy' id='ch_9'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-03-31</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_172'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_173'>2024-03-31</div></a></div><div class='ch_165'>2024-03-18</div><iframe class='ch_166' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id='ch_109'></iframe><hr class='ch_167' style="width:100%;"><iframe class='ch_166' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id='ch_13'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-03-06</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='oodb/README.md' target='_blank'><div class='ch_172'>oodb<br/>（面向对象数据库）</div><div class='ch_173'>2024-03-06</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_172'>面向对象数据库</div><div class='ch_173'>2024-03-06</div></a></div><div class='ch_165'>2024-02-13</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='miumapp/README.md' target='_blank'><div class='ch_172'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_173'>2024-02-13</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_172'>开发跨平台GUI应用</div><div class='ch_173'>2024-02-13</div></a></div><div class='ch_165'>2024-01-30</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_174'>秦时明月[项羽]·谪居</div><div class='ch_173'>2024-01-30</div></a></div><div class='ch_165'>2024-01-25</div><iframe class='ch_166' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id='ch_17'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-13</div><iframe class='ch_166' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id='ch_21'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-09</div><iframe class='ch_166' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id='ch_25'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-03</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_174'>产业升级与失业潮</div><div class='ch_173'>2024-01-03</div></a><a class='ch_169 ch_170 ch_171' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_172'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_173'>2024-01-03</div></a></div><iframe class='ch_166' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id='ch_29'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-01</div><iframe class='ch_166' src='thoughts/2024/新年题诗/index.html' loading='lazy' id='ch_33'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-12-28</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_172'>那些年，我们经历过的历史</div><div class='ch_173'>2023-12-28</div></a></div><div class='ch_165'>2023-12-22</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_172'>财富稳定型社会</div><div class='ch_173'>2023-12-22</div></a></div><div class='ch_165'>2023-12-11</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='CoolMemory-English/README.md' target='_blank'><div class='ch_172'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_173'>2023-12-11</div></a></div><div class='ch_165'>2023-11-12</div><iframe class='ch_166' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id='ch_37'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-11-02</div><iframe class='ch_166' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id='ch_41'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-10-24</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_172'>年轻人不结婚是文明的进步</div><div class='ch_173'>2023-10-24</div></a></div><div class='ch_165'>2023-10-09</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_172'>未经他人苦，莫劝他人善？</div><div class='ch_173'>2023-10-09</div></a></div><div class='ch_165'>2023-10-06</div><iframe class='ch_166' src='life/2023/更换微信账号了/index.html' loading='lazy' id='ch_113'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-09-22</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_172'>商业价值</div><div class='ch_173'>2023-09-22</div></a></div><div class='ch_165'>2023-09-20</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_172'>财富的本质</div><div class='ch_173'>2023-09-20</div></a></div><div class='ch_165'>2023-09-15</div><iframe class='ch_166' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id='ch_45'></iframe><hr class='ch_167' style="width:100%;"><iframe class='ch_166' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id='ch_49'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-09-08</div><iframe class='ch_166' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id='ch_53'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-08-18</div><iframe class='ch_166' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id='ch_57'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-08-17</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_172'>人们为什么希望拥有后代</div><div class='ch_173'>2023-08-17</div></a></div><div class='ch_165'>2023-08-06</div><iframe class='ch_166' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id='ch_61'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-30</div><iframe class='ch_166' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id='ch_65'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-20</div><iframe class='ch_166' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id='ch_69'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-19</div><iframe class='ch_166' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id='ch_73'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-11</div><iframe class='ch_166' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id='ch_77'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-10</div><iframe class='ch_166' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id='ch_81'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-09</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_172'>一元官司有意义吗？</div><div class='ch_173'>2023-07-09</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_172'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_173'>2023-07-09</div></a></div><div class='ch_165'>2023-07-06</div><iframe class='ch_166' src='thoughts/2023/保护好人/index.html' loading='lazy' id='ch_85'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-04</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_172'>心理学中个案研究有意义吗？</div><div class='ch_173'>2023-07-04</div></a></div><div class='ch_165'>2023-07-01</div><iframe class='ch_166' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id='ch_89'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-06-25</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_172'>时间模块</div><div class='ch_173'>2023-06-25</div></a></div><div class='ch_165'>2023-06-19</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_172'>正则表达式</div><div class='ch_173'>2023-06-19</div></a></div><div class='ch_165'>2023-06-18</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_174'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_173'>2023-06-18</div></a></div><div class='ch_165'>2023-06-09</div><iframe class='ch_166' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id='ch_93'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-06-07</div><iframe class='ch_166' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id='ch_97'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-05-26</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_172'>万物为什么会遵循着物理定律？</div><div class='ch_173'>2023-05-26</div></a></div><div class='ch_165'>2023-05-13</div><iframe class='ch_166' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id='ch_101'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-03-07</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='openai2/README.md' target='_blank'><div class='ch_172'>openai2<br/>（openai接口封装）</div><div class='ch_173'>2023-03-07</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_172'>对接ChatGPT</div><div class='ch_173'>2023-03-07</div></a></div><div class='ch_165'>2023-03-06</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_172'>ChatGPT已经有自我意识了</div><div class='ch_173'>2023-03-06</div></a></div><div class='ch_165'>2022-12-31</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_172'>务实与务虚</div><div class='ch_173'>2022-12-31</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_172'>人人平等是个伪概念</div><div class='ch_173'>2022-12-31</div></a></div><div class='ch_165'>2022-12-25</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_174'>人工智能会不会统治人类？</div><div class='ch_173'>2022-12-25</div></a></div><div class='ch_165'>2022-12-16</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_174'>广义的民主</div><div class='ch_173'>2022-12-16</div></a></div><div class='ch_165'>2022-11-25</div><iframe class='ch_166' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id='ch_117'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2022-09-27</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_174'>李连杰[霍元甲]·兰亭序</div><div class='ch_173'>2022-09-27</div></a></div><div class='ch_165'>2022-09-21</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_172'>堕胎自由权</div><div class='ch_173'>2022-09-21</div></a></div><div class='ch_165'>2022-09-08</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_174'>楚门的世界·五月雨</div><div class='ch_173'>2022-09-08</div></a></div><div class='ch_165'>2022-08-12</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_172'>被绑架</div><div class='ch_173'>2022-08-12</div></a></div><div class='ch_165'>2022-08-01</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_172'>怎么理解「迷信科学」？</div><div class='ch_173'>2022-08-01</div></a></div><div class='ch_165'>2022-06-15</div><iframe class='ch_166' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id='ch_105'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2021-07-28</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_174'>AI是这样画包拯的</div><div class='ch_173'>2021-07-28</div></a></div><div class='ch_165'>2021-06-11</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_172'>“自由意志”其实是“随机意志”</div><div class='ch_173'>2021-06-11</div></a></div><div class='ch_165'>2021-06-10</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_172'>有无相生，难易相成的启发</div><div class='ch_173'>2021-06-10</div></a></div><div class='ch_165'>2021-06-09</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_174'>占卜真的存在吗？</div><div class='ch_173'>2021-06-09</div></a></div><div class='ch_165'>2021-06-07</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_172'>我们可能处在人造世界</div><div class='ch_173'>2021-06-07</div></a></div><div class='ch_165'>2021-06-06</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='oomongo/README.md' target='_blank'><div class='ch_172'>oomongo<br/>（MongoDB ODM）</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_172'>操作MongoDB</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='oomysql/README.md' target='_blank'><div class='ch_172'>oomysql<br/>（MySQL ORM）</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_172'>操作MySQL</div><div class='ch_173'>2021-06-06</div></a></div><div class='ch_165'>2021-06-05</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_174'>轮回转世真的存在吗？</div><div class='ch_173'>2021-06-05</div></a></div><div class='ch_165'>2021-06-03</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_174'>唯有变化是不变的？</div><div class='ch_173'>2021-06-03</div></a></div><div class='ch_165'>2021-06-01</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_172'>忒修斯之船悖论</div><div class='ch_173'>2021-06-01</div></a></div><div class='ch_165'>2020-12-31</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_172'>燕山宝藏 第1章</div><div class='ch_173'>2020-12-31</div></a></div><div class='ch_165'>2019-08-05</div><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_172'>用37行代码实现AI五子棋</div><div class='ch_173'>2019-08-05</div></a></div><div class='ch_165'>2019-05-01</div><iframe class='ch_166' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id='ch_121'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2018-05-28</div><iframe class='ch_166' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id='ch_125'></iframe><hr class='ch_167' style="width:100%;"></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><h3 class='ch_176'>videos</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_174'>秦时明月[项羽]·谪居</div><div class='ch_173'>2024-01-30</div></a><a class='ch_169 ch_170 ch_171' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_174'>李连杰[霍元甲]·兰亭序</div><div class='ch_173'>2022-09-27</div></a><a class='ch_169 ch_170 ch_171' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_174'>楚门的世界·五月雨</div><div class='ch_173'>2022-09-08</div></a><a class='ch_169 ch_170 ch_171' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_174'>AI是这样画包拯的</div><div class='ch_173'>2021-07-28</div></a></div></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><h3 class='ch_176'>赚钱宝典</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_172'>财富的本质</div><div class='ch_173'>2023-09-20</div></a><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_172'>商业价值</div><div class='ch_173'>2023-09-22</div></a><a class='ch_169 ch_170 ch_171' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_172'>财富稳定型社会</div><div class='ch_173'>2023-12-22</div></a></div><h3 class='ch_176'>追英赶美</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_174'>产业升级与失业潮</div><div class='ch_173'>2024-01-03</div></a><a class='ch_169 ch_170 ch_171' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_172'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_173'>2024-01-03</div></a></div><h3 class='ch_176'>小民参政</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_174'>广义的民主</div><div class='ch_173'>2022-12-16</div></a><a class='ch_169 ch_170 ch_171' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_172'>年轻人不结婚是文明的进步</div><div class='ch_173'>2023-10-24</div></a></div><h3 class='ch_176'>批判那些伪文艺</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_172'>一元官司有意义吗？</div><div class='ch_173'>2023-07-09</div></a><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_174'>唯有变化是不变的？</div><div class='ch_173'>2021-06-03</div></a><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_172'>未经他人苦，莫劝他人善？</div><div class='ch_173'>2023-10-09</div></a><a class='ch_169 ch_170 ch_171' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_172'>务实与务虚</div><div class='ch_173'>2022-12-31</div></a></div><h3 class='ch_176'>万象思考</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_172'>ChatGPT已经有自我意识了</div><div class='ch_173'>2023-03-06</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_172'>怎么理解「迷信科学」？</div><div class='ch_173'>2022-08-01</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_172'>心理学中个案研究有意义吗？</div><div class='ch_173'>2023-07-04</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_174'>人工智能会不会统治人类？</div><div class='ch_173'>2022-12-25</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_172'>忒修斯之船悖论</div><div class='ch_173'>2021-06-01</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_172'>有无相生，难易相成的启发</div><div class='ch_173'>2021-06-10</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_172'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_173'>2023-07-09</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_172'>人们为什么希望拥有后代</div><div class='ch_173'>2023-08-17</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_172'>万物为什么会遵循着物理定律？</div><div class='ch_173'>2023-05-26</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_172'>堕胎自由权</div><div class='ch_173'>2022-09-21</div></a><a class='ch_169 ch_170 ch_171' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_172'>人人平等是个伪概念</div><div class='ch_173'>2022-12-31</div></a></div><h3 class='ch_176'>时空猜想</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_174'>轮回转世真的存在吗？</div><div class='ch_173'>2021-06-05</div></a><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_172'>我们可能处在人造世界</div><div class='ch_173'>2021-06-07</div></a><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_174'>占卜真的存在吗？</div><div class='ch_173'>2021-06-09</div></a><a class='ch_169 ch_170 ch_171' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_172'>“自由意志”其实是“随机意志”</div><div class='ch_173'>2021-06-11</div></a></div><h3 class='ch_176'>论时事</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_172'>那些年，我们经历过的历史</div><div class='ch_173'>2023-12-28</div></a><a class='ch_169 ch_170 ch_171' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_174'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_173'>2023-06-18</div></a></div><h3 class='ch_176'>小说 / 陆小凤新传</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_172'>燕山宝藏 第1章</div><div class='ch_173'>2020-12-31</div></a></div><h3 class='ch_176'>小说 / 一念天堂</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_172'>被绑架</div><div class='ch_173'>2022-08-12</div></a></div></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><div class='ch_165'>2024-04-03</div><iframe class='ch_166' src='thoughts/2024/做有趣的事情/index.html' loading='lazy' id='ch_6'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-03-18</div><iframe class='ch_166' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id='ch_11'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-25</div><iframe class='ch_166' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id='ch_15'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-13</div><iframe class='ch_166' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id='ch_19'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-09</div><iframe class='ch_166' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id='ch_23'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-03</div><iframe class='ch_166' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id='ch_27'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2024-01-01</div><iframe class='ch_166' src='thoughts/2024/新年题诗/index.html' loading='lazy' id='ch_31'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-11-12</div><iframe class='ch_166' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id='ch_35'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-11-02</div><iframe class='ch_166' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id='ch_39'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-09-15</div><iframe class='ch_166' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id='ch_43'></iframe><hr class='ch_167' style="width:100%;"><iframe class='ch_166' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id='ch_47'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-09-08</div><iframe class='ch_166' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id='ch_51'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-08-18</div><iframe class='ch_166' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id='ch_55'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-08-06</div><iframe class='ch_166' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id='ch_59'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-30</div><iframe class='ch_166' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id='ch_63'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-20</div><iframe class='ch_166' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id='ch_67'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-19</div><iframe class='ch_166' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id='ch_71'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-11</div><iframe class='ch_166' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id='ch_75'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-10</div><iframe class='ch_166' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id='ch_79'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-06</div><iframe class='ch_166' src='thoughts/2023/保护好人/index.html' loading='lazy' id='ch_83'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-07-01</div><iframe class='ch_166' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id='ch_87'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-06-09</div><iframe class='ch_166' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id='ch_91'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-06-07</div><iframe class='ch_166' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id='ch_95'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-05-13</div><iframe class='ch_166' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id='ch_99'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2022-06-15</div><iframe class='ch_166' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id='ch_103'></iframe><hr class='ch_167' style="width:100%;"></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><h3 class='ch_176'>software</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='CoolMemory-English/README.md' target='_blank'><div class='ch_172'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_173'>2023-12-11</div></a><a class='ch_169 ch_170 ch_171' href='miumapp/README.md' target='_blank'><div class='ch_172'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_173'>2024-02-13</div></a><a class='ch_169 ch_170 ch_171' href='oodb/README.md' target='_blank'><div class='ch_172'>oodb<br/>（面向对象数据库）</div><div class='ch_173'>2024-03-06</div></a><a class='ch_169 ch_170 ch_171' href='oomongo/README.md' target='_blank'><div class='ch_172'>oomongo<br/>（MongoDB ODM）</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='oomysql/README.md' target='_blank'><div class='ch_172'>oomysql<br/>（MySQL ORM）</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='openai2/README.md' target='_blank'><div class='ch_172'>openai2<br/>（openai接口封装）</div><div class='ch_173'>2023-03-07</div></a><a class='ch_169 ch_170 ch_171' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_172'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_173'>2024-03-31</div></a></div></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><h3 class='ch_176'>tutorials</h3><div class='ch_168'><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_172'>操作MySQL</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_172'>操作MongoDB</div><div class='ch_173'>2021-06-06</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_172'>开发跨平台GUI应用</div><div class='ch_173'>2024-02-13</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_172'>对接ChatGPT</div><div class='ch_173'>2023-03-07</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_172'>时间模块</div><div class='ch_173'>2023-06-25</div></a><a class='ch_169 ch_170 ch_171' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_172'>面向对象数据库</div><div class='ch_173'>2024-03-06</div></a><a class='ch_169 ch_170 ch_171' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_172'>用37行代码实现AI五子棋</div><div class='ch_173'>2019-08-05</div></a><a class='ch_169 ch_170 ch_171' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_172'>正则表达式</div><div class='ch_173'>2023-06-19</div></a></div></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164'><div class='ch_165'>2024-03-18</div><iframe class='ch_166' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id='ch_107'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2023-10-06</div><iframe class='ch_166' src='life/2023/更换微信账号了/index.html' loading='lazy' id='ch_111'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2022-11-25</div><iframe class='ch_166' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id='ch_115'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2019-05-01</div><iframe class='ch_166' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id='ch_119'></iframe><hr class='ch_167' style="width:100%;"><div class='ch_165'>2018-05-28</div><iframe class='ch_166' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id='ch_123'></iframe><hr class='ch_167' style="width:100%;"></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_163'><div class='ch_164' style="align-content:stretch;"><div class='ch_177 ch_178'><div class='ch_179 ch_180'>邮箱</div><div class='ch_181'><a class='ch_182 ch_183 ch_184' href='mailto:lcctoor@outlook.com'>lcctoor@outlook.com</a></div><div class='ch_179 ch_180'>微信</div><div class='ch_181'><img class='ch_185' src='./ip_static/WeChatQRC.jpg' style="max-width:15rem; height:auto;"></div><div class='ch_179 ch_180'>捐赠</div><div class='ch_181'><img class='ch_185' src='./ip_static/DonationQRC-0rmb.jpg' style="max-width:15rem; height:auto;"></div></div></div><div class='ch_175' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div></div>
+<script>
+ch.ch_1 = () => window.innerWidth > window.innerHeight
+ch.ch_2 = (ele, name, value) => {
+            ele.setAttribute(name, value)
+            ele[name] = value
+        }
+ch.ch_3 = document.body
+ch.ch_130 = () => {
+            let value = ch.ch_1()
+            if (value)
+                { ch.ch_2(ch.ch_3, 'is_x_screen', 'True') }
+            else
+                { ch.ch_2(ch.ch_3, 'is_x_screen', 'False') }
+            return value
+        }
+ch.ch_130()
+ch.ch_128 = document.getElementById("ch_127")
+ch.ch_135 = Array.from(ch.ch_128.querySelectorAll('.is_nav'))
+ch.ch_131 = (last_value, items) =>
+            value => {
+                if (last_value.get('last_value') !== value) {
+                    last_value.set('last_value', value)
+                    for (let set_value of items)
+                        {set_value(value)}
+                }
+            }
+ch.ch_132 = new Map([["last_value", null]])
+ch.ch_134 = (navigation, navs, value) => {
+            let index = Number(value)
+            if (Number.isInteger(index))  {  // 3.0、4.0 这种格式也会表现为 True
+                let nav = navs[parseInt(index) - 1]
+                if (nav) {
+                    for (let x of navs)
+                        { x.setAttribute('is_current_nav', 'False') }
+                    nav.setAttribute('is_current_nav', 'True')
+                    let nav_rect = nav.getBoundingClientRect()
+                    let navigation_rect = navigation.getBoundingClientRect()
+                    let right = nav_rect.right - navigation_rect.right
+                    let left = nav_rect.left - navigation_rect.left
+                    if (right > 0)
+                        { navigation.scrollLeft += right }
+                    else if (left < 0)
+                        { navigation.scrollLeft += left }
+                }
+            }
+        }
+ch.ch_138 = value => ch.ch_134(ch.ch_128, ch.ch_135, value)
+ch.ch_4 = async (ele, scrollLeft, seconds=0) => {
+            if (seconds) {
+                let start_time = performance.now()  // 立即获取当前时间，以尽可能让时间准确
+                ele.classList.add('ch_exec_smooth_to_scrollLeft')  // 立即设为 ch_exec_smooth_to_scrollLeft
+                let milliseconds = seconds * 1000
+                let end_time = start_time + milliseconds
+                let start_scrollLeft = ele.scrollLeft
+                let distance = scrollLeft - start_scrollLeft
+                let gradient = distance / milliseconds  // 斜率
+                let state = {'finished': false}
+                let scroll = () => {
+                    let current_time = performance.now()
+                    if (current_time < end_time)
+                        ele.scrollLeft = gradient * (current_time - start_time) + start_scrollLeft  // y = k*x + b
+                    else
+                        state['finished'] = true
+                }
+                while (true) {
+                    await new Promise(resolve => requestAnimationFrame(() => {scroll(); resolve()}))  // 在这一步会释放事件循环的loop
+                    // requestAnimationFrame 和 setTimeout 都可用于延迟运行。但前者是专为动画设计的，会在浏览器下一次重绘前被执行
+                    if (state['finished']) break
+                }
+                ele.classList.remove('ch_exec_smooth_to_scrollLeft')
+                ele.scrollLeft = scrollLeft  // 两个功能：确保最终位置正确、激活同步
+            }
+            else
+                ele.scrollLeft = scrollLeft
+        }
+ch.ch_139 = (pages_box, current_index, scroll_seconds) =>
+            async value => {
+                let index = Number(value)
+                if (Number.isInteger(index))  {  // 3.0、4.0 这种格式也会表现为 True
+                    index = parseInt(index)  // 转化为 3、4 这种真正的整数
+                    if ( index !== current_index.get('current_index') ) {
+                        let page = pages_box.children[index - 1]
+                        if (page) {
+                            current_index.set('current_index', index)
+                            if (scroll_seconds)
+                                await ch.ch_4(pages_box, page.offsetLeft, scroll_seconds)
+                            else
+                                pages_box.scrollLeft = page.offsetLeft
+                        }
+                    }
+                }
+            }
+ch.ch_141 = document.getElementById("ch_140")
+ch.ch_142 = new Map([["current_index", null]])
+ch.ch_144 = ch.ch_139(ch.ch_141, ch.ch_142, 0.2)
+ch.ch_145 = (ele, set_dict, value) => {
+            value = set_dict.has(value) ? set_dict.get(value) : value
+            ele.firstChild.textContent = value
+        }
+ch.ch_147 = document.getElementById("ch_146")
+ch.ch_148 = new Map([["1", "动态"], ["2", "视频"], ["3", "文章"], ["4", "想法"], ["5", "软件"], ["6", "Python教程"], ["7", "生活"], ["8", "自述"]])
+ch.ch_150 = value => ch.ch_145(ch.ch_147, ch.ch_148, value)
+ch.ch_133 = [ch.ch_138, ch.ch_144, ch.ch_150]
+ch.ch_136 = ch.ch_131(ch.ch_132, ch.ch_133)
+ch.ch_137 = (navigation, navs, sync_value) => {
+            navigation.addEventListener('click',
+                () => {
+                    let nav = event.target
+                    if (nav.classList.contains('is_nav'))
+                        {sync_value(String( navs.indexOf(nav)+1 ))}
+                }
+            )
+        }
+ch.ch_137(ch.ch_128, ch.ch_135, ch.ch_136)
+ch.ch_143 = (pages_box, current_index, sync_value) => {
+            pages_box.addEventListener('scroll',
+                () => {
+                    if (! pages_box.classList.contains('ch_exec_smooth_to_scrollLeft')) {
+                        let index = Math.round(pages_box.scrollLeft / pages_box.clientWidth) + 1
+                        if (index !== current_index.get('current_index')) {
+                            current_index.set('current_index', index)
+                            sync_value( String(index) )
+                        }
+                    }
+                }
+            )
+        }
+ch.ch_143(ch.ch_141, ch.ch_142, ch.ch_136)
+ch.ch_5 = window.MutationObserver || window.WebKitMutationObserver || window.MozMutationObserver
+ch.ch_149 = (sync_value, ele, last_value, set_dict) => {
+            let textNode = null
+            let firstSon = ele.firstChild
+            if (firstSon && firstSon.nodeName === '#text')
+                { textNode = firstSon }
+            else {
+                textNode = document.createTextNode('')
+                if (firstSon)
+                    { ele.insertBefore(textNode, firstSon) }
+                else
+                    { ele.appendChild(textNode) }
+            }
+            new ch.ch_5(
+                (records, _) => { sync_value(textNode.textContent) }
+            ).observe(textNode, {characterData: true})
+        }
+ch.ch_149(ch.ch_136, ch.ch_147, ch.ch_132, ch.ch_148)
+ch.ch_129 = (ele, px) => {
+                    ele.scrollLeft += px
+                    event.preventDefault()  // 阻止其它默认行为
+                }
+ch.ch_128.addEventListener('wheel', () => {ch.ch_129(ch.ch_128, event.deltaY)})
+ch.ch_7 = document.getElementById("ch_6")
+ch.ch_10 = document.getElementById("ch_9")
+ch.ch_12 = document.getElementById("ch_11")
+ch.ch_14 = document.getElementById("ch_13")
+ch.ch_16 = document.getElementById("ch_15")
+ch.ch_18 = document.getElementById("ch_17")
+ch.ch_20 = document.getElementById("ch_19")
+ch.ch_22 = document.getElementById("ch_21")
+ch.ch_24 = document.getElementById("ch_23")
+ch.ch_26 = document.getElementById("ch_25")
+ch.ch_28 = document.getElementById("ch_27")
+ch.ch_30 = document.getElementById("ch_29")
+ch.ch_32 = document.getElementById("ch_31")
+ch.ch_34 = document.getElementById("ch_33")
+ch.ch_36 = document.getElementById("ch_35")
+ch.ch_38 = document.getElementById("ch_37")
+ch.ch_40 = document.getElementById("ch_39")
+ch.ch_42 = document.getElementById("ch_41")
+ch.ch_44 = document.getElementById("ch_43")
+ch.ch_46 = document.getElementById("ch_45")
+ch.ch_48 = document.getElementById("ch_47")
+ch.ch_50 = document.getElementById("ch_49")
+ch.ch_52 = document.getElementById("ch_51")
+ch.ch_54 = document.getElementById("ch_53")
+ch.ch_56 = document.getElementById("ch_55")
+ch.ch_58 = document.getElementById("ch_57")
+ch.ch_60 = document.getElementById("ch_59")
+ch.ch_62 = document.getElementById("ch_61")
+ch.ch_64 = document.getElementById("ch_63")
+ch.ch_66 = document.getElementById("ch_65")
+ch.ch_68 = document.getElementById("ch_67")
+ch.ch_70 = document.getElementById("ch_69")
+ch.ch_72 = document.getElementById("ch_71")
+ch.ch_74 = document.getElementById("ch_73")
+ch.ch_76 = document.getElementById("ch_75")
+ch.ch_78 = document.getElementById("ch_77")
+ch.ch_80 = document.getElementById("ch_79")
+ch.ch_82 = document.getElementById("ch_81")
+ch.ch_84 = document.getElementById("ch_83")
+ch.ch_86 = document.getElementById("ch_85")
+ch.ch_88 = document.getElementById("ch_87")
+ch.ch_90 = document.getElementById("ch_89")
+ch.ch_92 = document.getElementById("ch_91")
+ch.ch_94 = document.getElementById("ch_93")
+ch.ch_96 = document.getElementById("ch_95")
+ch.ch_98 = document.getElementById("ch_97")
+ch.ch_100 = document.getElementById("ch_99")
+ch.ch_102 = document.getElementById("ch_101")
+ch.ch_104 = document.getElementById("ch_103")
+ch.ch_106 = document.getElementById("ch_105")
+ch.ch_108 = document.getElementById("ch_107")
+ch.ch_110 = document.getElementById("ch_109")
+ch.ch_112 = document.getElementById("ch_111")
+ch.ch_114 = document.getElementById("ch_113")
+ch.ch_116 = document.getElementById("ch_115")
+ch.ch_118 = document.getElementById("ch_117")
+ch.ch_120 = document.getElementById("ch_119")
+ch.ch_122 = document.getElementById("ch_121")
+ch.ch_124 = document.getElementById("ch_123")
+ch.ch_126 = document.getElementById("ch_125")
+ch.ch_8 = iframe => {
             let i_document = iframe.contentDocument || iframe.contentWindow.document
             try {
                 let anchor = i_document.querySelector('a[href^="https://lcctoor.github.io"]')
                 if (anchor) {anchor.parentElement.remove()}
-                for (let a of i_document.querySelectorAll('a')) {
-                    a.setAttribute('target', '_blank')
-                }
+                for (let a of i_document.querySelectorAll('a'))
+                    { a.setAttribute('target', '_blank') }
             }
             catch (e) {console.log('无法访问 iframe:', frame, e)}
             let styleElement = i_document.createElement('style')
             styleElement.textContent = `
                 body::-webkit-scrollbar {display: none;}
                 body {scrollbar-width: none; -ms-overflow-style: none; overflow: hidden;}
             `
@@ -154,80 +276,71 @@
                     iframe.contentWindow.removeEventListener('click', set_height)
                 }
             }
             iframe.contentWindow.addEventListener('mouseover', set_height)
             iframe.contentWindow.addEventListener('wheel', set_height)
             iframe.contentWindow.addEventListener('click', set_height)
         }
-    
-coolhtml.ch_284 = () => {{coolhtml.ch_139(coolhtml.ch_138, 40, 40)}}
-coolhtml.ch_285 = () => {{coolhtml.ch_122(coolhtml.ch_119, coolhtml.ch_121)}
-{coolhtml.ch_122(coolhtml.ch_140, coolhtml.ch_142)}}
-coolhtml.ch_286 = () => {{coolhtml.ch_122(coolhtml.ch_119, coolhtml.ch_124)}
-{coolhtml.ch_122(coolhtml.ch_140, coolhtml.ch_144)}}
-coolhtml.ch_287 = () => {{coolhtml.ch_122(coolhtml.ch_119, coolhtml.ch_126)}
-{coolhtml.ch_122(coolhtml.ch_140, coolhtml.ch_146)}
-{coolhtml.ch_122(coolhtml.ch_140, coolhtml.ch_146)}}
-coolhtml.ch_288 = () => {{coolhtml.ch_122(coolhtml.ch_119, coolhtml.ch_128)}
-{coolhtml.ch_122(coolhtml.ch_140, coolhtml.ch_148)}}
-coolhtml.ch_289 = () => {{coolhtml.ch_122(coolhtml.ch_119, coolhtml.ch_130)}
-{coolhtml.ch_122(coolhtml.ch_140, coolhtml.ch_150)}}
-coolhtml.ch_290 = () => {{coolhtml.ch_122(coolhtml.ch_119, coolhtml.ch_132)}
-{coolhtml.ch_122(coolhtml.ch_140, coolhtml.ch_152)}}
-coolhtml.ch_291 = () => {{coolhtml.ch_122(coolhtml.ch_119, coolhtml.ch_134)}
-{coolhtml.ch_122(coolhtml.ch_140, coolhtml.ch_154)}}
-coolhtml.ch_292 = () => {{coolhtml.ch_122(coolhtml.ch_119, coolhtml.ch_136)}
-{coolhtml.ch_122(coolhtml.ch_140, coolhtml.ch_156)}}
-coolhtml.ch_293 = () => {{coolhtml.ch_12(coolhtml.ch_14)}}
-coolhtml.ch_294 = () => {{coolhtml.ch_12(coolhtml.ch_18)}}
-coolhtml.ch_295 = () => {{coolhtml.ch_12(coolhtml.ch_22)}}
-coolhtml.ch_296 = () => {{coolhtml.ch_12(coolhtml.ch_26)}}
-coolhtml.ch_297 = () => {{coolhtml.ch_12(coolhtml.ch_30)}}
-coolhtml.ch_298 = () => {{coolhtml.ch_12(coolhtml.ch_34)}}
-coolhtml.ch_299 = () => {{coolhtml.ch_12(coolhtml.ch_38)}}
-coolhtml.ch_300 = () => {{coolhtml.ch_12(coolhtml.ch_106)}}
-coolhtml.ch_301 = () => {{coolhtml.ch_12(coolhtml.ch_42)}}
-coolhtml.ch_302 = () => {{coolhtml.ch_12(coolhtml.ch_46)}}
-coolhtml.ch_303 = () => {{coolhtml.ch_12(coolhtml.ch_50)}}
-coolhtml.ch_304 = () => {{coolhtml.ch_12(coolhtml.ch_54)}}
-coolhtml.ch_305 = () => {{coolhtml.ch_12(coolhtml.ch_58)}}
-coolhtml.ch_306 = () => {{coolhtml.ch_12(coolhtml.ch_62)}}
-coolhtml.ch_307 = () => {{coolhtml.ch_12(coolhtml.ch_66)}}
-coolhtml.ch_308 = () => {{coolhtml.ch_12(coolhtml.ch_70)}}
-coolhtml.ch_309 = () => {{coolhtml.ch_12(coolhtml.ch_74)}}
-coolhtml.ch_310 = () => {{coolhtml.ch_12(coolhtml.ch_78)}}
-coolhtml.ch_311 = () => {{coolhtml.ch_12(coolhtml.ch_82)}}
-coolhtml.ch_312 = () => {{coolhtml.ch_12(coolhtml.ch_86)}}
-coolhtml.ch_313 = () => {{coolhtml.ch_12(coolhtml.ch_90)}}
-coolhtml.ch_314 = () => {{coolhtml.ch_12(coolhtml.ch_94)}}
-coolhtml.ch_315 = () => {{coolhtml.ch_12(coolhtml.ch_98)}}
-coolhtml.ch_316 = () => {{coolhtml.ch_12(coolhtml.ch_110)}}
-coolhtml.ch_317 = () => {{coolhtml.ch_12(coolhtml.ch_102)}}
-coolhtml.ch_318 = () => {{coolhtml.ch_12(coolhtml.ch_114)}}
-coolhtml.ch_319 = () => {{coolhtml.ch_12(coolhtml.ch_118)}}
-coolhtml.ch_320 = () => {{coolhtml.ch_12(coolhtml.ch_11)}}
-coolhtml.ch_321 = () => {{coolhtml.ch_12(coolhtml.ch_16)}}
-coolhtml.ch_322 = () => {{coolhtml.ch_12(coolhtml.ch_20)}}
-coolhtml.ch_323 = () => {{coolhtml.ch_12(coolhtml.ch_24)}}
-coolhtml.ch_324 = () => {{coolhtml.ch_12(coolhtml.ch_28)}}
-coolhtml.ch_325 = () => {{coolhtml.ch_12(coolhtml.ch_32)}}
-coolhtml.ch_326 = () => {{coolhtml.ch_12(coolhtml.ch_36)}}
-coolhtml.ch_327 = () => {{coolhtml.ch_12(coolhtml.ch_40)}}
-coolhtml.ch_328 = () => {{coolhtml.ch_12(coolhtml.ch_44)}}
-coolhtml.ch_329 = () => {{coolhtml.ch_12(coolhtml.ch_48)}}
-coolhtml.ch_330 = () => {{coolhtml.ch_12(coolhtml.ch_52)}}
-coolhtml.ch_331 = () => {{coolhtml.ch_12(coolhtml.ch_56)}}
-coolhtml.ch_332 = () => {{coolhtml.ch_12(coolhtml.ch_60)}}
-coolhtml.ch_333 = () => {{coolhtml.ch_12(coolhtml.ch_64)}}
-coolhtml.ch_334 = () => {{coolhtml.ch_12(coolhtml.ch_68)}}
-coolhtml.ch_335 = () => {{coolhtml.ch_12(coolhtml.ch_72)}}
-coolhtml.ch_336 = () => {{coolhtml.ch_12(coolhtml.ch_76)}}
-coolhtml.ch_337 = () => {{coolhtml.ch_12(coolhtml.ch_80)}}
-coolhtml.ch_338 = () => {{coolhtml.ch_12(coolhtml.ch_84)}}
-coolhtml.ch_339 = () => {{coolhtml.ch_12(coolhtml.ch_88)}}
-coolhtml.ch_340 = () => {{coolhtml.ch_12(coolhtml.ch_92)}}
-coolhtml.ch_341 = () => {{coolhtml.ch_12(coolhtml.ch_96)}}
-coolhtml.ch_342 = () => {{coolhtml.ch_12(coolhtml.ch_100)}}
-coolhtml.ch_343 = () => {{coolhtml.ch_12(coolhtml.ch_104)}}
-coolhtml.ch_344 = () => {{coolhtml.ch_12(coolhtml.ch_108)}}
-coolhtml.ch_345 = () => {{coolhtml.ch_12(coolhtml.ch_112)}}
-coolhtml.ch_346 = () => {{coolhtml.ch_12(coolhtml.ch_116)}}</script></body></html>
+ch.ch_10.addEventListener('load', () => {ch.ch_8(ch.ch_10)})
+ch.ch_110.addEventListener('load', () => {ch.ch_8(ch.ch_110)})
+ch.ch_14.addEventListener('load', () => {ch.ch_8(ch.ch_14)})
+ch.ch_18.addEventListener('load', () => {ch.ch_8(ch.ch_18)})
+ch.ch_22.addEventListener('load', () => {ch.ch_8(ch.ch_22)})
+ch.ch_26.addEventListener('load', () => {ch.ch_8(ch.ch_26)})
+ch.ch_30.addEventListener('load', () => {ch.ch_8(ch.ch_30)})
+ch.ch_34.addEventListener('load', () => {ch.ch_8(ch.ch_34)})
+ch.ch_38.addEventListener('load', () => {ch.ch_8(ch.ch_38)})
+ch.ch_42.addEventListener('load', () => {ch.ch_8(ch.ch_42)})
+ch.ch_114.addEventListener('load', () => {ch.ch_8(ch.ch_114)})
+ch.ch_46.addEventListener('load', () => {ch.ch_8(ch.ch_46)})
+ch.ch_50.addEventListener('load', () => {ch.ch_8(ch.ch_50)})
+ch.ch_54.addEventListener('load', () => {ch.ch_8(ch.ch_54)})
+ch.ch_58.addEventListener('load', () => {ch.ch_8(ch.ch_58)})
+ch.ch_62.addEventListener('load', () => {ch.ch_8(ch.ch_62)})
+ch.ch_66.addEventListener('load', () => {ch.ch_8(ch.ch_66)})
+ch.ch_70.addEventListener('load', () => {ch.ch_8(ch.ch_70)})
+ch.ch_74.addEventListener('load', () => {ch.ch_8(ch.ch_74)})
+ch.ch_78.addEventListener('load', () => {ch.ch_8(ch.ch_78)})
+ch.ch_82.addEventListener('load', () => {ch.ch_8(ch.ch_82)})
+ch.ch_86.addEventListener('load', () => {ch.ch_8(ch.ch_86)})
+ch.ch_90.addEventListener('load', () => {ch.ch_8(ch.ch_90)})
+ch.ch_94.addEventListener('load', () => {ch.ch_8(ch.ch_94)})
+ch.ch_98.addEventListener('load', () => {ch.ch_8(ch.ch_98)})
+ch.ch_102.addEventListener('load', () => {ch.ch_8(ch.ch_102)})
+ch.ch_118.addEventListener('load', () => {ch.ch_8(ch.ch_118)})
+ch.ch_106.addEventListener('load', () => {ch.ch_8(ch.ch_106)})
+ch.ch_122.addEventListener('load', () => {ch.ch_8(ch.ch_122)})
+ch.ch_126.addEventListener('load', () => {ch.ch_8(ch.ch_126)})
+ch.ch_7.addEventListener('load', () => {ch.ch_8(ch.ch_7)})
+ch.ch_12.addEventListener('load', () => {ch.ch_8(ch.ch_12)})
+ch.ch_16.addEventListener('load', () => {ch.ch_8(ch.ch_16)})
+ch.ch_20.addEventListener('load', () => {ch.ch_8(ch.ch_20)})
+ch.ch_24.addEventListener('load', () => {ch.ch_8(ch.ch_24)})
+ch.ch_28.addEventListener('load', () => {ch.ch_8(ch.ch_28)})
+ch.ch_32.addEventListener('load', () => {ch.ch_8(ch.ch_32)})
+ch.ch_36.addEventListener('load', () => {ch.ch_8(ch.ch_36)})
+ch.ch_40.addEventListener('load', () => {ch.ch_8(ch.ch_40)})
+ch.ch_44.addEventListener('load', () => {ch.ch_8(ch.ch_44)})
+ch.ch_48.addEventListener('load', () => {ch.ch_8(ch.ch_48)})
+ch.ch_52.addEventListener('load', () => {ch.ch_8(ch.ch_52)})
+ch.ch_56.addEventListener('load', () => {ch.ch_8(ch.ch_56)})
+ch.ch_60.addEventListener('load', () => {ch.ch_8(ch.ch_60)})
+ch.ch_64.addEventListener('load', () => {ch.ch_8(ch.ch_64)})
+ch.ch_68.addEventListener('load', () => {ch.ch_8(ch.ch_68)})
+ch.ch_72.addEventListener('load', () => {ch.ch_8(ch.ch_72)})
+ch.ch_76.addEventListener('load', () => {ch.ch_8(ch.ch_76)})
+ch.ch_80.addEventListener('load', () => {ch.ch_8(ch.ch_80)})
+ch.ch_84.addEventListener('load', () => {ch.ch_8(ch.ch_84)})
+ch.ch_88.addEventListener('load', () => {ch.ch_8(ch.ch_88)})
+ch.ch_92.addEventListener('load', () => {ch.ch_8(ch.ch_92)})
+ch.ch_96.addEventListener('load', () => {ch.ch_8(ch.ch_96)})
+ch.ch_100.addEventListener('load', () => {ch.ch_8(ch.ch_100)})
+ch.ch_104.addEventListener('load', () => {ch.ch_8(ch.ch_104)})
+ch.ch_108.addEventListener('load', () => {ch.ch_8(ch.ch_108)})
+ch.ch_112.addEventListener('load', () => {ch.ch_8(ch.ch_112)})
+ch.ch_116.addEventListener('load', () => {ch.ch_8(ch.ch_116)})
+ch.ch_120.addEventListener('load', () => {ch.ch_8(ch.ch_120)})
+ch.ch_124.addEventListener('load', () => {ch.ch_8(ch.ch_124)})
+
+</script>
+</body>
+</html>
```

#### html2text {}

```diff
@@ -1,289 +1,295 @@
-å¨æ
-è§é¢
-æç« 
-æ³æ³
-è½¯ä»¶
-Pythonæç¨
-çæ´»
-èªè¿°
+动态视频文章想法软件Python教程生活自述
+2024-04-03
+===============================================================================
+2024-03-31
+_W_e_C_h_a_t_ _A_r_t_ _M_u_s_e_u_m
+_（_微_信_艺_术_馆_）
+_2_0_2_4_-_0_3_-_3_1
+2024-03-18
+===============================================================================
+===============================================================================
 2024-03-06
 _o_o_d_b
-_ï_¼__é__¢_å___å_¯_¹_è_±_¡_æ__°_æ__®_å_º__ï_¼_
+_（_面_向_对_象_数_据_库_）
 _2_0_2_4_-_0_3_-_0_6
-_é__¢_å___å_¯_¹_è_±_¡_æ__°_æ__®_å_º_
+_面_向_对_象_数_据_库
 _2_0_2_4_-_0_3_-_0_6
 2024-02-13
 _m_i_u_m_a_p_p
-_ï_¼__è_·_¨_å_¹_³_å__°_G_U_I_å_º__ç__¨_å_¼__å___å_·_¥_å__·_ï_¼_
+_（_跨_平_台_G_U_I_应_用_开_发_工_具_）
 _2_0_2_4_-_0_2_-_1_3
-_å_¼__å___è_·_¨_å_¹_³_å__°_G_U_I_å_º__ç__¨
+_开_发_跨_平_台_G_U_I_应_用
 _2_0_2_4_-_0_2_-_1_3
 2024-01-30
-_ç_§_¦_æ__¶_æ___æ___[_é_¡_¹_ç_¾_½_]_Â_·_è_°_ª_å_±_
+_秦_时_明_月_[_项_羽_]_·_谪_居
 _2_0_2_4_-_0_1_-_3_0
 2024-01-25
 ===============================================================================
 2024-01-13
 ===============================================================================
 2024-01-09
 ===============================================================================
 2024-01-03
-_ä_º_§_ä_¸__å___ç_º_§_ä_¸__å_¤_±_ä_¸__æ_½_®
+_产_业_升_级_与_失_业_潮
 _2_0_2_4_-_0_1_-_0_3
-_å__¨_C_h_a_t_G_P_T_å__²_å__»_ä_¸__ï_¼__æ___é__ _å__½_å_®_¶_ç_º_§_å__¬_å__±_ç__¥_è_¯__å_º__è_¿_«_å__¨_ç___ç__«
+_在_C_h_a_t_G_P_T_冲_击_下_，_打_造_国_家_级_公_共_知_识_库_迫_在_眉_睫
 _2_0_2_4_-_0_1_-_0_3
 ===============================================================================
 2024-01-01
 ===============================================================================
 2023-12-28
-_é__£_ä_º__å_¹_´_ï_¼__æ___ä_»_¬_ç_»__å___è_¿__ç___å___å__²
+_那_些_年_，_我_们_经_历_过_的_历_史
 _2_0_2_3_-_1_2_-_2_8
 2023-12-22
-_è_´_¢_å_¯__ç_¨_³_å_®__å___ç_¤_¾_ä_¼_
+_财_富_稳_定_型_社_会
 _2_0_2_3_-_1_2_-_2_2
 2023-12-11
 _C_o_o_l_M_e_m_o_r_y_-_E_n_g_l_i_s_h
-_ï_¼__å___è_¯__è_®_°_å_¿__è_½_¯_ä_»_¶_ï_¼_
+_（_单_词_记_忆_软_件_）
 _2_0_2_3_-_1_2_-_1_1
 2023-11-12
 ===============================================================================
 2023-11-02
 ===============================================================================
 2023-10-24
-_å_¹_´_è_½_»_ä_º_º_ä_¸__ç_»__å_©__æ__¯_æ___æ___ç___è_¿__æ_­_¥
+_年_轻_人_不_结_婚_是_文_明_的_进_步
 _2_0_2_3_-_1_0_-_2_4
 2023-10-09
-_æ__ª_ç_»__ä_»__ä_º_º_è__¦_ï_¼__è__«_å___ä_»__ä_º_º_å___ï_¼_
+_未_经_他_人_苦_，_莫_劝_他_人_善_？
 _2_0_2_3_-_1_0_-_0_9
 2023-10-06
 ===============================================================================
 2023-09-22
-_å___ä_¸__ä_»_·_å__¼
+_商_业_价_值
 _2_0_2_3_-_0_9_-_2_2
 2023-09-20
-_è_´_¢_å_¯__ç___æ__¬_è_´_¨
+_财_富_的_本_质
 _2_0_2_3_-_0_9_-_2_0
 2023-09-15
 ===============================================================================
 ===============================================================================
 2023-09-08
 ===============================================================================
 2023-08-18
 ===============================================================================
 2023-08-17
-_ä_º_º_ä_»_¬_ä_¸_º_ä_»__ä_¹__å_¸__æ___æ__¥_æ___å___ä_»_£
+_人_们_为_什_么_希_望_拥_有_后_代
 _2_0_2_3_-_0_8_-_1_7
 2023-08-06
 ===============================================================================
 2023-07-30
 ===============================================================================
 2023-07-20
 ===============================================================================
 2023-07-19
 ===============================================================================
 2023-07-11
 ===============================================================================
 2023-07-10
 ===============================================================================
 2023-07-09
-_ä_¸__å___å_®__å__¸_æ___æ___ä_¹__å___ï_¼_
+_一_元_官_司_有_意_义_吗_？
 _2_0_2_3_-_0_7_-_0_9
-_ç__µ_å_¢__é__½_æ__¯_å___ç___ï_¼__ç__µ_å___é__½_æ__¯_å_¥_½_ç___å___ï_¼_
+_熵_增_都_是_坏_的_，_熵_减_都_是_好_的_吗_？
 _2_0_2_3_-_0_7_-_0_9
 2023-07-06
 ===============================================================================
 2023-07-04
-_å_¿__ç___å_­_¦_ä_¸_­_ä_¸_ª_æ_¡__ç_ __ç_©_¶_æ___æ___ä_¹__å___ï_¼_
+_心_理_学_中_个_案_研_究_有_意_义_吗_？
 _2_0_2_3_-_0_7_-_0_4
 2023-07-01
 ===============================================================================
 2023-06-25
-_æ__¶_é__´_æ_¨_¡_å__
+_时_间_模_块
 _2_0_2_3_-_0_6_-_2_5
 2023-06-19
-_æ_­_£_å___è_¡_¨_è_¾_¾_å_¼_
+_正_则_表_达_式
 _2_0_2_3_-_0_6_-_1_9
 2023-06-18
-_è_¯__ä_»_·_å__¨_å___ä_º_¬_å_·_¥_ä_½__å__²_è_¿__å__º_ç___æ_¢__è_¥_¿_ç_²__ä_¸_
+_评_价_在_北_京_工_体_冲_进_场_的_梅_西_粉_丝
 _2_0_2_3_-_0_6_-_1_8
 2023-06-09
 ===============================================================================
 2023-06-07
 ===============================================================================
 2023-05-26
-_ä_¸__ç__©_ä_¸_º_ä_»__ä_¹__ä_¼__é__µ_å_¾_ª_ç___ç__©_ç___å_®__å_¾__ï_¼_
+_万_物_为_什_么_会_遵_循_着_物_理_定_律_？
 _2_0_2_3_-_0_5_-_2_6
 2023-05-13
 ===============================================================================
 2023-03-07
 _o_p_e_n_a_i_2
-_ï_¼__o_p_e_n_a_i_æ__¥_å__£_å_°__è_£__ï_¼_
+_（_o_p_e_n_a_i_接_口_封_装_）
 _2_0_2_3_-_0_3_-_0_7
-_å_¯_¹_æ__¥_C_h_a_t_G_P_T
+_对_接_C_h_a_t_G_P_T
 _2_0_2_3_-_0_3_-_0_7
 2023-03-06
-_C_h_a_t_G_P_T_å_·_²_ç_»__æ___è__ª_æ___æ___è_¯__ä_º_
+_C_h_a_t_G_P_T_已_经_有_自_我_意_识_了
 _2_0_2_3_-_0_3_-_0_6
 2022-12-31
-_å__¡_å_®__ä_¸__å__¡_è__
+_务_实_与_务_虚
 _2_0_2_2_-_1_2_-_3_1
-_ä_º_º_ä_º_º_å_¹_³_ç_­__æ__¯_ä_¸_ª_ä_¼_ª_æ_¦__å_¿_µ
+_人_人_平_等_是_个_伪_概_念
 _2_0_2_2_-_1_2_-_3_1
 2022-12-25
-_ä_º_º_å_·_¥_æ__º_è__½_ä_¼__ä_¸__ä_¼__ç_»__æ_²_»_ä_º_º_ç_±_»_ï_¼_
+_人_工_智_能_会_不_会_统_治_人_类_？
 _2_0_2_2_-_1_2_-_2_5
 2022-12-16
-_å_¹_¿_ä_¹__ç___æ_°__ä_¸_»
+_广_义_的_民_主
 _2_0_2_2_-_1_2_-_1_6
 2022-11-25
 ===============================================================================
 2022-09-27
-_æ___è_¿__æ__°_[_é___å___ç__²_]_Â_·_å__°_ä_º_­_å_º_
+_李_连_杰_[_霍_元_甲_]_·_兰_亭_序
 _2_0_2_2_-_0_9_-_2_7
 2022-09-21
-_å_ __è___è__ª_ç__±_æ__
+_堕_胎_自_由_权
 _2_0_2_2_-_0_9_-_2_1
 2022-09-08
-_æ_¥__é__¨_ç___ä_¸__ç___Â_·_ä_º__æ___é__¨
+_楚_门_的_世_界_·_五_月_雨
 _2_0_2_2_-_0_9_-_0_8
 2022-08-12
-_è_¢_«_ç_»__æ__¶
+_被_绑_架
 _2_0_2_2_-_0_8_-_1_2
 2022-08-01
-_æ___ä_¹__ç___è_§_£_ã___è_¿_·_ä_¿_¡_ç_§__å_­_¦_ã___ï_¼_
+_怎_么_理_解_「_迷_信_科_学_」_？
 _2_0_2_2_-_0_8_-_0_1
 2022-06-15
 ===============================================================================
 2021-07-28
-_A_I_æ__¯_è_¿__æ_ _·_ç__»_å___æ__¯_ç__
+_A_I_是_这_样_画_包_拯_的
 _2_0_2_1_-_0_7_-_2_8
 2021-06-11
-_â___è__ª_ç__±_æ___å_¿__â___å__¶_å_®__æ__¯_â___é___æ__º_æ___å_¿__â__
+_“_自_由_意_志_”_其_实_是_“_随_机_意_志_”
 _2_0_2_1_-_0_6_-_1_1
 2021-06-10
-_æ___æ__ _ç__¸_ç___ï_¼__é__¾_æ___ç__¸_æ___ç___å__¯_å__
+_有_无_相_生_，_难_易_相_成_的_启_发
 _2_0_2_1_-_0_6_-_1_0
 2021-06-09
-_å__ _å___ç___ç___å_­__å__¨_å___ï_¼_
+_占_卜_真_的_存_在_吗_？
 _2_0_2_1_-_0_6_-_0_9
 2021-06-07
-_æ___ä_»_¬_å__¯_è__½_å_¤__å__¨_ä_º_º_é__ _ä_¸__ç__
+_我_们_可_能_处_在_人_造_世_界
 _2_0_2_1_-_0_6_-_0_7
 2021-06-06
 _o_o_m_o_n_g_o
-_ï_¼__M_o_n_g_o_D_B_ _O_D_M_ï_¼_
+_（_M_o_n_g_o_D_B_ _O_D_M_）
 _2_0_2_1_-_0_6_-_0_6
-_æ___ä_½__M_o_n_g_o_D_B
+_操_作_M_o_n_g_o_D_B
 _2_0_2_1_-_0_6_-_0_6
 _o_o_m_y_s_q_l
-_ï_¼__M_y_S_Q_L_ _O_R_M_ï_¼_
+_（_M_y_S_Q_L_ _O_R_M_）
 _2_0_2_1_-_0_6_-_0_6
-_æ___ä_½__M_y_S_Q_L
+_操_作_M_y_S_Q_L
 _2_0_2_1_-_0_6_-_0_6
 2021-06-05
-_è_½_®_å___è_½_¬_ä_¸__ç___ç___å_­__å__¨_å___ï_¼_
+_轮_回_转_世_真_的_存_在_吗_？
 _2_0_2_1_-_0_6_-_0_5
 2021-06-03
-_å__¯_æ___å___å___æ__¯_ä_¸__å___ç___ï_¼_
+_唯_有_变_化_是_不_变_的_？
 _2_0_2_1_-_0_6_-_0_3
 2021-06-01
-_å_¿__ä_¿_®_æ__¯_ä_¹__è__¹_æ___è_®_º
+_忒_修_斯_之_船_悖_论
 _2_0_2_1_-_0_6_-_0_1
 2020-12-31
-_ç___å_±_±_å_®__è___ _ç_¬_¬_1_ç_«_ 
+_燕_山_宝_藏_ _第_1_章
 _2_0_2_0_-_1_2_-_3_1
 2019-08-05
-_ç__¨_3_7_è_¡__ä_»_£_ç_ __å_®__ç__°_A_I_ä_º__å_­__æ_£_
+_用_3_7_行_代_码_实_现_A_I_五_子_棋
 _2_0_1_9_-_0_8_-_0_5
 2019-05-01
 ===============================================================================
 2018-05-28
 ===============================================================================
 Copyright 2018-2024 lcctoor@outlook.com
 ******** vviiddeeooss ********
-_ç_§_¦_æ__¶_æ___æ___[_é_¡_¹_ç_¾_½_]_Â_·_è_°_ª_å_±_
+_秦_时_明_月_[_项_羽_]_·_谪_居
 _2_0_2_4_-_0_1_-_3_0
-_æ___è_¿__æ__°_[_é___å___ç__²_]_Â_·_å__°_ä_º_­_å_º_
+_李_连_杰_[_霍_元_甲_]_·_兰_亭_序
 _2_0_2_2_-_0_9_-_2_7
-_æ_¥__é__¨_ç___ä_¸__ç___Â_·_ä_º__æ___é__¨
+_楚_门_的_世_界_·_五_月_雨
 _2_0_2_2_-_0_9_-_0_8
-_A_I_æ__¯_è_¿__æ_ _·_ç__»_å___æ__¯_ç__
+_A_I_是_这_样_画_包_拯_的
 _2_0_2_1_-_0_7_-_2_8
 Copyright 2018-2024 lcctoor@outlook.com
-******** ?è?µ??é??±?å?®??å??¸ ********
-_è_´_¢_å_¯__ç___æ__¬_è_´_¨
+******** ?赚?钱?宝?典 ********
+_财_富_的_本_质
 _2_0_2_3_-_0_9_-_2_0
-_å___ä_¸__ä_»_·_å__¼
+_商_业_价_值
 _2_0_2_3_-_0_9_-_2_2
-_è_´_¢_å_¯__ç_¨_³_å_®__å___ç_¤_¾_ä_¼_
+_财_富_稳_定_型_社_会
 _2_0_2_3_-_1_2_-_2_2
-******** ?è?¿?½?è??±?è?µ?¶?ç?¾? ********
-_ä_º_§_ä_¸__å___ç_º_§_ä_¸__å_¤_±_ä_¸__æ_½_®
+******** ?追?英?赶?美 ********
+_产_业_升_级_与_失_业_潮
 _2_0_2_4_-_0_1_-_0_3
-_å__¨_C_h_a_t_G_P_T_å__²_å__»_ä_¸__ï_¼__æ___é__ _å__½_å_®_¶_ç_º_§_å__¬_å__±_ç__¥_è_¯__å_º__è_¿_«_å__¨_ç___ç__«
+_在_C_h_a_t_G_P_T_冲_击_下_，_打_造_国_家_级_公_共_知_识_库_迫_在_眉_睫
 _2_0_2_4_-_0_1_-_0_3
-******** ?å?°??æ?°??å???æ??¿ ********
-_å_¹_¿_ä_¹__ç___æ_°__ä_¸_»
+******** ?小?民?参?政 ********
+_广_义_的_民_主
 _2_0_2_2_-_1_2_-_1_6
-_å_¹_´_è_½_»_ä_º_º_ä_¸__ç_»__å_©__æ__¯_æ___æ___ç___è_¿__æ_­_¥
+_年_轻_人_不_结_婚_是_文_明_的_进_步
 _2_0_2_3_-_1_0_-_2_4
-******** ?æ??¹?å??¤?é??£?ä?º??ä?¼?ª?æ???è??º ********
-_ä_¸__å___å_®__å__¸_æ___æ___ä_¹__å___ï_¼_
+******** ?批?判?那?些?伪?文?艺 ********
+_一_元_官_司_有_意_义_吗_？
 _2_0_2_3_-_0_7_-_0_9
-_å__¯_æ___å___å___æ__¯_ä_¸__å___ç___ï_¼_
+_唯_有_变_化_是_不_变_的_？
 _2_0_2_1_-_0_6_-_0_3
-_æ__ª_ç_»__ä_»__ä_º_º_è__¦_ï_¼__è__«_å___ä_»__ä_º_º_å___ï_¼_
+_未_经_他_人_苦_，_莫_劝_他_人_善_？
 _2_0_2_3_-_1_0_-_0_9
-_å__¡_å_®__ä_¸__å__¡_è__
+_务_实_与_务_虚
 _2_0_2_2_-_1_2_-_3_1
-******** ?ä?¸??è?±?¡?æ???è?? ********
-_C_h_a_t_G_P_T_å_·_²_ç_»__æ___è__ª_æ___æ___è_¯__ä_º_
+******** ?万?象?思?考 ********
+_C_h_a_t_G_P_T_已_经_有_自_我_意_识_了
 _2_0_2_3_-_0_3_-_0_6
-_æ___ä_¹__ç___è_§_£_ã___è_¿_·_ä_¿_¡_ç_§__å_­_¦_ã___ï_¼_
+_怎_么_理_解_「_迷_信_科_学_」_？
 _2_0_2_2_-_0_8_-_0_1
-_å_¿__ç___å_­_¦_ä_¸_­_ä_¸_ª_æ_¡__ç_ __ç_©_¶_æ___æ___ä_¹__å___ï_¼_
+_心_理_学_中_个_案_研_究_有_意_义_吗_？
 _2_0_2_3_-_0_7_-_0_4
-_ä_º_º_å_·_¥_æ__º_è__½_ä_¼__ä_¸__ä_¼__ç_»__æ_²_»_ä_º_º_ç_±_»_ï_¼_
+_人_工_智_能_会_不_会_统_治_人_类_？
 _2_0_2_2_-_1_2_-_2_5
-_å_¿__ä_¿_®_æ__¯_ä_¹__è__¹_æ___è_®_º
+_忒_修_斯_之_船_悖_论
 _2_0_2_1_-_0_6_-_0_1
-_æ___æ__ _ç__¸_ç___ï_¼__é__¾_æ___ç__¸_æ___ç___å__¯_å__
+_有_无_相_生_，_难_易_相_成_的_启_发
 _2_0_2_1_-_0_6_-_1_0
-_ç__µ_å_¢__é__½_æ__¯_å___ç___ï_¼__ç__µ_å___é__½_æ__¯_å_¥_½_ç___å___ï_¼_
+_熵_增_都_是_坏_的_，_熵_减_都_是_好_的_吗_？
 _2_0_2_3_-_0_7_-_0_9
-_ä_º_º_ä_»_¬_ä_¸_º_ä_»__ä_¹__å_¸__æ___æ__¥_æ___å___ä_»_£
+_人_们_为_什_么_希_望_拥_有_后_代
 _2_0_2_3_-_0_8_-_1_7
-_ä_¸__ç__©_ä_¸_º_ä_»__ä_¹__ä_¼__é__µ_å_¾_ª_ç___ç__©_ç___å_®__å_¾__ï_¼_
+_万_物_为_什_么_会_遵_循_着_物_理_定_律_？
 _2_0_2_3_-_0_5_-_2_6
-_å_ __è___è__ª_ç__±_æ__
+_堕_胎_自_由_权
 _2_0_2_2_-_0_9_-_2_1
-_ä_º_º_ä_º_º_å_¹_³_ç_­__æ__¯_ä_¸_ª_ä_¼_ª_æ_¦__å_¿_µ
+_人_人_平_等_是_个_伪_概_念
 _2_0_2_2_-_1_2_-_3_1
-******** ?æ??¶?ç?©?º?ç???æ??³ ********
-_è_½_®_å___è_½_¬_ä_¸__ç___ç___å_­__å__¨_å___ï_¼_
+******** ?时?空?猜?想 ********
+_轮_回_转_世_真_的_存_在_吗_？
 _2_0_2_1_-_0_6_-_0_5
-_æ___ä_»_¬_å__¯_è__½_å_¤__å__¨_ä_º_º_é__ _ä_¸__ç__
+_我_们_可_能_处_在_人_造_世_界
 _2_0_2_1_-_0_6_-_0_7
-_å__ _å___ç___ç___å_­__å__¨_å___ï_¼_
+_占_卜_真_的_存_在_吗_？
 _2_0_2_1_-_0_6_-_0_9
-_â___è__ª_ç__±_æ___å_¿__â___å__¶_å_®__æ__¯_â___é___æ__º_æ___å_¿__â__
+_“_自_由_意_志_”_其_实_是_“_随_机_意_志_”
 _2_0_2_1_-_0_6_-_1_1
-******** ?è?®?º?æ??¶?ä?º? ********
-_é__£_ä_º__å_¹_´_ï_¼__æ___ä_»_¬_ç_»__å___è_¿__ç___å___å__²
+******** ?论?时?事 ********
+_那_些_年_，_我_们_经_历_过_的_历_史
 _2_0_2_3_-_1_2_-_2_8
-_è_¯__ä_»_·_å__¨_å___ä_º_¬_å_·_¥_ä_½__å__²_è_¿__å__º_ç___æ_¢__è_¥_¿_ç_²__ä_¸_
+_评_价_在_北_京_工_体_冲_进_场_的_梅_西_粉_丝
 _2_0_2_3_-_0_6_-_1_8
-******** ?å?°??è?¯?´ // ?é???å?°??å??¤?æ??°?ä?¼?  ********
-_ç___å_±_±_å_®__è___ _ç_¬_¬_1_ç_«_ 
+******** ?小?说 // ?陆?小?凤?新?传 ********
+_燕_山_宝_藏_ _第_1_章
 _2_0_2_0_-_1_2_-_3_1
-******** ?å?°??è?¯?´ // ?ä?¸??å?¿?µ?å?¤?©?å? ? ********
-_è_¢_«_ç_»__æ__¶
+******** ?小?说 // ?一?念?天?堂 ********
+_被_绑_架
 _2_0_2_2_-_0_8_-_1_2
 Copyright 2018-2024 lcctoor@outlook.com
+2024-04-03
+===============================================================================
+2024-03-18
+===============================================================================
 2024-01-25
 ===============================================================================
 2024-01-13
 ===============================================================================
 2024-01-09
 ===============================================================================
 2024-01-03
@@ -324,59 +330,64 @@
 2023-05-13
 ===============================================================================
 2022-06-15
 ===============================================================================
 Copyright 2018-2024 lcctoor@outlook.com
 ******** ssooffttwwaarree ********
 _C_o_o_l_M_e_m_o_r_y_-_E_n_g_l_i_s_h
-_ï_¼__å___è_¯__è_®_°_å_¿__è_½_¯_ä_»_¶_ï_¼_
+_（_单_词_记_忆_软_件_）
 _2_0_2_3_-_1_2_-_1_1
 _m_i_u_m_a_p_p
-_ï_¼__è_·_¨_å_¹_³_å__°_G_U_I_å_º__ç__¨_å_¼__å___å_·_¥_å__·_ï_¼_
+_（_跨_平_台_G_U_I_应_用_开_发_工_具_）
 _2_0_2_4_-_0_2_-_1_3
 _o_o_d_b
-_ï_¼__é__¢_å___å_¯_¹_è_±_¡_æ__°_æ__®_å_º__ï_¼_
+_（_面_向_对_象_数_据_库_）
 _2_0_2_4_-_0_3_-_0_6
 _o_o_m_o_n_g_o
-_ï_¼__M_o_n_g_o_D_B_ _O_D_M_ï_¼_
+_（_M_o_n_g_o_D_B_ _O_D_M_）
 _2_0_2_1_-_0_6_-_0_6
 _o_o_m_y_s_q_l
-_ï_¼__M_y_S_Q_L_ _O_R_M_ï_¼_
+_（_M_y_S_Q_L_ _O_R_M_）
 _2_0_2_1_-_0_6_-_0_6
 _o_p_e_n_a_i_2
-_ï_¼__o_p_e_n_a_i_æ__¥_å__£_å_°__è_£__ï_¼_
+_（_o_p_e_n_a_i_接_口_封_装_）
 _2_0_2_3_-_0_3_-_0_7
-Copyright 2018-2024 lcctoor@outlook.com
-2023-10-06
-===============================================================================
-2022-11-25
-===============================================================================
-2019-05-01
-===============================================================================
-2018-05-28
-===============================================================================
+_W_e_C_h_a_t_ _A_r_t_ _M_u_s_e_u_m
+_（_微_信_艺_术_馆_）
+_2_0_2_4_-_0_3_-_3_1
 Copyright 2018-2024 lcctoor@outlook.com
 ******** ttuuttoorriiaallss ********
-_æ___ä_½__M_y_S_Q_L
+_操_作_M_y_S_Q_L
 _2_0_2_1_-_0_6_-_0_6
-_æ___ä_½__M_o_n_g_o_D_B
+_操_作_M_o_n_g_o_D_B
 _2_0_2_1_-_0_6_-_0_6
-_å_¼__å___è_·_¨_å_¹_³_å__°_G_U_I_å_º__ç__¨
+_开_发_跨_平_台_G_U_I_应_用
 _2_0_2_4_-_0_2_-_1_3
-_å_¯_¹_æ__¥_C_h_a_t_G_P_T
+_对_接_C_h_a_t_G_P_T
 _2_0_2_3_-_0_3_-_0_7
-_æ__¶_é__´_æ_¨_¡_å__
+_时_间_模_块
 _2_0_2_3_-_0_6_-_2_5
-_é__¢_å___å_¯_¹_è_±_¡_æ__°_æ__®_å_º_
+_面_向_对_象_数_据_库
 _2_0_2_4_-_0_3_-_0_6
-_ç__¨_3_7_è_¡__ä_»_£_ç_ __å_®__ç__°_A_I_ä_º__å_­__æ_£_
+_用_3_7_行_代_码_实_现_A_I_五_子_棋
 _2_0_1_9_-_0_8_-_0_5
-_æ_­_£_å___è_¡_¨_è_¾_¾_å_¼_
+_正_则_表_达_式
 _2_0_2_3_-_0_6_-_1_9
 Copyright 2018-2024 lcctoor@outlook.com
-é®ç®±
+2024-03-18
+===============================================================================
+2023-10-06
+===============================================================================
+2022-11-25
+===============================================================================
+2019-05-01
+===============================================================================
+2018-05-28
+===============================================================================
+Copyright 2018-2024 lcctoor@outlook.com
+邮箱
 _l_c_c_t_o_o_r_@_o_u_t_l_o_o_k_._c_o_m
-å¾®ä¿¡
+微信
 [./ip_static/WeChatQRC.jpg]
-æèµ 
+捐赠
 [./ip_static/DonationQRC-0rmb.jpg]
 Copyright 2018-2024 lcctoor@outlook.com
```

### Comparing `arts-2024.3.6/arts/life/2018/莆田学院·毕业生留影/index.html` & `arts-2024.4.3/arts/life/2018/莆田学院·毕业生留影/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/life/2019/苏州市虎丘山/index.html` & `arts-2024.4.3/arts/life/2019/苏州市虎丘山/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 <body>
 <pre>
 苏州市虎丘山
 
 在苏州出差，趁五一和孙同事一起到虎丘山观览景盛。景区很大，景点很多，游客也很多。景区里面有美食摊点，在里面走累了可以购买食物补充能量。
 </pre>
     <script>
-        media = ['ip_static/01.jpg', 'ip_static/02.jpg', 'ip_static/03.jpg', 'ip_static/04.jpg', 'ip_static/05.jpg', 'ip_static/06.jpg', 'ip_static/07.jpg',
-                    'ip_static/08.jpg', 'ip_static/09.jpg', 'ip_static/10.jpg', 'ip_static/11.jpg', 'ip_static/12.jpg', 'ip_static/13.jpg', 'ip_static/14.jpg',
-                    'ip_static/15.jpg', 'ip_static/16.jpg'
+        media = [
+            'ip_static/01.jpg', 'ip_static/02.jpg', 'ip_static/03.jpg', 'ip_static/04.jpg', 'ip_static/05.jpg', 'ip_static/06.jpg', 'ip_static/07.jpg',
+            'ip_static/08.jpg', 'ip_static/09.jpg', 'ip_static/10.jpg', 'ip_static/11.jpg', 'ip_static/12.jpg', 'ip_static/13.jpg', 'ip_static/14.jpg',
+            'ip_static/15.jpg', 'ip_static/16.jpg'
         ]
     </script>
     <script src="https://lcctoor.github.io/arts/arts/ip_static/01/article_js.js"></script>
     <script src="C:/bpath/offline_files/lcctoor.github.io/arts/ip_static/01/article_js.js"></script>
 </body>
 </html>
```

### Comparing `arts-2024.3.6/arts/life/2022/泉州市丰泽区·雨后街道/index.html` & `arts-2024.4.3/arts/life/2022/泉州市丰泽区·雨后街道/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 <body>
 <pre>
 泉州丰泽区·雨后街道
 
 下班，看到雨把大地冲洗得格外清新，便没有骑车，沿途欣赏风景和拍照。
 </pre>
     <script>
-        media = ['ip_static/01.jpg', 'ip_static/02.jpg', 'ip_static/03.jpg', 'ip_static/04.jpg', 'ip_static/05.jpg', 'ip_static/06.jpg', 'ip_static/07.jpg',
-                    'ip_static/08.jpg'
+        media = [
+            'ip_static/01.jpg', 'ip_static/02.jpg', 'ip_static/03.jpg', 'ip_static/04.jpg', 'ip_static/05.jpg', 'ip_static/06.jpg', 'ip_static/07.jpg',
+            'ip_static/08.jpg'
         ]
     </script>
     <script src="https://lcctoor.github.io/arts/arts/ip_static/01/article_js.js"></script>
     <script src="C:/bpath/offline_files/lcctoor.github.io/arts/ip_static/01/article_js.js"></script>
 </body>
 </html>
```

### Comparing `arts-2024.3.6/arts/life/2023/更换微信账号了/index.html` & `arts-2024.4.3/arts/life/2023/更换微信账号了/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     <meta charset='utf-8'>
     <meta content='width=device-width, initial-scale=1.0' name='viewport'>
     <link rel="stylesheet" href="https://lcctoor.github.io/arts/arts/ip_static/01/article_css.css">
     <link rel="stylesheet" href="C:/bpath/offline_files/lcctoor.github.io/arts/ip_static/01/article_css.css">
 </head>
 <body>
 <pre>
-由于一些原因，我的原微信账号已无法登录，也无法查看好友，请朋友们看到后添加我的新账号。
+由于一些原因，我的原微信账号已无法登录，也无法查看好友，请朋友们看到后添加我的新账号。有些朋友，我无法告知他们这件事情，有点遗憾。
 </pre>
     <script>
         media = ['https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg']
     </script>
     <script src="https://lcctoor.github.io/arts/arts/ip_static/01/article_js.js"></script>
     <script src="C:/bpath/offline_files/lcctoor.github.io/arts/ip_static/01/article_js.js"></script>
 </body>
```

#### html2text {}

```diff
@@ -1 +1 @@
-由于一些原因，我的原微信账号已无法登录，也无法查看好友，请朋友们看到后添加我的新账号。
+由于一些原因，我的原微信账号已无法登录，也无法查看好友，请朋友们看到后添加我的新账号。有些朋友，我无法告知他们这件事情，有点遗憾。
```

### Comparing `arts-2024.3.6/arts/miumapp/LICENSE` & `arts-2024.4.3/arts/miumapp/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/miumapp/README.md` & `arts-2024.4.3/arts/miumapp/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
 我们所采用的技术栈组合是经过深思熟虑的，通过结合 **Python** 与  **HTML** 这两种高效、灵活、易用的技术栈，意味着您正在选择一个能够大大减少开发时间、简化开发流程、拥有丰富的第三方扩展的解决方案。与其它工具相比，我们的优势在于对新技术的快速适应、更为强大的社区支持，以及持续的更新和改进。
 
 # 作者
 
 [江南雨上](mailto:lcctoor@outlook.com)
 
-[主页](https://lcctoor.github.io/arts/) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
+[主页](https://lcctoor.github.io/arts) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
+你可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
 
 # 安装
 
 ```
 pip install miumapp
 ```
```

### Comparing `arts-2024.3.6/arts/miumapp/_core.py` & `arts-2024.4.3/arts/miumapp/_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio, socket, os, __main__
 from time import time as timestamp
 from weakref import WeakKeyDictionary
 from os.path import abspath
 from pathlib import Path
 from json import loads as json_loads
-from json import dumps as json_dumps
 from typing import Dict, Any
 from tornado.web import RequestHandler, Application
 from pyppeteer.launcher import Launcher, DEFAULT_ARGS
 from pyppeteer.page import Page
+from arts.cooltypes import json_chinese, get_chrome_path
 
 
 # 使不会提示'缺少 Google API 密钥, 因此 Chromium 的部分功能将不可使用。'
 os.environ["GOOGLE_API_KEY"] = "no"
 os.environ["GOOGLE_DEFAULT_CLIENT_ID"] = "no"
 os.environ["GOOGLE_DEFAULT_CLIENT_SECRET"] = "no"
 
@@ -38,26 +38,14 @@
     '--disable-hang-monitor',
     '--disable-default-apps',
     '--no-first-run',
     '--disable-popup-blocking',
     '--disable-session-crashed-bubble',
 ]
 
-def get_chrome_path():
-    for chrome in [
-        rf'C:\Program Files\Google\Chrome\Application\chrome.exe',  # Chrome [已校验]
-        rf'C:\Users\{os.getlogin()}\AppData\Local\360ChromeX\Chrome\Application\360ChromeX.exe',  # 360极速浏览器X [已校验]
-        rf'C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe',  # Edge [已校验] 32位的, 置底
-        rf'/Applications/Google Chrome.app/Contents/MacOS/Google Chrome',  # Mac Chrome
-        rf'/usr/bin/chromium-browser',  # Linux chromium
-        rf'/usr/bin/google-chrome',  # Linux Chrome
-    ]:
-        if Path(chrome).is_file():
-            return chrome
-    return None
 
 # 为 Page.goto 添加 title 参数
 native_goto = Page.goto
 async def goto(self:Page, url:str, title='', options=None, **kwargs):
     r = await native_goto(self, url, options, **kwargs)
     if title:
         await self.evaluate(f"document.title = '{title}'")
@@ -156,40 +144,36 @@
     async def start(self):
 
         class home_text(RequestHandler):
             async def get(TorSelf):
                 TorSelf.set_header("Access-Control-Allow-Origin", "*")
                 return TorSelf.write( self._home_text )
         
-        class callpy(RequestHandler):            
+        class callpy(RequestHandler):
             async def post(TorSelf):
+                code, msg, data = 'success', '', None
                 try:
-                    try:
-                        TorSelf.set_header("Access-Control-Allow-Origin", "*")
-                        body: dict = json_loads(TorSelf.request.body)
-                        method_name = body['method_name']
-                        kwargs = body['kwargs'] or {}
-                        if method_name[:1] == '_':
-                            code, msg, data = 2, "For the server's security, calling methods starting with '_' is prohibited.", None
+                    TorSelf.set_header("Access-Control-Allow-Origin", "*")
+                    body: dict = json_loads(TorSelf.request.body)
+                    method_name = body['method_name']
+                    kwargs = body['kwargs'] or {}
+                    if method_name[:1] == '_':
+                        code, msg, data = 'security_error', "为了服务器的安全, 不支持调用以 '_' 开头的方法.", None
+                    else:
+                        func = getattr(self, method_name)
+                        __func__ = func.__func__ if hasattr(func, '__func__') else func
+                        if __func__ in _allow_callpy_funcs:
+                            code, msg, data = 'success', '', await func(**kwargs)
                         else:
-                            func = getattr(self, method_name)
-                            __func__ = func.__func__ if hasattr(func, '__func__') else func
-                            if __func__ in _allow_callpy_funcs:
-                                code, msg, data = 0, '', await func(**kwargs)
-                            else:
-                                code, msg, data = 3, 'This method does not allow calling.', None
-                        try:
-                            r = json_dumps({'code':code, 'msg':msg, 'data':data}, ensure_ascii=False)
-                        except:
-                            r = json_dumps({'code':code, 'msg':msg, 'data':str(data)}, ensure_ascii=False)
-                        return TorSelf.write(r)
-                    except Exception as e:
-                        return TorSelf.write( json_dumps({'code':1, 'msg':str(e), 'data':None}, ensure_ascii=False) )
+                            code, msg, data = 'allow_callpy_error', '方法未注册, 不支持调用.', None
+                    return TorSelf.write( json_chinese(dict(code=code, msg=msg, data=data)) )
                 except Exception as e:
-                    print(e)
+                    code, msg = type(e).__name__, str(e)
+                    if data is not None: data = str(data)
+                    return TorSelf.write( json_chinese(dict(code=code, msg=msg, data=data)) )
         
         # 查找一个空闲端口
         sock = socket.socket()
         sock.bind(('localhost', 0))
         self._server_port = sock.getsockname()[1]
         sock.close()
         Application(handlers=[('/callpy/?', callpy), ('/?', home_text)], debug=False).listen(port=self._server_port, address="localhost")
```

### Comparing `arts-2024.3.6/arts/miumapp/licenses/pyppeteer/LICENSE` & `arts-2024.4.3/arts/miumapp/licenses/pyppeteer/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/miumapp/licenses/tornado/LICENSE` & `arts-2024.4.3/arts/miumapp/licenses/tornado/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/miumapp/miumapp/demo.html` & `arts-2024.4.3/arts/miumapp/miumapp/demo.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/miumapp/miumapp/demo.py` & `arts-2024.4.3/arts/miumapp/miumapp/demo.py`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/miumapp/pyproject.toml` & `arts-2024.4.3/arts/miumapp/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "miumapp"
-version = "1.0.8"
+version = "1.0.9"
 description = "一个使用 Python + HTML 开发桌面 GUI 应用的框架，支持 Windows、Mac、Linux 平台。"
-dependencies = ["arts>=2024.3.6"]
+dependencies = ["arts>=2024.3.6.3"]
 keywords = ["electron", "flutter", "uniapp", "pyqt5", "miumapp"]
 
 
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `arts-2024.3.6/arts/oodb/LICENSE` & `arts-2024.4.3/arts/oodb/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/oodb/README.md` & `arts-2024.4.3/arts/oodb/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 如果你不需要使用继承、重写等特性，而只是需要一个用来操作 MongoDB 的 ODM，我们为你准备了另一款更合适的工具 —— [oomongo](https://lcctoor.github.io/arts/arts/oomongo) 。
 
 # 作者
 
 [江南雨上](mailto:lcctoor@outlook.com)
 
-[主页](https://lcctoor.github.io/arts/) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
+[主页](https://lcctoor.github.io/arts) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
+你可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
 
 # 安装
 
 ```
 pip install oodb
 ```
 
@@ -29,15 +29,15 @@
 ## 导入
 
 ```python
 from pymongo import MongoClient
 from oodb import OOM, Row, mc, mf, mo, mpy
 ```
 
-## 创建 OOM
+## 创建OOM
 
 ```python
 class OOM_2(OOM):
     def mkconn(self):
         return MongoClient(host='localhost', port=27017)  # MongoDB 连接器，用来写入和读取数据
 
 oom = OOM_2()          # 账户OOM
@@ -180,102 +180,103 @@
 id_128G_白_联通合作 = sheet.insert({'版本名称': '128G-白色-联通合作'}, bases=[id_128G_白]).inserted_id
 ```
 
 在此例中，我们在新增 `row_128G_白_联通合作` 对象时，继承了 `row_128G_白` 对象，并重写了 `版本名称` 属性。
 
 ## 方法
 
-让我们定义一个方法：该方法接收一个 `name` 参数，然后返回一个字符串 —— `<当前时间> 你好，<name>！我是【<版本名称>】版本的 iPhone15，很高兴成为你的移动助理！` 。
+让我们定义一个方法：该方法接收一个 `name` 参数，然后返回一个字符串 —— `[<当前时间>] 你好，<name>！我是【<版本名称>】版本的 iPhone15，很高兴成为你的移动助理！` 。
 
 ```python
 # 创建对象方法
 @mpy.method
 def say_hello(self: 'Row', name: 'str'):
     import time
     版本名称 = self['版本名称']
     return f"[{int(time.time())}] 你好，{name}！我是【{版本名称}】版本的 iPhone15，很高兴成为你的移动助理！"
 
 # 将对象方法赋值给基对象base, 它的子孙对象都将继承此方法
-next( sheet[mc._id == id_base].find() ).update({'say_hello': say_hello})
+base_obj = next( sheet[mc._id == id_base].find() )
+base_obj.update({'say_hello': say_hello})
 
 # 调用对象方法
-for _id in (id_128G_黑, id_128G_白, id_128G_白_联通合作):
-    say_hello = next( sheet[mc._id == _id].find() )['say_hello']
+for _id in [id_128G_黑, id_128G_白, id_128G_白_联通合作]:
+    obj = next( sheet[mc._id == _id].find() )
+    say_hello = obj['say_hello']
     print(say_hello('程序猿'))
 
 # >>> [1709654174] 你好，程序猿！我是【128G-黑色】版本的 iPhone15，很高兴成为你的移动助理！
 # >>> [1709654174] 你好，程序猿！我是【128G-白色】版本的 iPhone15，很高兴成为你的移动助理！
 # >>> [1709654174] 你好，程序猿！我是【128G-白色-联通合作】版本的 iPhone15，很高兴成为你的移动助理！
 ```
 
 ### 讲解
 
 1、使用 `@mpy.method` 装饰一个普通函数，该函数就会变成对象方法。
 
-2、注意到这行代码 `def say_hello(self: 'Row', name: 'str'):` 中， `'Row'` 和 `'str'` 被加了引号，当我们为对象方法的参数做类型提示时，必须以字符串的格式。以下这种方式是错误的： `def say_hello(self: Row, name: str):` 。当然，类型提示只是用来让编辑器提示代码的，它可有可无，不是必要的。
+2、注意到这行代码 `def say_hello(self: 'Row', name: 'str'):` 中， `'Row'` 和 `'str'` 被加了引号 —— 当我们为对象方法的参数做类型提示时，必须以字符串的格式。以下这种方式是错误的： `def say_hello(self: Row, name: str):` 。当然，类型提示只是用来让编辑器提示代码的，它可有可无，不是必要的。
 
-3、可以在对象方法内导入并使用任何 Python 包，包括标准库、第三方包、当前环境变量内的包。
+3、可以在对象方法内导入并使用任何【标准库】和【第三方包】。
 
 4、调用对象方法时，既可以使用位置传参，也可以使用关键词传参。例如，这两种方式都是可行的： `say_hello('程序猿')` 、 `say_hello(name='程序猿')` 。
 
-5、对象方法是以人类易读的文本格式（[查看图示](https://lcctoor.github.io/arts/arts/oodb/ip_static/对象方法.png)）存储在 MongoDB 中的，可直接通过 Navicat 等管理工具灵活修改。
+5、对象方法是以人类易读的文本格式存储在 MongoDB 中的（[查看图示](https://lcctoor.github.io/arts/arts/oodb/ip_static/对象方法.png)），可直接通过 Navicat 等管理工具灵活修改。
 
 ## 动态属性
 
-让我们用一个统计学生总数的案例来讲解【动态属性】：
+让我们用一个统计学生总数的案例来讲解【动态属性】。
 
 ```python
 # 新增四个班级对象
 C1 = sheet.insert({'班级编号': 1, '学生数量': 10}).inserted_id
 C2 = sheet.insert({'班级编号': 2, '学生数量': 20}).inserted_id
 C3 = sheet.insert({'班级编号': 3, '学生数量': 30}).inserted_id
 C4 = sheet.insert({'班级编号': 4, '学生数量': 40}).inserted_id
 
 # 创建一个获取学生总数量的动态属性值
 @mpy.dynamic(C1, C2, id3=C3, id4=C4)
 def get_students_count(self: 'Row', id1, id2, id3, id4):
-    from oodb import Row
-    parent = self.parent
-    rows = [Row(parent=parent, _id=x) for x in (id1, id2, id3, id4)]
+    from oodb import Row  # Row 在实例化时需要接收两个参数: (parent: Sheet, _id)
+    rows = [Row(parent=self.parent, _id=x) for x in (id1, id2, id3, id4)]
     return sum( [x['学生数量'] for x in rows] )
 
-# 新增一个年级对象，并将 动态属性值 赋值给 '学生总数量'属性
+# 新增一个年级对象，并将【动态属性值】赋值给【学生总数量】属性
 gid = sheet.insert({'年级': '五年级', '学生总数量': get_students_count}).inserted_id
 
 # 查询动态属性值
 grade = next( sheet[mc._id == gid].find() )
 print(grade['学生总数量'])  # >>> 100
 ```
 
-如果我们修改某个班级的学生数量，年级的'学生总数量'的返回值也会相应变化：
+如果我们修改某个班级的学生数量，年级的【学生总数量】的返回值也会相应变化：
 
 ```python
 next( sheet[mc._id == C1].find() ).update({'学生数量': 15})
 print(grade['学生总数量'])  # >>> 105
 ```
 
 ### 讲解
 
 1、使用 `@mpy.dynamic(...)` 装饰一个普通函数，该函数就会变成动态属性。
 
-2、注意到这行代码 `def get_students_count(self: 'Row', id1, id2, id3, id4):` 中， `'Row'` 被加了引号，当我们为动态属性的参数做类型提示时，必须以字符串的格式。以下这种方式是错误的： `def get_students_count(self: Row, id1, id2, id3, id4):` 。当然，类型提示只是用来让编辑器提示代码的，它可有可无，不是必要的。
+2、注意到这行代码 `def get_students_count(self: 'Row', id1, id2, id3, id4):` 中， `'Row'` 被加了引号 —— 当我们为动态属性的参数做类型提示时，必须以字符串的格式。以下这种方式是错误的： `def get_students_count(self: Row, id1, id2, id3, id4):` 。当然，类型提示只是用来让编辑器提示代码的，它可有可无，不是必要的。
 
-3、可以在动态属性内导入并使用任何 Python 包，包括标准库、第三方包、当前环境变量内的包。
+3、可以在动态属性内导入并使用任何【标准库】和【第三方包】。
 
 4、创建动态属性时，必须将所需要的参数值在 `@mpy.dynamic(...)` 的括号内传入。比如：我们定义的 `get_students_count` 需要 `id1, id2, id3, id4` 这四个参数，相对应地，我们在 `@mpy.dynamic(...)` 中传递了 `C1, C2, id3=C3, id4=C4` 这四个参数值。传递参数值时，既可以使用位置传参，也可以使用关键词传参，例如： `C1, C2` 使用了位置传参，而 `id3=C3, id4=C4` 使用了关键词传参。
 
-5、动态属性是以人类易读的文本格式（[查看图示](https://lcctoor.github.io/arts/arts/oodb/ip_static/动态属性.png)）存储在 MongoDB 中的，可直接通过 Navicat 等管理工具灵活修改。
+5、动态属性是以人类易读的文本格式存储在 MongoDB 中的（[查看图示](https://lcctoor.github.io/arts/arts/oodb/ip_static/动态属性.png)），可直接通过 Navicat 等管理工具灵活修改。
 
 ## 面向对象特性综述
 
-【继承】和【动态属性】的特性都是动态模拟的，而非把数据写死在数据库里，因此：
+继承、方法、动态属性等特性都是动态解析的，当一个子对象继承一个父对象时，数据库中只会存储这两个对象的父子关系，而非把父对象的全部属性复制到子对象。因此：
 
-1、当我们修改某个父对象的属性值时，仅该对象的（在硬盘上的）实际存储值会发生变化，而它的子孙对象的（在硬盘上的）实际存储值不会发生任何变化。
+1、当我们修改某个父对象的属性值时，仅该父对象的（在硬盘上的）实际存储值会发生变化，而它的子孙对象的（在硬盘上的）实际存储值不会发生任何变化，并且不会影响这两个对象的继承关系。
 
-2、当我们欲修改某个对象的属性值时，除了使用 oodb（即本软件）的接口修改以外，也可以直接通过 Navicat 等管理工具手动修改，二者的效果是一致的。
+2、当我们欲修改任意一个对象的属性值时，除了使用 oodb（即本软件）的接口修改以外，也可以直接通过 Navicat 等管理工具手动修改，二者的效果是完全一致的。
 
 ## 条件筛选
 
 ### 示例一：理解条件筛选的基本范式
 
 筛选【年龄>13，且视力≧4.6，且性别为女】的数据，并进行查改删：
 
@@ -283,33 +284,33 @@
 
 **修改**：`sheet[mc.年龄 > 13][mc.视力 >= 4.6][mc.性别 == '女'].update( {'年级':'五年级', '爱好':'画画,跳绳'} )`
 
 **删除**：`sheet[mc.年龄 > 13][mc.视力 >= 4.6][mc.性别 == '女'].delete( )`
 
 ### 筛选操作清单
 
-| **代码**                                                       | 解释                                            |
-| -------------------------------------------------------------------- | ----------------------------------------------- |
-| mc.年龄 > 10                                                         | 大于                                            |
-| mc.年龄 >= 10                                                        | 大于或等于                                      |
-| mc.年龄 < 10                                                         | 小于                                            |
-| mc.年龄 <= 10                                                        | 小于或等于                                      |
-| mc.年龄 == 10                                                        | 等于                                            |
-| mc.年龄 != 10                                                        | 不等于                                          |
-| mc.年级 == mf.isin( '初三', '高二' )                                 | 若字段值是传入值的成员，则符合                  |
-| mc.年龄 == mf.notin( 10, 30, 45 )                                    | 若字段值不是传入值的成员，则符合                |
-| mc.爱好 == mf.contain_all( '画画', '足球' )                          | 若（列表）字段值包含传入值的所有元素，则符合    |
-| mc.爱好 == mf.contain_any( '画画', '足球' )                          | 若（列表）字段值包含传入值的至少1个元素，则符合 |
-| mc.爱好 == mf.contain_none( '画画', '足球' )                         | 若（列表）字段值不包含传入值的任何元素，则符合  |
-| mc.姓名 == mf.re( '小' )                                             | 正则匹配                                        |
-| `[mc.年龄 > 3][mc.年龄 < 100]`                                     | 交集（方式一）                                  |
-| [ (mc.年龄 > 3) & (mc.年龄 < 100) ]                                  | 交集（方式二）                                  |
-| `[(mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None)]` | 并集                                            |
-| [ (mc.年龄 > 3) - (mc.年龄 > 100) ]                                  | 差集                                            |
-| [ ~(mc.年龄 > 100) ]                                                 | 补集                                            |
+| **代码**                                                                 | 解释                                            |
+| ------------------------------------------------------------------------------ | ----------------------------------------------- |
+| mc.年龄 > 10                                                                   | 大于                                            |
+| mc.年龄 >= 10                                                                  | 大于或等于                                      |
+| mc.年龄 < 10                                                                   | 小于                                            |
+| mc.年龄 <= 10                                                                  | 小于或等于                                      |
+| mc.年龄 == 10                                                                  | 等于                                            |
+| mc.年龄 != 10                                                                  | 不等于                                          |
+| mc.年级 == mf.isin( '初三', '高二' )                                           | 若字段值是传入值的成员，则符合                  |
+| mc.年龄 == mf.notin( 10, 30, 45 )                                              | 若字段值不是传入值的成员，则符合                |
+| mc.爱好 == mf.contain_all( '画画', '足球' )                                    | 若（列表）字段值包含传入值的所有元素，则符合    |
+| mc.爱好 == mf.contain_any( '画画', '足球' )                                    | 若（列表）字段值包含传入值的至少1个元素，则符合 |
+| mc.爱好 == mf.contain_none( '画画', '足球' )                                   | 若（列表）字段值不包含传入值的任何元素，则符合  |
+| mc.姓名 == mf.re( '小' )                                                       | 正则匹配                                        |
+| \[mc.年龄 > 3\][mc.年龄 < 100]                                                 | 交集（方式一）                                  |
+| [ (mc.年龄 > 3) & (mc.年龄 < 100) ]                                            | 交集（方式二）                                  |
+| [(mc.年龄<30)&#124; (mc.年龄>30) &#124; (mc.年龄==30) &#124; (mc.年龄==None)] | 并集                                            |
+| [ (mc.年龄 > 3) - (mc.年龄 > 100) ]                                            | 差集                                            |
+| [ ~(mc.年龄 > 100) ]                                                           | 补集                                            |
 
 注：
 
 1、isin、notin 用于判断（普通）字段的值是否传入值的成员，针对普通字段。
 
 2、contain_any、contain_none 用于判断传入值是否（列表）字段的值的成员，针对列表字段。
```

### Comparing `arts-2024.3.6/arts/oodb/_core.py` & `arts-2024.4.3/arts/oodb/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
         return sheet.delete_one( {'_id': self._id} )
 
 
 class mpy:
     def _serialize_func(func):
         func_string = getsource(func)
         indent = len( re.search(r'''( *)@''', func_string).group(1) )
-        defined, func_name = re.search(rf'''\n( {{{indent}}}def +([^\s]+)\(.+)''', func_string, re.S).group(1, 2)
+        defined, func_name = re.search(rf'''\n( {{{indent}}}def +([^\s\(]+)\(.+)''', func_string, re.S).group(1, 2)
         return indent, defined, func_name
     
     @classmethod
     def method(cls, func):
         indent, defined, func_name = cls._serialize_func(func)
         return {'__oodb__': [ dict(pipeline='method', indent=indent, defined=defined, func_name=func_name) ]}
```

### Comparing `arts-2024.3.6/arts/oodb/licenses/pymongo/LICENSE` & `arts-2024.4.3/arts/oodb/licenses/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/oodb/pyproject.toml` & `arts-2024.4.3/arts/oodb/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "oodb"
-version = "1.0"
+version = "1.0.1"
 description = "面向对象数据库 —— 引入了 Python 中类的特性，如：继承、重写、方法、动态属性等。"
 dependencies = ["arts>=2024.3.6"]
 keywords = ["OODBMS", "OODBS", "oodb"]
 
 
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
```

### Comparing `arts-2024.3.6/arts/oomongo/LICENSE` & `arts-2024.4.3/arts/oomongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/oomongo/README.md` & `arts-2024.4.3/arts/oomongo/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 一个非常优雅的 MongoDB ODM 。
 
 # 作者
 
 [江南雨上](mailto:lcctoor@outlook.com)
 
-[主页](https://lcctoor.github.io/arts/) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
+[主页](https://lcctoor.github.io/arts) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
+你可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
 
 # 安装
 
 ```
 pip install oomongo
 ```
 
@@ -26,15 +26,15 @@
 
 ```python
 from pymongo import MongoClient
 from motor.motor_asyncio import AsyncIOMotorClient
 from oomongo import ODM, mc, mf, mo
 ```
 
-## 创建 ODM
+## 创建ODM
 
 ```python
 class ODM_2(ODM):
 
     def mkconn(self):  # 定义同步连接器
         return MongoClient(host='localhost', port=27017)
   
@@ -103,33 +103,33 @@
 
 **修改**：`sheet[mc.年龄 > 13][mc.视力 >= 4.6][mc.性别 == '女'].update( {'年级':'初一', '爱好':'画画,跳绳'} )`
 
 **删除**：`sheet[mc.年龄 > 13][mc.视力 >= 4.6][mc.性别 == '女'].delete( )`
 
 ### 筛选操作清单
 
-| **代码**                                                       | 解释                                            |
-| -------------------------------------------------------------------- | ----------------------------------------------- |
-| mc.年龄 > 10                                                         | 大于                                            |
-| mc.年龄 >= 10                                                        | 大于或等于                                      |
-| mc.年龄 < 10                                                         | 小于                                            |
-| mc.年龄 <= 10                                                        | 小于或等于                                      |
-| mc.年龄 == 10                                                        | 等于                                            |
-| mc.年龄 != 10                                                        | 不等于                                          |
-| mc.年级 == mf.isin( '初三', '高二' )                                 | 若字段值是传入值的成员，则符合                  |
-| mc.年龄 == mf.notin( 10, 30, 45 )                                    | 若字段值不是传入值的成员，则符合                |
-| mc.爱好 == mf.contain_all( '画画', '足球' )                          | 若（列表）字段值包含传入值的所有元素，则符合    |
-| mc.爱好 == mf.contain_any( '画画', '足球' )                          | 若（列表）字段值包含传入值的至少1个元素，则符合 |
-| mc.爱好 == mf.contain_none( '画画', '足球' )                         | 若（列表）字段值不包含传入值的任何元素，则符合  |
-| mc.姓名 == mf.re( '小' )                                             | 正则匹配                                        |
-| `[mc.年龄 > 3][mc.年龄 < 100]`                                     | 交集（方式一）                                  |
-| [ (mc.年龄 > 3) & (mc.年龄 < 100) ]                                  | 交集（方式二）                                  |
-| `[(mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None)]` | 并集                                            |
-| [ (mc.年龄 > 3) - (mc.年龄 > 100) ]                                  | 差集                                            |
-| [ ~(mc.年龄 > 100) ]                                                 | 补集                                            |
+| **代码**                                                                 | 解释                                            |
+| ------------------------------------------------------------------------------ | ----------------------------------------------- |
+| mc.年龄 > 10                                                                   | 大于                                            |
+| mc.年龄 >= 10                                                                  | 大于或等于                                      |
+| mc.年龄 < 10                                                                   | 小于                                            |
+| mc.年龄 <= 10                                                                  | 小于或等于                                      |
+| mc.年龄 == 10                                                                  | 等于                                            |
+| mc.年龄 != 10                                                                  | 不等于                                          |
+| mc.年级 == mf.isin( '初三', '高二' )                                           | 若字段值是传入值的成员，则符合                  |
+| mc.年龄 == mf.notin( 10, 30, 45 )                                              | 若字段值不是传入值的成员，则符合                |
+| mc.爱好 == mf.contain_all( '画画', '足球' )                                    | 若（列表）字段值包含传入值的所有元素，则符合    |
+| mc.爱好 == mf.contain_any( '画画', '足球' )                                    | 若（列表）字段值包含传入值的至少1个元素，则符合 |
+| mc.爱好 == mf.contain_none( '画画', '足球' )                                   | 若（列表）字段值不包含传入值的任何元素，则符合  |
+| mc.姓名 == mf.re( '小' )                                                       | 正则匹配                                        |
+| \[mc.年龄 > 3\][mc.年龄 < 100]                                                 | 交集（方式一）                                  |
+| [ (mc.年龄 > 3) & (mc.年龄 < 100) ]                                            | 交集（方式二）                                  |
+| [(mc.年龄<30)&#124; (mc.年龄>30) &#124; (mc.年龄==30) &#124; (mc.年龄==None)] | 并集                                            |
+| [ (mc.年龄 > 3) - (mc.年龄 > 100) ]                                            | 差集                                            |
+| [ ~(mc.年龄 > 100) ]                                                           | 补集                                            |
 
 注：
 
 1、isin、notin 用于判断（普通）字段的值是否传入值的成员，针对普通字段。
 
 2、contain_any、contain_none 用于判断传入值是否（列表）字段的值的成员，针对列表字段。
```

### Comparing `arts-2024.3.6/arts/oomongo/_core.py` & `arts-2024.4.3/arts/oomongo/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/oomongo/licenses/motor/LICENSE` & `arts-2024.4.3/arts/oomongo/licenses/motor/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/oomongo/licenses/pymongo/LICENSE` & `arts-2024.4.3/arts/oomongo/licenses/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/oomongo/pyproject.toml` & `arts-2024.4.3/arts/oomongo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/oomysql/LICENSE` & `arts-2024.4.3/arts/oomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/oomysql/README.md` & `arts-2024.4.3/arts/oomysql/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 一个优雅的 mysql ORM ，无须做模型映射，所有操作都同时提供同步、异步两种方式。
 
 # 作者
 
 [江南雨上](mailto:lcctoor@outlook.com)
 
-[主页](https://lcctoor.github.io/arts/) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
+[主页](https://lcctoor.github.io/arts) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
+你可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
 
 # 安装
 
 ```
 pip install oomysql
 ```
 
@@ -25,15 +25,15 @@
 ## 导入
 
 ```python
 import pymysql, aiomysql
 from oomysql import ORM, mc
 ```
 
-## 创建 ORM
+## 创建ORM
 
 ```python
 class ORM_2(ORM):
 
     def mkconn(self):  # 定义同步连接器
         return pymysql.connect(
             host = 'localhost',
@@ -102,30 +102,30 @@
 
 **修改**：`sheet[mc.年龄 > 13][mc.视力 >= 4.6][mc.性别 == '女'].update( {'年级':'初一', '爱好':'画画,跳绳'} )`
 
 **删除**：`sheet[mc.年龄 > 13][mc.视力 >= 4.6][mc.性别 == '女'].delete( )`
 
 ### 筛选操作清单
 
-| **代码**                                                       | **解释**                   |
-| -------------------------------------------------------------------- | -------------------------------- |
-| mc.年龄 > 10                                                         | 大于                             |
-| mc.年龄 >= 10                                                        | 大于或等于                       |
-| mc.年龄 < 10                                                         | 小于                             |
-| mc.年龄 <= 10                                                        | 小于或等于                       |
-| mc.年龄 == 10                                                        | 等于                             |
-| mc.年龄 != 10                                                        | 不等于                           |
-| mc.年级.isin( '初三', '高二' )                                       | 若字段值是传入值的成员，则符合   |
-| mc.年龄.notin( 10, 30, 45 )                                          | 若字段值不是传入值的成员，则符合 |
-| mc.姓名.re( '小' )                                                   | 正则匹配                         |
-| `[mc.年龄 > 3][mc.年龄 < 100]`                                     | 交集（方式一）                   |
-| [ (mc.年龄 > 3) & (mc.年龄 < 100) ]                                  | 交集（方式二）                   |
-| `[(mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None)]` | 并集                             |
-| [ (mc.年龄 > 3) - (mc.年龄 > 100) ]                                  | 差集                             |
-| [ ~(mc.年龄 > 100) ]                                                 | 补集                             |
+| **代码**                                                                 | **解释**                   |
+| ------------------------------------------------------------------------------ | -------------------------------- |
+| mc.年龄 > 10                                                                   | 大于                             |
+| mc.年龄 >= 10                                                                  | 大于或等于                       |
+| mc.年龄 < 10                                                                   | 小于                             |
+| mc.年龄 <= 10                                                                  | 小于或等于                       |
+| mc.年龄 == 10                                                                  | 等于                             |
+| mc.年龄 != 10                                                                  | 不等于                           |
+| mc.年级.isin( '初三', '高二' )                                                 | 若字段值是传入值的成员，则符合   |
+| mc.年龄.notin( 10, 30, 45 )                                                    | 若字段值不是传入值的成员，则符合 |
+| mc.姓名.re( '小' )                                                             | 正则匹配                         |
+| \[mc.年龄 > 3\][mc.年龄 < 100]                                                 | 交集（方式一）                   |
+| [ (mc.年龄 > 3) & (mc.年龄 < 100) ]                                            | 交集（方式二）                   |
+| [(mc.年龄<30)&#124; (mc.年龄>30) &#124; (mc.年龄==30) &#124; (mc.年龄==None)] | 并集                             |
+| [ (mc.年龄 > 3) - (mc.年龄 > 100) ]                                            | 差集                             |
+| [ ~(mc.年龄 > 100) ]                                                           | 补集                             |
 
 注：
 
 1、isin、notin 的传入值都不必是同类型的数据，以 isin 为例：可以这样使用：mc.tag.isin( 3, 3.5, '学生', None )  ，传入值含有 int、float、str、NoneType 等多种类型。
 
 2、成员运算符未传入任何值时的处理方式：
```

### Comparing `arts-2024.3.6/arts/oomysql/_core.py` & `arts-2024.4.3/arts/oomysql/_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 empset = FALSE()
 undefined = FALSE()
 
 class ORMIndexError(IndexError):
     def __repr__(self):
         return 'ORMIndexError'
 
-def JChinese(data): return dumps(data, ensure_ascii=False)
+def dump_data(data): return dumps(data, ensure_ascii=False)
 
 
 class ORM():
 
     def __init__(self):
         self._connpool = deque([], maxlen=1)
         self._aconnpool = deque([], maxlen=1)
@@ -425,15 +425,15 @@
                 else:
                     return r[::-S]
             else:
                 return []
 
     def update(self, data: dict):
         key = self._parse_slice()
-        data = ', '.join([f"{k}={v.field}" if isinstance(v,Filter) else f"{k}={JChinese(v)}" for k,v in data.items()])
+        data = ', '.join([f"{k}={v.field}" if isinstance(v,Filter) else f"{k}={dump_data(v)}" for k,v in data.items()])
         # [::]
         if isinstance(key, list):
             L, R, S = key[0], key[1], key[2] or 1
             if S in [None, 1]:
                 if (L in [None, 1] and R in [None, -1]) or (L == -1 and R == 1):
                     rdata, cursor = self.execute(f"update {self.sheet_name} set {data}{self._parse_where()}")
                     return cursor
@@ -456,15 +456,15 @@
                     rdata, cursor = self.execute(f"update {self.sheet_name} set {data} where 1 = 2")
             else:
                 rdata, cursor = self.execute(f"update {self.sheet_name} set {data}{mc[pk] == pks[pk]} limit 1")
         return cursor
 
     async def aupdate(self, data: dict):
         key = self._parse_slice()
-        data = ', '.join([f"{k}={v.field}" if isinstance(v,Filter) else f"{k}={JChinese(v)}" for k,v in data.items()])
+        data = ', '.join([f"{k}={v.field}" if isinstance(v,Filter) else f"{k}={dump_data(v)}" for k,v in data.items()])
         # [::]
         if isinstance(key, list):
             L, R, S = key[0], key[1], key[2] or 1
             if S in [None, 1]:
                 if (L in [None, 1] and R in [None, -1]) or (L == -1 and R == 1):
                     rdata, cursor = await self.aexecute(f"update {self.sheet_name} set {data}{self._parse_where()}")
                     return cursor
@@ -615,15 +615,15 @@
             lines = lines[0]
         # 更新到数据库
         if records:
             blocks = []
             for field, kvs in records.items():
                 s = [f"{field} = ", '    case']
                 for k, v in kvs.items():
-                    s.append(f"        when {pk} = {JChinese(k)} then {JChinese(v)}")
+                    s.append(f"        when {pk} = {dump_data(k)} then {dump_data(v)}")
                 s.append(f"else {field}")
                 s.append('end')
                 blocks.append('\n'.join(s))
             blocks = ' ,\n'.join(blocks)
             sql = f"update {self.sheet_name} set \n{blocks}"
             self.execute(sql=sql)
             return dict(data=lines)
@@ -660,15 +660,15 @@
             lines = lines[0]
         # 更新到数据库
         if records:
             blocks = []
             for field, kvs in records.items():
                 s = [f"{field} = ", '    case']
                 for k, v in kvs.items():
-                    s.append(f"        when {pk} = {JChinese(k)} then {JChinese(v)}")
+                    s.append(f"        when {pk} = {dump_data(k)} then {dump_data(v)}")
                 s.append(f"else {field}")
                 s.append('end')
                 blocks.append('\n'.join(s))
             blocks = ' ,\n'.join(blocks)
             sql = f"update {self.sheet_name} set \n{blocks}"
             await self.aexecute(sql=sql)
             return dict(data=lines)
@@ -684,15 +684,15 @@
         for key, line in data.items():
             for field, value in line.items():
                 records.setdefault(field, {})[key] = value
         blocks = []
         for field, kvs in records.items():
             s = [f"{field} = ", '    case']
             for k, v in kvs.items():
-                s.append(f"        when {pk} = {JChinese(k)} then {JChinese(v)}")
+                s.append(f"        when {pk} = {dump_data(k)} then {dump_data(v)}")
             s.append(f"else {field}")
             s.append('end')
             blocks.append('\n'.join(s))
         blocks = ' ,\n'.join(blocks)
         sql = f"update {self.sheet_name} set \n{blocks}"
         r, cursor = self.execute(sql=sql)
         return cursor
@@ -703,15 +703,15 @@
         for key, line in data.items():
             for field, value in line.items():
                 records.setdefault(field, {})[key] = value
         blocks = []
         for field, kvs in records.items():
             s = [f"{field} = ", '    case']
             for k, v in kvs.items():
-                s.append(f"        when {pk} = {JChinese(k)} then {JChinese(v)}")
+                s.append(f"        when {pk} = {dump_data(k)} then {dump_data(v)}")
             s.append(f"else {field}")
             s.append('end')
             blocks.append('\n'.join(s))
         blocks = ' ,\n'.join(blocks)
         sql = f"update {self.sheet_name} set \n{blocks}"
         r, cursor = await self.aexecute(sql=sql)
         return cursor
@@ -772,43 +772,43 @@
 
     def __init__(self, field):
         self.field = field
 
     def __eq__(self, obj):
         if obj is None:
             return Factory(f"{self.field} is null")
-        return Factory(f"{self.field} = {JChinese(obj)}")
+        return Factory(f"{self.field} = {dump_data(obj)}")
 
     def __ne__(self, obj):
         if obj is None:
             return Factory(f"{self.field} is not null")
-        return Factory(f"{self.field} != {JChinese(obj)}")
+        return Factory(f"{self.field} != {dump_data(obj)}")
 
-    def __lt__(self, obj): return Factory(f"{self.field} < {JChinese(obj)}")
-    def __le__(self, obj): return Factory(f"{self.field} <= {JChinese(obj)}")
-    def __gt__(self, obj): return Factory(f"{self.field} > {JChinese(obj)}")
-    def __ge__(self, obj): return Factory(f"{self.field} >= {JChinese(obj)}")
-    def re(self, pattern): return Factory(f"{self.field} regexp {JChinese(pattern or '')}")
+    def __lt__(self, obj): return Factory(f"{self.field} < {dump_data(obj)}")
+    def __le__(self, obj): return Factory(f"{self.field} <= {dump_data(obj)}")
+    def __gt__(self, obj): return Factory(f"{self.field} > {dump_data(obj)}")
+    def __ge__(self, obj): return Factory(f"{self.field} >= {dump_data(obj)}")
+    def re(self, pattern): return Factory(f"{self.field} regexp {dump_data(pattern or '')}")
 
     def isin(self, *lis):
         if not lis: return Factory(empset)
         if len(lis) == 1: return self == lis[0]
         null = False
         type_item = {str:set(), int:set(), float:set()}
         for i, x in enumerate(lis):
             if x is None:
                 null = True
             else:
                 type_item[type(x)].add(x)
         sumlis = []
         for lis in type_item.values():
             if len(lis) == 1:
-                sumlis.append(f"{self.field} = {JChinese(list(lis)[0])}")
+                sumlis.append(f"{self.field} = {dump_data(list(lis)[0])}")
             elif len(lis) > 1:
-                sumlis.append(f"{self.field} in ({', '.join(JChinese(x) for x in lis)})")
+                sumlis.append(f"{self.field} in ({', '.join(dump_data(x) for x in lis)})")
         if null:
             sumlis.append(f"{self.field} is null")
         if len(sumlis) == 1:
             return Factory(sumlis[0])
         else:
             return Factory(' or '.join(f"({x})" for x in sumlis))
 
@@ -821,17 +821,17 @@
             if x is None:
                 null = True
             else:
                 type_item[type(x)].add(x)
         sumlis = []
         for lis in type_item.values():
             if len(lis) == 1:
-                sumlis.append(f"{self.field} != {JChinese(list(lis)[0])}")
+                sumlis.append(f"{self.field} != {dump_data(list(lis)[0])}")
             elif len(lis) > 1:
-                sumlis.append(f"{self.field} not in ({', '.join(JChinese(x) for x in lis)})")
+                sumlis.append(f"{self.field} not in ({', '.join(dump_data(x) for x in lis)})")
         if null:
             sumlis.append(f"{self.field} is not null")
             sumlis = sumlis[0] if len(sumlis) == 1 else ' and '.join(f"({x})" for x in sumlis)
         else:
             sumlis = sumlis[0] if len(sumlis) == 1 else ' and '.join(f"({x})" for x in sumlis)
             sumlis = f"({sumlis}) or ({self.field} is null)"
         return Factory(sumlis)
```

### Comparing `arts-2024.3.6/arts/oomysql/licenses/aiomysql/LICENSE` & `arts-2024.4.3/arts/oomysql/licenses/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/oomysql/licenses/pymysql/LICENSE` & `arts-2024.4.3/arts/oomysql/licenses/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/oomysql/pyproject.toml` & `arts-2024.4.3/arts/oomysql/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/openai2/LICENSE` & `arts-2024.4.3/arts/openai2/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/openai2/README.md` & `arts-2024.4.3/arts/openai2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。
 
 # 作者
 
 [江南雨上](mailto:lcctoor@outlook.com)
 
-[主页](https://lcctoor.github.io/arts/) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
+[主页](https://lcctoor.github.io/arts) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
+你可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
 
 # 安装
 
 ```
 pip install openai2
 ```
```

### Comparing `arts-2024.3.6/arts/openai2/_core/GroupChat.py` & `arts-2024.4.3/arts/openai2/_core/GroupChat.py`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/openai2/_core/chat.py` & `arts-2024.4.3/arts/openai2/_core/chat.py`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/openai2/_core/chat_in_cmd.py` & `arts-2024.4.3/arts/openai2/_core/chat_in_cmd.py`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/openai2/licenses/openai/LICENSE` & `arts-2024.4.3/arts/openai2/licenses/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/openai2/pyproject.toml` & `arts-2024.4.3/arts/openai2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/skybox/README.md` & `arts-2024.4.3/arts/skybox/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/skybox/skybox/files_hashes` & `arts-2024.4.3/arts/skybox/skybox/files_hashes`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 CoolMemory-English                         
     v1.0 -binary -20231211.zip                 -info {"size": 742544827, "sha-512": "d495b3c0e22479a7ec8f3c1ce1310b41502d2d1dcbb5e75e726efcfb058c347fde1d87b598e6974838c74cf93827af920a80b20374cf5ae6880467d6121e9b47", "sha3-512": "0abde1cf89dd66b0f5d80bc714aade0bc131c28457625b7b6e7bf5c96d71b89408f168aa3a12f9213d8c16fd41b27ef2e44d9d11b23d7fef04440d62fadc599e"}
     v1.0 -source -20231211.zip                 -info {"size": 597636983, "sha-512": "77e40a18d8e1498a2bd513705aeb46d3460b1dcf9b3036bdd8d5b9dd0d2f696e552aa59733840a2a5ae8174fa117184d834ca82c266605246e6e8b80ea48d686", "sha3-512": "f06683d43e8242cf925a344e7f012d08560d06f6aecbd3e7a7cf2128ed92f8aa9ea0b96ab27e961accf3ab066c8ebab2cb730a5d01f0d8b2a3d88a748a97f0ff"}
     v1.0 -使用演示 -20231209.mp4               -info {"size": 10600883, "sha-512": "5491253c44503d4803ea2435cbfcdc0ba3e8950624020b5a6b48ee577b7cbcede20a32edcb8bb6ca19feb6e35c864c388f709e2827cc8f252936bf1457e71080", "sha3-512": "7da5a731c6b29fe6482c5f7aaf876a7af3643bf86055358fb7e969572c8b2621f93bfa285ccee8baa5eea0f266e1492cda74190e3785899af3f4ac3964aad6bf"}
     独家版权词汇 -11679个 -20231210.zip        -info {"size": 123934860, "sha-512": "e76c02d86ebbac94eec1332dad4884bb1ab33ca0673be2cc0cd273989fc3f97be5bb90829f69440397927eefd7f3c767d3f90404c241085c0e88c5374cfb14bc", "sha3-512": "437e69b287656bc216f9765b9327214a1688f6fc3160a7f4348539f789f984420b66c7b9363d2def248a4facc7838e746f4c9390de8db48c0515691e9d636510"}
 PyPi                                       
-    arts-2023.12.20.zip                        -info {"size": 458736, "sha-512": "c66a317122f7f7656adb1f63b5021379da2fc8458588d2668d374bb29ad1d35a89985f139899b3928e51d2678a49022bac82a99afc3309ec6292659c38c60a03", "sha3-512": "b07cd2bb78d4f9115bf6d73cfe29202a8232cb95d92459e5bd57858798fb0f2a1a4bc3dd57a8af650ba1e349febd5eb39dbd64e34f34d5f4806d60f4ce5b2930"}
-    arts-2024.1.17.zip                         -info {"size": 571603, "sha-512": "327342199a59a3678a8e09e3706a7885b0ad83ebd3c3183f74b7c95ce6e5e6350dad1a26ce32cdc08c3b2fee2e7f467000c571a4e366002063a683076bbf1a39", "sha3-512": "e21b1ba2bf287a6c356b96b8c9c08c439d99dab8d877669d087991479b3906eb5f25540c674655b7e4d99ca07e9d4eac62183d0c34815dd9c5c9862be62135cf"}
-    arts-2024.1.30.zip                         -info {"size": 582125, "sha-512": "f33c6f44f62871b7f3660c91d19b80b9a03fa1f93d537b461a37e479e5b4fd823a57c97d52d0c6160d92d1bf8ae0a6e61101c5d759792303c094d5c8e5ec68fb", "sha3-512": "af8bf7c9d2b342de2296756c2048e5f4b14ee09fee032559a18f05ce471a85ad56c01d72b40f13369c848a0fff136be0d700b09ffc9df4fbe104a795abac1a99"}
-    arts-2024.2.13.zip                         -info {"size": 633463, "sha-512": "335fc45861fd8785c077baa2b2035702340a1e0cd815ae11db258f61979948edf55139757d2991d3800a2398e89ac225dbff8150418aae0c9df980d92c895110", "sha3-512": "d4381233c7c640d474fea34eeebfa9e7cc0d2ba07b3bfe9ea9bad81a34d83828f511b395bf7b6b7d4d474798cb4950181d569200d95091ffd08b099e181e270a"}
-    arts-2024.2.25.zip                         -info {"size": 662003, "sha-512": "430648c7c3e2623f4addad65ed6897d8d70b994c65612217cccb5f106596910e9eeadf5417d5036532921a4b8161cda8d93f73d6acf5572b1089cf7084a290e2", "sha3-512": "d0f228a0e9a5c8f6fcfca392fded9abfda2ab1b82939cb50a45b4977b00bd427c81913289924d704bdda8c21bc61eb3ef22cb6b09d311b768a2d52a62eafccdc"}
+    arts -2023.12.20.zip                       -info {"size": 458736, "sha-512": "c66a317122f7f7656adb1f63b5021379da2fc8458588d2668d374bb29ad1d35a89985f139899b3928e51d2678a49022bac82a99afc3309ec6292659c38c60a03", "sha3-512": "b07cd2bb78d4f9115bf6d73cfe29202a8232cb95d92459e5bd57858798fb0f2a1a4bc3dd57a8af650ba1e349febd5eb39dbd64e34f34d5f4806d60f4ce5b2930"}
+    arts -2024.1.17.zip                        -info {"size": 571603, "sha-512": "327342199a59a3678a8e09e3706a7885b0ad83ebd3c3183f74b7c95ce6e5e6350dad1a26ce32cdc08c3b2fee2e7f467000c571a4e366002063a683076bbf1a39", "sha3-512": "e21b1ba2bf287a6c356b96b8c9c08c439d99dab8d877669d087991479b3906eb5f25540c674655b7e4d99ca07e9d4eac62183d0c34815dd9c5c9862be62135cf"}
+    arts -2024.1.30.zip                        -info {"size": 582125, "sha-512": "f33c6f44f62871b7f3660c91d19b80b9a03fa1f93d537b461a37e479e5b4fd823a57c97d52d0c6160d92d1bf8ae0a6e61101c5d759792303c094d5c8e5ec68fb", "sha3-512": "af8bf7c9d2b342de2296756c2048e5f4b14ee09fee032559a18f05ce471a85ad56c01d72b40f13369c848a0fff136be0d700b09ffc9df4fbe104a795abac1a99"}
+    arts -2024.2.13.zip                        -info {"size": 633463, "sha-512": "335fc45861fd8785c077baa2b2035702340a1e0cd815ae11db258f61979948edf55139757d2991d3800a2398e89ac225dbff8150418aae0c9df980d92c895110", "sha3-512": "d4381233c7c640d474fea34eeebfa9e7cc0d2ba07b3bfe9ea9bad81a34d83828f511b395bf7b6b7d4d474798cb4950181d569200d95091ffd08b099e181e270a"}
+    arts -2024.2.25.zip                        -info {"size": 662003, "sha-512": "430648c7c3e2623f4addad65ed6897d8d70b994c65612217cccb5f106596910e9eeadf5417d5036532921a4b8161cda8d93f73d6acf5572b1089cf7084a290e2", "sha3-512": "d0f228a0e9a5c8f6fcfca392fded9abfda2ab1b82939cb50a45b4977b00bd427c81913289924d704bdda8c21bc61eb3ef22cb6b09d311b768a2d52a62eafccdc"}
+    arts -2024.3.25.zip                        -info {"size": 731537, "sha-512": "ab80e3c2c0e583552c45134a01991c40f7b02379249299ce19cd01fa411b7e034cb6cc9d8078b93a183577261f20ef6fcca8a0ba05e781d492c7e8d5d2192604", "sha3-512": "0e532cac08a44498c3f001ebdd262fd21e471165a6503264bca0b26b81d63b9de869cda5d94d741b6187e12f93b5167c5bda34ea274398a9da66168538f5a565"}
+    arts -2024.3.31.zip                        -info {"size": 784894, "sha-512": "d14e1defcd1845602c68dfa1e2b01f08b970eaa0c2c08426eab9f7c2acc265ed2eaee024c7f9cb935e05477fc1e078e43cd2f09b2806d57a77880542e179a570", "sha3-512": "ee6ee0dd3247be1bbacde5819d8fb8e2a35422ce7e4c4ce20fef13ac80598ed654d65182d550e0f29d4a694dfba38eef825747a6565265af954a217d9c20ab86"}
+    arts -2024.3.6.zip                         -info {"size": 729443, "sha-512": "f7d02e0c59ca5da9460ef8af9ed08d2c3c2bc903a3cec85411588badc42f81b64c0df2841b5fb790d24fb3eeb6728e2e7cb363d8bfa859afd7b23b8b997cd83b", "sha3-512": "8fa2af71bcb48993cb6be156c6e07a4ad052fb83cd1d35c89fcb237d135a0a05c2f3aeea7490b5874d3f0b8f61d0e72560163cc2d0c8ff6d58cd86bc902942f8"}
     wss -20231220.zip                          -info {"size": 8614060, "sha-512": "473d3652c54b15af6fde766cea58974e63b66ba086d44d09b4de6b50d275d07bac4d4c4d6b632dde6e85e971d35566f958efd1b6741d6b96ae67ee6f2ee362b2", "sha3-512": "5f4c6eb204872dc7893c607afabb016ceec67561ddbe76bfb65610d91a3d7dfcce7a0a27da7c81d4f9bee442a97609bfa3d62bee15c2fd435c19ad3152693785"}
+    wss -20240325.zip                          -info {"size": 8200568, "sha-512": "2539dd1162403630a705148c90d79b393e9f4a3b9eb81231bfa9fcfe31d1fe185e68c3226bf0d3ae76377c8e3465452e32497e5f470bfe07b60b6fabdd0d509c", "sha3-512": "d510ad8925838c974f2807c79b500a9a7eceddf7dc9f62169615cebfe24f4af484eddecd1ca7c7413e99b8f0a0870b2fe7b6184f475b77736bb754ccd2977f34"}
+    wss -20240331.zip                          -info {"size": 8370828, "sha-512": "d644b57284a09ef8fcaeb516dad6d97a997d40cfc0dbcfa3f1f55593b8f76000d93c3708c43d5fc50e5d6255f0d8ca9e52016e618a595d32657bdd466849d772", "sha3-512": "05d33f34bdfcce247dc5ddf27ad9845f01c656711938ffef1f3d006c78c26d08b9d6a6c0f961d85a07393d26cc5c346bc7f27cb94e786d90434fbc70fc3b4284"}
+    wss -20240401.zip                          -info {"size": 8422919, "sha-512": "528343b0345c8797713efc2603bb7657215f878ccb06f963424daf4e397cfa1e4296af8af03e4f8457341fa947995e317f6d2e1de8d10954c800a26dc0f40fdb", "sha3-512": "ca09072ed27cecc6990a6c1a7612d4c30f80571039f7f351a4434da7d3d1daf0febc7b50b69595efa63f354a483e8c0e6805fceda9ecf26e10354510459896ad"}
 富文本笔记本.png                               -info {"size": 644251, "sha-512": "e8293b799d49e53501fb50e85f7025d3d1f7c83e05f8982af51cc75c309d5014a17fb2326b8476335575b6bf4f8c2d4ffe2f4de9c3c423ef92adc3766996832f", "sha3-512": "82aecb03ab4abb583a6791b32301d76dafc451a70ee2f22b0c2c71428a0f100471beae02195681b61d1f6d7d1efdeaac719ffafbce9410b2c5065fe05841b009"}
 按键行为和鼠标行为采集装置                 
     2023-09-12.zip                             -info {"size": 939254, "sha-512": "939a9ee1132c5a5ef837f3f77b2bb005caafcd4f7cbc8ea1d219f2b1a1f512c7b71faf2c7a96ab961f7f62918992f1122e497c08c435f9579ff6c5d13f00b90f", "sha3-512": "efedfc0ece0c44d2ea1fb705dac8ab5283e74faf6e3e973a91ce447ffae1cc85359f96b1b33092fe61032a1424c62ed6e37a9fb9107f9029008474f3977a4446"}
 捷鸟.jpg                                       -info {"size": 793233, "sha-512": "96da3cf6df87d85d59bbdf80ccbbf0c841fcdd52d37ca2556219020c94978c01cf648df52d51dc2733f5bc773b734d9ba5b17e9cc8056278857a9059f5c756e3", "sha3-512": "99dfdb17c8663587c7db7b18621c11743e89cb67f6ab8be395c5901adae0a3fe7838175fcba7194927deb1c3ae509c1577eb2ad4b4d3c04890c94b77b00cc311"}
 桌面APP导航栏.png                              -info {"size": 256699, "sha-512": "b5cc935b98f28f0354b401e5f6d8e9768376ba6be7be1996247155459792a2a27131fee396bf0c8384c9e504115eb84d86f713e5d229f132889fd2b03b44f1e8", "sha3-512": "64c1edea61003c4147974a0f81eb748d98de1678d5a3ec13149297219526de25656942b8eb6c21b0546a3ea2dc9af367def29f6a60e81aab01796e146fdb5f4a"}
 短视频                                     
     AI是这样画包拯的.mp4                       -info {"size": 1927086, "sha-512": "eab1c2640c96826a1e15166bbdfcd5bd0011b5561ec3548d3c067f24627060354db699e49dd700e48ecbdeddd5d1492dabaa6ad08de8a5f66554dfd18a7eb96a", "sha3-512": "357b5252450d3b530b76e208d0ac3934df007dbe80259f1e5cabe6a9f4f9b23a76da858af1725dadaafcc762dea4a2ddb7a961d1bab794c10b89f5829c39156d"}
```

### Comparing `arts-2024.3.6/arts/thoughts/2022/现代工人的螺丝钉处境/index.html` & `arts-2024.4.3/arts/thoughts/2022/现代工人的螺丝钉处境/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html` & `arts-2024.4.3/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/专利是个公平的赛道/index.html` & `arts-2024.4.3/arts/thoughts/2023/保护好人/index.html`

 * *Files 19% similar despite different names*

```diff
@@ -4,20 +4,17 @@
     <meta charset='utf-8'>
     <meta content='width=device-width, initial-scale=1.0' name='viewport'>
     <link rel="stylesheet" href="https://lcctoor.github.io/arts/arts/ip_static/01/article_css.css">
     <link rel="stylesheet" href="C:/bpath/offline_files/lcctoor.github.io/arts/ip_static/01/article_css.css">
 </head>
 <body>
 <pre>
-普通人由于缺乏人脉和资源，想通过创业赚钱难度较大。对于普通人而言，一个相对公平的赚钱赛道是做专利。
+没有谁是天生的样子。
 
-做专利凭借的是一个人的天赋和才华，而非祖上三代人的努力。
+但尽管如此，还没变坏的人，比已经变坏的人在当下更值得被善待。
 
-我的第一个专利已经快写好了：
+保护现在的好人，保护曾经的好人（坏人可能曾经是好人）。
 </pre>
-    <script>
-        media = ['ip_static/01.jpg']
-    </script>
     <script src="https://lcctoor.github.io/arts/arts/ip_static/01/article_js.js"></script>
     <script src="C:/bpath/offline_files/lcctoor.github.io/arts/ip_static/01/article_js.js"></script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
-普通人由于缺乏人脉和资源，想通过创业赚钱难度较大。对于普通人而言，一个相对公平的赚钱赛道是做专利。
+没有谁是天生的样子。
 
-做专利凭借的是一个人的天赋和才华，而非祖上三代人的努力。
+但尽管如此，还没变坏的人，比已经变坏的人在当下更值得被善待。
 
-我的第一个专利已经快写好了：
+保护现在的好人，保护曾经的好人（坏人可能曾经是好人）。
```

### Comparing `arts-2024.3.6/arts/thoughts/2023/事情的真实性是由度的/index.html` & `arts-2024.4.3/arts/thoughts/2023/事情的真实性是由度的/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/人无法摆脱兽性/index.html` & `arts-2024.4.3/arts/thoughts/2023/人无法摆脱兽性/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/什么是极端？/index.html` & `arts-2024.4.3/arts/thoughts/2023/什么是极端？/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/保护好人/index.html` & `arts-2024.4.3/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,15 @@
     <meta charset='utf-8'>
     <meta content='width=device-width, initial-scale=1.0' name='viewport'>
     <link rel="stylesheet" href="https://lcctoor.github.io/arts/arts/ip_static/01/article_css.css">
     <link rel="stylesheet" href="C:/bpath/offline_files/lcctoor.github.io/arts/ip_static/01/article_css.css">
 </head>
 <body>
 <pre>
-没有谁是天生的样子。
+强人工智能真的出现了，那就是 chatgpt-4 。
 
-但尽管如此，还没变坏的人，比已经变坏的人在当下更值得被善待。
-
-保护现在的好人，保护曾经的好人（坏人可能曾经是好人）。
+之所以现在 chatgpt-4 是否强人工智能还有争议，那是因为和人对比，要是和狗、猫这些低智商的物种对比，chatgpt-4 是妥妥的强人工智能。
 </pre>
     <script src="https://lcctoor.github.io/arts/arts/ip_static/01/article_js.js"></script>
     <script src="C:/bpath/offline_files/lcctoor.github.io/arts/ip_static/01/article_js.js"></script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,3 @@
-没有谁是天生的样子。
+强人工智能真的出现了，那就是 chatgpt-4 。
 
-但尽管如此，还没变坏的人，比已经变坏的人在当下更值得被善待。
-
-保护现在的好人，保护曾经的好人（坏人可能曾经是好人）。
+之所以现在 chatgpt-4 是否强人工智能还有争议，那是因为和人对比，要是和狗、猫这些低智商的物种对比，chatgpt-4 是妥妥的强人工智能。
```

### Comparing `arts-2024.3.6/arts/thoughts/2023/只筛选，不教化/index.html` & `arts-2024.4.3/arts/thoughts/2023/只筛选，不教化/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/喊高考加油是刷存在感/index.html` & `arts-2024.4.3/arts/thoughts/2023/喊高考加油是刷存在感/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html` & `arts-2024.4.3/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html` & `arts-2024.4.3/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/想去国外了解自己/index.html` & `arts-2024.4.3/arts/thoughts/2023/想去国外了解自己/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/现代化的分工合作机制/index.html` & `arts-2024.4.3/arts/thoughts/2023/现代化的分工合作机制/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/用理性处理简单的事情/index.html` & `arts-2024.4.3/arts/thoughts/2023/用理性处理简单的事情/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/真正的问题无法通过花招解决/index.html` & `arts-2024.4.3/arts/thoughts/2023/真正的问题无法通过花招解决/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html` & `arts-2024.4.3/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html` & `arts-2024.4.3/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2024/不要害怕犯错/index.html` & `arts-2024.4.3/arts/thoughts/2024/不要害怕犯错/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2024/新年题诗/index.html` & `arts-2024.4.3/arts/thoughts/2024/新年题诗/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html` & `arts-2024.4.3/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html` & `arts-2024.4.3/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html` & `arts-2024.4.3/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/tutorials/600-用37行代码实现AI五子棋/README.md` & `arts-2024.4.3/arts/tutorials/600-用37行代码实现AI五子棋/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/arts/tutorials/750-正则表达式/README.md` & `arts-2024.4.3/arts/tutorials/750-正则表达式/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.3.6/pyproject.toml` & `arts-2024.4.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "arts"
-version = "2024.3.6"
+version = "2024.4.3"
 description = "对 Python 开发中常用功能的封装"
 dependencies = ["openai>=1.2.4", "numpy", "pymysql", "aiomysql", "pymongo", "motor", "pyppeteer>=2.0.0", "tornado"]
 
 
 requires-python = ">=3.10"
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
```

