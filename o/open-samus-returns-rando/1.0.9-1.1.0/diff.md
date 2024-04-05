# Comparing `tmp/open_samus_returns_rando-1.0.9.tar.gz` & `tmp/open_samus_returns_rando-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_samus_returns_rando-1.0.9.tar", last modified: Thu Feb 22 16:46:24 2024, max compression
+gzip compressed data, was "open_samus_returns_rando-1.1.0.tar", last modified: Fri Apr  5 23:42:24 2024, max compression
```

## Comparing `open_samus_returns_rando-1.0.9.tar` & `open_samus_returns_rando-1.1.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.768037 open_samus_returns_rando-1.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.748037 open_samus_returns_rando-1.0.9/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.748037 open_samus_returns_rando-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-02-22 16:46:24.768037 open_samus_returns_rando-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 16:46:24.768037 open_samus_returns_rando-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.744037 open_samus_returns_rando-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.752037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.752037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/__pyinstaller/hook-open_samus_returns_rando.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.752037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.752037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/doors.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/guilib.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/heatzone.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/room_names.lua
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/savestation.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/scenario.lua
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/ship.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.756037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/
--rw-r--r--   0 runner    (1001) docker     (127)    26256 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s000_surface.lua
--rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s010_area1.lua
--rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s020_area2.lua
--rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s025_area2b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s028_area2c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    27077 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s030_area3.lua
--rw-r--r--   0 runner    (1001) docker     (127)    40471 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s033_area3b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    22969 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s036_area3c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    29891 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s040_area4.lua
--rw-r--r--   0 runner    (1001) docker     (127)    34499 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s050_area5.lua
--rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s060_area6.lua
--rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s065_area6b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    18231 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s067_area6c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    41935 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s070_area7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s090_area9.lua
--rw-r--r--   0 runner    (1001) docker     (127)    39148 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s100_area10.lua
--rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.760038 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerbabyhatchling.lua
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerenergyshield.lua
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerenergywave.lua
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerphasedisplacement.lua
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerreservetankm.lua
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerscanningpulse.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizersuit.lua
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.744037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.744037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.744037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.744037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.760038 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.760038 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.744037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.744037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.744037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.760038 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    43927 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    21015 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.764037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/cc_to_room_name.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/chozoseal_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/cosmetics.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/custom_init.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/metroid_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/progressive_model_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15612 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/lua_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.764037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/collision_camera_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/exefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/spawn_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/text_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/patch_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.764037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/pickups/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/pickups/custom_pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/pickups/model_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/pickups/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/samus_returns_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.768037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/door_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/game_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/heat_room_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/hint_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/map_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/metroid_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/static_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/tunable_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-22 16:46:24.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.768037 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-02-22 16:46:24.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-02-22 16:46:24.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 16:46:24.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 16:46:24.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-22 16:46:24.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-22 16:46:24.000000 open_samus_returns_rando-1.0.9/src/open_samus_returns_rando.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.768037 open_samus_returns_rando-1.0.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 16:46:24.768037 open_samus_returns_rando-1.0.9/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/tests/test_files/item_models_test.json
--rw-r--r--   0 runner    (1001) docker     (127)   146805 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/tests/test_files/starter_preset_patcher.json
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-22 16:46:07.000000 open_samus_returns_rando-1.0.9/tests/test_lua_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.713219 open_samus_returns_rando-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.693219 open_samus_returns_rando-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.693219 open_samus_returns_rando-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-05 23:42:24.713219 open_samus_returns_rando-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:42:24.713219 open_samus_returns_rando-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.689219 open_samus_returns_rando-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.693219 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.697219 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/__pyinstaller/hook-open_samus_returns_rando.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.697219 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.697219 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/doors.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/guilib.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/heatzone.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/room_names.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/savestation.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/scenario.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/ship.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.701218 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/
+-rw-r--r--   0 runner    (1001) docker     (127)    26256 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s000_surface.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s010_area1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s020_area2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s025_area2b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s028_area2c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    27509 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s030_area3.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    40894 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s033_area3b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s036_area3c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s040_area4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    34925 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s050_area5.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s060_area6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s065_area6b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18231 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s067_area6c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    41935 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s070_area7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s090_area9.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    39148 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s100_area10.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.705218 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerbabyhatchling.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerenergyshield.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerenergywave.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerphasedisplacement.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerreservetankm.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerscanningpulse.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizersuit.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.689219 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.689219 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.689219 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.689219 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.705218 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.705218 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.689219 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.689219 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.689219 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.705218 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    43927 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    22095 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.705218 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/cc_to_room_name.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/chozoseal_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/cosmetics.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/custom_init.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/metroid_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/progressive_model_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/lua_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.709218 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/collision_camera_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/exefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/spawn_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/text_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.709218 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/pickups/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/pickups/custom_pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/pickups/model_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/pickups/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/samus_returns_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.709218 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/door_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/game_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/heat_room_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/hint_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/map_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/metroid_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/static_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/tunable_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 23:42:24.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.709218 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-05 23:42:24.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-05 23:42:24.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:42:24.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 23:42:24.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 23:42:24.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 23:42:24.000000 open_samus_returns_rando-1.1.0/src/open_samus_returns_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.709218 open_samus_returns_rando-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:42:24.709218 open_samus_returns_rando-1.1.0/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/tests/test_files/item_models_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)   146805 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/tests/test_files/starter_preset_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-05 23:42:15.000000 open_samus_returns_rando-1.1.0/tests/test_lua_util.py
```

### Comparing `open_samus_returns_rando-1.0.9/.github/dependabot.yml` & `open_samus_returns_rando-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/.github/workflows/python.yml` & `open_samus_returns_rando-1.1.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/.gitignore` & `open_samus_returns_rando-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/LICENSE` & `open_samus_returns_rando-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/PKG-INFO` & `open_samus_returns_rando-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_samus_returns_rando
-Version: 1.0.9
+Version: 1.1.0
 Summary: An open source randomizer patcher for Metroid: Samus Returns.
 Project-URL: Homepage, https://github.com/randovania/open-samus-returns-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -22,15 +22,15 @@
 - Pickups
 - Items on Metroids
 - Shuffled DNA/Baby Metroid
 
 ## Installation and Usage
 `pip install open-samus-returns-rando`
 
-You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/src/open-samus-returns-rando/blob/main/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
+You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-samus-returns-rando/blob/main/src/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
 
 The patcher expects a path to an extracted romfs directory of Metroid: Samus Returns as well as the desired output directory. Output files are in a format compatible with either Luma3DS or Citra.
 
 With a JSON file:
 `python -m open-samus-returns-rando --input-path path/to/samus-returns/romfs --output-path path/to/the/output/mod --input-json path/to/patcher-config.json`
 
 ## Development
```

### Comparing `open_samus_returns_rando-1.0.9/README.md` & `open_samus_returns_rando-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 - Pickups
 - Items on Metroids
 - Shuffled DNA/Baby Metroid
 
 ## Installation and Usage
 `pip install open-samus-returns-rando`
 
-You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/src/open-samus-returns-rando/blob/main/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
+You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-samus-returns-rando/blob/main/src/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
 
 The patcher expects a path to an extracted romfs directory of Metroid: Samus Returns as well as the desired output directory. Output files are in a format compatible with either Luma3DS or Citra.
 
 With a JSON file:
 `python -m open-samus-returns-rando --input-path path/to/samus-returns/romfs --output-path path/to/the/output/mod --input-json path/to/patcher-config.json`
 
 ## Development
```

### Comparing `open_samus_returns_rando-1.0.9/pyproject.toml` & `open_samus_returns_rando-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
 write_to = "src/open_samus_returns_rando/version.py"
 
 [tool.ruff]
 line-length = 120
