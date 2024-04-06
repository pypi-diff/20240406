# Comparing `tmp/ffxiv_stats-0.4.1.tar.gz` & `tmp/ffxiv_stats-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffxiv_stats-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ffxiv_stats-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ffxiv_stats-0.4.1.tar` & `ffxiv_stats-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      106 2023-12-24 23:30:17.666831 ffxiv_stats-0.4.1/.gitignore
--rw-r--r--   0        0        0    11558 2023-08-06 18:15:32.993652 ffxiv_stats-0.4.1/LICENSE
--rw-r--r--   0        0        0     4996 2024-02-04 04:04:49.060347 ffxiv_stats-0.4.1/README.md
--rw-r--r--   0        0        0   262348 2024-02-04 03:52:04.000902 ffxiv_stats-0.4.1/examples/deterministic-rotations.ipynb
--rw-r--r--   0        0        0    51264 2023-11-03 01:32:29.636143 ffxiv_stats-0.4.1/examples/smn-rotation-comparison/fryte-results.csv
--rw-r--r--   0        0        0   501435 2023-11-03 01:32:29.639995 ffxiv_stats-0.4.1/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb
--rw-r--r--   0        0        0    20959 2023-11-03 01:32:29.641016 ffxiv_stats-0.4.1/examples/smn-rotation-comparison/smn-rotation.csv
--rw-r--r--   0        0        0  1620366 2024-02-04 03:52:04.014901 ffxiv_stats-0.4.1/examples/stochastic-rotations.ipynb
--rw-r--r--   0        0        0      441 2024-02-07 03:43:11.873266 ffxiv_stats-0.4.1/ffxiv_stats/__init__.py
--rw-r--r--   0        0        0    25175 2024-02-04 04:05:03.469574 ffxiv_stats-0.4.1/ffxiv_stats/jobs.py
--rw-r--r--   0        0        0      299 2023-12-24 23:30:17.668826 ffxiv_stats-0.4.1/ffxiv_stats/modifiers.py
--rw-r--r--   0        0        0    47554 2024-02-07 03:43:11.874269 ffxiv_stats-0.4.1/ffxiv_stats/moments.py
--rw-r--r--   0        0        0     6564 2024-02-04 03:52:04.023903 ffxiv_stats-0.4.1/ffxiv_stats/rate.py
--rw-r--r--   0        0        0      593 2024-01-10 06:09:20.789049 ffxiv_stats-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 ffxiv_stats-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      106 2023-12-24 23:30:17.666831 ffxiv_stats-0.4.2/.gitignore
+-rw-r--r--   0        0        0    11558 2023-08-06 18:15:32.993652 ffxiv_stats-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4996 2024-02-04 04:04:49.060347 ffxiv_stats-0.4.2/README.md
+-rw-r--r--   0        0        0   262348 2024-02-04 03:52:04.000902 ffxiv_stats-0.4.2/examples/deterministic-rotations.ipynb
+-rw-r--r--   0        0        0    51264 2023-11-03 01:32:29.636143 ffxiv_stats-0.4.2/examples/smn-rotation-comparison/fryte-results.csv
+-rw-r--r--   0        0        0   501435 2023-11-03 01:32:29.639995 ffxiv_stats-0.4.2/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb
+-rw-r--r--   0        0        0    20959 2023-11-03 01:32:29.641016 ffxiv_stats-0.4.2/examples/smn-rotation-comparison/smn-rotation.csv
+-rw-r--r--   0        0        0  1620366 2024-02-04 03:52:04.014901 ffxiv_stats-0.4.2/examples/stochastic-rotations.ipynb
+-rw-r--r--   0        0        0      441 2024-04-06 20:58:50.509930 ffxiv_stats-0.4.2/ffxiv_stats/__init__.py
+-rw-r--r--   0        0        0    28461 2024-04-06 21:31:09.108589 ffxiv_stats-0.4.2/ffxiv_stats/jobs.py
+-rw-r--r--   0        0        0      299 2023-12-24 23:30:17.668826 ffxiv_stats-0.4.2/ffxiv_stats/modifiers.py
+-rw-r--r--   0        0        0    47554 2024-02-07 03:43:11.874269 ffxiv_stats-0.4.2/ffxiv_stats/moments.py
+-rw-r--r--   0        0        0     6564 2024-02-04 03:52:04.023903 ffxiv_stats-0.4.2/ffxiv_stats/rate.py
+-rw-r--r--   0        0        0      593 2024-01-10 06:09:20.789049 ffxiv_stats-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 ffxiv_stats-0.4.2/PKG-INFO
```

### Comparing `ffxiv_stats-0.4.1/LICENSE` & `ffxiv_stats-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.1/README.md` & `ffxiv_stats-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.1/examples/deterministic-rotations.ipynb` & `ffxiv_stats-0.4.2/examples/deterministic-rotations.ipynb`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.1/examples/smn-rotation-comparison/fryte-results.csv` & `ffxiv_stats-0.4.2/examples/smn-rotation-comparison/fryte-results.csv`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.1/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb` & `ffxiv_stats-0.4.2/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.1/examples/smn-rotation-comparison/smn-rotation.csv` & `ffxiv_stats-0.4.2/examples/smn-rotation-comparison/smn-rotation.csv`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.1/examples/stochastic-rotations.ipynb` & `ffxiv_stats-0.4.2/examples/stochastic-rotations.ipynb`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.1/ffxiv_stats/jobs.py` & `ffxiv_stats-0.4.2/ffxiv_stats/jobs.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 from .moments import Rotation
 from .modifiers import level_mod
 
 
 class BaseStats(Rotation):
     def __init__(
         self,
-        attack_power,
-        trait,
-        main_stat,
-        det,
-        crit_stat,
-        dh_stat,
-        dot_speed_stat,
-        auto_speed_stat,
-        weapon_damage,
+        attack_power: int,
+        trait: int,
+        main_stat: int,
+        det: int,
+        crit_stat: int,
+        dh_stat: int,
+        dot_speed_stat: int,
+        auto_speed_stat: int,
+        weapon_damage: int,
         delay,
-        strength=None,
-        tenacity=400,
-        pet_attack_power=None,
-        pet_job_attribute=None,
-        pet_trait=None,
-        pet_atk_mod=195,
-        level=90,
+        strength: int = None,
+        tenacity: int = 400,
+        pet_attack_power: int = None,
+        pet_attack_power_scalar: int = None,
+        pet_attack_power_offset: int = None,
+        pet_job_attribute: int = 100,
+        pet_atk_mod: int = 195,
+        level: int = 90,
     ) -> None:
         """
         Base class for converting potency to base damage dealt. Not meant to be used alone.
         Instead use a `ROLE` class, which inherits this class and applies/sets the correct attributes and stats.
         """
         # Level dependent parameters
         # currently for lvl 90
