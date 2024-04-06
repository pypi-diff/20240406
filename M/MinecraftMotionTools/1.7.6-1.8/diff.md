# Comparing `tmp/MinecraftMotionTools-1.7.6.tar.gz` & `tmp/MinecraftMotionTools-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MinecraftMotionTools-1.7.6.tar", last modified: Mon Apr  1 14:55:01 2024, max compression
+gzip compressed data, was "MinecraftMotionTools-1.8.tar", last modified: Sat Apr  6 11:03:05 2024, max compression
```

## Comparing `MinecraftMotionTools-1.7.6.tar` & `MinecraftMotionTools-1.8.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-01 14:55:01.740114 MinecraftMotionTools-1.7.6/
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     1083 2024-04-01 14:50:13.000000 MinecraftMotionTools-1.7.6/LICENSE
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     5406 2024-04-01 14:55:01.732113 MinecraftMotionTools-1.7.6/PKG-INFO
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     5083 2024-04-01 14:53:59.000000 MinecraftMotionTools-1.7.6/README.md
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      481 2024-04-01 14:51:52.000000 MinecraftMotionTools-1.7.6/pyproject.toml
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       38 2024-04-01 14:55:01.740694 MinecraftMotionTools-1.7.6/setup.cfg
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-01 14:55:01.592615 MinecraftMotionTools-1.7.6/src/
-drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-01 14:55:01.721433 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     5406 2024-04-01 14:55:01.000000 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/PKG-INFO
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      301 2024-04-01 14:55:01.000000 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/SOURCES.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        1 2024-04-01 14:55:01.000000 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/dependency_links.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       14 2024-04-01 14:55:01.000000 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/requires.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       23 2024-04-01 14:55:01.000000 MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/top_level.txt
--rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    10267 2024-04-01 14:50:13.000000 MinecraftMotionTools-1.7.6/src/minecraft_motion_tools.py
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-06 11:03:05.957154 MinecraftMotionTools-1.8/
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     1083 2024-04-06 09:11:02.000000 MinecraftMotionTools-1.8/LICENSE
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6887 2024-04-06 11:03:05.948627 MinecraftMotionTools-1.8/PKG-INFO
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6581 2024-04-06 10:19:59.000000 MinecraftMotionTools-1.8/README.md
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      479 2024-04-06 11:01:23.000000 MinecraftMotionTools-1.8/pyproject.toml
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       38 2024-04-06 11:03:05.958722 MinecraftMotionTools-1.8/setup.cfg
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-06 11:03:05.665670 MinecraftMotionTools-1.8/src/
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-06 11:03:05.935523 MinecraftMotionTools-1.8/src/MinecraftMotionTools.egg-info/
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)     6887 2024-04-06 11:03:05.000000 MinecraftMotionTools-1.8/src/MinecraftMotionTools.egg-info/PKG-INFO
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      392 2024-04-06 11:03:05.000000 MinecraftMotionTools-1.8/src/MinecraftMotionTools.egg-info/SOURCES.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        1 2024-04-06 11:03:05.000000 MinecraftMotionTools-1.8/src/MinecraftMotionTools.egg-info/dependency_links.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       14 2024-04-06 11:03:05.000000 MinecraftMotionTools-1.8/src/MinecraftMotionTools.egg-info/requires.txt
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)       23 2024-04-06 11:03:05.000000 MinecraftMotionTools-1.8/src/MinecraftMotionTools.egg-info/top_level.txt
+drwxrwxrwx   0 orhy3     (1000) orhy3     (1000)        0 2024-04-06 11:03:05.900267 MinecraftMotionTools-1.8/src/minecraft_motion_tools/
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)      669 2024-04-06 09:17:42.000000 MinecraftMotionTools-1.8/src/minecraft_motion_tools/__init__.py
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    12034 2024-04-06 10:15:19.000000 MinecraftMotionTools-1.8/src/minecraft_motion_tools/acceleration.py
+-rwxrwxrwx   0 orhy3     (1000) orhy3     (1000)    10267 2024-04-06 09:11:02.000000 MinecraftMotionTools-1.8/src/minecraft_motion_tools/velocity.py
```

### Comparing `MinecraftMotionTools-1.7.6/LICENSE` & `MinecraftMotionTools-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `MinecraftMotionTools-1.7.6/PKG-INFO` & `MinecraftMotionTools-1.8/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,91 @@
-Metadata-Version: 2.1
-Name: MinecraftMotionTools
-Version: 1.7.6
-Summary: A library to compute entities' motion in Minecraft.
-Author: OrHy3
-Project-URL: Homepage, https://github.com/OrHy3/MinecraftMotionTools
-Project-URL: Issues, https://github.com/OrHy3/MinecraftMotionTools/issues
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: scipy>=1.12.0
-
-# MinecraftMotionTools
-MinecraftMotionTools is a collection of functions whose purpose is to ease prediction of the velocity and the position of entities simulated into Minecraft.
-# How does it work?
-Minecraft updates velocity in a different way from real-physics objects, plus it complicates everything just by being a video game and having to update the values in a finite unit of time (the tick).
-
-Minecraft's Wiki got [some information](https://minecraft.wiki/w/Entity#Motion_of_entities) about how it works, but [here](https://hackmd.io/ySiQhr_SSUatNc6qAkbFcw) is the reasoning behind the velocity equations.
-
-Another complication comes from what I, in the code, refer to as [acceleration drag](https://minecraft.wiki/w/Entity#cite_note-gravityBefore-4), which initially required forking the formulas for every different case (see [old sheet](https://hackmd.io/V9oMODQbT5mBA-o4OM76pA)), before I decided to generalize the formulas, introducing the coefficient `k`.
-
-Acceleration drag works the following way:
-
-$\text{position}\_{new}=\text{position}_{old}+\text{velocity}-k\cdot\text{acceleration}$
-
-Finally, [here](https://hackmd.io/1t0ACyplTDKSgo-a1jA7nQ) is the formulas' sheet I wrote down. Take in mind that a fair amount of them make use of [Lambert's W function](https://en.wikipedia.org/wiki/Lambert_W_function).
-# Entities' parameter table
-|Type|Acceleration|Vertical drag|Horizontal drag|Applies drag|k coefficient|
-|-|-|-|-|-|-|
-|Players, mobs and armor stands|0.08|0.019999980926513672|0.0899999737739563|After|0|
-|Entities with slow falling|0.01|0.019999980926513672|0.0899999737739563|After|0|
-|Items, falling blocks and TNTs|0.04|0.02|0.02|After|1|
-|Minecarts|0.04|0.05|0.05|After|1|
-|Boats|0.03999999910593033|0|0.10000002384185791|-|1|
-|Thrown eggs, snowballs and ender pearls|0.029999999329447746|0.009999990463256836|0.009999990463256836|Before|0|
-|Thrown potions|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
-|Thrown experience bottles|0.07000000029802322|0.009999990463256836|0.009999990463256836|Before|0|
-|Experience orbs|0.03|0.02|0.019999980926513672|After|1|
-|Thrown fishing bobbers|0.03|0.08|0.08|After|1|
-|Llama spit|0.05999999865889549|0.009999990463256836|0.009999990463256836|Before|0|
-|Fired arrows and thrown tridents|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
-|Fireballs, wither skulls and dragon fireballs|0.1|0.050000011920928955|0.050000011920928955|After|0|
-|Dangerous wither skulls|0.1|0.26999998092651367|0.26999998092651367|After|0|
-|Wind charges|0.1|0|0|-|0|
-
-NOTES:
-- For fireballs and alike, use negative acceleration (see [here](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0) why).
-- Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.45399993658065796.
-- The maximum general velocity value is 10. Any greater value is reset to 0.
-- Minecarts have a maximum horizontal velocity of 0.4. Any greater value is reset to that number.
-- Boats' horizontal position gets updated using next tick's velocity instead of the current one.
-# Function list
-v0: initial velocity<br>
-t: ticks passed<br>
-v: current velocity<br>
-p: current relative position<br>
-h: maximum height<br>
-a: acceleration<br>
-d: drag force<br>
-after: whether drag is applied after or before gravity acceleration<br>
-k: acceleration drag coefficient<br>
-|Name|Required arguments|Optional arguments|Brief description|
-|-|-|-|-|
-|v_from_t|v0, t|a, d, after|Retrieves velocity from an initial velocity and the time that has passed, in ticks.|
-|p_from_t|v0, t|a, d, after, k|Retrieves relative position from an initial velocity and the time that has passed, in ticks.|
-|max_height_tick_from_v0|v0|a, d, after, k|Retrieves the time in ticks the maximum relative height is reached.|
-|max_height_from_v0|v0|a, d, after, k|Retrieves the maximum relative height reached (using integer approximation of the tick).|
-|v0_from_max_height|h|a, d, after, k|Retrieves a tuple of up to 2 solutions, each one belonging to the possible arcs with the specified height.|
-|v0_from_v_t|v, t|a, d, after|Retrieves initial velocity from a pair of current velocity and time passed, in ticks.|
-|v0_from_p_t|p, t|a, d, after, k|Retrieves initial velocity from a pair of current relative position and time passed, in ticks.|
-|t_from_v0_v|v0, v|a, d, after|Retrieves the time passed (in ticks) since velocity was v0 to become v.|
-|t_from_v0_p|v0, p|a, d, after, k|Retrieves the time passed (in ticks) to reach the relative position specified.|
-|v0_t_from_v_p|v, p|a, d, after, k|Retrieves a pair of initial velocity and time passed (in ticks) to reach the state of current velocity/position specified.|
-# How to install?
-Install Python 3 and pip, then run
-```
-pip install MinecraftMotionTools
-```
-To update the package to its latest version run
-```
-pip install --upgrade MinecraftMotionTools
-```
-# How to use?
-Check some of the code examples for common uses.
-
-Functions' parameters are set to Falling Blocks by default.
+# MinecraftMotionTools
+MinecraftMotionTools is a collection of functions whose purpose is to ease prediction of the velocity and the position of entities simulated into Minecraft.
+# How does it work?
+Minecraft updates velocity in a different way from real-physics objects, plus it complicates everything just by being a video game and having to update the values in a finite unit of time (the tick).
+
+Minecraft's Wiki got [some information](https://minecraft.wiki/w/Entity#Motion_of_entities) about how it works, but [here](https://hackmd.io/ySiQhr_SSUatNc6qAkbFcw) is the reasoning behind the velocity equations.
+
+Another complication comes from what I, in the code, refer to as [acceleration drag](https://minecraft.wiki/w/Entity#cite_note-gravityBefore-4), which initially required forking the formulas for every different case (see [old sheet](https://hackmd.io/V9oMODQbT5mBA-o4OM76pA)), before I decided to generalize the formulas, introducing the coefficient `k`.
+
+Acceleration drag works the following way:
+
+$\text{position}\_{new}=\text{position}_{old}+\text{velocity}-k\cdot\text{acceleration}$
+
+Finally, [here](https://hackmd.io/1t0ACyplTDKSgo-a1jA7nQ) is the formulas' sheet I wrote down. Take in mind that a fair amount of them make use of [Lambert's W function](https://en.wikipedia.org/wiki/Lambert_W_function).
+
+For the acceleration's formulas refer to [this sheet](https://hackmd.io/vvFAdzekSn6R7vc9Mw8lxg?view) instead.
+# Entities' parameter table
+|Type|Acceleration|Vertical drag|Horizontal drag|Applies drag|k coefficient|
+|-|-|-|-|-|-|
+|Players, mobs and armor stands|0.08|0.019999980926513672|0.0899999737739563|After|0|
+|Entities with slow falling|0.01|0.019999980926513672|0.0899999737739563|After|0|
+|Items, falling blocks and TNTs|0.04|0.02|0.02|After|1|
+|Minecarts|0.04|0.05|0.05|After|1|
+|Boats|0.03999999910593033|0|0.10000002384185791|-|1|
+|Thrown eggs, snowballs and ender pearls|0.029999999329447746|0.009999990463256836|0.009999990463256836|Before|0|
+|Thrown potions|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
+|Thrown experience bottles|0.07000000029802322|0.009999990463256836|0.009999990463256836|Before|0|
+|Experience orbs|0.03|0.02|0.019999980926513672|After|1|
+|Thrown fishing bobbers|0.03|0.08|0.08|After|1|
+|Llama spit|0.05999999865889549|0.009999990463256836|0.009999990463256836|Before|0|
+|Fired arrows and thrown tridents|0.05000000074505806|0.009999990463256836|0.009999990463256836|Before|0|
+|Fireballs, wither skulls and dragon fireballs|0.1|0.050000011920928955|0.050000011920928955|After|0|
+|Dangerous wither skulls|0.1|0.26999998092651367|0.26999998092651367|After|0|
+|Wind charges|0.1|0|0|-|0|
+
+NOTES:
+- For fireballs and alike, use negative acceleration (see [here](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0) why).
+- Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.45399993658065796.
+- The maximum general velocity value is 10. Any greater value is reset to 0.
+- Even though 10 is the maximum velocity that can be set, entities with 0 drag force can gain infinite velocity due to acceleration.
+- Minecarts have a maximum horizontal velocity of 0.4. Any greater value is reset to that number.
+- Boats' horizontal position gets updated using next tick's velocity instead of the current one.
+# Function list
+v0: initial velocity<br>
+t: ticks passed<br>
+v: current velocity<br>
+p: current relative position<br>
+h: maximum height<br>
+a: acceleration<br>
+d: drag force<br>
+after: whether drag is applied after or before gravity acceleration<br>
+k: acceleration drag coefficient<br>
+
+Default parameters are set to Falling Blocks.<br>
+|Name|Required arguments|Optional arguments|Brief description|
+|-|-|-|-|
+|v_from_t|v0, t|a, d, after|Retrieves velocity from an initial velocity and the time that has passed, in ticks.|
+|p_from_t|v0, t|a, d, after, k|Retrieves relative position from an initial velocity and the time that has passed, in ticks.|
+|max_height_tick_from_v0|v0|a, d, after, k|Retrieves the time in ticks the maximum relative height is reached.|
+|max_height_from_v0|v0|a, d, after, k|Retrieves the maximum relative height reached (using integer approximation of the tick).|
+|v0_from_max_height|h|a, d, after, k|Retrieves a tuple of up to 2 solutions, each one belonging to the possible arcs with the specified height.|
+|v0_from_v_t|v, t|a, d, after|Retrieves initial velocity from a pair of current velocity and time passed, in ticks.|
+|v0_from_p_t|p, t|a, d, after, k|Retrieves initial velocity from a pair of current relative position and time passed, in ticks.|
+|t_from_v0_v|v0, v|a, d, after|Retrieves the time passed (in ticks) since velocity was v0 to become v.|
+|t_from_v0_p|v0, p|a, d, after, k|Retrieves the time passed (in ticks) to reach the relative position specified.|
+|v0_t_from_v_p|v, p|a, d, after, k|Retrieves a pair of initial velocity and time passed (in ticks) to reach the state of current velocity/position specified.|
+### Acceleration related functions
+These functions retrieve the acceleration from 2 state pairs of the wanted trajectory.<br>
+Functions involving a velocity/position state pair are not guaranteed to retrieve all the solutions, though that should be a limit case.<br>
+If drag is set to 0, all the functions will use safe algorithms, meaning iterative approximation algorithms won't be used.
+
+Default parameters are set to Fireballs.<br>
+|Name|Required arguments|Optional arguments|Brief description|
+|-|-|-|-|
+|a_from_double_v_t|(v1, t1), (v2, t2)|d, after|Retrieves acceleration from 2 states of velocity/time.|
+|a_from_double_p_t|(p1, t1), (p2, t2)|d, after, k|Retrieves acceleration from 2 states of position/time.|
+|a_from_double_v_p|(v1, p1), (v2, p2)|d, after, k|Attempts to retrieve the acceleration from 2 states of velocity/position.|
+|a_from_v_t_p_t|(v1, t1), (p2, t2)|d, after, k|Retrieves acceleration from 2 states of velocity/time and position/time.|
+|a_from_v_t_v_p|(v1, t1), (v2, p2)|d, after, k|Attempts to retrieve the acceleration from 2 states of velocity/time and velocity/position.|
+|a_from_p_t_v_p|(p1, t1), (v2, p2)|d, after, k|Attempts to retrieve the acceleration from 2 states of position/time and velocity/position.|
+# How to install?
+Install Python 3 and pip, then run
+```
+pip install MinecraftMotionTools
+```
+To update the package to its latest version run
+```
+pip install --upgrade MinecraftMotionTools
+```
+# How to use?
+Check some of the code examples for common use cases.
```