-select = [
+lint.select = [
     "E", "F", "W", "C90", "I", "UP", "C4",
     "RSE",
     "TCH",
     "PTH",
     "COM818", "COM819",
     "ISC",
     "PIE",
@@ -57,11 +57,11 @@
     "PLR0133", "PLR0124",
     "PLW",
 ]
 
 # Version to target for generated code.
 target-version = "py39"
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 # Flag errors (`C901`) whenever the complexity level exceeds 25.
 # Defaults to 10, but we're being very flexible right now
 max-complexity = 25
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/cli.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/constants.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/constants.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/debug.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/debug.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/doors.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/doors.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/guilib.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/guilib.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/heatzone.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/heatzone.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/room_names.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/room_names.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/savestation.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/savestation.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/scenario.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/scenario.lua`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,17 @@
 end
 
 function Scenario.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
   Scenario.UpdateProgressiveItemModels()
   Scenario.UpdateRoomName(new_subarea)
 end
 
-function Scenario.SetMetroidSpawngroupOnCurrentScenario(created_actor, group_name, is_multi)
+function Scenario.SetMetroidSpawngroupOnCurrentScenario(created_actor, group_name)
   if created_actor ~= nil and created_actor.sName ~= nil then
     CurrentScenario.currentMetroidSpawngroup = group_name
-    CurrentScenario.isMultiGamma = is_multi or false
   end
 end
 
 function Scenario.InitGUI()
   Cosmetics.UpdateGUI()
   GUILib.AddDNACounter()
   GUILib.UpdateTotalDNAColor()
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/custom/ship.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/custom/ship.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s000_surface.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s000_surface.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s010_area1.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s010_area1.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s020_area2.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s020_area2.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s025_area2b.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s025_area2b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s028_area2c.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s028_area2c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s030_area3.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s030_area3.lua`

 * *Files 7% similar despite different names*

```diff
@@ -6,130 +6,132 @@
 function s030_area3.main()
   Scenario.InitGUI()
 end
 function s030_area3.GetOnDeathOverrides()
   return {GoToMainMenu = false}
 end
 function s030_area3.OnEnter_SetCheckpoint_Gamma_005()
-  Game.SetBossCheckPointNames("ST_SG_Gamma_005", "ST_SG_Gamma_005", "SG_Gamma_005_A", "SG_Gamma_005_B", "SG_Gamma_005_C")
-end
-function s030_area3.OnGamma_005_A_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_005", "A")
-end
-function s030_area3.OnGamma_005_Intro_A_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_005_Intro_A") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_005_Intro_A").ANIMATION:SetAction("spawn")
-  end
-  s030_area3.OnGamma_005_A_Generated(_ARG_0_, _ARG_1_)
-end
-function s030_area3.OnGamma_005_A_Generated(_ARG_0_, _ARG_1_)
-  if _ARG_1_ ~= nil then
-    -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door015")
-    _ARG_1_.AI.bPlaceholder = false
-    _ARG_1_.AI:AddBossCamera("CAM_Gamma")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_A_001")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_A_002")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_A_003")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_A_001")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_A_002")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_A_003")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma005_A_001")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma005_A_002")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma005_A_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_A_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_A_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_A_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_A_mines_004")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_A_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_A_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_A_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_A_mines_004")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_A_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_A_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_A_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_A_mines_004")
-    _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma005_A_Idle")
-    Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
-    if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_A_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_A_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-    if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_A_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_A_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-  end
-end
-function s030_area3.OnGamma_005_B_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_005", "B")
-end
-function s030_area3.OnGamma_005_Intro_B_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_005_Intro_B") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_005_Intro_B").ANIMATION:SetAction("spawn")
-  end
-  s030_area3.OnGamma_005_B_Generated(_ARG_0_, _ARG_1_)
-end
-function s030_area3.OnGamma_005_B_Generated(_ARG_0_, _ARG_1_)
-  if _ARG_1_ ~= nil then
-    -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door015")
-    _ARG_1_.AI.bPlaceholder = false
-    _ARG_1_.AI:AddBossCamera("CAM_Gamma")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_B_003")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_B_003")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma005_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma005_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_B_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_B_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_B_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_B_mines_003")
-    _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma005_B_Idle")
-    Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
-    if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_B_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_B_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-    if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_B_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_B_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-  end
+  Game.SetBossCheckPointNames("ST_SG_Gamma_005", "ST_SG_Gamma_005", "", "", "SG_Gamma_005_C")
 end
+-- function s030_area3.OnGamma_005_A_Trigger()
+--   Gamma.OnMultiArenaTrigger("Gamma_005", "A")
+-- end
+-- function s030_area3.OnGamma_005_Intro_A_Generated(_ARG_0_, _ARG_1_)
+--   if Game.GetEntity("LE_Valve_Gamma_005_Intro_A") ~= nil then
+--     Game.GetEntity("LE_Valve_Gamma_005_Intro_A").ANIMATION:SetAction("spawn")
+--   end
+--   s030_area3.OnGamma_005_A_Generated(_ARG_0_, _ARG_1_)
+-- end
+-- function s030_area3.OnGamma_005_A_Generated(_ARG_0_, _ARG_1_)
+--   if _ARG_1_ ~= nil then
+--     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door015")
+--     _ARG_1_.AI.bPlaceholder = false
+--     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_A_001")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_A_002")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_A_003")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_A_001")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_A_002")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_A_003")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma005_A_001")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma005_A_002")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma005_A_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_A_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_A_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_A_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_A_mines_004")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_A_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_A_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_A_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_A_mines_004")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_A_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_A_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_A_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_A_mines_004")
+--     _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma005_A_Idle")
+--     Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_A_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_A_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_A_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_A_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--   end
+-- end
+-- function s030_area3.OnGamma_005_B_Trigger()
+--   Gamma.OnMultiArenaTrigger("Gamma_005", "B")
+-- end
+-- function s030_area3.OnGamma_005_Intro_B_Generated(_ARG_0_, _ARG_1_)
+--   if Game.GetEntity("LE_Valve_Gamma_005_Intro_B") ~= nil then
+--     Game.GetEntity("LE_Valve_Gamma_005_Intro_B").ANIMATION:SetAction("spawn")
+--   end
+--   s030_area3.OnGamma_005_B_Generated(_ARG_0_, _ARG_1_)
+-- end
+-- function s030_area3.OnGamma_005_B_Generated(_ARG_0_, _ARG_1_)
+--   if _ARG_1_ ~= nil then
+--     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door015")
+--     _ARG_1_.AI.bPlaceholder = false
+--     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_B_003")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_B_003")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma005_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma005_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma005_B_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma005_B_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma005_B_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma005_B_mines_003")
+--     _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma005_B_Idle")
+--     Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_B_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_B_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_B_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_005_B_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--   end
+-- end
 function s030_area3.OnGamma_005_C_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_005", "C")
+  if Game.GetEntity("SG_Gamma_005_C") ~= nil and Scenario.ReadFromBlackboard("entity_TG_Gamma_005_C_enabled", true) then
+    Game.GetEntity("SG_Gamma_005_C").SPAWNGROUP:EnableSpawnGroup()
+  end
 end
 function s030_area3.OnGamma_005_Intro_C_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_005_C_002") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_005_C_002").ANIMATION:SetAction("spawn")
-  end
+  -- if Game.GetEntity("LE_Valve_Gamma_005_C_002") ~= nil then
+  --   Game.GetEntity("LE_Valve_Gamma_005_C_002").ANIMATION:SetAction("spawn")
+  -- end
   s030_area3.OnGamma_005_C_Generated(_ARG_0_, _ARG_1_)
 end
 function s030_area3.OnGamma_005_C_Generated(_ARG_0_, _ARG_1_)
-  Scenario.SetMetroidSpawngroupOnCurrentScenario(_ARG_0_, "SG_Gamma_005_C", true)
+  Scenario.SetMetroidSpawngroupOnCurrentScenario(_ARG_0_, "SG_Gamma_005_C")
   if _ARG_1_ ~= nil then
     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door015")
     _ARG_1_.AI.bPlaceholder = false
     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_C_001")
     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_C_002")
     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma005_C_003")
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s033_area3b.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s033_area3b.lua`

 * *Files 3% similar despite different names*

```diff
@@ -339,77 +339,79 @@
       Game.GetBoss().AI.bIgnoreAttack = true
     else
       Game.AddSF(0.1, "CurrentScenario.OnEnter_Gamma_003_DisableAttack", "")
     end
   end
 end
 function s033_area3b.OnEnter_SetCheckpoint_Gamma_004()
-  Game.SetBossCheckPointNames("ST_SG_Gamma_004", "ST_SG_Gamma_004", "SG_Gamma_004_A", "SG_Gamma_004_B", "SG_Gamma_004_C")
-end
-function s033_area3b.OnGamma_004_A_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_004", "A")
-end
-function s033_area3b.OnGamma_004_Intro_A_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_004_Intro_A") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_004_Intro_A").ANIMATION:SetAction("spawn")
-  end
-  s033_area3b.OnGamma_004_A_Generated(_ARG_0_, _ARG_1_)
-end
-function s033_area3b.OnGamma_004_A_Generated(_ARG_0_, _ARG_1_)
-  if _ARG_1_ ~= nil then
-    -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door014")
-    _ARG_1_.AI.bPlaceholder = false
-    _ARG_1_.AI:AddBossCamera("CAM_Gamma")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_A_001")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_A_002")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_A_003")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_A_001")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_A_002")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_A_003")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_A_001")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_A_002")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_A_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_A_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_A_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_A_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_A_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_A_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_A_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_A_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_A_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_A_mines_003")
-    _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma004_A_Idle")
-    Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
-    if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_A_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_A_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-    if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_A_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_A_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-  end
+  Game.SetBossCheckPointNames("ST_SG_Gamma_004", "ST_SG_Gamma_004", "", "SG_Gamma_004_B", "")
 end
+-- function s033_area3b.OnGamma_004_A_Trigger()
+--   Gamma.OnMultiArenaTrigger("Gamma_004", "A")
+-- end
+-- function s033_area3b.OnGamma_004_Intro_A_Generated(_ARG_0_, _ARG_1_)
+--   if Game.GetEntity("LE_Valve_Gamma_004_Intro_A") ~= nil then
+--     Game.GetEntity("LE_Valve_Gamma_004_Intro_A").ANIMATION:SetAction("spawn")
+--   end
+--   s033_area3b.OnGamma_004_A_Generated(_ARG_0_, _ARG_1_)
+-- end
+-- function s033_area3b.OnGamma_004_A_Generated(_ARG_0_, _ARG_1_)
+--   if _ARG_1_ ~= nil then
+--     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door014")
+--     _ARG_1_.AI.bPlaceholder = false
+--     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_A_001")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_A_002")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_A_003")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_A_001")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_A_002")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_A_003")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_A_001")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_A_002")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_A_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_A_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_A_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_A_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_A_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_A_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_A_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_A_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_A_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_A_mines_003")
+--     _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma004_A_Idle")
+--     Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_A_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_A_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_A_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_A_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--   end
+-- end
 function s033_area3b.OnGamma_004_B_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_004", "B")
+  if Game.GetEntity("SG_Gamma_004_B") ~= nil and Scenario.ReadFromBlackboard("entity_TG_Gamma_004_B_enabled", true) then
+    Game.GetEntity("SG_Gamma_004_B").SPAWNGROUP:EnableSpawnGroup()
+  end
 end
 function s033_area3b.OnGamma_004_Intro_B_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_004_Intro_B") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_004_Intro_B").ANIMATION:SetAction("spawn")
-  end
+  -- if Game.GetEntity("LE_Valve_Gamma_004_Intro_B") ~= nil then
+  --   Game.GetEntity("LE_Valve_Gamma_004_Intro_B").ANIMATION:SetAction("spawn")
+  -- end
   s033_area3b.OnGamma_004_B_Generated(_ARG_0_, _ARG_1_)
 end
 function s033_area3b.OnGamma_004_B_Generated(_ARG_0_, _ARG_1_)
-  Scenario.SetMetroidSpawngroupOnCurrentScenario(_ARG_0_, "SG_Gamma_004_B", true)
+  Scenario.SetMetroidSpawngroupOnCurrentScenario(_ARG_0_, "SG_Gamma_004_B")
   if _ARG_1_ ~= nil then
     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door014")
     _ARG_1_.AI.bPlaceholder = false
     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_B_001")
     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_B_002")
     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_B_003")
@@ -442,64 +444,64 @@
     --   _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_B_002")
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
     -- end
   end
 end
-function s033_area3b.OnGamma_004_C_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_004", "C")
-end
-function s033_area3b.OnGamma_004_Intro_C_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_004_Intro_C") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_004_Intro_C").ANIMATION:SetAction("spawn")
-  end
-  s033_area3b.OnGamma_004_C_Generated(_ARG_0_, _ARG_1_)
-end
-function s033_area3b.OnGamma_004_C_Generated(_ARG_0_, _ARG_1_)
-  if _ARG_1_ ~= nil then
-    -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door014")
-    _ARG_1_.AI.bPlaceholder = false
-    _ARG_1_.AI:AddBossCamera("CAM_Gamma")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_C_001")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_C_002")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_C_003")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_C_001")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_C_002")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_C_003")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_C_001")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_C_002")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_C_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_C_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_C_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_C_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_C_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_C_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_C_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_C_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_C_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_C_mines_003")
-    _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma004_C_Idle")
-    Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
-    if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_C_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_C_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-    if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_C_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_C_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-  end
-end
+-- function s033_area3b.OnGamma_004_C_Trigger()
+--   Gamma.OnMultiArenaTrigger("Gamma_004", "C")
+-- end
+-- function s033_area3b.OnGamma_004_Intro_C_Generated(_ARG_0_, _ARG_1_)
+--   if Game.GetEntity("LE_Valve_Gamma_004_Intro_C") ~= nil then
+--     Game.GetEntity("LE_Valve_Gamma_004_Intro_C").ANIMATION:SetAction("spawn")
+--   end
+--   s033_area3b.OnGamma_004_C_Generated(_ARG_0_, _ARG_1_)
+-- end
+-- function s033_area3b.OnGamma_004_C_Generated(_ARG_0_, _ARG_1_)
+--   if _ARG_1_ ~= nil then
+--     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door014")
+--     _ARG_1_.AI.bPlaceholder = false
+--     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_C_001")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_C_002")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma004_C_003")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_C_001")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_C_002")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma004_C_003")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_C_001")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_C_002")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma004_C_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_C_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_C_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma004_C_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_C_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_C_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma004_C_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_C_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_C_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma004_C_mines_003")
+--     _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma004_C_Idle")
+--     Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_C_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_C_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_C_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_004_C_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--   end
+-- end
 function s033_area3b.OnEnter_Gamma_004_Dead()
   if Scenario.ReadFromBlackboard("Arena_Gamma_004_AllDead", false) then
     Game.SetSubAreaCurrentSetup("collision_camera_033", "PostGamma_004", true)
     Game.SetSubAreaCurrentSetup("collision_camera_034", "PostGamma_004", true)
     Game.SetSubAreaCurrentSetup("collision_camera_035", "PostGamma_004", true)
     Game.DisableTrigger("TG_SetCheckpoint_Gamma_004")
     if Game.GetEntity("SpawnGroup014") ~= nil then
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s036_area3c.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s036_area3c.lua`

 * *Files 4% similar despite different names*

```diff
@@ -209,27 +209,29 @@
     Game.SetSubAreaCurrentSetup("collision_camera_030", "PostGamma_006", true)
     if Game.GetEntity("SpawnGroup007") ~= nil then
       Game.GetEntity("SpawnGroup007").SPAWNGROUP:EnableSpawnGroup()
     end
   end
 end
 function s036_area3c.OnGamma_007_A_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_007", "A")
+  if Game.GetEntity("SG_Gamma_007_A") ~= nil and Scenario.ReadFromBlackboard("entity_TG_Gamma_007_A_enabled", true) then
+    Game.GetEntity("SG_Gamma_007_A").SPAWNGROUP:EnableSpawnGroup()
+  end
 end
 function s036_area3c.OnGamma_007_Intro_A_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_007_Intro_A") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_007_Intro_A").ANIMATION:SetAction("spawn")
-  end
+  -- if Game.GetEntity("LE_Valve_Gamma_007_Intro_A") ~= nil then
+  --   Game.GetEntity("LE_Valve_Gamma_007_Intro_A").ANIMATION:SetAction("spawn")
+  -- end
   s036_area3c.OnGamma_007_A_Generated(_ARG_0_, _ARG_1_)
 end
 function s036_area3c.OnEnter_SetCheckpoint_001_Gamma_007()
-  Game.SetBossCheckPointNames("ST_SG_Gamma_007", "ST_SG_Gamma_007", "SG_Gamma_007_A", "SG_Gamma_007_B", "SG_Gamma_007_C")
+  Game.SetBossCheckPointNames("ST_SG_Gamma_007", "ST_SG_Gamma_007", "SG_Gamma_007_A", "", "")
 end
 function s036_area3c.OnGamma_007_A_Generated(_ARG_0_, _ARG_1_)
-  Scenario.SetMetroidSpawngroupOnCurrentScenario(_ARG_0_, "SG_Gamma_007_A", true)
+  Scenario.SetMetroidSpawngroupOnCurrentScenario(_ARG_0_, "SG_Gamma_007_A")
   if _ARG_1_ ~= nil then
     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door006")
     _ARG_1_.AI.bPlaceholder = false
     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
     _ARG_1_.AI:AddBossCameraCeilingLandmark("LM_Gamma_007A_Ceiling")
     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma007_A_001")
     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma007_A_002")
@@ -266,65 +268,65 @@
     --   _ARG_1_.AI:AddValve("LE_Valve_Gamma_007_A_002")
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
     -- end
   end
 end
-function s036_area3c.OnGamma_007_B_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_007", "B")
-end
-function s036_area3c.OnGamma_007_Intro_B_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_007_Intro_B") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_007_Intro_B").ANIMATION:SetAction("spawn")
-  end
-  s036_area3c.OnGamma_007_B_Generated(_ARG_0_, _ARG_1_)
-end
-function s036_area3c.OnGamma_007_B_Generated(_ARG_0_, _ARG_1_)
-  if _ARG_1_ ~= nil then
-    -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door006")
-    _ARG_1_.AI.bPlaceholder = false
-    _ARG_1_.AI:AddBossCamera("CAM_Gamma")
-    _ARG_1_.AI:AddBossCameraCeilingLandmark("LM_Gamma_007B_Ceiling")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma007_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma007_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma007_B_003")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma007_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma007_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma007_B_003")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma007_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma007_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma007_B_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma007_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma007_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma007_B_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma007_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma007_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma007_B_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma007_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma007_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma007_B_mines_003")
-    _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma007_B_Idle")
-    Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
-    if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_007_B_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_007_B_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-    if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_007_B_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_007_B_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-  end
-end
+-- function s036_area3c.OnGamma_007_B_Trigger()
+--   Gamma.OnMultiArenaTrigger("Gamma_007", "B")
+-- end
+-- function s036_area3c.OnGamma_007_Intro_B_Generated(_ARG_0_, _ARG_1_)
+--   if Game.GetEntity("LE_Valve_Gamma_007_Intro_B") ~= nil then
+--     Game.GetEntity("LE_Valve_Gamma_007_Intro_B").ANIMATION:SetAction("spawn")
+--   end
+--   s036_area3c.OnGamma_007_B_Generated(_ARG_0_, _ARG_1_)
+-- end
+-- function s036_area3c.OnGamma_007_B_Generated(_ARG_0_, _ARG_1_)
+--   if _ARG_1_ ~= nil then
+--     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door006")
+--     _ARG_1_.AI.bPlaceholder = false
+--     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
+--     _ARG_1_.AI:AddBossCameraCeilingLandmark("LM_Gamma_007B_Ceiling")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma007_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma007_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma007_B_003")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma007_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma007_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma007_B_003")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma007_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma007_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma007_B_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma007_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma007_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma007_B_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma007_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma007_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma007_B_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma007_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma007_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma007_B_mines_003")
+--     _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma007_B_Idle")
+--     Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_007_B_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_007_B_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_007_B_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_007_B_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--   end
+-- end
 function s036_area3c.OnEnter_Gamma_007_Dead()
   if Scenario.ReadFromBlackboard("Arena_Gamma_007_AllDead", false) then
     Game.SetSubAreaCurrentSetup("collision_camera_013", "PostGamma_007", true)
     Game.SetSubAreaCurrentSetup("collision_camera_027", "PostGamma_007", true)
     if Game.GetEntity("SpawnGroup008") ~= nil then
       Game.GetEntity("SpawnGroup008").SPAWNGROUP:EnableSpawnGroup()
     end
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s040_area4.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s040_area4.lua`

 * *Files 8% similar despite different names*

```diff
@@ -40,27 +40,29 @@
     Game.SetSubAreaCurrentSetup("collision_camera_007", "PostAlpha_001", true)
     if Game.GetEntity("SpawnGroup018") ~= nil then
       Game.GetEntity("SpawnGroup018").SPAWNGROUP:EnableSpawnGroup()
     end
   end
 end
 function s040_area4.OnEnter_SetCheckpoint_Gamma_001()
-  Game.SetBossCheckPointNames("ST_SG_Gamma_001", "ST_SG_Gamma_001", "SG_Gamma_001_A", "SG_Gamma_001_B", "SG_Gamma_001_C")
+  Game.SetBossCheckPointNames("ST_SG_Gamma_001", "ST_SG_Gamma_001", "SG_Gamma_001_A", "", "")
 end
 function s040_area4.OnGamma_001_A_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_001", "A")
+  if Game.GetEntity("SG_Gamma_001_A") ~= nil and Scenario.ReadFromBlackboard("entity_TG_Gamma_001_A_enabled", true)  then
+    Game.GetEntity("SG_Gamma_001_A").SPAWNGROUP:EnableSpawnGroup()
+  end
 end
 function s040_area4.OnGamma_001_Intro_A_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_001_Intro_A") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_001_Intro_A").ANIMATION:SetAction("spawn")
-  end
+  -- if Game.GetEntity("LE_Valve_Gamma_001_Intro_A") ~= nil then
+  --   Game.GetEntity("LE_Valve_Gamma_001_Intro_A").ANIMATION:SetAction("spawn")
+  -- end
   s040_area4.OnGamma_001_A_Generated(_ARG_0_, _ARG_1_)
 end
 function s040_area4.OnGamma_001_A_Generated(_ARG_0_, _ARG_1_)
-  Scenario.SetMetroidSpawngroupOnCurrentScenario(_ARG_0_, "SG_Gamma_001_A", true)
+  Scenario.SetMetroidSpawngroupOnCurrentScenario(_ARG_0_, "SG_Gamma_001_A")
   if _ARG_1_ ~= nil then
     -- _ARG_1_.AI:AddBossDoor("Door011")
     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door004")
     Game.DisableTrigger("TG_SetCheckpoint_Gamma_001")
     _ARG_1_.AI.bPlaceholder = false
     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_A_001")
@@ -95,116 +97,116 @@
     --   _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_A_002")
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
     -- end
   end
 end
-function s040_area4.OnGamma_001_B_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_001", "B")
-end
-function s040_area4.OnGamma_001_Intro_B_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_001_B_002") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_001_B_002").ANIMATION:SetAction("spawn")
-  end
-  s040_area4.OnGamma_001_B_Generated(_ARG_0_, _ARG_1_)
-end
-function s040_area4.OnGamma_001_B_Generated(_ARG_0_, _ARG_1_)
-  if _ARG_1_ ~= nil then
-    -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door004")
-    _ARG_1_.AI.bPlaceholder = false
-    _ARG_1_.AI:AddBossCamera("CAM_Gamma")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_B_003")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_B_003")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_B_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_B_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_B_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_B_mines_003")
-    _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma001_B_Idle")
-    Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
-    if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_B_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_B_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-    if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_B_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_B_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-  end
-end
-function s040_area4.OnGamma_001_C_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_001", "C")
-end
-function s040_area4.OnGamma_001_Intro_C_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_001_Intro_C") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_001_Intro_C").ANIMATION:SetAction("spawn")
-  end
-  s040_area4.OnGamma_001_C_Generated(_ARG_0_, _ARG_1_)
-end
-function s040_area4.OnGamma_001_C_Generated(_ARG_0_, _ARG_1_)
-  if _ARG_1_ ~= nil then
-    -- _ARG_1_.AI:AddBossDoor("Door010")
-    -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door004")
-    _ARG_1_.AI.bPlaceholder = false
-    _ARG_1_.AI:AddBossCamera("CAM_Gamma")
-    _ARG_1_.AI:AddBossCameraFloorLandmark("LM_Gamma_001_C")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_C_001")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_C_002")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_C_003")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_C_001")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_C_002")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_C_003")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_C_001")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_C_002")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_C_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_C_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_C_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_C_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_C_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_C_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_C_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_C_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_C_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_C_mines_003")
-    _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma001_C_Idle")
-    Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
-    if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_C_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_C_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-    if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_C_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_C_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-  end
-end
+-- function s040_area4.OnGamma_001_B_Trigger()
+--   Gamma.OnMultiArenaTrigger("Gamma_001", "B")
+-- end
+-- function s040_area4.OnGamma_001_Intro_B_Generated(_ARG_0_, _ARG_1_)
+--   if Game.GetEntity("LE_Valve_Gamma_001_B_002") ~= nil then
+--     Game.GetEntity("LE_Valve_Gamma_001_B_002").ANIMATION:SetAction("spawn")
+--   end
+--   s040_area4.OnGamma_001_B_Generated(_ARG_0_, _ARG_1_)
+-- end
+-- function s040_area4.OnGamma_001_B_Generated(_ARG_0_, _ARG_1_)
+--   if _ARG_1_ ~= nil then
+--     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door004")
+--     _ARG_1_.AI.bPlaceholder = false
+--     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_B_003")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_B_003")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_B_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_B_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_B_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_B_mines_003")
+--     _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma001_B_Idle")
+--     Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_B_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_B_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_B_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_B_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--   end
+-- end
+-- function s040_area4.OnGamma_001_C_Trigger()
+--   Gamma.OnMultiArenaTrigger("Gamma_001", "C")
+-- end
+-- function s040_area4.OnGamma_001_Intro_C_Generated(_ARG_0_, _ARG_1_)
+--   if Game.GetEntity("LE_Valve_Gamma_001_Intro_C") ~= nil then
+--     Game.GetEntity("LE_Valve_Gamma_001_Intro_C").ANIMATION:SetAction("spawn")
+--   end
+--   s040_area4.OnGamma_001_C_Generated(_ARG_0_, _ARG_1_)
+-- end
+-- function s040_area4.OnGamma_001_C_Generated(_ARG_0_, _ARG_1_)
+--   if _ARG_1_ ~= nil then
+--     -- _ARG_1_.AI:AddBossDoor("Door010")
+--     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door004")
+--     _ARG_1_.AI.bPlaceholder = false
+--     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
+--     _ARG_1_.AI:AddBossCameraFloorLandmark("LM_Gamma_001_C")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_C_001")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_C_002")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma001_C_003")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_C_001")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_C_002")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma001_C_003")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_C_001")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_C_002")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma001_C_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_C_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_C_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma001_C_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_C_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_C_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma001_C_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_C_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_C_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma001_C_mines_003")
+--     _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma001_C_Idle")
+--     Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_C_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_C_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_C_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_001_C_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--   end
+-- end
 function s040_area4.OnEnter_Gamma_001_Dead()
   if Scenario.ReadFromBlackboard("Arena_Gamma_001_AllDead", false) then
     Game.SetSubAreaCurrentSetup("collision_camera_005", "PostGamma_001", true)
     Game.SetSubAreaCurrentSetup("collision_camera_012", "PostGamma_001", true)
     Game.SetSubAreaCurrentSetup("collision_camera_013", "PostGamma_001", true)
     if Game.GetEntity("SpawnGroup019") ~= nil then
       Game.GetEntity("SpawnGroup019").SPAWNGROUP:EnableSpawnGroup()
@@ -213,23 +215,14 @@
       Game.GetEntity("SpawnGroup020").SPAWNGROUP:EnableSpawnGroup()
     end
     if Game.GetEntity("SpawnGroup021") ~= nil then
       Game.GetEntity("SpawnGroup021").SPAWNGROUP:EnableSpawnGroup()
     end
   end
 end
-function s040_area4.DelayedWarp()
-  Game.SetPlayerInputEnabled(false, true)
-  Game.FadeIn(2.5)
-  Game.GetPlayer().vPos = InitialPosition
-  Game.AddSF(1.5, "s040_area4.DelayedInput", "")
-end
-function s040_area4.DelayedInput()
-  Game.SetPlayerInputEnabled(true, true)
-end
 s040_area4.tDNAScanLandmarks = {
   SG_Alpha_001 = {
     "LM_ADNScanner_Samus_Alpha_001_001",
     "LM_ADNScanner_Samus_Alpha_001_002",
     "LM_ADNScanner_Samus_Alpha_001_003",
     "LM_ADNScanner_Samus_Alpha_001_004",
     "LM_ADNScanner_Samus_Alpha_001_005",
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s050_area5.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s050_area5.lua`

 * *Files 3% similar despite different names*

```diff
@@ -111,27 +111,29 @@
 end
 function s050_area5.OnExit()
 end
 function s050_area5.OnEnter_ActivationTeleport_05_01()
   Game.OnTeleportApproached("LE_Teleporter_05_01")
 end
 function s050_area5.OnEnter_SetCheckpoint_Gamma_002()
-  Game.SetBossCheckPointNames("ST_SG_Gamma_002", "ST_SG_Gamma_002", "SG_Gamma_002_A", "SG_Gamma_002_B", "SG_Gamma_002_C")
+  Game.SetBossCheckPointNames("ST_SG_Gamma_002", "ST_SG_Gamma_002", "SG_Gamma_002_A", "", "")
 end
 function s050_area5.OnGamma_002_A_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_002", "A")
+  if Game.GetEntity("SG_Gamma_002_A") ~= nil and Scenario.ReadFromBlackboard("entity_TG_Gamma_002_A_enabled", true) then
+    Game.GetEntity("SG_Gamma_002_A").SPAWNGROUP:EnableSpawnGroup()
+  end
 end
 function s050_area5.OnGamma_002_Intro_A_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_002_Intro_A") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_002_Intro_A").ANIMATION:SetAction("spawn")
-  end
+  -- if Game.GetEntity("LE_Valve_Gamma_002_Intro_A") ~= nil then
+  --   Game.GetEntity("LE_Valve_Gamma_002_Intro_A").ANIMATION:SetAction("spawn")
+  -- end
   s050_area5.OnGamma_002_A_Generated(_ARG_0_, _ARG_1_)
 end
 function s050_area5.OnGamma_002_A_Generated(_ARG_0_, _ARG_1_)
-  Scenario.SetMetroidSpawngroupOnCurrentScenario(_ARG_0_, "SG_Gamma_002_A", true)
+  Scenario.SetMetroidSpawngroupOnCurrentScenario(_ARG_0_, "SG_Gamma_002_A")
   if _ARG_1_ ~= nil then
     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door014")
     _ARG_1_.AI.bPlaceholder = false
     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
     _ARG_1_.AI:AddBossCameraFloorLandmark("LM_Gamma_002_A")
     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_A_001")
     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_A_002")
@@ -165,115 +167,115 @@
     --   _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_A_002")
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
     --   _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
     -- end
   end
 end
-function s050_area5.OnGamma_002_B_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_002", "B")
-end
-function s050_area5.OnGamma_002_Intro_B_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_002_Intro_B") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_002_Intro_B").ANIMATION:SetAction("spawn")
-  end
-  s050_area5.OnGamma_002_B_Generated(_ARG_0_, _ARG_1_)
-end
-function s050_area5.OnGamma_002_B_Generated(_ARG_0_, _ARG_1_)
-  if _ARG_1_ ~= nil then
-    -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door014")
-    _ARG_1_.AI.bPlaceholder = false
-    _ARG_1_.AI:AddBossCamera("CAM_Gamma")
-    _ARG_1_.AI:AddBossCameraFloorLandmark("LM_Gamma_002_B")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_B_003")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_B_003")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_B_001")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_B_002")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_B_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_B_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_B_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_B_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_B_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_B_mines_003")
-    _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma002_B_Idle_001")
-    Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
-    if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_B_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_B_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-    if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_B_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_B_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-  end
-end
-function s050_area5.OnGamma_002_C_Trigger()
-  Gamma.OnMultiArenaTrigger("Gamma_002", "C")
-end
-function s050_area5.OnGamma_002_Intro_C_Generated(_ARG_0_, _ARG_1_)
-  if Game.GetEntity("LE_Valve_Gamma_002_Intro_C") ~= nil then
-    Game.GetEntity("LE_Valve_Gamma_002_Intro_C").ANIMATION:SetAction("spawn")
-  end
-  s050_area5.OnGamma_002_C_Generated(_ARG_0_, _ARG_1_)
-end
-function s050_area5.OnGamma_002_C_Generated(_ARG_0_, _ARG_1_)
-  if _ARG_1_ ~= nil then
-    -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door014")
-    _ARG_1_.AI.bPlaceholder = false
-    _ARG_1_.AI:AddBossCamera("CAM_Gamma")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_C_001")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_C_002")
-    _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_C_003")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_C_001")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_C_002")
-    _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_C_003")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_C_001")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_C_002")
-    _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_C_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_C_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_C_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_C_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_C_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_C_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_C_mines_003")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_C_mines_001")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_C_mines_002")
-    _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_C_mines_003")
-    _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma002_C_Idle_001")
-    Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
-    if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_C_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_C_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-    if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_C_001")
-      _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_C_002")
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
-      _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
-    end
-  end
-end
+-- function s050_area5.OnGamma_002_B_Trigger()
+--   Gamma.OnMultiArenaTrigger("Gamma_002", "B")
+-- end
+-- function s050_area5.OnGamma_002_Intro_B_Generated(_ARG_0_, _ARG_1_)
+--   if Game.GetEntity("LE_Valve_Gamma_002_Intro_B") ~= nil then
+--     Game.GetEntity("LE_Valve_Gamma_002_Intro_B").ANIMATION:SetAction("spawn")
+--   end
+--   s050_area5.OnGamma_002_B_Generated(_ARG_0_, _ARG_1_)
+-- end
+-- function s050_area5.OnGamma_002_B_Generated(_ARG_0_, _ARG_1_)
+--   if _ARG_1_ ~= nil then
+--     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door014")
+--     _ARG_1_.AI.bPlaceholder = false
+--     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
+--     _ARG_1_.AI:AddBossCameraFloorLandmark("LM_Gamma_002_B")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_B_003")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_B_003")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_B_001")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_B_002")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_B_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_B_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_B_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_B_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_B_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_B_mines_003")
+--     _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma002_B_Idle_001")
+--     Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_B_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_B_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_B_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_B_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--   end
+-- end
+-- function s050_area5.OnGamma_002_C_Trigger()
+--   Gamma.OnMultiArenaTrigger("Gamma_002", "C")
+-- end
+-- function s050_area5.OnGamma_002_Intro_C_Generated(_ARG_0_, _ARG_1_)
+--   if Game.GetEntity("LE_Valve_Gamma_002_Intro_C") ~= nil then
+--     Game.GetEntity("LE_Valve_Gamma_002_Intro_C").ANIMATION:SetAction("spawn")
+--   end
+--   s050_area5.OnGamma_002_C_Generated(_ARG_0_, _ARG_1_)
+-- end
+-- function s050_area5.OnGamma_002_C_Generated(_ARG_0_, _ARG_1_)
+--   if _ARG_1_ ~= nil then
+--     -- _ARG_1_.AI:AddBossDoorUnlockedOnDeath("Door014")
+--     _ARG_1_.AI.bPlaceholder = false
+--     _ARG_1_.AI:AddBossCamera("CAM_Gamma")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_C_001")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_C_002")
+--     _ARG_1_.AI:AddPresetLogicPath(0, "PATH_Gamma002_C_003")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_C_001")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_C_002")
+--     _ARG_1_.AI:AddPresetLogicPath(1, "PATH_Gamma002_C_003")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_C_001")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_C_002")
+--     _ARG_1_.AI:AddPresetLogicPath(2, "PATH_Gamma002_C_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_C_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_C_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(0, "PATH_Gamma002_C_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_C_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_C_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(1, "PATH_Gamma002_C_mines_003")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_C_mines_001")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_C_mines_002")
+--     _ARG_1_.AI:AddElectricMinesLogicPath(2, "PATH_Gamma002_C_mines_003")
+--     _ARG_1_.AI:AddIdleLogicPath("PATH_Gamma002_C_Idle_001")
+--     Gamma.SetArenaLife(_ARG_0_, _ARG_1_)
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 0 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_C_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_C_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.6)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 60)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--     if Gamma.GetNumValveUsed(_ARG_0_) == 1 then
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_C_001")
+--       _ARG_1_.AI:AddValve("LE_Valve_Gamma_002_C_002")
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveLifePct", 0.3)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveTime", 90)
+--       _ARG_1_.AI:AddBlackboardParam("fGotoValveSamusLife", 99)
+--     end
+--   end
+-- end
 function s050_area5.OnEnter_Gamma_002_Dead()
   if Scenario.ReadFromBlackboard("Arena_Gamma_002_AllDead", false) then
     Game.SetSubAreaCurrentSetup("collision_camera_009", "PostGamma_002", true)
     Game.SetSubAreaCurrentSetup("collision_camera_015", "PostGamma_002", true)
     Game.SetSubAreaCurrentSetup("collision_camera_017", "PostGamma_002", true)
     if Game.GetEntity("SpawnGroup019") ~= nil then
       Game.GetEntity("SpawnGroup019").SPAWNGROUP:EnableSpawnGroup()
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s060_area6.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s060_area6.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s065_area6b.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s065_area6b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s067_area6c.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s067_area6c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s070_area7.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s070_area7.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s090_area9.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s090_area9.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s100_area10.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s100_area10.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizersuit.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizersuit.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/schema.json` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9941176470588236%*

 * *Differences: {"'properties'": "{'door_patches': OrderedDict([('type', 'array'), ('description', 'Changes the "*

 * *                 "door types'), ('items', OrderedDict([('type', 'object'), ('properties', "*

 * *                 "OrderedDict([('actor', OrderedDict([('$ref', "*

 * *                 "'#/$defs/actor_reference_with_layer')])), ('door_type', OrderedDict([('type', "*

 * *                 "'string'), ('enum', ['frame', 'power_beam', 'charge_beam', 'spazer_beam', "*

 * *                 "'plasma_beam', 'wave_beam', 'missile', 'super_m […]*

```diff
@@ -331,14 +331,46 @@
                     "location",
                     "collision_camera_name"
                 ],
                 "type": "object"
             },
             "type": "array"
         },
+        "door_patches": {
+            "default": [],
+            "description": "Changes the door types",
+            "items": {
+                "additionalProperties": false,
+                "properties": {
+                    "actor": {
+                        "$ref": "#/$defs/actor_reference_with_layer"
+                    },
+                    "door_type": {
+                        "enum": [
+                            "frame",
+                            "power_beam",
+                            "charge_beam",
+                            "spazer_beam",
+                            "plasma_beam",
+                            "wave_beam",
+                            "missile",
+                            "super_missile",
+                            "power_bomb"
+                        ],
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "actor",
+                    "door_type"
+                ],
+                "type": "object"
+            },
+            "type": "array"
+        },
         "elevators": {
             "items": {
                 "properties": {
                     "destination": {
                         "$ref": "#/$defs/actor_reference"
                     },
                     "teleporter": {
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/chozoseal_template.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/chozoseal_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/cosmetics.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/cosmetics.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/custom_init.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/custom_init.lua`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,17 @@
   })
   for _FORV_3_, _FORV_4_ in pairs(Init.tNewGameInventory) do
     Blackboard.SetProp("PLAYER_INVENTORY", _FORV_3_, "f", _FORV_4_)
     if string.sub(_FORV_3_, 0, 14) == "ITEM_RANDO_DNA" then
       local current_amount = Blackboard.GetProp("PLAYER_INVENTORY", "ITEM_ADN") or 0
       Blackboard.SetProp("PLAYER_INVENTORY", "ITEM_ADN", "f", current_amount + 1)
     end