@@ -59,157 +60,31 @@
         self.auto_speed_stat = auto_speed_stat
         self.delay = delay
 
         # Pet attributes, if not specified, pet methods will not work
         # Python formatter makes this a tuple, IDK why.
         self.pet_job_attribute = pet_job_attribute
         self.pet_attack_power = pet_attack_power
-        self.pet_trait = pet_trait
+        self.pet_attack_power_scalar = pet_attack_power_scalar
+        self.pet_attack_power_offset = pet_attack_power_offset
+
+        # Apply pet scalar and offset for an effective pet attack power
+        self.pet_effective_attack_power = nf(
+            self.pet_attack_power_scalar
+            * (self.pet_attack_power + self.pet_attack_power_offset)
+        )
+
         self.pet_atk_mod = pet_atk_mod
 
         self.attack_multiplier = self.f_atk()
         self.determination_multiplier = self.f_det()
         self.tenacity_multiplier = self.f_ten()
         self.weapon_damage_multiplier = self.f_wd()
         pass
 
-    def add_role(self, role):
-        """
-        Add a role attribute to the object.
-
-        inputs:
-        role - str, which role is being modeled.
-        """
-        self.role = role
-        pass
-
-    def add_job_name(self, job_name):
-        """
-        Add a job attribute to the object.
-
-        inputs:
-        role - str, which job is being modeled.
-        """
-        self.job = job_name
-        pass
-
-    def add_description(self, description):
-        """
-        Add a description to the object. For example this could be a specific build, rotation, etc.
-
-        inputs:
-        role - str, description of this object.
-        """
-        self.description = description
-        pass
-
-    def f_wd(self):
-        """
-        Calculate weapon damage multiplier.
-        """
-        return np.floor(
-            (self.lvl_main * self.job_attribute / 1000) + self.weapon_damage
-        )
-
-    def f_atk(self, ap_adjust=0):
-        """
-        Calculate attack multiplier.
-
-        Inputs
-        ap_adjust - int, additional amount to add to attack power (main stat). Used to account for medication.
-        """
-        return (
-            np.floor(
-                self.atk_mod
-                * ((self.attack_power + ap_adjust) - self.lvl_main)
-                / self.lvl_main
-            )
-            + 100
-        )
-
-    def f_det(self):
-        """
-        Calculate determination multiplier.
-        """
-        return np.floor(140 * (self.det - self.lvl_main) / self.lvl_div + 1000)
-
-    def f_ten(self):
-        """
-        Calculate tenacity damage multiplier.
-        """
-        return np.floor(100 * (self.tenacity - self.lvl_sub) / self.lvl_div + 1000)
-
-    def f_speed_dot(self):
-        """
-        Calculate speed multiplier for damage over time attacks.
-        """
-        return np.floor(
-            130 * (self.dot_speed_stat - self.lvl_sub) / self.lvl_div + 1000
-        )
-
-    def f_speed_auto(self):
-        """
-        Calculate speed multiplier for auto attacks.
-        """
-        return np.floor(
-            130 * (self.auto_speed_stat - self.lvl_sub) / self.lvl_div + 1000
-        )
-
-    def f_auto(self):
-        return np.floor(self.f_wd() * self.delay / 3)
-
-    def get_gcd(self):
-        # TODO: add GCD (probably not essential?)
-        pass
-
-    @staticmethod
-    def undo_main_stat_party_bonus(percent_bonus, main_stat_with_bonus):
-        """
-        Estimate how much main stat is applied by the party bonus.
-        Used for subtracting out for pet potency.
-        It is an estimate because of floor rounding, but should be within 1 point.
-        """
-        undone_stat_float = main_stat_with_bonus / percent_bonus
-
-        # Try to account for integer math by taking the floor and ceiling and seeing which one leads to the correct party bonus value
-        floored_undone_stat = int(np.floor(undone_stat_float))
-        ceilinged_undone_stat = int(np.ceil(undone_stat_float))
-
-        if np.floor(floored_undone_stat * percent_bonus) == main_stat_with_bonus:
-            return floored_undone_stat
-
-        else:
-            return ceilinged_undone_stat
-
-    pass
-
-    def pet_f_wd(self):
-        """
-        Calculate weapon damage multiplier.
-        """
-        return np.floor(
-            (self.lvl_main * self.pet_job_attribute / 1000) + self.weapon_damage
-        )
-
-    def pet_f_atk(self, ap_adjust=0):
-        """
-        Calculate attack multiplier.
-
-        Inputs
-        ap_adjust - int, additional amount to add to attack power (main stat). Used to account for medication.
-        """
-        return (
-            np.floor(
-                self.pet_atk_mod
-                * ((self.pet_attack_power + ap_adjust) - self.lvl_main)
-                / self.lvl_main
-            )
-            + 100
-        )
-
     def attach_rotation(self, rotation_df, t, action_delta=10, rotation_delta=100):
         """
         Attach a rotation data frame and compute the corresponding DPS distribution.
 
         Inputs
         rotation_df - pandas dataframe, dataframe containing rotation attributes. Should have the following columns:
                       action_name: str, unique name of an action. Unique action depends on `buffs`, `p`, and `l_c` present.
@@ -295,14 +170,103 @@
         rotation_df["is_dot"] = is_dot
 
         super().__init__(
             rotation_df, t, action_delta=action_delta, rotation_delta=rotation_delta
         )
         pass
 
+    def add_role(self, role):
+        """
+        Add a role attribute to the object.
+
+        inputs:
+        role - str, which role is being modeled.
+        """
+        self.role = role
+        pass
+
+    def add_job_name(self, job_name):
+        """
+        Add a job attribute to the object.
+
+        inputs:
+        role - str, which job is being modeled.
+        """
+        self.job = job_name
+        pass
+
+    def add_description(self, description):
+        """
+        Add a description to the object. For example this could be a specific build, rotation, etc.
+
+        inputs:
+        role - str, description of this object.
+        """
+        self.description = description
+        pass
+
+    def f_wd(self):
+        """
+        Calculate weapon damage multiplier.
+        """
+        return np.floor(
+            (self.lvl_main * self.job_attribute / 1000) + self.weapon_damage
+        )
+
+    def f_atk(self, ap_adjust=0):
+        """
+        Calculate attack multiplier.
+
+        Inputs
+        ap_adjust - int, additional amount to add to attack power (main stat). Used to account for medication.
+        """
+        return (
+            np.floor(
+                self.atk_mod
+                * ((self.attack_power + ap_adjust) - self.lvl_main)
+                / self.lvl_main
+            )
+            + 100
+        )
+
+    def f_det(self):
+        """
+        Calculate determination multiplier.
+        """
+        return np.floor(140 * (self.det - self.lvl_main) / self.lvl_div + 1000)
+
+    def f_ten(self):
+        """
+        Calculate tenacity damage multiplier.
+        """
+        return np.floor(100 * (self.tenacity - self.lvl_sub) / self.lvl_div + 1000)
+
+    def f_speed_dot(self):
+        """
+        Calculate speed multiplier for damage over time attacks.
+        """
+        return np.floor(
+            130 * (self.dot_speed_stat - self.lvl_sub) / self.lvl_div + 1000
+        )
+
+    def f_speed_auto(self):
+        """
+        Calculate speed multiplier for auto attacks.
+        """
+        return np.floor(
+            130 * (self.auto_speed_stat - self.lvl_sub) / self.lvl_div + 1000
+        )
+
+    def f_auto(self):
+        return np.floor(self.f_wd() * self.delay / 3)
+
+    def get_gcd(self):
+        # TODO: add GCD (probably not essential?)
+        pass
+
     def auto_attack_d2(self, potency, ap_adjust=0, stat_override=None):
         """
         Get base damage of an auto-attack before any variability.
 
         inputs:
         potency - int, potency of an attack
         ap_adjust - int, amount of main stat to add. Used to account for medication.
