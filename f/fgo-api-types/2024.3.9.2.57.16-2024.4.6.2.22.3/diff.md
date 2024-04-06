# Comparing `tmp/fgo_api_types-2024.3.9.2.57.16.tar.gz` & `tmp/fgo_api_types-2024.4.6.2.22.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2024.3.9.2.57.16.tar", max compression
+gzip compressed data, was "fgo_api_types-2024.4.6.2.22.3.tar", max compression
```

## Comparing `fgo_api_types-2024.3.9.2.57.16.tar` & `fgo_api_types-2024.4.6.2.22.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2024-03-09 02:57:01.167484 fgo_api_types-2024.3.9.2.57.16/LICENSE
--rw-r--r--   0        0        0      449 2024-03-09 02:57:01.167484 fgo_api_types-2024.3.9.2.57.16/README.md
--rw-r--r--   0        0        0        0 2024-03-09 02:57:16.371475 fgo_api_types-2024.3.9.2.57.16/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2024-03-09 02:57:16.371475 fgo_api_types-2024.3.9.2.57.16/fgo_api_types/base.py
--rw-r--r--   0        0        0     4322 2024-03-09 02:57:16.371475 fgo_api_types-2024.3.9.2.57.16/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3762 2024-03-09 02:57:16.371475 fgo_api_types-2024.3.9.2.57.16/fgo_api_types/common.py
--rw-r--r--   0        0        0    40588 2024-03-09 02:57:16.371475 fgo_api_types-2024.3.9.2.57.16/fgo_api_types/enums.py
--rw-r--r--   0        0        0   175029 2024-03-09 02:57:16.371475 fgo_api_types-2024.3.9.2.57.16/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    85075 2024-03-09 02:57:16.371475 fgo_api_types-2024.3.9.2.57.16/fgo_api_types/nice.py
--rw-r--r--   0        0        0    58668 2024-03-09 02:57:16.371475 fgo_api_types-2024.3.9.2.57.16/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4518 2024-03-09 02:57:16.371475 fgo_api_types-2024.3.9.2.57.16/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    19285 2024-03-09 02:57:16.371475 fgo_api_types-2024.3.9.2.57.16/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2024-03-09 02:57:16.687474 fgo_api_types-2024.3.9.2.57.16/pyproject.toml
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 fgo_api_types-2024.3.9.2.57.16/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-06 02:21:48.273692 fgo_api_types-2024.4.6.2.22.3/LICENSE
+-rw-r--r--   0        0        0      449 2024-04-06 02:21:48.273692 fgo_api_types-2024.4.6.2.22.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4368 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3762 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/common.py
+-rw-r--r--   0        0        0    40655 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   176026 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    85618 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    59051 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4518 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    19285 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2024-04-06 02:22:03.705703 fgo_api_types-2024.4.6.2.22.3/pyproject.toml
+-rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 fgo_api_types-2024.4.6.2.22.3/PKG-INFO
```

### Comparing `fgo_api_types-2024.3.9.2.57.16/LICENSE` & `fgo_api_types-2024.4.6.2.22.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.3.9.2.57.16/fgo_api_types/basic.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 class BasicFunction(BaseModelORJson):
     funcId: int
     funcType: NiceFuncType
     funcTargetType: NiceFuncTargetType
     funcTargetTeam: FuncApplyTarget
     functvals: list[NiceTrait]
+    overWriteTvalsList: list[list[NiceTrait]]
     funcquestTvals: list[NiceTrait]
     traitVals: list[NiceTrait] = []
     buffs: Sequence[BasicBuff]
 
 
 class BasicSkill(BaseModelORJson):
     id: int
```

### Comparing `fgo_api_types-2024.3.9.2.57.16/fgo_api_types/common.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.3.9.2.57.16/fgo_api_types/enums.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -998,14 +998,15 @@
     buffBuffSuccessRateUp = "buffBuffSuccessRateUp"
     groupServant = "groupServant"
     takeruDummyTrait = "takeruDummyTrait"
     artsBuff = "artsBuff"
     busterBuff = "busterBuff"
     quickBuff = "quickBuff"
     FSNServant = "FSNServant"