### Comparing `MinecraftMotionTools-1.7.6/src/MinecraftMotionTools.egg-info/PKG-INFO` & `MinecraftMotionTools-1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MinecraftMotionTools
-Version: 1.7.6
+Version: 1.8
 Summary: A library to compute entities' motion in Minecraft.
 Author: OrHy3
 Project-URL: Homepage, https://github.com/OrHy3/MinecraftMotionTools
 Project-URL: Issues, https://github.com/OrHy3/MinecraftMotionTools/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,14 +20,16 @@
 Another complication comes from what I, in the code, refer to as [acceleration drag](https://minecraft.wiki/w/Entity#cite_note-gravityBefore-4), which initially required forking the formulas for every different case (see [old sheet](https://hackmd.io/V9oMODQbT5mBA-o4OM76pA)), before I decided to generalize the formulas, introducing the coefficient `k`.
 
 Acceleration drag works the following way:
 
 $\text{position}\_{new}=\text{position}_{old}+\text{velocity}-k\cdot\text{acceleration}$
 
 Finally, [here](https://hackmd.io/1t0ACyplTDKSgo-a1jA7nQ) is the formulas' sheet I wrote down. Take in mind that a fair amount of them make use of [Lambert's W function](https://en.wikipedia.org/wiki/Lambert_W_function).
+
+For the acceleration's formulas refer to [this sheet](https://hackmd.io/vvFAdzekSn6R7vc9Mw8lxg?view) instead.
 # Entities' parameter table
 |Type|Acceleration|Vertical drag|Horizontal drag|Applies drag|k coefficient|
 |-|-|-|-|-|-|
 |Players, mobs and armor stands|0.08|0.019999980926513672|0.0899999737739563|After|0|
 |Entities with slow falling|0.01|0.019999980926513672|0.0899999737739563|After|0|
 |Items, falling blocks and TNTs|0.04|0.02|0.02|After|1|
 |Minecarts|0.04|0.05|0.05|After|1|
@@ -43,44 +45,59 @@
 |Dangerous wither skulls|0.1|0.26999998092651367|0.26999998092651367|After|0|
 |Wind charges|0.1|0|0|-|0|
 
 NOTES:
 - For fireballs and alike, use negative acceleration (see [here](https://minecraft.wiki/w/Entity#cite_ref-boom_5-0) why).
 - Players, mobs and armor stands whose OnGround property is set to 1 have an horizontal drag force of 0.45399993658065796.
 - The maximum general velocity value is 10. Any greater value is reset to 0.
+- Even though 10 is the maximum velocity that can be set, entities with 0 drag force can gain infinite velocity due to acceleration.
 - Minecarts have a maximum horizontal velocity of 0.4. Any greater value is reset to that number.
 - Boats' horizontal position gets updated using next tick's velocity instead of the current one.
 # Function list
 v0: initial velocity<br>
 t: ticks passed<br>
 v: current velocity<br>
 p: current relative position<br>
 h: maximum height<br>
 a: acceleration<br>
 d: drag force<br>
 after: whether drag is applied after or before gravity acceleration<br>
 k: acceleration drag coefficient<br>
+
+Default parameters are set to Falling Blocks.<br>
 |Name|Required arguments|Optional arguments|Brief description|
 |-|-|-|-|
 |v_from_t|v0, t|a, d, after|Retrieves velocity from an initial velocity and the time that has passed, in ticks.|
 |p_from_t|v0, t|a, d, after, k|Retrieves relative position from an initial velocity and the time that has passed, in ticks.|
 |max_height_tick_from_v0|v0|a, d, after, k|Retrieves the time in ticks the maximum relative height is reached.|
 |max_height_from_v0|v0|a, d, after, k|Retrieves the maximum relative height reached (using integer approximation of the tick).|
 |v0_from_max_height|h|a, d, after, k|Retrieves a tuple of up to 2 solutions, each one belonging to the possible arcs with the specified height.|
 |v0_from_v_t|v, t|a, d, after|Retrieves initial velocity from a pair of current velocity and time passed, in ticks.|
 |v0_from_p_t|p, t|a, d, after, k|Retrieves initial velocity from a pair of current relative position and time passed, in ticks.|
 |t_from_v0_v|v0, v|a, d, after|Retrieves the time passed (in ticks) since velocity was v0 to become v.|
 |t_from_v0_p|v0, p|a, d, after, k|Retrieves the time passed (in ticks) to reach the relative position specified.|
 |v0_t_from_v_p|v, p|a, d, after, k|Retrieves a pair of initial velocity and time passed (in ticks) to reach the state of current velocity/position specified.|
+### Acceleration related functions
+These functions retrieve the acceleration from 2 state pairs of the wanted trajectory.<br>
+Functions involving a velocity/position state pair are not guaranteed to retrieve all the solutions, though that should be a limit case.<br>
+If drag is set to 0, all the functions will use safe algorithms, meaning iterative approximation algorithms won't be used.
+
+Default parameters are set to Fireballs.<br>
+|Name|Required arguments|Optional arguments|Brief description|
+|-|-|-|-|
+|a_from_double_v_t|(v1, t1), (v2, t2)|d, after|Retrieves acceleration from 2 states of velocity/time.|
+|a_from_double_p_t|(p1, t1), (p2, t2)|d, after, k|Retrieves acceleration from 2 states of position/time.|
+|a_from_double_v_p|(v1, p1), (v2, p2)|d, after, k|Attempts to retrieve the acceleration from 2 states of velocity/position.|
+|a_from_v_t_p_t|(v1, t1), (p2, t2)|d, after, k|Retrieves acceleration from 2 states of velocity/time and position/time.|
+|a_from_v_t_v_p|(v1, t1), (v2, p2)|d, after, k|Attempts to retrieve the acceleration from 2 states of velocity/time and velocity/position.|
+|a_from_p_t_v_p|(p1, t1), (v2, p2)|d, after, k|Attempts to retrieve the acceleration from 2 states of position/time and velocity/position.|
 # How to install?
 Install Python 3 and pip, then run
 ```
 pip install MinecraftMotionTools
 ```
 To update the package to its latest version run
 ```
 pip install --upgrade MinecraftMotionTools
 ```
 # How to use?
-Check some of the code examples for common uses.
-
-Functions' parameters are set to Falling Blocks by default.
+Check some of the code examples for common use cases.
```

### Comparing `MinecraftMotionTools-1.7.6/src/minecraft_motion_tools.py` & `MinecraftMotionTools-1.8/src/minecraft_motion_tools/velocity.py`

 * *Files identical despite different names*