-    if string.sub(_FORV_3_, 1, 17) == "ITEM_RESERVE_TANK" then
-      if _FORV_3_ ~= "ITEM_RESERVE_TANK_MISSILE" or Blackboard.GetProp("PLAYER_INVENTORY", "ITEM_WEAPON_MISSILE_LAUNCHER") then
+    if string.sub(_FORV_3_, 1, 17) == "ITEM_RESERVE_TANK" and _FORV_4_ > 0 then
+      local missile_launcher = Init.tNewGameInventory["ITEM_WEAPON_MISSILE_LAUNCHER"]
+      if _FORV_3_ ~= "ITEM_RESERVE_TANK_MISSILE" or (missile_launcher ~= nil and missile_launcher > 0) then
         Blackboard.SetProp("GAME", _FORV_3_ .. "_ACTIVE", "b", true)
         Blackboard.SetProp("GAME", _FORV_3_ .. "_FULL", "b", true)
       end
     end
   end
   Blackboard.SetProp("PLAYER_INVENTORY", "ITEM_METROID_COUNT", "f", 0)
   Blackboard.SetProp("PLAYER_INVENTORY", "ITEM_CURRENT_LIFE", "f", Init.tNewGameInventory.ITEM_MAX_LIFE)
@@ -67,14 +68,15 @@
 
 function Init.InitNewGame(arg1, arg2, arg3, arg4, arg4)
     Init.tBoxesSeen = 0
     Game.LoadScenario("c10_samus", Init.sStartingScenario, Init.sStartingActor, "samus", 1)
     if Init.bRevealMap then
       Game.AddGUISF(0.0, Game.ScanVisitDiscoverEverything, "", "")
     end