+    fieldDarkness = "fieldDarkness"
 
 
 TRAIT_NAME: dict[int, Trait] = {
     1: Trait.genderMale,
     2: Trait.genderFemale,
     3: Trait.genderUnknown,
     100: Trait.classSaber,
@@ -1191,14 +1192,15 @@
     2875: Trait.caitCuCerpriestessAscension0To2,
     2876: Trait.caitCuCerpriestessAscension3To4,
     2878: Trait.fieldAir,
     2879: Trait.caitCuCerpriestessOnTheField,
     2880: Trait.elementalsWrath,
     2881: Trait.groupServant,
     2883: Trait.FSNServant,
+    2884: Trait.fieldDarkness,
     # 2xxx: CQ or Story quests buff
     3000: Trait.attackPhysical,  # Normal attack, including NP
     3001: Trait.attackProjectile,
     3002: Trait.attackMagical,
     3004: Trait.buffPositiveEffect,
     3005: Trait.buffNegativeEffect,  # mutually exclusive with 3004
     3006: Trait.buffIncreaseDamage,  # catch all damage: atk, np, powermod, ...
```

### Comparing `fgo_api_types-2024.3.9.2.57.16/fgo_api_types/gameenums.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/gameenums.py`

 * *Files 0% similar despite different names*

```diff
@@ -751,14 +751,15 @@
     WAR_BOARD_NOT_ATTACKED = 183
     WAR_BOARD_IGNORE_DEFEATPOINT = 184
     SKILL_AFTER_FUNCTION = 185
     TREASURE_DEVICE_AFTER_FUNCTION = 186
     SKILL_AFTER_FUNCTION_MAIN_ONLY = 187
     TREASURE_DEVICE_AFTER_FUNCTION_MAIN_ONLY = 188
     PREVENT_INVISIBLE_WHEN_INSTANT_DEATH = 189
+    OVERWRITE_SUBATTRIBUTE = 190
     TO_FIELD_CHANGE_FIELD = 10001
     TO_FIELD_AVOID_BUFF = 10002
     TO_FIELD_SUB_INDIVIDUALITY_FIELD = 10003
 
 
 class NiceBuffType(StrEnum):
     """Buff Type Enum"""
@@ -933,14 +934,15 @@
     warBoardNotAttacked = "warBoardNotAttacked"
     warBoardIgnoreDefeatpoint = "warBoardIgnoreDefeatpoint"
     skillAfterFunction = "skillAfterFunction"
     treasureDeviceAfterFunction = "treasureDeviceAfterFunction"
     skillAfterFunctionMainOnly = "skillAfterFunctionMainOnly"
     treasureDeviceAfterFunctionMainOnly = "treasureDeviceAfterFunctionMainOnly"
     preventInvisibleWhenInstantDeath = "preventInvisibleWhenInstantDeath"
+    overwriteSubattribute = "overwriteSubattribute"
     toFieldChangeField = "toFieldChangeField"
     toFieldAvoidBuff = "toFieldAvoidBuff"
     toFieldSubIndividualityField = "toFieldSubIndividualityField"
 
 
 BUFF_TYPE_NAME: dict[int, NiceBuffType] = {
     0: NiceBuffType.none,
@@ -1113,14 +1115,15 @@
     183: NiceBuffType.warBoardNotAttacked,
     184: NiceBuffType.warBoardIgnoreDefeatpoint,
     185: NiceBuffType.skillAfterFunction,
     186: NiceBuffType.treasureDeviceAfterFunction,
     187: NiceBuffType.skillAfterFunctionMainOnly,
     188: NiceBuffType.treasureDeviceAfterFunctionMainOnly,
     189: NiceBuffType.preventInvisibleWhenInstantDeath,
+    190: NiceBuffType.overwriteSubattribute,
     10001: NiceBuffType.toFieldChangeField,
     10002: NiceBuffType.toFieldAvoidBuff,
     10003: NiceBuffType.toFieldSubIndividualityField,
 }
 
 
 class BuffAction(IntEnum):
@@ -1248,14 +1251,15 @@
     FUNCTION_ATTACK_AFTER_MAIN_ONLY = 121
     FUNCTION_SKILL_AFTER = 122
     FUNCTION_SKILL_AFTER_MAIN_ONLY = 123
     FUNCTION_TREASURE_DEVICE_AFTER = 124
     FUNCTION_TREASURE_DEVICE_AFTER_MAIN_ONLY = 125
     GUTS = 126
     PREVENT_INVISIBLE_WHEN_INSTANT_DEATH = 127
+    OVERWRITE_SUBATTRIBUTE = 128
 
 
 class NiceBuffAction(StrEnum):
     """Buff Action Type Enum"""
 
     none = "none"
     commandAtk = "commandAtk"
@@ -1381,14 +1385,15 @@
     functionAttackAfterMainOnly = "functionAttackAfterMainOnly"
     functionSkillAfter = "functionSkillAfter"
     functionSkillAfterMainOnly = "functionSkillAfterMainOnly"
     functionTreasureDeviceAfter = "functionTreasureDeviceAfter"
     functionTreasureDeviceAfterMainOnly = "functionTreasureDeviceAfterMainOnly"
     guts = "guts"
     preventInvisibleWhenInstantDeath = "preventInvisibleWhenInstantDeath"
+    overwriteSubattribute = "overwriteSubattribute"
 
 
 BUFF_ACTION_NAME: dict[int, NiceBuffAction] = {
     0: NiceBuffAction.none,
     1: NiceBuffAction.commandAtk,
     2: NiceBuffAction.commandDef,
     3: NiceBuffAction.atk,
@@ -1512,14 +1517,15 @@
     121: NiceBuffAction.functionAttackAfterMainOnly,
     122: NiceBuffAction.functionSkillAfter,
     123: NiceBuffAction.functionSkillAfterMainOnly,
     124: NiceBuffAction.functionTreasureDeviceAfter,
     125: NiceBuffAction.functionTreasureDeviceAfterMainOnly,
     126: NiceBuffAction.guts,
     127: NiceBuffAction.preventInvisibleWhenInstantDeath,
+    128: NiceBuffAction.overwriteSubattribute,
 }
 
 
 class BuffLimit(IntEnum):
     NONE = 0
     UPPER = 1
     LOWER = 2
@@ -1688,14 +1694,16 @@
     ProgressTurnOnBoard = 141
     CheckTargetResurrectable = 142
     CancelTransform = 143
     UnSubStateWhenContinue = 144
     CheckTargetHaveDefeatPoint = 145
     NPFixedDamageValue = 146
     IgnoreShiftSafeDamage = 147
+    ActAttackFunction = 148
+    DelayRemoveBuffExpiredOnPlayerTurn = 149
 
 
 class ClassRelationOverwriteType(IntEnum):
     OVERWRITE_FORCE = 0
     OVERWRITE_MORE_THAN_TARGET = 1
     OVERWRITE_LESS_THAN_TARGET = 2
 
@@ -2328,14 +2336,15 @@
     TREASURE_DEVICE_ACCELERATE = 208
     PLAY_QUEST_PHASE = 209
     NOT_PLAY_QUEST_PHASE = 210
     EVENT_START_TO_END = 211
     COMMON_VALUE_ABOVE = 212
     COMMON_VALUE_BELOW = 213
     COMMON_VALUE_EQUAL = 214
+    ELAPSED_TIME_AFTER_QUEST_CLEAR = 215
 
 
 class NiceCondType(StrEnum):
     """Condition Type Enum"""
 
     none = "none"
     questClear = "questClear"
@@ -2545,14 +2554,15 @@
     treasureDeviceAccelerate = "treasureDeviceAccelerate"
     playQuestPhase = "playQuestPhase"
     notPlayQuestPhase = "notPlayQuestPhase"
     eventStartToEnd = "eventStartToEnd"
     commonValueAbove = "commonValueAbove"
     commonValueBelow = "commonValueBelow"
     commonValueEqual = "commonValueEqual"
+    elapsedTimeAfterQuestClear = "elapsedTimeAfterQuestClear"
 
 
 COND_TYPE_NAME: dict[int, NiceCondType] = {
     0: NiceCondType.none,
     1: NiceCondType.questClear,
     2: NiceCondType.itemGet,
     3: NiceCondType.useItemEternity,
@@ -2760,14 +2770,15 @@
     208: NiceCondType.treasureDeviceAccelerate,
     209: NiceCondType.playQuestPhase,
     210: NiceCondType.notPlayQuestPhase,
     211: NiceCondType.eventStartToEnd,
     212: NiceCondType.commonValueAbove,
     213: NiceCondType.commonValueBelow,
     214: NiceCondType.commonValueEqual,
+    215: NiceCondType.elapsedTimeAfterQuestClear,
 }
 
 
 class VoiceCondType(IntEnum):
     BIRTH_DAY = 1
     EVENT = 2
     FRIENDSHIP = 3
@@ -3058,15 +3069,15 @@
     CLOSED_HIDE_TREND_CLASS = 2048
     CLOSED_HIDE_REWARD = 4096
     NO_DISPLAY_CONSUME = 8192
     SUPER_BOSS = 16384
     NO_DISPLAY_MISSION_NOTIFY = 32768
     HIDE_PROGRESS = 65536
     DROP_FIRST_TIME_ONLY = 131072
-    CHAPTER_SUB_ID_JAPANESE_NUMERALS = 262144
+    CHAPTER_SUB_ID_JAPANESE_NUMERALS_CALLIGRAPHY = 262144
     SUPPORT_ONLY_FORCE_BATTLE = 524288
     EVENT_DECK_NO_SUPPORT = 1048576
     FATIGUE_BATTLE = 2097152
     SUPPORT_SELECT_AFTER_SCRIPT = 4194304
     BRANCH = 8388608
     USER_EVENT_DECK = 16777216
     NO_DISPLAY_RAID_REMAIN = 33554432
@@ -3100,14 +3111,15 @@
     ENEMY_IMMEDIATE_APPEAR = 18014398509481984
     NO_SUPPORT_LIST = 36028797018963968
     LIVE = 72057594037927936
     FORCE_DISPLAY_ENEMY_INFO = 144115188075855872
     ALLOUT_BATTLE = 288230376151711744
     RECOLLECTION = 576460752303423488
     NOT_SINGLE_SUPPORT_ONLY = 1152921504606846976
+    DISABLE_CHAPTER_SUB = 2305843009213693952
 
 
 class NiceQuestFlag(StrEnum):
     """Quest Flag Enum"""
 
     none = "none"
     noBattle = "noBattle"
@@ -3123,15 +3135,15 @@
     closedHideTrendClass = "closedHideTrendClass"
     closedHideReward = "closedHideReward"
     noDisplayConsume = "noDisplayConsume"
     superBoss = "superBoss"
     noDisplayMissionNotify = "noDisplayMissionNotify"
     hideProgress = "hideProgress"
     dropFirstTimeOnly = "dropFirstTimeOnly"
-    chapterSubIdJapaneseNumerals = "chapterSubIdJapaneseNumerals"
+    chapterSubIdJapaneseNumeralsCalligraphy = "chapterSubIdJapaneseNumeralsCalligraphy"
     supportOnlyForceBattle = "supportOnlyForceBattle"
     eventDeckNoSupport = "eventDeckNoSupport"
     fatigueBattle = "fatigueBattle"
     supportSelectAfterScript = "supportSelectAfterScript"
     branch = "branch"
     userEventDeck = "userEventDeck"
     noDisplayRaidRemain = "noDisplayRaidRemain"
@@ -3165,14 +3177,15 @@
     enemyImmediateAppear = "enemyImmediateAppear"
     noSupportList = "noSupportList"
     live = "live"
     forceDisplayEnemyInfo = "forceDisplayEnemyInfo"
     alloutBattle = "alloutBattle"
     recollection = "recollection"
     notSingleSupportOnly = "notSingleSupportOnly"
+    disableChapterSub = "disableChapterSub"
 
 
 Quest_FLAG_NAME: dict[int, NiceQuestFlag] = {
     1: NiceQuestFlag.none,
     2: NiceQuestFlag.noBattle,
     4: NiceQuestFlag.raid,
     8: NiceQuestFlag.raidConnection,
@@ -3186,15 +3199,15 @@
     2048: NiceQuestFlag.closedHideTrendClass,
     4096: NiceQuestFlag.closedHideReward,
     8192: NiceQuestFlag.noDisplayConsume,
     16384: NiceQuestFlag.superBoss,
     32768: NiceQuestFlag.noDisplayMissionNotify,
     65536: NiceQuestFlag.hideProgress,
     131072: NiceQuestFlag.dropFirstTimeOnly,
-    262144: NiceQuestFlag.chapterSubIdJapaneseNumerals,
+    262144: NiceQuestFlag.chapterSubIdJapaneseNumeralsCalligraphy,
     524288: NiceQuestFlag.supportOnlyForceBattle,
     1048576: NiceQuestFlag.eventDeckNoSupport,
     2097152: NiceQuestFlag.fatigueBattle,
     4194304: NiceQuestFlag.supportSelectAfterScript,
     8388608: NiceQuestFlag.branch,
     16777216: NiceQuestFlag.userEventDeck,
     33554432: NiceQuestFlag.noDisplayRaidRemain,
@@ -3228,14 +3241,15 @@
     18014398509481984: NiceQuestFlag.enemyImmediateAppear,
     36028797018963968: NiceQuestFlag.noSupportList,
     72057594037927936: NiceQuestFlag.live,
     144115188075855872: NiceQuestFlag.forceDisplayEnemyInfo,
     288230376151711744: NiceQuestFlag.alloutBattle,
     576460752303423488: NiceQuestFlag.recollection,
     1152921504606846976: NiceQuestFlag.notSingleSupportOnly,
+    2305843009213693952: NiceQuestFlag.disableChapterSub,
 }
 
 
 class StatusRank(IntEnum):
     A = 11
     A_PLUS = 12
     A_PLUS2 = 13
@@ -3489,14 +3503,15 @@
     WHITE_MARK_UNDER_BOARD = 262144
     SUB_FOLDER = 524288
     DISP_EARTH_POINT_WITHOUT_MAP = 1048576
     IS_WAR_ICON_FREE = 2097152
     IS_WAR_ICON_CENTER = 4194304
     NOTICE_BOARD = 8388608
     CHANGE_DISP_CLOSED_MESSAGE = 16777216
+    CHAPTER_SUB_ID_JAPANESE_NUMERALS_NORMAL = 33554432
 
 
 class NiceWarFlag(StrEnum):
     """War Flag Enum"""
 
     withMap = "withMap"
     showOnMaterial = "showOnMaterial"
@@ -3518,14 +3533,15 @@
     whiteMarkUnderBoard = "whiteMarkUnderBoard"
     subFolder = "subFolder"
     dispEarthPointWithoutMap = "dispEarthPointWithoutMap"
     isWarIconFree = "isWarIconFree"
     isWarIconCenter = "isWarIconCenter"
     noticeBoard = "noticeBoard"
     changeDispClosedMessage = "changeDispClosedMessage"
+    chapterSubIdJapaneseNumeralsNormal = "chapterSubIdJapaneseNumeralsNormal"
 
 
 WAR_FLAG_NAME: dict[int, NiceWarFlag] = {
     2: NiceWarFlag.withMap,
     4: NiceWarFlag.showOnMaterial,
     8: NiceWarFlag.folderSortPrior,
     16: NiceWarFlag.storyShortcut,
@@ -3545,14 +3561,15 @@
     262144: NiceWarFlag.whiteMarkUnderBoard,
     524288: NiceWarFlag.subFolder,
     1048576: NiceWarFlag.dispEarthPointWithoutMap,
     2097152: NiceWarFlag.isWarIconFree,
     4194304: NiceWarFlag.isWarIconCenter,
     8388608: NiceWarFlag.noticeBoard,
     16777216: NiceWarFlag.changeDispClosedMessage,
+    33554432: NiceWarFlag.chapterSubIdJapaneseNumeralsNormal,
 }
 
 
 class WarEntityStartType(IntEnum):
     NONE = 0
     SCRIPT = 1
     QUEST = 2
@@ -5139,39 +5156,43 @@
     3: NiceRestrictionRangeType.above,
     4: NiceRestrictionRangeType.below,
     5: NiceRestrictionRangeType.between,
 }
 
 
 class FrequencyType(IntEnum):