@@ -410,93 +374,136 @@
                         * self.trait
                     )
                     / 100
                 )
                 + 1
             )
 
+    @staticmethod
+    def undo_main_stat_party_bonus(percent_bonus, main_stat_with_bonus):
+        """
+        Estimate how much main stat is applied by the party bonus.
+        Used for subtracting out for pet potency.
+        It is an estimate because of floor rounding, but should be within 1 point.
+        """
+        undone_stat_float = main_stat_with_bonus / percent_bonus
+
+        # Try to account for integer math by taking the floor and ceiling and seeing which one leads to the correct party bonus value
+        floored_undone_stat = int(np.floor(undone_stat_float))
+        ceilinged_undone_stat = int(np.ceil(undone_stat_float))
+
+        if np.floor(floored_undone_stat * percent_bonus) == main_stat_with_bonus:
+            return floored_undone_stat
+
+        else:
+            return ceilinged_undone_stat
+
+    pass
+
+    def pet_f_atk(self, ap_adjust=0):
+        """
+        Calculate attack multiplier.
+
+        Inputs
+        ap_adjust - int, additional amount to add to attack power (main stat). Used to account for medication.
+        """
+        return (
+            np.floor(
+                self.pet_atk_mod
+                * ((self.pet_effective_attack_power + ap_adjust) - self.lvl_main)
+                / self.lvl_main
+            )
+            + 100
+        )
+
+    def pet_f_wd(self):
+        """
+        Calculate weapon damage multiplier.
+        """
+        return np.floor(
+            (self.lvl_main * self.pet_job_attribute / 1000) + self.weapon_damage
+        )
+
     def pet_direct_d2(self, potency, ap_adjust=0):
         """
         Get base damage of direct damage before any variability.
         Can be called directly or is automatically called by the `attach_rotation` method.
 
         inputs:
         potency - int, potency of an attack
         ap_adjust - int, amount of main stat to add. Used to account for medication.
         """
         d1 = nf(nf(nf(potency * self.pet_f_atk(ap_adjust) * self.f_det()) / 100) / 1000)
 
