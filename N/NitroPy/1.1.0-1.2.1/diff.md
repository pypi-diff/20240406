# Comparing `tmp/NitroPy-1.1.0.tar.gz` & `tmp/NitroPy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NitroPy-1.1.0.tar", last modified: Tue Apr  2 16:08:10 2024, max compression
+gzip compressed data, was "NitroPy-1.2.1.tar", last modified: Fri Apr  5 21:25:38 2024, max compression
```

## Comparing `NitroPy-1.1.0.tar` & `NitroPy-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 16:08:10.042399 NitroPy-1.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-02 16:08:10.033915 NitroPy-1.1.0/NitroPy.egg-info/
--rw-rw-rw-   0        0        0      384 2024-04-02 16:08:07.000000 NitroPy-1.1.0/NitroPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-02 16:08:07.000000 NitroPy-1.1.0/NitroPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 16:08:07.000000 NitroPy-1.1.0/NitroPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-02 16:08:07.000000 NitroPy-1.1.0/NitroPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-02 16:08:07.000000 NitroPy-1.1.0/NitroPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      384 2024-04-02 16:08:10.040384 NitroPy-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-23 07:14:07.000000 NitroPy-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 16:08:10.038137 NitroPy-1.1.0/nitrotype/
--rw-rw-rw-   0        0        0       27 2024-04-02 16:03:12.000000 NitroPy-1.1.0/nitrotype/__init__.py
--rw-rw-rw-   0        0        0     2319 2024-04-02 16:03:12.000000 NitroPy-1.1.0/nitrotype/_nitrotype.py
--rw-rw-rw-   0        0        0       42 2024-04-02 16:08:10.046193 NitroPy-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      757 2024-04-02 16:06:06.000000 NitroPy-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:25:38.095192 NitroPy-1.2.1/
+drwxrwxrwx   0        0        0        0 2024-04-05 21:25:38.046462 NitroPy-1.2.1/NitroPy.egg-info/
+-rw-rw-rw-   0        0        0     5693 2024-04-05 21:25:32.000000 NitroPy-1.2.1/NitroPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-05 21:25:32.000000 NitroPy-1.2.1/NitroPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 21:25:32.000000 NitroPy-1.2.1/NitroPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-05 21:25:32.000000 NitroPy-1.2.1/NitroPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 21:25:32.000000 NitroPy-1.2.1/NitroPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5693 2024-04-05 21:25:38.095192 NitroPy-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5270 2024-04-04 07:59:57.000000 NitroPy-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 21:25:38.091672 NitroPy-1.2.1/nitrotype/
+-rw-rw-rw-   0        0        0      187 2024-04-05 19:58:00.000000 NitroPy-1.2.1/nitrotype/__init__.py
+-rw-rw-rw-   0        0        0      902 2024-04-04 07:39:05.000000 NitroPy-1.2.1/nitrotype/_news.py
+-rw-rw-rw-   0        0        0    14224 2024-04-04 07:32:14.000000 NitroPy-1.2.1/nitrotype/_nitromath.py
+-rw-rw-rw-   0        0        0     2638 2024-04-05 15:58:54.000000 NitroPy-1.2.1/nitrotype/_nitromathteam.py
+-rw-rw-rw-   0        0        0     2289 2024-04-04 02:06:45.000000 NitroPy-1.2.1/nitrotype/_nitrotype.py
+-rw-rw-rw-   0        0        0     2638 2024-04-04 07:42:18.000000 NitroPy-1.2.1/nitrotype/_nitrotypeteam.py
+-rw-rw-rw-   0        0        0       42 2024-04-05 21:25:38.103218 NitroPy-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      858 2024-04-05 21:08:04.000000 NitroPy-1.2.1/setup.py
```

### Comparing `NitroPy-1.1.0/nitrotype/_nitrotype.py` & `NitroPy-1.2.1/nitrotype/_nitrotype.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,25 @@
     def __init__(self, username):
         self.username = username
         self._scraper = cloudscraper.create_scraper()
         self._racer_info = self._get_user_info()
         self._initialize_attributes()
 
     def _get_user_info(self):
-        response = self._scraper.get(f'https://www.nitromath.com/racer/{self.username}').text
+        response = self._scraper.get(f'https://www.nitrotype.com/racer/{self.username}').text
         soup = BeautifulSoup(response, 'html.parser')
 
         racer_info = {}
         for script in soup.find_all('script'):
             if 'RACER_INFO' in str(script):
                 racer_info = json.loads(re.findall('{".+}', str(script))[0])
                 return racer_info
 
         return None
+        
 
     def _initialize_attributes(self):
         # Initialize attributes
         racer_info = self._racer_info
         self.userID = racer_info['userID']
         self.username = racer_info['username']
         self.membership = racer_info['membership']
@@ -37,25 +38,26 @@
         self.title = racer_info['title']
         self.experience = racer_info['experience']
         self.level = racer_info['level']
         self.teamID = racer_info['teamID']
         self.lookingForTeam = racer_info['lookingForTeam']
         self.carID = racer_info['carID']
         self.carHueAngle = racer_info['carHueAngle']
-        self.totalCars = racer_info['totalCars']
+        self.totalCars = len(racer_info['garage'])
         self.nitros = racer_info['nitros']
         self.nitrosUsed = racer_info['nitrosUsed']
         self.racesPlayed = racer_info['racesPlayed']
         self.longestSession = racer_info['longestSession']
         self.avgSpeed = racer_info['avgSpeed']
         self.highestSpeed = racer_info['highestSpeed']
         self.allowFriendRequests = racer_info['allowFriendRequests']
         self.profileViews = racer_info['profileViews']
         self.createdStamp = racer_info['createdStamp']
         self.tag = racer_info['tag']
         self.tagColor = racer_info['tagColor']
-        self.garage = racer_info['garage']
+
+
 
     def __getattr__(self, attr):
         if attr in self._racer_info:
             return self._racer_info[attr]
-        raise AttributeError(f"'NitrotypeRacer' object has no attribute '{attr}'")
+        raise AttributeError(f"'NitrotypeRacer' object has no attribute '{attr}'")
```