+    NONE = 0
     ONCE = 1
     ONCE_UNTIL_REBOOT = 2
     EVERY_TIME = 3
     VALENTINE = 4
     EVERY_TIME_AFTER = 5
+    EVERY_TIME_BEFORE = 6
 
 
 class NiceFrequencyType(StrEnum):
     """Frequency Type"""
 
+    none = "none"
     once = "once"
     onceUntilReboot = "onceUntilReboot"
     everyTime = "everyTime"
     valentine = "valentine"
     everyTimeAfter = "everyTimeAfter"
-    none = "none"
+    everyTimeBefore = "everyTimeBefore"
 
 
 FREQUENCY_TYPE_NAME: dict[int, NiceFrequencyType] = {
+    0: NiceFrequencyType.none,
     1: NiceFrequencyType.once,
     2: NiceFrequencyType.onceUntilReboot,
     3: NiceFrequencyType.everyTime,
     4: NiceFrequencyType.valentine,
     5: NiceFrequencyType.everyTimeAfter,
-    0: NiceFrequencyType.none,
+    6: NiceFrequencyType.everyTimeBefore,
 }
 
 
 class CommandCardAttackType(IntEnum):
     ONE = 1
     ALL = 2
```

### Comparing `fgo_api_types-2024.3.9.2.57.16/fgo_api_types/nice.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,14 +394,16 @@
     ProgressTurnOnBoard: int | None = None
     CheckTargetResurrectable: int | None = None
     CancelTransform: int | None = None
     UnSubStateWhenContinue: int | None = None
     CheckTargetHaveDefeatPoint: int | None = None
     NPFixedDamageValue: int | None = None
     IgnoreShiftSafeDamage: int | None = None