-        return nf(
-            nf(
-                nf(nf(nf(nf(d1 * self.f_ten()) / 1000) * self.pet_f_wd()) / 100)
-                * self.pet_trait
-            )
-            / 100
-        )
+        return nf(nf(nf(nf(nf(d1 * self.f_ten()) / 1000) * self.pet_f_wd()) / 100) * self.trait / 100)
 
 
 class Healer(BaseStats):
     def __init__(
         self,
-        mind,
-        strength,
-        det,
-        spell_speed,
-        crit_stat,
-        dh_stat,
-        weapon_damage,
-        delay,
-        pet_attack_power=None,
-        pet_job_attribute=None,
-        pet_trait=None,
-        pet_atk_mod=195,
-        level=90,
+        mind: int,
+        strength: int,
+        det: int,
+        spell_speed: int,
+        crit_stat: int,
+        dh_stat: int,
+        weapon_damage: int,
+        delay: float,
+        pet_attack_power: int = None,
+        pet_attack_power_scalar: float = 1.058,
+        pet_attack_power_offset: int = 0,
+        pet_job_attribute: int = 100,
+        pet_atk_mod: int = 195,
+        level: int = 90,
         intelligence=None,
         dexterity=None,
         vit=None,
         tenacity=None,
     ) -> None:
