# Comparing `tmp/telegram_bot_reporter-0.1.7.tar.gz` & `tmp/telegram_bot_reporter-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_bot_reporter-0.1.7.tar", max compression
+gzip compressed data, was "telegram_bot_reporter-0.1.8.tar", max compression
```

## Comparing `telegram_bot_reporter-0.1.7.tar` & `telegram_bot_reporter-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1020 2024-03-30 08:06:04.026651 telegram_bot_reporter-0.1.7/README.md
--rw-r--r--   0        0        0     2293 2024-04-01 17:44:54.787154 telegram_bot_reporter-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      111 2024-03-30 10:03:53.561341 telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 06:03:42.268386 telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/__init__.py
--rw-r--r--   0        0        0     2684 2024-03-30 10:03:53.473339 telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/async_bot.py
--rw-r--r--   0        0        0      921 2024-04-01 17:44:27.743363 telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/base_bot.py
--rw-r--r--   0        0        0     2531 2024-03-30 10:03:53.473339 telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/sync_bot.py
--rw-r--r--   0        0        0     1657 1970-01-01 00:00:00.000000 telegram_bot_reporter-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1461 2024-04-06 08:32:39.233383 telegram_bot_reporter-0.1.8/README.md
+-rw-r--r--   0        0        0     2293 2024-04-06 08:32:39.169384 telegram_bot_reporter-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      111 2024-03-30 10:03:53.561341 telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 06:03:42.268386 telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/__init__.py
+-rw-r--r--   0        0        0     2684 2024-03-30 10:03:53.473339 telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/async_bot.py
+-rw-r--r--   0        0        0      921 2024-04-01 17:44:27.743363 telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/base_bot.py
+-rw-r--r--   0        0        0     2531 2024-03-30 10:03:53.473339 telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/sync_bot.py
+-rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 telegram_bot_reporter-0.1.8/PKG-INFO
```

### Comparing `telegram_bot_reporter-0.1.7/pyproject.toml` & `telegram_bot_reporter-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "telegram-bot-reporter"
-version = "0.1.7"
+version = "0.1.8"
 description = "Library for sending messages and files using a Telegram bot."
 authors = ["deskent <battenetciz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Deskent/bot_reporter"
 homepage = "https://pypi.org/project/telegram-bot-reporter/"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 niquests = "^3.5.5"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 flake8 = "^7.0.0"
 ruff = "^0.3.4"
@@ -26,15 +26,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 
 [tool.black]
 line-length = 79
-target-version = ['py311']
+target-version = ['py310']
 include = '\.pyi?$'
 extend-exclude = '''
 /(
   # The following are specific to Black, you probably don't want those.
   tests/data
   | profiling
 )/
@@ -88,16 +88,16 @@
     "migrations",
     "spam",
     "*.toml",
     "test_migrations/staff/utils",
 ]
 line-length = 79
 
-# Assume Python 3.11
-target-version = "py311"
+# Assume Python 3.10
+target-version = "py310"
 
 
 [tool.ruff.format]
 ## Like Black, use single quotes for strings.
 quote-style = "single"
 
 ## Like Black, indent with spaces, rather than tabs.
```

### Comparing `telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/async_bot.py` & `telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/async_bot.py`

 * *Files identical despite different names*

### Comparing `telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/base_bot.py` & `telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/base_bot.py`

 * *Files identical despite different names*

### Comparing `telegram_bot_reporter-0.1.7/src/telegram_bot_reporter/core/sync_bot.py` & `telegram_bot_reporter-0.1.8/src/telegram_bot_reporter/core/sync_bot.py`

 * *Files identical despite different names*

### Comparing `telegram_bot_reporter-0.1.7/PKG-INFO` & `telegram_bot_reporter-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,135 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7465 6c65  : 2.1.Name: tele
 00000020: 6772 616d 2d62 6f74 2d72 6570 6f72 7465  gram-bot-reporte
-00000030: 720a 5665 7273 696f 6e3a 2030 2e31 2e37  r.Version: 0.1.7
+00000030: 720a 5665 7273 696f 6e3a 2030 2e31 2e38  r.Version: 0.1.8
 00000040: 0a53 756d 6d61 7279 3a20 4c69 6272 6172  .Summary: Librar
 00000050: 7920 666f 7220 7365 6e64 696e 6720 6d65  y for sending me
 00000060: 7373 6167 6573 2061 6e64 2066 696c 6573  ssages and files
 00000070: 2075 7369 6e67 2061 2054 656c 6567 7261   using a Telegra
 00000080: 6d20 626f 742e 0a48 6f6d 652d 7061 6765  m bot..Home-page
 00000090: 3a20 6874 7470 733a 2f2f 7079 7069 2e6f  : https://pypi.o
 000000a0: 7267 2f70 726f 6a65 6374 2f74 656c 6567  rg/project/teleg
 000000b0: 7261 6d2d 626f 742d 7265 706f 7274 6572  ram-bot-reporter
 000000c0: 2f0a 4c69 6365 6e73 653a 204d 4954 0a41  /.License: MIT.A
 000000d0: 7574 686f 723a 2064 6573 6b65 6e74 0a41  uthor: deskent.A
 000000e0: 7574 686f 722d 656d 6169 6c3a 2062 6174  uthor-email: bat
 000000f0: 7465 6e65 7463 697a 4067 6d61 696c 2e63  tenetciz@gmail.c
 00000100: 6f6d 0a52 6571 7569 7265 732d 5079 7468  om.Requires-Pyth
-00000110: 6f6e 3a20 3e3d 332e 3131 2c3c 342e 300a  on: >=3.11,<4.0.
+00000110: 6f6e 3a20 3e3d 332e 3130 2c3c 342e 300a  on: >=3.10,<4.0.
 00000120: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
 00000130: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
 00000140: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
 00000150: 7365 0a43 6c61 7373 6966 6965 723a 2050  se.Classifier: P
 00000160: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
 00000170: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
 00000180: 2033 0a43 6c61 7373 6966 6965 723a 2050   3.Classifier: P
 00000190: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
 000001a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000001b0: 2033 2e31 310a 436c 6173 7369 6669 6572   3.11.Classifier
+000001b0: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
 000001c0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
 000001d0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000001e0: 203a 3a20 332e 3132 0a52 6571 7569 7265   :: 3.12.Require
-000001f0: 732d 4469 7374 3a20 6e69 7175 6573 7473  s-Dist: niquests
-00000200: 2028 3e3d 332e 352e 352c 3c34 2e30 2e30   (>=3.5.5,<4.0.0
-00000210: 290a 5072 6f6a 6563 742d 5552 4c3a 2052  ).Project-URL: R
-00000220: 6570 6f73 6974 6f72 792c 2068 7474 7073  epository, https
-00000230: 3a2f 2f67 6974 6875 622e 636f 6d2f 4465  ://github.com/De
-00000240: 736b 656e 742f 626f 745f 7265 706f 7274  skent/bot_report
-00000250: 6572 0a44 6573 6372 6970 7469 6f6e 2d43  er.Description-C
-00000260: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000270: 742f 6d61 726b 646f 776e 0a0a 2323 2320  t/markdown..### 
-00000280: 496e 7374 616c 6c61 7469 6f6e 0a0a 2020  Installation..  
-00000290: 2020 7069 7020 696e 7374 616c 6c20 7465    pip install te
-000002a0: 6c65 6772 616d 2d62 6f74 2d72 6570 6f72  legram-bot-repor
-000002b0: 7465 720a 0a23 2323 2055 7361 6765 2053  ter..### Usage S
-000002c0: 796e 630a 0a20 2020 2066 726f 6d20 7465  ync..    from te
-000002d0: 6c65 6772 616d 5f62 6f74 5f72 6570 6f72  legram_bot_repor
-000002e0: 7465 7220 696d 706f 7274 2042 6f74 0a0a  ter import Bot..
-000002f0: 2020 2020 626f 7420 3d20 426f 7428 626f      bot = Bot(bo
-00000300: 745f 746f 6b65 6e3d 5445 4c45 424f 545f  t_token=TELEBOT_
-00000310: 544f 4b45 4e2c 2063 6861 745f 6964 3d43  TOKEN, chat_id=C
-00000320: 4841 545f 4944 290a 0a20 2020 2023 2053  HAT_ID)..    # S
-00000330: 656e 6420 6d65 7373 6167 650a 2020 2020  end message.    
-00000340: 626f 742e 7365 6e64 5f6d 6573 7361 6765  bot.send_message
-00000350: 2827 4865 6c6c 6f2c 2077 6f72 6c64 2729  ('Hello, world')
-00000360: 0a0a 2020 2020 2320 5365 6e64 2066 696c  ..    # Send fil
-00000370: 650a 2020 2020 7465 6d70 5f66 696c 6520  e.    temp_file 
-00000380: 3d20 5061 7468 2827 7465 7374 2e74 7874  = Path('test.txt
-00000390: 2729 0a20 2020 2077 6974 6820 6f70 656e  ').    with open
-000003a0: 2874 656d 705f 6669 6c65 2c20 6d6f 6465  (temp_file, mode
-000003b0: 3d27 7727 2c20 656e 636f 6469 6e67 3d27  ='w', encoding='
-000003c0: 7574 662d 3827 2920 6173 2066 3a0a 2020  utf-8') as f:.  
-000003d0: 2020 2020 2020 662e 7772 6974 6528 2754        f.write('T
-000003e0: 6573 7420 6d65 7373 6167 6527 290a 2020  est message').  
-000003f0: 2020 626f 742e 7365 6e64 5f64 6f63 756d    bot.send_docum
-00000400: 656e 7428 7465 6d70 5f66 696c 6529 0a0a  ent(temp_file)..
-00000410: 2020 2020 2320 5365 6e64 206c 6f6e 6720      # Send long 
-00000420: 6d65 7373 6167 6520 286d 6f72 6520 7468  message (more th
-00000430: 616e 2034 3030 3020 7379 6d62 6f6c 7329  an 4000 symbols)
-00000440: 0a20 2020 2062 6f74 2e73 656e 645f 6d65  .    bot.send_me
-00000450: 7373 6167 6528 2756 6572 7920 6c6f 6e67  ssage('Very long
-00000460: 206d 6573 7361 6765 206f 7665 7220 3430   message over 40
-00000470: 3030 2073 796d 626f 6c73 272c 2073 706c  00 symbols', spl
-00000480: 6974 5f6d 6573 7361 6765 3d54 7275 6529  it_message=True)
-00000490: 0a0a 2323 2320 5573 6167 6520 4173 796e  ..### Usage Asyn
-000004a0: 630a 0a20 2020 2066 726f 6d20 7465 6c65  c..    from tele
-000004b0: 6772 616d 5f62 6f74 5f72 6570 6f72 7465  gram_bot_reporte
-000004c0: 7220 696d 706f 7274 2041 7379 6e63 426f  r import AsyncBo
-000004d0: 740a 0a20 2020 2062 6f74 203d 2041 7379  t..    bot = Asy
-000004e0: 6e63 426f 7428 626f 745f 746f 6b65 6e3d  ncBot(bot_token=
-000004f0: 5445 4c45 424f 545f 544f 4b45 4e2c 2063  TELEBOT_TOKEN, c
-00000500: 6861 745f 6964 3d43 4841 545f 4944 290a  hat_id=CHAT_ID).
-00000510: 0a20 2020 2061 7761 6974 2062 6f74 2e73  .    await bot.s
-00000520: 656e 645f 6d65 7373 6167 6528 2748 656c  end_message('Hel
-00000530: 6c6f 2c20 776f 726c 6427 290a 0a20 2020  lo, world')..   
-00000540: 2023 2053 656e 6420 6669 6c65 0a20 2020   # Send file.   
-00000550: 2074 656d 705f 6669 6c65 203d 2050 6174   temp_file = Pat
-00000560: 6828 2774 6573 742e 7478 7427 290a 2020  h('test.txt').  
-00000570: 2020 7769 7468 206f 7065 6e28 7465 6d70    with open(temp
-00000580: 5f66 696c 652c 206d 6f64 653d 2777 272c  _file, mode='w',
-00000590: 2065 6e63 6f64 696e 673d 2775 7466 2d38   encoding='utf-8
-000005a0: 2729 2061 7320 663a 0a20 2020 2020 2020  ') as f:.       
-000005b0: 2066 2e77 7269 7465 2827 5465 7374 206d   f.write('Test m
-000005c0: 6573 7361 6765 2729 0a20 2020 2061 7761  essage').    awa
-000005d0: 6974 2062 6f74 2e73 656e 645f 646f 6375  it bot.send_docu
-000005e0: 6d65 6e74 2874 656d 705f 6669 6c65 290a  ment(temp_file).
-000005f0: 0a20 2020 2023 2053 656e 6420 6c6f 6e67  .    # Send long
-00000600: 206d 6573 7361 6765 2028 6d6f 7265 2074   message (more t
-00000610: 6861 6e20 3430 3030 2073 796d 626f 6c73  han 4000 symbols
-00000620: 290a 2020 2020 6177 6169 7420 626f 742e  ).    await bot.
-00000630: 7365 6e64 5f6d 6573 7361 6765 2827 5665  send_message('Ve
-00000640: 7279 206c 6f6e 6720 6d65 7373 6167 6520  ry long message 
-00000650: 6f76 6572 2034 3030 3020 7379 6d62 6f6c  over 4000 symbol
-00000660: 7327 2c20 7370 6c69 745f 6d65 7373 6167  s', split_messag
-00000670: 653d 5472 7565 290a 0a                   e=True)..
+000001e0: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
+000001f0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000200: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000210: 686f 6e20 3a3a 2033 2e31 320a 5265 7175  hon :: 3.12.Requ
+00000220: 6972 6573 2d44 6973 743a 206e 6971 7565  ires-Dist: nique
+00000230: 7374 7320 283e 3d33 2e35 2e35 2c3c 342e  sts (>=3.5.5,<4.
+00000240: 302e 3029 0a50 726f 6a65 6374 2d55 524c  0.0).Project-URL
+00000250: 3a20 5265 706f 7369 746f 7279 2c20 6874  : Repository, ht
+00000260: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000270: 2f44 6573 6b65 6e74 2f62 6f74 5f72 6570  /Deskent/bot_rep
+00000280: 6f72 7465 720a 4465 7363 7269 7074 696f  orter.Descriptio
+00000290: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+000002a0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
+000002b0: 2323 2053 7461 636b 3a0a 0a2d 205b 785d  ## Stack:..- [x]
+000002c0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000002d0: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
+000002e0: 2f22 3e3c 696d 6720 7372 633d 2268 7474  /"><img src="htt
+000002f0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000300: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f64  sercontent.com/d
+00000310: 6576 6963 6f6e 732f 6465 7669 636f 6e2f  evicons/devicon/
+00000320: 6d61 7374 6572 2f69 636f 6e73 2f70 7974  master/icons/pyt
+00000330: 686f 6e2f 7079 7468 6f6e 2d70 6c61 696e  hon/python-plain
+00000340: 2e73 7667 2220 616c 743d 2270 7974 686f  .svg" alt="pytho
+00000350: 6e22 2077 6964 7468 3d22 3135 2220 6865  n" width="15" he
+00000360: 6967 6874 3d22 3135 222f 3e0a 2020 5079  ight="15"/>.  Py
+00000370: 7468 6f6e 2033 2e31 302b 203c 6272 2f3e  thon 3.10+ <br/>
+00000380: 3c2f 613e 0a2d 205b 785d 203c 6120 6872  </a>.- [x] <a hr
+00000390: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000003a0: 7562 2e63 6f6d 2f6a 6177 6168 2f6e 6971  ub.com/jawah/niq
+000003b0: 7565 7374 7322 3e3c 696d 6720 7372 633d  uests"><img src=
+000003c0: 2268 7474 7073 3a2f 2f75 7365 722d 696d  "https://user-im
+000003d0: 6167 6573 2e67 6974 6875 6275 7365 7263  ages.githubuserc
+000003e0: 6f6e 7465 6e74 2e63 6f6d 2f39 3332 3637  ontent.com/93267
+000003f0: 3030 2f32 3832 3835 3231 3338 2d31 3630  00/282852138-160
+00000400: 6633 3265 392d 6536 6366 2d34 3935 662d  f32e9-e6cf-495f-
+00000410: 6233 3964 2d39 3938 3931 3630 3261 6366  b39d-99891602acf
+00000420: 392e 706e 6722 2061 6c74 3d22 6e69 7175  9.png" alt="niqu
+00000430: 6573 7473 2220 7769 6474 683d 2231 3522  ests" width="15"
+00000440: 2068 6569 6768 743d 2231 3522 2f3e 0a20   height="15"/>. 
+00000450: 204e 6971 7565 7374 7320 332e 352e 352b   Niquests 3.5.5+
+00000460: 203c 6272 2f3e 0a0a 2323 2320 496e 7374   <br/>..### Inst
+00000470: 616c 6c61 7469 6f6e 0a0a 2020 2020 7069  allation..    pi
+00000480: 7020 696e 7374 616c 6c20 7465 6c65 6772  p install telegr
+00000490: 616d 2d62 6f74 2d72 6570 6f72 7465 720a  am-bot-reporter.
+000004a0: 0a23 2323 2055 7361 6765 2053 796e 630a  .### Usage Sync.
+000004b0: 0a20 2020 2066 726f 6d20 7465 6c65 6772  .    from telegr
+000004c0: 616d 5f62 6f74 5f72 6570 6f72 7465 7220  am_bot_reporter 
+000004d0: 696d 706f 7274 2042 6f74 0a0a 2020 2020  import Bot..    
+000004e0: 626f 7420 3d20 426f 7428 626f 745f 746f  bot = Bot(bot_to
+000004f0: 6b65 6e3d 5445 4c45 424f 545f 544f 4b45  ken=TELEBOT_TOKE
+00000500: 4e2c 2063 6861 745f 6964 3d43 4841 545f  N, chat_id=CHAT_
+00000510: 4944 290a 0a20 2020 2023 2053 656e 6420  ID)..    # Send 
+00000520: 6d65 7373 6167 650a 2020 2020 626f 742e  message.    bot.
+00000530: 7365 6e64 5f6d 6573 7361 6765 2827 4865  send_message('He
+00000540: 6c6c 6f2c 2077 6f72 6c64 2729 0a0a 2020  llo, world')..  
+00000550: 2020 2320 5365 6e64 2066 696c 650a 2020    # Send file.  
+00000560: 2020 7465 6d70 5f66 696c 6520 3d20 5061    temp_file = Pa
+00000570: 7468 2827 7465 7374 2e74 7874 2729 0a20  th('test.txt'). 
+00000580: 2020 2077 6974 6820 6f70 656e 2874 656d     with open(tem
+00000590: 705f 6669 6c65 2c20 6d6f 6465 3d27 7727  p_file, mode='w'
+000005a0: 2c20 656e 636f 6469 6e67 3d27 7574 662d  , encoding='utf-
+000005b0: 3827 2920 6173 2066 3a0a 2020 2020 2020  8') as f:.      
+000005c0: 2020 662e 7772 6974 6528 2754 6573 7420    f.write('Test 
+000005d0: 6d65 7373 6167 6527 290a 2020 2020 626f  message').    bo
+000005e0: 742e 7365 6e64 5f64 6f63 756d 656e 7428  t.send_document(
+000005f0: 7465 6d70 5f66 696c 6529 0a0a 2020 2020  temp_file)..    
+00000600: 2320 5365 6e64 206c 6f6e 6720 6d65 7373  # Send long mess
+00000610: 6167 6520 286d 6f72 6520 7468 616e 2034  age (more than 4
+00000620: 3030 3020 7379 6d62 6f6c 7329 0a20 2020  000 symbols).   
+00000630: 2062 6f74 2e73 656e 645f 6d65 7373 6167   bot.send_messag
+00000640: 6528 2756 6572 7920 6c6f 6e67 206d 6573  e('Very long mes
+00000650: 7361 6765 206f 7665 7220 3430 3030 2073  sage over 4000 s
+00000660: 796d 626f 6c73 272c 2073 706c 6974 5f6d  ymbols', split_m
+00000670: 6573 7361 6765 3d54 7275 6529 0a0a 2323  essage=True)..##
+00000680: 2320 5573 6167 6520 4173 796e 630a 0a20  # Usage Async.. 
+00000690: 2020 2066 726f 6d20 7465 6c65 6772 616d     from telegram
+000006a0: 5f62 6f74 5f72 6570 6f72 7465 7220 696d  _bot_reporter im
+000006b0: 706f 7274 2041 7379 6e63 426f 740a 0a20  port AsyncBot.. 
+000006c0: 2020 2062 6f74 203d 2041 7379 6e63 426f     bot = AsyncBo
+000006d0: 7428 626f 745f 746f 6b65 6e3d 5445 4c45  t(bot_token=TELE
+000006e0: 424f 545f 544f 4b45 4e2c 2063 6861 745f  BOT_TOKEN, chat_
+000006f0: 6964 3d43 4841 545f 4944 290a 0a20 2020  id=CHAT_ID)..   
+00000700: 2061 7761 6974 2062 6f74 2e73 656e 645f   await bot.send_
+00000710: 6d65 7373 6167 6528 2748 656c 6c6f 2c20  message('Hello, 
+00000720: 776f 726c 6427 290a 0a20 2020 2023 2053  world')..    # S
+00000730: 656e 6420 6669 6c65 0a20 2020 2074 656d  end file.    tem
+00000740: 705f 6669 6c65 203d 2050 6174 6828 2774  p_file = Path('t
+00000750: 6573 742e 7478 7427 290a 2020 2020 7769  est.txt').    wi
+00000760: 7468 206f 7065 6e28 7465 6d70 5f66 696c  th open(temp_fil
+00000770: 652c 206d 6f64 653d 2777 272c 2065 6e63  e, mode='w', enc
+00000780: 6f64 696e 673d 2775 7466 2d38 2729 2061  oding='utf-8') a
+00000790: 7320 663a 0a20 2020 2020 2020 2066 2e77  s f:.        f.w
+000007a0: 7269 7465 2827 5465 7374 206d 6573 7361  rite('Test messa
+000007b0: 6765 2729 0a20 2020 2061 7761 6974 2062  ge').    await b
+000007c0: 6f74 2e73 656e 645f 646f 6375 6d65 6e74  ot.send_document
+000007d0: 2874 656d 705f 6669 6c65 290a 0a20 2020  (temp_file)..   
+000007e0: 2023 2053 656e 6420 6c6f 6e67 206d 6573   # Send long mes
+000007f0: 7361 6765 2028 6d6f 7265 2074 6861 6e20  sage (more than 
+00000800: 3430 3030 2073 796d 626f 6c73 290a 2020  4000 symbols).  
+00000810: 2020 6177 6169 7420 626f 742e 7365 6e64    await bot.send
+00000820: 5f6d 6573 7361 6765 2827 5665 7279 206c  _message('Very l
+00000830: 6f6e 6720 6d65 7373 6167 6520 6f76 6572  ong message over
+00000840: 2034 3030 3020 7379 6d62 6f6c 7327 2c20   4000 symbols', 
+00000850: 7370 6c69 745f 6d65 7373 6167 653d 5472  split_message=Tr
+00000860: 7565 290a 0a                             ue)..
```