+    ActAttackFunction: int | None = None
+    DelayRemoveBuffExpiredOnPlayerTurn: int | None = None
     # Extra dataval from SkillLvEntty.DIC_KEY_APPLY_SUPPORT_SVT
     ApplySupportSvt: Optional[int] = None
     # These are not DataVals but guesses from SkillLvEntity and EventDropUpValInfo
     Individuality: Optional[int] = None
     EventId: Optional[int] = None
     AddCount: Optional[int] = None
     RateCount: Optional[int] = None
@@ -488,14 +490,18 @@
     nameTotal: str
     name: str
     icon: Optional[HttpUrl] = None
     priority: int
     isDispValue: bool
 
 
+class FunctionScript(BaseModel):
+    overwriteTvals: list[list[NiceTrait]] | None = None
+
+
 class NiceBaseFunction(BaseModelORJson):
     funcId: int = Field(..., title="Function ID", description="Function ID")
     funcType: NiceFuncType = Field(
         ..., title="Function type", description="Function type"
     )
     funcTargetType: NiceFuncTargetType = Field(
         ...,
@@ -518,20 +524,29 @@
     )
     functvals: list[NiceTrait] = Field(
         ...,
         title="Function tvals",
         description="Function tvals: If available, function's targets or their buffs "
         "need to satisfy the traits given here.",
     )