-        """
-        Set healer-specific stats with this class like main stat, traits, etc.
+        """Set Healer stats to compute damage from potency.
 
-        inputs:
-        mind - int, mind stat
-        intelligence - int, intelligence stat
-        vitality - int, vitality stat
-        strength, - int, strength stat
-        dexterity - int, strength stat
-        det - int, determination stat
-        skill_speed - int, skill speed stat
-        spell_speed - int, spell speed stat
-        tenacity - tenacity stat
-        crit_stat - critical hit stat
-        dh_stat - direct hit rate stat
-        weapon_damage - weapon damage stat
-        delay - weapon delay stat
-        pet_job_attribute - optional, pet-based job attribute. For Earthly Star in EW, this is 115.
-        pet_main_stat_adjust - amount to adjust attack power by. For Earthly Star in EW, this is 0.
-        pet_trait - optional, pet-based trait bonus. For Earthly Star in EW, this is 134 (Maim and Mend + 4% hidden).
-        pet_atk_mod - optional, pet-based attack modifier. For Earthly Star in EW, this is 195.
-        level - Player level, default of 90, can be 70, 80, or 90.
+        Many of the pet stats are used to compute an effective pet attack power, given by:
+        effective_pet_attack_power = floor(pet_attack_power_scalar * (pet_attack_power + pet_attack_power_offset))
+
+        Args:
+            mind (int): Mind
+            strength (int): Strength stat, for auto attacks.
+            det (int): Determination stat.
+            spell_speed (int): Spell speed stat.
+            crit_stat (int): Critical hit stat.
+            dh_stat (int): Direct hit rate stat.
+            weapon_damage (int): Weapon damage
+            delay (float): Weapon delay stat, for auto attacks.
+            pet_attack_power (int, optional): Pet attack power for AST's Earthly Star, which is attack power - n% power bonus. Defaults to None.
+            pet_attack_power_scalar (float, optional): Pet attack power scalar,. Defaults to 1.058.
+            pet_attack_power_offset (int, optional): Pet attack power offset, which is also multiplied by pet_attack_power_scalar. Defaults to 0.
+            pet_job_attribute (int, optional): Pet job attribute, which is different from the player job attribute. Defaults to 100.
+            pet_atk_mod (int, optional): Pet attack modifier, which is the same as the player attack modifier. Defaults to 195.
+            level (int, optional): Player level. Defaults to 90.
+            intelligence (None, optional): Deprecated argument for intelligence. Defaults to None.
+            dexterity (None, optional): Deprecated argument for dexterity. Defaults to None.
+            vit (None, optional): Deprecated argument for vitality. Defaults to None.
+            tenacity (None, optional): Deprecated argument for tenacity. Defaults to None.
         """
         super().__init__(
             attack_power=mind,
             trait=130,
             main_stat=mind,
             strength=strength,
             det=det,
             crit_stat=crit_stat,
             dh_stat=dh_stat,
             dot_speed_stat=spell_speed,
             auto_speed_stat=400,
             weapon_damage=weapon_damage,
             delay=delay,
             pet_attack_power=pet_attack_power,
+            pet_attack_power_scalar=pet_attack_power_scalar,
+            pet_attack_power_offset=pet_attack_power_offset,
             pet_job_attribute=pet_job_attribute,
-            pet_trait=pet_trait,
             pet_atk_mod=pet_atk_mod,
             level=level,
         )
 
         self.auto_trait = 100
         self.atk_mod = 195
         self.job_attribute = 115
@@ -525,62 +532,60 @@
         skill_speed: int,
         tenacity: int,
         crit_stat: int,
         dh_stat: int,
         weapon_damage: int,
         delay: float,
         job: str,
-        pet_attack_power=None,
-        pet_job_attribute=None,
-        pet_trait=None,
-        pet_atk_mod=195,
-        level=90,
+        pet_attack_power: int = None,
+        pet_attack_power_scalar: float = 1.,
+        pet_attack_power_offset: int = -18,
+        pet_job_attribute: int = 100,
+        pet_atk_mod: int = 195,
+        level: int = 90,
     ) -> None:
-        """
-        Set tank-specific stats with this class like main stat, traits, etc.
-        Most importantly this adjusts the attack modifier.
+        """Set tank stats, most notably the attack modifier.
+
+        Many of the pet stats are used to compute an effective pet attack power, given by:
+        effective_pet_attack_power = floor(pet_attack_power_scalar * (pet_attack_power + pet_attack_power_offset))
+
+        Args:
+            strength (int): Strength stat.
+            det (int): Determination stat.
+            skill_speed (int): Skill speed stat.
+            tenacity (int): Tenacity stat.
+            crit_stat (int): Critical hit stat.
+            dh_stat (int): Direct hit rate stat.
+            weapon_damage (int): Weapon damage stat.
+            delay (float): Weapon delay stat, for auto attacks
+            job (str): Job, used to set job modifier. Allowed values are: {"Warrior", "Paladin", "DarkKnight", "Gunbreaker"}
+            pet_attack_power (int, optional): Pet attack power, typically attack power - n% party bonus. Defaults to None.
+            pet_attack_power_scalar (float, optional): Scalar to multiply pet attack power by. Defaults to 1, the scalar for DRK's Esteem.
+            pet_attack_power_offset (int, optional): Pet attack power offset, also multiplied by the pet scalar. Defaults to -18, the offset for DRK's Esteem.
+            pet_job_attribute (int, optional): Pet job attribute, which is not the same as the player. Defaults to 100.
+            pet_atk_mod (int, optional): Pet attack modifier, which is not the same as the player. Defaults to 195.
+            level (int, optional): _description_. Defaults to 90.
 
-        inputs:
-        mind - int, mind stat
-        intelligence - int, intelligence stat
-        vitality - int, vitality stat
-        strength, - int, strength stat
-        dexterity - int, strength stat
-        det - int, determination stat
-        skill_speed - int, skill speed stat
-        spell_speed - int, spell speed stat
-        tenacity - tenacity stat
-        crit_stat - critical hit stat
-        dh_stat - direct hit rate stat
-        weapon_damage - weapon damage stat
-        delay - weapon delay stat
-        job - job name, required to correctly set job modifier. Follow FFLogs job naming API convention:
-              "Warrior", "Paladin", "DarkKnight", or "Gunbreaker".
-        pet_job_attribute - optional, pet-based job attribute. For Living Shadow in EW, this is 100.
-        pet_main_stat_adjust - amount to adjust attack power by. For Living Shadow, this is the difference between strength racial bonus
-                               between the player's race and a midlander (+3).
-        pet_trait - optional, pet-based trait bonus. For Living Shadow in EW, this is 100
-        pet_atk_mod - optional, pet-based attack modifier. For Living Shadow in EW, this is 195
-        level - Player level, default of 90, can be 70, 80, or 90.
         """
         super().__init__(
             attack_power=strength,
             trait=100,
             main_stat=strength,
             det=det,
             tenacity=tenacity,
             crit_stat=crit_stat,
             dh_stat=dh_stat,
             auto_speed_stat=skill_speed,
             dot_speed_stat=skill_speed,
             weapon_damage=weapon_damage,
             delay=delay,
             pet_attack_power=pet_attack_power,
+            pet_attack_power_scalar=pet_attack_power_scalar,
+            pet_attack_power_offset=pet_attack_power_offset,
             pet_job_attribute=pet_job_attribute,
-            pet_trait=pet_trait,
             pet_atk_mod=pet_atk_mod,
             level=level,
         )
 
         if (job == "Warrior") | (job == "DarkKnight"):
             self.job_attribute = 105
         elif (job == "Paladin") | (job == "Gunbreaker"):