+    Game.SaveGame("savedata", "", Init.sStartingActor, true)
   end
 
 Game.SetForceSkipCutscenes(true)
 
 -- Only required for ils test code
 -- ALL_SCENARIOS = {
 --   "s000_surface",
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/metroid_template.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/metroid_template.lua`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,49 @@
 Metroid = Metroid or {}
 function Metroid.Dummy()
 end
 
-function Metroid.DisableSpawnGroup(spawnGroupName)
-    local spawnGroup = Game.GetEntity(spawnGroupName)
-    if spawnGroup ~= nil and spawnGroup.SPAWNGROUP ~= nil then
-        spawnGroup.SPAWNGROUP:DisableSpawnGroup()
-        Scenario.WriteToBlackboard("entity_" .. spawnGroupName .. "_dead", "b", true)
-        Scenario.WriteToBlackboard("entity_" .. spawnGroupName .. "_deaths", "i", 1)
-        Scenario.WriteToBlackboard("entity_" .. spawnGroupName .. "_enabled", "b", false)
-    end
-end
-
-function Metroid.DelayedDelete(spawnGroupName)
-    Game.DeleteEntity(spawnGroupName)
-    if spawnGroupName == "SG_Gamma_001_A" then
-        InitialPosition = Game.GetPlayer().vPos
-        Game.GetPlayer().vPos = Game.GetEntity("ST_SG_Gamma_001").vPos
-        Game.SetPlayerInputEnabled(false, true)
-        Game.AddSF(0.5, "s040_area4.DelayedWarp", "")
-        CurrentScenario.OnEnter_Gamma_001_Dead()
-    elseif spawnGroupName == "SG_Gamma_002_A" then
-        CurrentScenario.OnEnter_Gamma_002_Dead()
-    elseif spawnGroupName == "SG_Gamma_004_B" then
-        CurrentScenario.OnEnter_Gamma_004_Dead()
-    elseif spawnGroupName == "SG_Gamma_005_C" then
-        CurrentScenario.OnEnter_Gamma_005_Dead()
-    elseif spawnGroupName == "SG_Gamma_007_A" then
-        CurrentScenario.OnEnter_Gamma_007_Dead()
-    end
-    -- TODO: Add proper checkpoints
-end
-
 function Metroid.RemoveMetroid(_ARG_0_)
     local spawnGroupName = CurrentScenario.currentMetroidSpawngroup
     if spawnGroupName ~= nil then
-        -- disable all spawn groups in case of multi arena gamma
-        if CurrentScenario.isMultiGamma then
-            local endingLetters = {"A", "B", "C"}
-            for index, letter in pairs(endingLetters) do
-                local otherSpawnGroupName = string.sub(spawnGroupName, 0, -2) .. letter
-                Metroid.DisableSpawnGroup(otherSpawnGroupName)
-            end
+        -- disable multi arena gamma spawngroups
+        if #spawnGroupName == 14 then
             local allDead = "Arena_" .. string.sub(spawnGroupName, 4, -3) .. "_AllDead"
-            Scenario.WriteToBlackboard(allDead, "b", true)
-            if spawnGroupName == "SG_Gamma_001_A" then
-                Game.SetPlayerInputEnabled(false, true)
+            local gamma = string.sub(spawnGroupName, 10, 14)
+            if spawnGroupName == "SG_Gamma_" .. gamma then
+                Scenario.WriteToBlackboard("entity_" .. "TG_Gamma_" .. gamma .."_enabled", "b", false)
             end
-            Game.AddSF(4.0, "Metroid.DelayedDelete", "s", spawnGroupName)
-        -- disable single arena metroid
-        else
-            Metroid.DisableSpawnGroup(spawnGroupName)
+            Scenario.WriteToBlackboard(allDead, "b", true)
+        end
+
+        local spawnGroup = Game.GetEntity(spawnGroupName)
+        if spawnGroup ~= nil and spawnGroup.SPAWNGROUP ~= nil then
+            spawnGroup.SPAWNGROUP:DisableSpawnGroup()
+            Scenario.WriteToBlackboard("entity_" .. spawnGroupName .. "_dead", "b", true)
+            Scenario.WriteToBlackboard("entity_" .. spawnGroupName .. "_deaths", "i", 1)
+            Scenario.WriteToBlackboard("entity_" .. spawnGroupName .. "_enabled", "b", false)
         end
 
         local count = Game.GetItemAmount(Game.GetPlayerName(), "ITEM_METROID_COUNT") + 1
         Game.SetItemAmount(Game.GetPlayerName(), "ITEM_METROID_COUNT", count)
         Game.IncrementMetroidTotalCount(0)
 
         local scenario = Scenario.CurrentScenarioID
         if scenario ~= nil and Metroid.Pickups ~= nil and
                 Metroid.Pickups[scenario] ~= nil and
                 Metroid.Pickups[scenario][spawnGroupName] ~= nil and
                 Metroid.Pickups[scenario][spawnGroupName].OnPickedUp ~= nil then
             Metroid.Pickups[scenario][spawnGroupName].OnPickedUp()
         end
         Game.SetInGameMusicState("RELAX")
-        if not CurrentScenario.isMultiGamma then
-            Game.SaveGame("checkpoint", "AfterNewAbilityAcquired", "", true)
-        end
         if scenario == "s000_surface" then
             Game.DisableEntity("TG_Intro_Alpha")
             Scenario.WriteToBlackboard("alpha_killed", "b", true)
         end
+        Game.SaveGame("checkpoint", "AfterNewAbilityAcquired", "", true)
     else
         GUI.LaunchMessage("Oops 2", "Metroid.Dummy", "")
     end
     CurrentScenario.currentMetroidSpawngroup = nil
-    CurrentScenario.isMultiGamma = nil
 end
 
 Metroid.Pickups = TEMPLATE("mapping")
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/lua_editor.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/lua_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,14 +207,15 @@
 
         # increase starting HP if starting with etanks
         if "ITEM_ENERGY_TANKS" in inventory:
             etanks = inventory.pop("ITEM_ENERGY_TANKS")
             max_life += etanks * energy_per_tank
 
         # use _MAX if main is unlocked to unlock the ammo too
+        # FIXME: These checks are kinda wrong if you use something like `"ITEM_WEAPON_MISSILE_LAUNCHER": 0`
         if "ITEM_WEAPON_MISSILE_LAUNCHER" in inventory and "ITEM_MISSILE_TANKS" in inventory:
             inventory["ITEM_WEAPON_MISSILE_MAX"] = inventory.pop("ITEM_MISSILE_TANKS")
         if "ITEM_WEAPON_SUPER_MISSILE" in inventory and "ITEM_SUPER_MISSILE_TANKS" in inventory:
             inventory["ITEM_WEAPON_SUPER_MISSILE_MAX"] = inventory.pop("ITEM_SUPER_MISSILE_TANKS")
         if "ITEM_WEAPON_POWER_BOMB" in inventory and "ITEM_POWER_BOMB_TANKS" in inventory:
             inventory["ITEM_WEAPON_POWER_BOMB_MAX"] = inventory.pop("ITEM_POWER_BOMB_TANKS")
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/collision_camera_table.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/collision_camera_table.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/credits.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/credits.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/lua_util.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/lua_util.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/spawn_points.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/spawn_points.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/misc_patches/text_patches.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/misc_patches/text_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/patch_util.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/patch_util.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/patcher_editor.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/patcher_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 from construct import Container
 from mercury_engine_data_structures.file_tree_editor import FileTreeEditor
 from mercury_engine_data_structures.formats import BaseResource, Bmsld
 from mercury_engine_data_structures.game_check import Game
 
-from open_samus_returns_rando.constants import ALL_SCENARIOS
+from open_samus_returns_rando.constants import ALL_SCENARIOS, get_package_name
 
 T = typing.TypeVar("T")
 
 
 def path_for_level(level_name: str) -> str:
     return f"maps/levels/c10_samus/{level_name}/{level_name}"
 
@@ -35,15 +35,15 @@
         def get_nested_list():
             for scenario in ALL_SCENARIOS:
                 yield self.get_level_pkgs(scenario)
         return [pkg for all_level_pkgs in get_nested_list() for pkg in all_level_pkgs]
 
     def ensure_present_in_scenario(self, scenario: str, asset):
         for pkg in self.get_level_pkgs(scenario):
-            self.ensure_present(pkg, asset)
+            self.ensure_present(get_package_name(pkg, asset), asset)
 
     def get_scenario(self, name: str) -> Bmsld:
         return self.get_file(path_for_level(name) + ".bmsld", Bmsld)
 
     def resolve_actor_reference(self, ref: dict) -> Container:
         scenario = self.get_scenario(ref["scenario"])
         # FIXME: There is no "default" as layer in SR
@@ -71,8 +71,13 @@
         layer = reference["layer"]
         actor_name = reference["actor"]
 
         scenario.raw.actors[layer].pop(actor_name)
         scenario.remove_actor_from_all_groups(actor_name)
 
     def get_asset_names_in_folder(self, folder: str) -> typing.Iterator[str]:
-        yield from (name for name in self._name_for_asset_id.values() if name.startswith(folder))
+        yield from (
+            name
+            for name in self._name_for_asset_id.values()
+            if name.startswith(folder) and self.does_asset_exists(name)
+        )
+
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/pickups/custom_pickups.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/pickups/custom_pickups.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/pickups/model_data.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/pickups/model_data.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/pickups/pickup.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/pickups/pickup.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/samus_returns_patcher.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/samus_returns_patcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     patch_custom_spawn_points(editor)
     debug_spawn_points(editor, configuration["debug_spawn_points"])
 
     # Fix unheated heat rooms
     patch_heat_rooms(editor)
 
     # Patch door types and make shields on both sides
-    patch_doors(editor)
+    patch_doors(editor, configuration["door_patches"])
 
     # Patch tunables
     tunable_patches.patch_tunables(editor, configuration.get("reserves_per_tank", {}))
 
     # Patch cosmetics
     cosmetic_patches.patch_cosmetics(editor, configuration.get("cosmetic_patches", {}))
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,18 +101,17 @@
     NewChozoSeal(
         "s090_area9", [-5550.0, -3000.0, 0.0], [-5550.0, -3000.0, 0.0], 206, ["collision_camera_016"]
     ),
     NewChozoSeal(
         "s100_area10", [-4100.0, 11200.0, 0.0], [-4100.0, 11200.0, 0.0], 253,
         ["collision_camera_022", "collision_camera_024"]
     ),
-    # Currently breaks Ridley if added :(
-    # NewChozoSeal(
-    #     "s110_surfaceb", [-28150.0, 300.0, 0.0], [-28150.0, 300.0, 0.0], 145, ["collision_camera_017"]
-    # ),
+    NewChozoSeal(
+        "s110_surfaceb", [-28150.0, 300.0, 0.0], [-28150.0, 300.0, 0.0], 145, ["collision_camera_017"]
+    ),
 ]
 
 def add_chozo_seals(editor: PatcherEditor, new_seal: NewChozoSeal):
     template_ap = editor.get_scenario("s000_surface").raw.actors[16]["LE_ChozoUnlockAreaDNA"]
     template_platform = editor.get_scenario("s000_surface").raw.actors[10]["LE_Platform_ChozoUnlockAreaDNA"]
 
     CHOZO_SEAL_ICON = Container({
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/game_patches.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/game_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/heat_room_patches.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/heat_room_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/map_icons.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/map_icons.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/metroid_patches.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/metroid_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/specific_patches/tunable_patches.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/specific_patches/tunable_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando/validator_with_default.py` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando.egg-info/PKG-INFO` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_samus_returns_rando
-Version: 1.0.9
+Version: 1.1.0
 Summary: An open source randomizer patcher for Metroid: Samus Returns.
 Project-URL: Homepage, https://github.com/randovania/open-samus-returns-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -22,15 +22,15 @@
 - Pickups
 - Items on Metroids
 - Shuffled DNA/Baby Metroid
 
 ## Installation and Usage
 `pip install open-samus-returns-rando`
 
-You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/src/open-samus-returns-rando/blob/main/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
+You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-samus-returns-rando/blob/main/src/open_samus_returns_rando/files/schema.json) in order to successfully patch the game.
 
 The patcher expects a path to an extracted romfs directory of Metroid: Samus Returns as well as the desired output directory. Output files are in a format compatible with either Luma3DS or Citra.
 
 With a JSON file:
 `python -m open-samus-returns-rando --input-path path/to/samus-returns/romfs --output-path path/to/the/output/mod --input-json path/to/patcher-config.json`
 
 ## Development
```

### Comparing `open_samus_returns_rando-1.0.9/src/open_samus_returns_rando.egg-info/SOURCES.txt` & `open_samus_returns_rando-1.1.0/src/open_samus_returns_rando.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/tests/test_files/item_models_test.json` & `open_samus_returns_rando-1.1.0/tests/test_files/item_models_test.json`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.0.9/tests/test_files/starter_preset_patcher.json` & `open_samus_returns_rando-1.1.0/tests/test_files/starter_preset_patcher.json`

 * *Files identical despite different names*