+    overWriteTvalsList: list[list[NiceTrait]] = Field(
+        ...,
+        title="Overwrite Tvals List",
+        description="Overwrite functvals if given. Two-dimensional list, the inner trait list acts as a combined trait in functvals",
+    )
     funcquestTvals: list[NiceTrait] = Field(
         ...,
         title="Function quest traits",
         description="Function quest traits. "
         "The current quest needs this traits for the function to works.",
     )
+    script: FunctionScript = Field(
+        ...,
+        title="Function script",
+    )
     funcGroup: list[NiceFuncGroup] = Field(
         ...,
         title="Function group details",
         description="Some more details for event drop up, bond point up functions",
     )
     traitVals: list[NiceTrait] = Field(
         [],
@@ -772,14 +787,15 @@
     releaseConditions: list[NiceCommonRelease]
     extraAssets: ExtraMCAssets
 
 
 class NiceMysticCode(BaseModelORJson):
     id: int
     name: str
+    shortName: str
     originalName: str
     detail: str
     maxLv: int
     extraAssets: ExtraMCAssets
     skills: list[NiceSkill]
     expRequired: list[int]
     costumes: list[NiceMysticCodeCostume]
```

### Comparing `fgo_api_types-2024.3.9.2.57.16/fgo_api_types/raw.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 class MstFunc(BaseModelORJson):
     vals: list[int]  # [208],
     expandedVals: list[BuffEntityNoReverse] = []
     tvals: list[int]  # [106],
     questTvals: list[int]  # [94000015],
     effectList: list[int]  # [332],
     popupTextColor: int  # 2,
+    script: dict[str, Any] | None = None
+    overWriteTvalsList: list[list[int]] | None = None
     id: int  # 657,
     cond: int = 0  # 0,
     funcType: int  # 16,
     targetType: int  # 0,
     applyTarget: int  # 3,
     popupIconId: int  # 302,
     popupText: str  # "STR Up\nvs. Lancer"
@@ -558,14 +560,15 @@
     condUserLv: int  # 1
     maxLv: int  # 10
     maleImageId: int  # 21
     femaleImageId: int  # 22
     imageId: int  # 20
     maleSpellId: int  # 1
     femaleSpellId: int  # 2
+    shortName: str | None = None
 
 
 class MstEquipExp(BaseModelORJson):
     equipId: int  # 160
     lv: int  # 5
     exp: int  # 1218000
     skillLv1: int  # 5
@@ -863,14 +866,15 @@
     id: int
     svtId: int
 
 
 class MstSvtMultiPortrait(BaseModelORJson):
     commonPosition: list[int]
     summonPosition: list[int]
+    withMasterPhotoPosition: list[int] | None = None
     svtId: int
     limitCount: int
     idx: int
     portraitImageId: int
     displayPriority: int
 
 
@@ -1237,14 +1241,15 @@
     targetId: int
     isRare: bool
     iconId: int
     bannerId: int
     priority: int
     maxNum: int
     detail: str
+    boxGachaTalkId: list[int] | None = None
 
 
 class MstBoxGachaTalk(BaseModelORJson):
     befVoiceIds: list[str]
     aftVoiceIds: list[str]
     id: int
     guideImageId: int
@@ -1347,14 +1352,15 @@
     createdAt: int | None = None
 
 
 class MstEventQuest(BaseModelORJson):
     eventId: int
     questId: int
     phase: int
+    isExcepted: int | None = None
     createdAt: int | None = None
 
 
 class MstEventBulletinBoard(BaseModelORJson):
     id: int
     eventId: int
     message: str
@@ -1712,14 +1718,15 @@
     name: str
     objectId: int
     x: float
     y: float
     condTargetType: int
     condTargetId: int
     condTargetNum: int
+    flag: int | None = None
 
 
 class MstSpotAdd(BaseModelORJson):
     spotId: int
     priority: int
     overrideType: int
     targetId: int
@@ -1821,25 +1828,28 @@
     condId: int
     condNum: int
     closedMessageId: int
     overlayClosedMessage: str
     eventId: int
     startedAt: int
     endedAt: int
+    leftIndent: int | None = None
 
 
 class MstQuestConsumeItem(BaseModelORJson):
     itemIds: list[int]  # [94032205, 94032206]
     nums: list[int]  # [160, 220]
     questId: int  # 94032410
 
 
 class MstClosedMessage(BaseModelORJson):
     id: int
     message: str
+    leftIndent: int | None = None
+    flag: int | None = None
 
 
 class MstBattleMessage(BaseModelORJson):
     id: int
     idx: int
     priority: int
     commonReleaseId: int
```

### Comparing `fgo_api_types-2024.3.9.2.57.16/fgo_api_types/rayshift.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.3.9.2.57.16/fgo_api_types/search.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.3.9.2.57.16/pyproject.toml` & `fgo_api_types-2024.4.6.2.22.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2024.03.09.02.57.16"
+version = "2024.04.06.02.22.03"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2024.3.9.2.57.16/PKG-INFO` & `fgo_api_types-2024.4.6.2.22.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2024.3.9.2.57.16
+Version: 2024.4.6.2.22.3
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