@@ -597,14 +602,81 @@
             self.atk_mod = 115
 
         self.dot_speed_stat = skill_speed
         self.auto_speed_stat = skill_speed
         pass
 
 
+class MagicalRanged(BaseStats):
+    def __init__(
+        self,
+        intelligence: int,
+        strength: int,
+        det: int,
+        spell_speed: int,
+        crit_stat: int,
+        dh_stat: int,
+        weapon_damage: int,
+        delay: float,
+        pet_attack_power: int = None,
+        pet_attack_power_scalar: float = 0.88,
+        pet_attack_power_offset: int = -48,
+        pet_job_attribute: int = 100,
+        pet_atk_mod: int = 195,
+        level: int = 90,
+    ) -> None:
+        """Set stats specific to magical ranged, to compute damage from potency.
+
+        Many of the pet stats are used to compute an effective pet attack power, given by:
+        effective_pet_attack_power = floor(pet_attack_power_scalar * (pet_attack_power + pet_attack_power_offset))
+        Args:
+            intelligence (int): intelligence stat.
+            strength (int): strength stat, for auto attacks.
+            det (int): determination stat.
+            spell_speed (int): spell speed stat.
+            crit_stat (int): critical hit stat.
+            dh_stat (int): direct hit rate stat
+            weapon_damage (int): weapon damage stat.
+            delay (float): weapon delay stat, for auto attacks
+            pet_attack_power (int, optional): Attack power of pet, typically intelligence without the n% party bonus. Defaults to None.
+            pet_attack_power_scalar (float, optional): Scalar to apply to pet attack power to account for pet potency. Defaults to 0.88, the default value for SMN.
+            pet_attack_power_offset (int, optional): Attack power amount to add to attack power. Usually -48 to subtract out hidden trait stats. This value is also multiplied by pet_attack_power_scalar. Defaults to -48, the default value for SMN.
+            pet_job_attribute (int, optional): Pet job attribute, which is different from that of the player. Defaults to 100.
+            pet_atk_mod (int, optional): Pet attack modifier, which is usually the same as the player. Defaults to 195.
+            level (int, optional): Player level. Defaults to 90.
+        """
+        super().__init__(
+            attack_power=intelligence,
+            trait=130,
+            main_stat=intelligence,
+            strength=strength,
+            det=det,
+            crit_stat=crit_stat,
+            dh_stat=dh_stat,
+            dot_speed_stat=spell_speed,
+            auto_speed_stat=400,
+            weapon_damage=weapon_damage,
+            delay=delay,
+            pet_attack_power=pet_attack_power,
+            pet_attack_power_scalar=pet_attack_power_scalar,
+            pet_attack_power_offset=pet_attack_power_offset,
+            pet_job_attribute=pet_job_attribute,
+            pet_atk_mod=pet_atk_mod,
+            level=level,
+        )
+
+        self.add_role("Caster")
+
+        self.auto_trait = 100
+        self.dot_speed_stat = spell_speed
+        self.auto_speed_stat = 400
+
+        pass
+
+
 # class PhysicalRanged(BaseStats):
 #     def __init__(self, mind, intelligence, vitality, strength, dexterity, det,
 #                  skill_speed, spell_speed, tenacity, crit_stat, dh_stat, weapon_damage, delay, level=90) -> None:
 #         """
 #         Set physical ranged-specific stats with this class like main stat, traits, etc.
 
 #         inputs:
