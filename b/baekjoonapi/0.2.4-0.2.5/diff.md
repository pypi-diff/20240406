# Comparing `tmp/baekjoonapi-0.2.4.tar.gz` & `tmp/baekjoonapi-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baekjoonapi-0.2.4.tar", max compression
+gzip compressed data, was "baekjoonapi-0.2.5.tar", last modified: Sat Apr  6 13:47:33 2024, max compression
```

## Comparing `baekjoonapi-0.2.4.tar` & `baekjoonapi-0.2.5.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      456 2023-04-30 07:05:06.371000 baekjoonapi-0.2.4/LICENSE.md
--rw-r--r--   0        0        0       99 2023-04-30 07:05:06.371000 baekjoonapi-0.2.4/README.md
--rw-r--r--   0        0        0     6091 2023-06-20 06:59:33.139000 baekjoonapi-0.2.4/bojapi/__init__.py
--rw-r--r--   0        0        0      477 2023-06-20 06:59:58.610000 baekjoonapi-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 baekjoonapi-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      456 2024-02-27 03:18:03.808147 baekjoonapi-0.2.5/LICENSE.md
+-rw-r--r--   0        0        0       99 2024-02-27 03:18:03.808147 baekjoonapi-0.2.5/README.md
+-rw-r--r--   0        0        0      493 2024-04-06 13:47:33.314148 baekjoonapi-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5995 2024-04-03 04:35:10.712510 baekjoonapi-0.2.5/src/baekjoonapi/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-03 04:35:10.712510 baekjoonapi-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 baekjoonapi-0.2.5/PKG-INFO
```

### Comparing `baekjoonapi-0.2.4/bojapi/__init__.py` & `baekjoonapi-0.2.5/src/baekjoonapi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         self.unsolved_q = soup.select_one("#u-failed").text
         self.submit_time = soup.select_one("#statics > tbody > tr:nth-child(4) > td").text
         self.status = soup.find('blockquote', {'class': 'no-mathjax'}).text
         self.correct_q = soup.select_one('#u-solved').text
 
 class BaekjoonProb:
     """백준 문제의 정보 클래스 (Baekjoon Problem Information Class)"""
-    def __init__(self, number):
+    def __init__(self, number, url: str = "https://www.acmicpc.net/problem/"):
         """문제의 정보를 가져옵니다 (Get problem information)"""
-        soup = BeautifulSoup(get(f"https://www.acmicpc.net/problem/{number}", headers=__get_user_agent__()).text, "lxml")
+        soup = BeautifulSoup(get(f"{url}{number}", headers=__get_user_agent__()).text, "lxml")
         self.number = number
         self.question = soup.select_one("#problem_description > p").text
         if soup.select_one("#problem_input > p") is not None:
             self.input = soup.select_one("#problem_input > p").text
         else:
             self.input = None
         if soup.select_one("#problem_output > p") is not None:
@@ -95,10 +95,8 @@
         self.reverseRivalCount = int(apire["reverseRivalCount"])
         self.maxStreak = int(apire["maxStreak"])
         self.coins = int(apire["coins"])
         self.stardusts = int(apire["stardusts"])
         self.joinedAt = apire["joinedAt"]
         self.bannedUntil = apire["bannedUntil"]
         self.proUntil = apire["proUntil"]
-        self.rank = int(apire["rank"])
-        self.isRival = apire["isRival"] == 'true'
-        self.isReverseRival = apire["isReversedRival"] == 'true'
+        self.rank = int(apire["rank"])
```

