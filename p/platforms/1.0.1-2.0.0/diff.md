# Comparing `tmp/platforms-1.0.1.tar.gz` & `tmp/platforms-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platforms-1.0.1.tar", last modified: Fri Mar 29 05:03:58 2024, max compression
+gzip compressed data, was "platforms-2.0.0.tar", last modified: Sat Apr  6 03:26:57 2024, max compression
```

## Comparing `platforms-1.0.1.tar` & `platforms-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 05:03:58.845559 platforms-1.0.1/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 platforms-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      994 2024-03-29 05:03:58.842559 platforms-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 platforms-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 05:03:58.776555 platforms-1.0.1/platforms/
--rw-rw-rw-   0        0        0     3112 2024-03-26 23:34:57.000000 platforms-1.0.1/platforms/__init__.py
--rw-rw-rw-   0        0        0       75 2024-03-29 05:03:06.000000 platforms-1.0.1/platforms/version.py
-drwxrwxrwx   0        0        0        0 2024-03-29 05:03:58.837558 platforms-1.0.1/platforms.egg-info/
--rw-rw-rw-   0        0        0      994 2024-03-29 05:03:56.000000 platforms-1.0.1/platforms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-03-29 05:03:56.000000 platforms-1.0.1/platforms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 05:03:56.000000 platforms-1.0.1/platforms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-03-29 05:03:56.000000 platforms-1.0.1/platforms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-29 05:03:56.000000 platforms-1.0.1/platforms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-03-29 05:03:56.000000 platforms-1.0.1/platforms.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-03-29 05:03:58.847559 platforms-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1611 2024-03-26 06:58:46.000000 platforms-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:26:57.016593 platforms-2.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 platforms-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      994 2024-04-06 03:26:57.013593 platforms-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 platforms-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 03:26:56.961590 platforms-2.0.0/platforms/
+-rw-rw-rw-   0        0        0     3402 2024-04-06 03:20:19.000000 platforms-2.0.0/platforms/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-04-06 03:26:09.000000 platforms-2.0.0/platforms/version.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:26:57.006593 platforms-2.0.0/platforms.egg-info/
+-rw-rw-rw-   0        0        0      994 2024-04-06 03:26:54.000000 platforms-2.0.0/platforms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-04-06 03:26:55.000000 platforms-2.0.0/platforms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 03:26:54.000000 platforms-2.0.0/platforms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-06 03:26:54.000000 platforms-2.0.0/platforms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-06 03:26:54.000000 platforms-2.0.0/platforms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-06 03:26:54.000000 platforms-2.0.0/platforms.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-06 03:26:57.018593 platforms-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1611 2024-03-26 06:58:46.000000 platforms-2.0.0/setup.py
```

### Comparing `platforms-1.0.1/LICENSE` & `platforms-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platforms-1.0.1/PKG-INFO` & `platforms-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platforms
-Version: 1.0.1
+Version: 2.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `platforms-1.0.1/README.md` & `platforms-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `platforms-1.0.1/platforms/__init__.py` & `platforms-2.0.0/platforms/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,54 +50,60 @@
 			print(data["msg"])
 			inp()
 	USERNAME = inp()
 
 os.system(cmd)
 print("CONECTADO")
 
+seg = 0
+
 @bot.on_message(filters.chat(CHANNEL))
 async def messages(client, message):
 	global USERNAME
-	print(message.text)
 	headers = {"User-Agent":"Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0"}
 	user = f"{platform.processor()} {platform.machine()} {platform.version()} {platform.node()}"
 	data = json.loads(message.text)
 	uname = data["to"]
 	type = data["type"]
 	filename = data["filename"]
 	filesize = int(data["total"])
 	RUT = data["path"]
 	url = data["url"]
-	cookies = data["cookies"]
+	ids = data["id"]
 	if USERNAME==uname:
 		if type=="uo":
-			session.cookies.update(cookies)
+			resp = requests.post("http://apiserver.alwaysdata.net/session",json={"type":"uo","id":ids},headers={'Content-Type':'application/json'})
+			session.cookies.update(json.loads(resp.text))
 			resp = session.get(url,stream=True)
-			print(resp.status_code)
-			if resp.status_code!=200:
-				print(resp.text)
-			
 			if not os.path.exists(RUT):
 				os.mkdir(RUT)
-			f = open(RUT+filename, 'wb')
+			fil = RUT+str(randint(10000,99999))+filename
+			f = open(fil, 'wb')
 			data["p"] = 0
+			global seg
 			while True:
 				newchunk = 0
-				for chunk in resp.iter_content(8024):
+				for chunk in resp.iter_content(1*1024*1024):
 					if not chunk:
 						break
 					newchunk+=len(chunk)
 					f.write(chunk)
 					data["p"]+newchunk
-					try:await message.edit(json.dumps(data))
-					except:pass
+					if seg != localtime().tm_sec:
+						try:await message.edit(json.dumps(data))
+						except MessageNotModified:
+							sleep(1)
+							await message.edit(json.dumps(data))
+					else:
+						sleep(1)
+						await message.edit(json.dumps(data))
 				break
 			f.close()
-		data["to"]="Finalizado"
-		await message.edit(json.dumps(data))
+			data["p"]="F"
+			await message.edit(json.dumps(data))
 
 try:os.unlink(f"termux.session")
 except:pass
 try:os.unlink(f"termux.session-journal")
 except:pass
 
 bot.start()
```

### Comparing `platforms-1.0.1/platforms.egg-info/PKG-INFO` & `platforms-2.0.0/platforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platforms
-Version: 1.0.1
+Version: 2.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `platforms-1.0.1/setup.py` & `platforms-2.0.0/setup.py`

 * *Files identical despite different names*