@@ -627,43 +699,14 @@
 
 #         self.add_role('Physical Ranged')
 
 #         self.skill_speed = skill_speed
 #         self.spell_speed = spell_speed
 #         pass
 
-# class MagicalRanged(BaseStats):
-#     def __init__(self, mind, intelligence, vitality, strength, dexterity, det,
-#                  skill_speed, spell_speed, tenacity, crit_stat, dh_stat, weapon_damage, delay, level=90) -> None:
-#         """
-#         Set magical ranged-specific stats with this class like main stat, traits, etc.
-
-#         inputs:
-#         mind - int, mind stat
-#         intelligence - int, intelligence stat
-#         vitality - int, vitality stat
-#         strength, - int, strength stat
-#         dexterity - int, strength stat
-#         det - int, determination stat
-#         skill_speed - int, skill speed stat
-#         spell_speed - int, spell speed stat
-#         tenacity - tenacity stat
-#         crit_stat - critical hit stat
-#         dh_stat - direct hit rate stat
-#         weapon_damage - weapon damage stat
-#         delay - weapon delay stat
-#         """
-#         super().__init__(intelligence, 130, intelligence, mind, intelligence, vitality, strength, dexterity, det,
-#                          tenacity, crit_stat, dh_stat, spell_speed, skill_speed, weapon_damage, delay, level=90)
-
-#         self.add_role('Caster')
-
-#         self.skill_speed = skill_speed
-#         self.spell_speed = spell_speed
-
 
 # class Melee(BaseStats):
 #     def __init__(self, mind, intelligence, vitality, strength, dexterity,
 #                  det, skill_speed, spell_speed, tenacity, crit_stat, dh_stat, weapon_damage, delay, level=90) -> None:
 #         """
 #         Set melee-specific stats with this class like main stat, traits, etc.
```

### Comparing `ffxiv_stats-0.4.1/ffxiv_stats/moments.py` & `ffxiv_stats-0.4.2/ffxiv_stats/moments.py`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.1/ffxiv_stats/rate.py` & `ffxiv_stats-0.4.2/ffxiv_stats/rate.py`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.1/pyproject.toml` & `ffxiv_stats-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.1/PKG-INFO` & `ffxiv_stats-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffxiv_stats
-Version: 0.4.1
+Version: 0.4.2
 Summary: Compute damage variability in the critically acclaimed MMORPG Final Fantasy XIV.
 Author-email: Acerola Paracletus <ffxivacerola@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: numpy >= 1.20.2
 Requires-Dist: matplotlib >= 3.4.2
```

