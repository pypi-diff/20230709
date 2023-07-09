# Comparing `tmp/pmdsky_debug_py-7.0.0-py3-none-any.whl.zip` & `tmp/pmdsky_debug_py-7.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 846636 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Jul-08 04:27 pmdsky_debug_py/__init__.py
--rw-r--r--  2.0 unx       30 b- defN 23-Jul-08 04:27 pmdsky_debug_py/_release.py
--rw-r--r--  2.0 unx   778876 b- defN 23-Jul-08 04:27 pmdsky_debug_py/eu.py
--rw-r--r--  2.0 unx   745946 b- defN 23-Jul-08 04:27 pmdsky_debug_py/eu_itcm.py
--rw-r--r--  2.0 unx   766996 b- defN 23-Jul-08 04:27 pmdsky_debug_py/jp.py
--rw-r--r--  2.0 unx   745946 b- defN 23-Jul-08 04:27 pmdsky_debug_py/jp_itcm.py
--rw-r--r--  2.0 unx   786343 b- defN 23-Jul-08 04:27 pmdsky_debug_py/na.py
--rw-r--r--  2.0 unx   745957 b- defN 23-Jul-08 04:27 pmdsky_debug_py/na_itcm.py
--rw-r--r--  2.0 unx   243248 b- defN 23-Jul-08 04:27 pmdsky_debug_py/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 04:27 pmdsky_debug_py/py.typed
--rw-r--r--  2.0 unx     1320 b- defN 23-Jul-08 04:28 pmdsky_debug_py-7.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 04:28 pmdsky_debug_py-7.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-08 04:28 pmdsky_debug_py-7.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1155 b- defN 23-Jul-08 04:28 pmdsky_debug_py-7.0.0.dist-info/RECORD
-14 files, 4817756 bytes uncompressed, 844738 bytes compressed:  82.5%
+Zip file size: 852335 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jul-09 04:27 pmdsky_debug_py/__init__.py
+-rw-r--r--  2.0 unx       30 b- defN 23-Jul-09 04:27 pmdsky_debug_py/_release.py
+-rw-r--r--  2.0 unx   783396 b- defN 23-Jul-09 04:27 pmdsky_debug_py/eu.py
+-rw-r--r--  2.0 unx   750244 b- defN 23-Jul-09 04:27 pmdsky_debug_py/eu_itcm.py
+-rw-r--r--  2.0 unx   771294 b- defN 23-Jul-09 04:27 pmdsky_debug_py/jp.py
+-rw-r--r--  2.0 unx   750244 b- defN 23-Jul-09 04:27 pmdsky_debug_py/jp_itcm.py
+-rw-r--r--  2.0 unx   790641 b- defN 23-Jul-09 04:27 pmdsky_debug_py/na.py
+-rw-r--r--  2.0 unx   750255 b- defN 23-Jul-09 04:27 pmdsky_debug_py/na_itcm.py
+-rw-r--r--  2.0 unx   244540 b- defN 23-Jul-09 04:27 pmdsky_debug_py/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 04:27 pmdsky_debug_py/py.typed
+-rw-r--r--  2.0 unx     1320 b- defN 23-Jul-09 04:28 pmdsky_debug_py-7.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 04:28 pmdsky_debug_py-7.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-09 04:28 pmdsky_debug_py-7.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1155 b- defN 23-Jul-09 04:28 pmdsky_debug_py-7.0.1.dist-info/RECORD
+14 files, 4845058 bytes uncompressed, 850437 bytes compressed:  82.4%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pmdsky_debug_py/protocol.py
 Comment: 
 
 Filename: pmdsky_debug_py/py.typed
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.0.dist-info/METADATA
+Filename: pmdsky_debug_py-7.0.1.dist-info/METADATA
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.0.dist-info/WHEEL
+Filename: pmdsky_debug_py-7.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.0.dist-info/top_level.txt
+Filename: pmdsky_debug_py-7.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pmdsky_debug_py-7.0.0.dist-info/RECORD
+Filename: pmdsky_debug_py-7.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmdsky_debug_py/_release.py

```diff
@@ -1 +1 @@
-RELEASE = "v0.7.0+2a97086e57"
+RELEASE = "v0.7.0+1c49ae6a6d"
```

## pmdsky_debug_py/eu.py

```diff
@@ -2746,18 +2746,17 @@
     )
 
     FindWanTableEntry = Symbol(
         [0x1D370],
         [0x201D370],
         None,
         (
-            "Search in the given table (in practice always seems to be"
-            " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
-            " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
-            " if not found"
+            "Search in the given table (in practice always seems to be WAN_TABLE) for"
+            " an entry with the given file name.\n\nr0: table pointer\nr1: file"
+            " name\nreturn: index of the found file, if found, or -1 if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         [0x1D3D0],
         [0x201D3D0],
         None,
@@ -2833,14 +2832,49 @@
         (
             "Likely a linker-generated veneer for DeleteWanTableEntry.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
             " wan_table_ptr\nr1: wan_id"
         ),
     )
 
+    WanHasAnimationGroup = Symbol(
+        [0x1DAE0],
+        [0x201DAE0],
+        None,
+        (
+            "Check if the input WAN file loaded in memory has an animation group with"
+            " this ID\nValid means that the animation group is in the range of existing"
+            " animation, and that it has at least one animation.\n\nr0: pointer to the"
+            " header of the WAN\nr1: id of the animation group\nreturn: whether the WAN"
+            " file has the given animation group"
+        ),
+    )
+
+    WanTableSpriteHasAnimationGroup = Symbol(
+        [0x1DB1C],
+        [0x201DB1C],
+        None,
+        (
+            "Check if the sprite in the global WAN table has the given animation"
+            " group\nsee WanHasAnimationGroup for more detail\n\nr0: sprite id in the"
+            " WAN table\nr1: animation group id\nreturn: whether the associated sprite"
+            " has the given animation group"
+        ),
+    )
+
+    SpriteTypeInWanTable = Symbol(
+        [0x1DD0C],
+        [0x201DD0C],
+        None,
+        (
+            "Look up the sprite in the WAN table, and return its type\n\nr0: sprite id"
+            " in the WAN table\nreturn: sprite type"
+        ),
+    )
+
     LoadWteFromRom = Symbol(
         [0x1DEE8],
         [0x201DEE8],
         None,
         (
             "Loads a SIR0-wrapped WTE file from ROM, and returns a handle to it\n\nr0:"
             " [output] pointer to wte handle\nr1: file path string\nr2: load file flags"
@@ -5112,15 +5146,19 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: name",
     )
 
     GetSpriteIndex = Symbol(
         [0x52A24, 0x52A40, 0x52A5C],
         [0x2052A24, 0x2052A40, 0x2052A5C],
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: sprite index",
+        (
+            "Return the sprite index for this monster (inside m_attack.bin,"
+            " m_ground.bin and monster.bin)\nAll three sprites have the same"
+            " index\n\nr0: monster id\nreturn: sprite index"
+        ),
     )
 
     GetDexNumber = Symbol(
         [0x52A78],
         [0x2052A78],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: dex number",
@@ -8198,19 +8236,19 @@
         0x4,
         (
             "[Runtime] Points to the contents of the move data table loaded from"
             " waza_p.bin\n\ntype: struct move_data_table*"
         ),
     )
 
-    LOADED_WAN_TABLE_PTR = Symbol(
-        None,
+    WAN_TABLE = Symbol(
+        [0xB0524],
+        [0x20B0524],
         None,
-        None,
-        "pointer to a wan table\n\nNote: unverified, ported from Irdkwia's notes",
+        "pointer to the list of wan sprite loaded in RAM\n\nstruct wan_table*",
     )
 
     LANGUAGE_INFO_DATA = Symbol([0xB05A8], [0x20B05A8], None, "[Runtime]")
 
     TBL_TALK_GROUP_STRING_ID_START = Symbol(
         None,
         None,
@@ -14023,34 +14061,75 @@
         (
             "Loads the animation (WAN) data for a given object index?\n\nr0: animation"
             " pointer\nr1: object index\nr2: flags"
         ),
     )
 
     InitAnimDataFromOtherAnimDataVeneer = Symbol(
-        None,
-        None,
+        [0x1AD28],
+        [0x22F78A8],
         None,
         (
             "Likely a linker-generated veneer for InitAnimDataFromOtherAnimData.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
             " dst\nr1: src"
         ),
     )
 
     AnimRelatedFunction = Symbol(
-        None,
-        None,
+        [0x1AD34, 0x1AE84],
+        [0x22F78B4, 0x22F7A04],
         None,
         (
             "Does more stuff related to animations...probably?\n\nr0: animation"
             " pointer?\nothers: ?"
         ),
     )
 
+    AllocAndInitPartnerFollowDataAndLiveActorList = Symbol(
+        [0x1BADC],
+        [0x22F865C],
+        None,
+        (
+            "Allocate and initialize the partner follow data and the live actor list"
+            " (in GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
+    InitPartnerFollowDataAndLiveActorList = Symbol(
+        [0x1BB38],
+        [0x22F86B8],
+        None,
+        (
+            "Initialize the partner follow data and the live actor list (in"
+            " GROUND_STATE_PTRS, doesn’t perform the allocation of the"
+            " structures)\n\nNo params."
+        ),
+    )
+
+    DeleteLiveActor = Symbol(
+        [0x1C398],
+        [0x22F8F18],
+        None,
+        (
+            "Remove the actor from the overworld actor list (in"
+            " GROUND_STATE_PTRS)\n\nr0: the index of the actor in the live actor list"
+        ),
+    )
+
+    InitPartnerFollowData = Symbol(
+        [0x1F848],
+        [0x22FC3C8],
+        None,
+        (
+            "Initialize the partner follow data structure, without allocating it (in"
+            " GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
     SprintfStatic = Symbol(
         [0x2CCE8],
         [0x2309868],
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -17522,14 +17601,55 @@
         None,
         (
             "Zeroes the damage data struct, which is output by the damage calculation"
             " function.\n\nr0: damage data pointer"
         ),
     )
 
+    FreeLoadedAttackSpriteAndMore = Symbol(
+        [0x1AD48],
+        [0x22F78C8],
+        None,
+        (
+            "Among other things, free another data structure in the attack sprite"
+            " storage area/data\n\nNo params."
+        ),
+    )
+
+    SetAndLoadCurrentAttackAnimation = Symbol(
+        [0x1ADA0],
+        [0x22F7920],
+        None,
+        (
+            "Load given sprite into the currently loaded attack sprite structure,"
+            " replacing the previous one if already loaded.\n\nr0: pack id\nr1: file"
+            " index\nreturn: sprite id in the loaded wan list"
+        ),
+    )
+
+    ClearLoadedAttackSprite = Symbol(
+        [0x1AE40],
+        [0x22F79C0],
+        None,
+        (
+            "Delete the data of the currently loaded attack sprite, if any.\nDoesn’t"
+            " free the structure, which can continue to be used.\n\nNo params."
+        ),
+    )
+
+    GetLoadedAttackSpriteId = Symbol(
+        [0x1AE88],
+        [0x22F7A08],
+        None,
+        (
+            "Get the sprite ID (in the loaded WAN list) of the currently loaded attack"
+            " sprite, or 0 if none.\n\nreturn: sprite ID"
+        ),
+    )
+
     DungeonGetTotalSpriteFileSize = Symbol(
         [0x1AEA0],
         [0x22F7A20],
         None,
         (
             "Checks Castform and Cherrim\n\nNote: unverified, ported from Irdkwia's"
             " notes\n\nr0: monster ID\nreturn: sprite file size"
@@ -24235,15 +24355,15 @@
     MAP_COLOR_TABLE = Symbol(
         None,
         None,
         None,
         (
             "In order: white, black, red, green, blue, magenta, dark pink, chartreuse,"
             " light orange\n\nNote: unverified, ported from Irdkwia's notes\n\ntype:"
-            " struct rgb[9]"
+            " struct rgba[9]"
         ),
     )
 
     CORNER_CARDINAL_NEIGHBOR_IS_OPEN = Symbol(
         [0x770A4],
         [0x2353C24],
         0x20,
@@ -24345,14 +24465,34 @@
         (
             "[Runtime] An array of 5 integers corresponding to the last value generated"
             " for each secondary LCG sequence.\n\nBased on the assembly, this appears"
             " to be its own global array, separate from DUNGEON_PRNG_STATE."
         ),
     )
 
+    LOADED_ATTACK_SPRITE_FILE_INDEX = Symbol(
+        [0x7762C],
+        [0x23541AC],
+        0x2,
+        (
+            "[Runtime] The file index of the currently loaded attack sprite.\n\ntype:"
+            " uint16_t"
+        ),
+    )
+
+    LOADED_ATTACK_SPRITE_PACK_ID = Symbol(
+        [0x7762E],
+        [0x23541AE],
+        0x2,
+        (
+            "[Runtime] The pack id of the currently loaded attack sprite. Should"
+            " correspond to the id of m_attack.bin\n\ntype: enum pack_file_id"
+        ),
+    )
+
     EXCL_ITEM_EFFECTS_WEATHER_ATK_SPEED_BOOST = Symbol(
         [0x77630],
         [0x23541B0],
         0x8,
         (
             "Array of IDs for exclusive item effects that increase attack speed with"
             " certain weather conditions."
@@ -25324,14 +25464,25 @@
     TURNING_ON_THE_SPOT_FLAG = Symbol(
         [0x37D5A6],
         [0x237D5A6],
         0x1,
         "[Runtime] Flag for whether the player is turning on the spot (pressing Y).",
     )
 
+    LOADED_ATTACK_SPRITE_DATA = Symbol(
+        [0x37D5AC],
+        [0x237D5AC],
+        0x4,
+        (
+            "[Runtime] Pointer to the dynamically allocated structure relating to the"
+            " currently loaded attack sprite, in dungeon mode.\n\ntype: struct"
+            " loaded_attack_sprite_data*"
+        ),
+    )
+
     ROLLOUT_ICE_BALL_MISSED = Symbol(
         None,
         None,
         None,
         (
             "[Runtime] Appears to be set to true whenever a hit from Rollout or Ice"
             " Ball fails to deal damage."
```

## pmdsky_debug_py/eu_itcm.py

```diff
@@ -2659,18 +2659,17 @@
     )
 
     FindWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "Search in the given table (in practice always seems to be"
-            " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
-            " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
-            " if not found"
+            "Search in the given table (in practice always seems to be WAN_TABLE) for"
+            " an entry with the given file name.\n\nr0: table pointer\nr1: file"
+            " name\nreturn: index of the found file, if found, or -1 if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         None,
         None,
         None,
@@ -2746,14 +2745,49 @@
         (
             "Likely a linker-generated veneer for DeleteWanTableEntry.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
             " wan_table_ptr\nr1: wan_id"
         ),
     )
 
+    WanHasAnimationGroup = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Check if the input WAN file loaded in memory has an animation group with"
+            " this ID\nValid means that the animation group is in the range of existing"
+            " animation, and that it has at least one animation.\n\nr0: pointer to the"
+            " header of the WAN\nr1: id of the animation group\nreturn: whether the WAN"
+            " file has the given animation group"
+        ),
+    )
+
+    WanTableSpriteHasAnimationGroup = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Check if the sprite in the global WAN table has the given animation"
+            " group\nsee WanHasAnimationGroup for more detail\n\nr0: sprite id in the"
+            " WAN table\nr1: animation group id\nreturn: whether the associated sprite"
+            " has the given animation group"
+        ),
+    )
+
+    SpriteTypeInWanTable = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Look up the sprite in the WAN table, and return its type\n\nr0: sprite id"
+            " in the WAN table\nreturn: sprite type"
+        ),
+    )
+
     LoadWteFromRom = Symbol(
         None,
         None,
         None,
         (
             "Loads a SIR0-wrapped WTE file from ROM, and returns a handle to it\n\nr0:"
             " [output] pointer to wte handle\nr1: file path string\nr2: load file flags"
@@ -4944,15 +4978,19 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: name",
     )
 
     GetSpriteIndex = Symbol(
         None,
         None,
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: sprite index",
+        (
+            "Return the sprite index for this monster (inside m_attack.bin,"
+            " m_ground.bin and monster.bin)\nAll three sprites have the same"
+            " index\n\nr0: monster id\nreturn: sprite index"
+        ),
     )
 
     GetDexNumber = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: dex number",
@@ -7957,19 +7995,19 @@
         None,
         (
             "[Runtime] Points to the contents of the move data table loaded from"
             " waza_p.bin\n\ntype: struct move_data_table*"
         ),
     )
 
-    LOADED_WAN_TABLE_PTR = Symbol(
+    WAN_TABLE = Symbol(
         None,
         None,
         None,
-        "pointer to a wan table\n\nNote: unverified, ported from Irdkwia's notes",
+        "pointer to the list of wan sprite loaded in RAM\n\nstruct wan_table*",
     )
 
     LANGUAGE_INFO_DATA = Symbol(None, None, None, "[Runtime]")
 
     TBL_TALK_GROUP_STRING_ID_START = Symbol(
         None,
         None,
@@ -13747,14 +13785,55 @@
         None,
         (
             "Does more stuff related to animations...probably?\n\nr0: animation"
             " pointer?\nothers: ?"
         ),
     )
 
+    AllocAndInitPartnerFollowDataAndLiveActorList = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Allocate and initialize the partner follow data and the live actor list"
+            " (in GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
+    InitPartnerFollowDataAndLiveActorList = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the partner follow data and the live actor list (in"
+            " GROUND_STATE_PTRS, doesn’t perform the allocation of the"
+            " structures)\n\nNo params."
+        ),
+    )
+
+    DeleteLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Remove the actor from the overworld actor list (in"
+            " GROUND_STATE_PTRS)\n\nr0: the index of the actor in the live actor list"
+        ),
+    )
+
+    InitPartnerFollowData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the partner follow data structure, without allocating it (in"
+            " GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
     SprintfStatic = Symbol(
         None,
         None,
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -17081,14 +17160,55 @@
         None,
         (
             "Zeroes the damage data struct, which is output by the damage calculation"
             " function.\n\nr0: damage data pointer"
         ),
     )
 
+    FreeLoadedAttackSpriteAndMore = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Among other things, free another data structure in the attack sprite"
+            " storage area/data\n\nNo params."
+        ),
+    )
+
+    SetAndLoadCurrentAttackAnimation = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load given sprite into the currently loaded attack sprite structure,"
+            " replacing the previous one if already loaded.\n\nr0: pack id\nr1: file"
+            " index\nreturn: sprite id in the loaded wan list"
+        ),
+    )
+
+    ClearLoadedAttackSprite = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Delete the data of the currently loaded attack sprite, if any.\nDoesn’t"
+            " free the structure, which can continue to be used.\n\nNo params."
+        ),
+    )
+
+    GetLoadedAttackSpriteId = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Get the sprite ID (in the loaded WAN list) of the currently loaded attack"
+            " sprite, or 0 if none.\n\nreturn: sprite ID"
+        ),
+    )
+
     DungeonGetTotalSpriteFileSize = Symbol(
         None,
         None,
         None,
         (
             "Checks Castform and Cherrim\n\nNote: unverified, ported from Irdkwia's"
             " notes\n\nr0: monster ID\nreturn: sprite file size"
@@ -23612,15 +23732,15 @@
     MAP_COLOR_TABLE = Symbol(
         None,
         None,
         None,
         (
             "In order: white, black, red, green, blue, magenta, dark pink, chartreuse,"
             " light orange\n\nNote: unverified, ported from Irdkwia's notes\n\ntype:"
-            " struct rgb[9]"
+            " struct rgba[9]"
         ),
     )
 
     CORNER_CARDINAL_NEIGHBOR_IS_OPEN = Symbol(
         None,
         None,
         None,
@@ -23722,14 +23842,34 @@
         (
             "[Runtime] An array of 5 integers corresponding to the last value generated"
             " for each secondary LCG sequence.\n\nBased on the assembly, this appears"
             " to be its own global array, separate from DUNGEON_PRNG_STATE."
         ),
     )
 
+    LOADED_ATTACK_SPRITE_FILE_INDEX = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] The file index of the currently loaded attack sprite.\n\ntype:"
+            " uint16_t"
+        ),
+    )
+
+    LOADED_ATTACK_SPRITE_PACK_ID = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] The pack id of the currently loaded attack sprite. Should"
+            " correspond to the id of m_attack.bin\n\ntype: enum pack_file_id"
+        ),
+    )
+
     EXCL_ITEM_EFFECTS_WEATHER_ATK_SPEED_BOOST = Symbol(
         None,
         None,
         None,
         (
             "Array of IDs for exclusive item effects that increase attack speed with"
             " certain weather conditions."
@@ -24691,14 +24831,25 @@
     TURNING_ON_THE_SPOT_FLAG = Symbol(
         None,
         None,
         None,
         "[Runtime] Flag for whether the player is turning on the spot (pressing Y).",
     )
 
+    LOADED_ATTACK_SPRITE_DATA = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] Pointer to the dynamically allocated structure relating to the"
+            " currently loaded attack sprite, in dungeon mode.\n\ntype: struct"
+            " loaded_attack_sprite_data*"
+        ),
+    )
+
     ROLLOUT_ICE_BALL_MISSED = Symbol(
         None,
         None,
         None,
         (
             "[Runtime] Appears to be set to true whenever a hit from Rollout or Ice"
             " Ball fails to deal damage."
```

## pmdsky_debug_py/jp.py

```diff
@@ -2744,18 +2744,17 @@
     )
 
     FindWanTableEntry = Symbol(
         [0x1D32C],
         [0x201D32C],
         None,
         (
-            "Search in the given table (in practice always seems to be"
-            " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
-            " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
-            " if not found"
+            "Search in the given table (in practice always seems to be WAN_TABLE) for"
+            " an entry with the given file name.\n\nr0: table pointer\nr1: file"
+            " name\nreturn: index of the found file, if found, or -1 if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         [0x1D38C],
         [0x201D38C],
         None,
@@ -2831,14 +2830,49 @@
         (
             "Likely a linker-generated veneer for DeleteWanTableEntry.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
             " wan_table_ptr\nr1: wan_id"
         ),
     )
 
+    WanHasAnimationGroup = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Check if the input WAN file loaded in memory has an animation group with"
+            " this ID\nValid means that the animation group is in the range of existing"
+            " animation, and that it has at least one animation.\n\nr0: pointer to the"
+            " header of the WAN\nr1: id of the animation group\nreturn: whether the WAN"
+            " file has the given animation group"
+        ),
+    )
+
+    WanTableSpriteHasAnimationGroup = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Check if the sprite in the global WAN table has the given animation"
+            " group\nsee WanHasAnimationGroup for more detail\n\nr0: sprite id in the"
+            " WAN table\nr1: animation group id\nreturn: whether the associated sprite"
+            " has the given animation group"
+        ),
+    )
+
+    SpriteTypeInWanTable = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Look up the sprite in the WAN table, and return its type\n\nr0: sprite id"
+            " in the WAN table\nreturn: sprite type"
+        ),
+    )
+
     LoadWteFromRom = Symbol(
         [0x1DEA4],
         [0x201DEA4],
         None,
         (
             "Loads a SIR0-wrapped WTE file from ROM, and returns a handle to it\n\nr0:"
             " [output] pointer to wte handle\nr1: file path string\nr2: load file flags"
@@ -5110,15 +5144,19 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: name",
     )
 
     GetSpriteIndex = Symbol(
         [0x52A28, 0x52A44, 0x52A60],
         [0x2052A28, 0x2052A44, 0x2052A60],
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: sprite index",
+        (
+            "Return the sprite index for this monster (inside m_attack.bin,"
+            " m_ground.bin and monster.bin)\nAll three sprites have the same"
+            " index\n\nr0: monster id\nreturn: sprite index"
+        ),
     )
 
     GetDexNumber = Symbol(
         [0x52A7C],
         [0x2052A7C],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: dex number",
@@ -8183,19 +8221,19 @@
         None,
         (
             "[Runtime] Points to the contents of the move data table loaded from"
             " waza_p.bin\n\ntype: struct move_data_table*"
         ),
     )
 
-    LOADED_WAN_TABLE_PTR = Symbol(
+    WAN_TABLE = Symbol(
         None,
         None,
         None,
-        "pointer to a wan table\n\nNote: unverified, ported from Irdkwia's notes",
+        "pointer to the list of wan sprite loaded in RAM\n\nstruct wan_table*",
     )
 
     LANGUAGE_INFO_DATA = Symbol(None, None, None, "[Runtime]")
 
     TBL_TALK_GROUP_STRING_ID_START = Symbol(
         None,
         None,
@@ -13979,14 +14017,55 @@
         None,
         (
             "Does more stuff related to animations...probably?\n\nr0: animation"
             " pointer?\nothers: ?"
         ),
     )
 
+    AllocAndInitPartnerFollowDataAndLiveActorList = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Allocate and initialize the partner follow data and the live actor list"
+            " (in GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
+    InitPartnerFollowDataAndLiveActorList = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the partner follow data and the live actor list (in"
+            " GROUND_STATE_PTRS, doesn’t perform the allocation of the"
+            " structures)\n\nNo params."
+        ),
+    )
+
+    DeleteLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Remove the actor from the overworld actor list (in"
+            " GROUND_STATE_PTRS)\n\nr0: the index of the actor in the live actor list"
+        ),
+    )
+
+    InitPartnerFollowData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the partner follow data structure, without allocating it (in"
+            " GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
     SprintfStatic = Symbol(
         [0x2CB98],
         [0x230A478],
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -17325,14 +17404,55 @@
         None,
         (
             "Zeroes the damage data struct, which is output by the damage calculation"
             " function.\n\nr0: damage data pointer"
         ),
     )
 
+    FreeLoadedAttackSpriteAndMore = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Among other things, free another data structure in the attack sprite"
+            " storage area/data\n\nNo params."
+        ),
+    )
+
+    SetAndLoadCurrentAttackAnimation = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load given sprite into the currently loaded attack sprite structure,"
+            " replacing the previous one if already loaded.\n\nr0: pack id\nr1: file"
+            " index\nreturn: sprite id in the loaded wan list"
+        ),
+    )
+
+    ClearLoadedAttackSprite = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Delete the data of the currently loaded attack sprite, if any.\nDoesn’t"
+            " free the structure, which can continue to be used.\n\nNo params."
+        ),
+    )
+
+    GetLoadedAttackSpriteId = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Get the sprite ID (in the loaded WAN list) of the currently loaded attack"
+            " sprite, or 0 if none.\n\nreturn: sprite ID"
+        ),
+    )
+
     DungeonGetTotalSpriteFileSize = Symbol(
         [0x1AD54],
         [0x22F8634],
         None,
         (
             "Checks Castform and Cherrim\n\nNote: unverified, ported from Irdkwia's"
             " notes\n\nr0: monster ID\nreturn: sprite file size"
@@ -23873,15 +23993,15 @@
     MAP_COLOR_TABLE = Symbol(
         None,
         None,
         None,
         (
             "In order: white, black, red, green, blue, magenta, dark pink, chartreuse,"
             " light orange\n\nNote: unverified, ported from Irdkwia's notes\n\ntype:"
-            " struct rgb[9]"
+            " struct rgba[9]"
         ),
     )
 
     CORNER_CARDINAL_NEIGHBOR_IS_OPEN = Symbol(
         None,
         None,
         None,
@@ -23983,14 +24103,34 @@
         (
             "[Runtime] An array of 5 integers corresponding to the last value generated"
             " for each secondary LCG sequence.\n\nBased on the assembly, this appears"
             " to be its own global array, separate from DUNGEON_PRNG_STATE."
         ),
     )
 
+    LOADED_ATTACK_SPRITE_FILE_INDEX = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] The file index of the currently loaded attack sprite.\n\ntype:"
+            " uint16_t"
+        ),
+    )
+
+    LOADED_ATTACK_SPRITE_PACK_ID = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] The pack id of the currently loaded attack sprite. Should"
+            " correspond to the id of m_attack.bin\n\ntype: enum pack_file_id"
+        ),
+    )
+
     EXCL_ITEM_EFFECTS_WEATHER_ATK_SPEED_BOOST = Symbol(
         None,
         None,
         None,
         (
             "Array of IDs for exclusive item effects that increase attack speed with"
             " certain weather conditions."
@@ -24955,14 +25095,25 @@
     TURNING_ON_THE_SPOT_FLAG = Symbol(
         None,
         None,
         None,
         "[Runtime] Flag for whether the player is turning on the spot (pressing Y).",
     )
 
+    LOADED_ATTACK_SPRITE_DATA = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] Pointer to the dynamically allocated structure relating to the"
+            " currently loaded attack sprite, in dungeon mode.\n\ntype: struct"
+            " loaded_attack_sprite_data*"
+        ),
+    )
+
     ROLLOUT_ICE_BALL_MISSED = Symbol(
         None,
         None,
         None,
         (
             "[Runtime] Appears to be set to true whenever a hit from Rollout or Ice"
             " Ball fails to deal damage."
```

## pmdsky_debug_py/jp_itcm.py

```diff
@@ -2659,18 +2659,17 @@
     )
 
     FindWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "Search in the given table (in practice always seems to be"
-            " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
-            " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
-            " if not found"
+            "Search in the given table (in practice always seems to be WAN_TABLE) for"
+            " an entry with the given file name.\n\nr0: table pointer\nr1: file"
+            " name\nreturn: index of the found file, if found, or -1 if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         None,
         None,
         None,
@@ -2746,14 +2745,49 @@
         (
             "Likely a linker-generated veneer for DeleteWanTableEntry.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
             " wan_table_ptr\nr1: wan_id"
         ),
     )
 
+    WanHasAnimationGroup = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Check if the input WAN file loaded in memory has an animation group with"
+            " this ID\nValid means that the animation group is in the range of existing"
+            " animation, and that it has at least one animation.\n\nr0: pointer to the"
+            " header of the WAN\nr1: id of the animation group\nreturn: whether the WAN"
+            " file has the given animation group"
+        ),
+    )
+
+    WanTableSpriteHasAnimationGroup = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Check if the sprite in the global WAN table has the given animation"
+            " group\nsee WanHasAnimationGroup for more detail\n\nr0: sprite id in the"
+            " WAN table\nr1: animation group id\nreturn: whether the associated sprite"
+            " has the given animation group"
+        ),
+    )
+
+    SpriteTypeInWanTable = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Look up the sprite in the WAN table, and return its type\n\nr0: sprite id"
+            " in the WAN table\nreturn: sprite type"
+        ),
+    )
+
     LoadWteFromRom = Symbol(
         None,
         None,
         None,
         (
             "Loads a SIR0-wrapped WTE file from ROM, and returns a handle to it\n\nr0:"
             " [output] pointer to wte handle\nr1: file path string\nr2: load file flags"
@@ -4944,15 +4978,19 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: name",
     )
 
     GetSpriteIndex = Symbol(
         None,
         None,
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: sprite index",
+        (
+            "Return the sprite index for this monster (inside m_attack.bin,"
+            " m_ground.bin and monster.bin)\nAll three sprites have the same"
+            " index\n\nr0: monster id\nreturn: sprite index"
+        ),
     )
 
     GetDexNumber = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: dex number",
@@ -7957,19 +7995,19 @@
         None,
         (
             "[Runtime] Points to the contents of the move data table loaded from"
             " waza_p.bin\n\ntype: struct move_data_table*"
         ),
     )
 
-    LOADED_WAN_TABLE_PTR = Symbol(
+    WAN_TABLE = Symbol(
         None,
         None,
         None,
-        "pointer to a wan table\n\nNote: unverified, ported from Irdkwia's notes",
+        "pointer to the list of wan sprite loaded in RAM\n\nstruct wan_table*",
     )
 
     LANGUAGE_INFO_DATA = Symbol(None, None, None, "[Runtime]")
 
     TBL_TALK_GROUP_STRING_ID_START = Symbol(
         None,
         None,
@@ -13747,14 +13785,55 @@
         None,
         (
             "Does more stuff related to animations...probably?\n\nr0: animation"
             " pointer?\nothers: ?"
         ),
     )
 
+    AllocAndInitPartnerFollowDataAndLiveActorList = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Allocate and initialize the partner follow data and the live actor list"
+            " (in GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
+    InitPartnerFollowDataAndLiveActorList = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the partner follow data and the live actor list (in"
+            " GROUND_STATE_PTRS, doesn’t perform the allocation of the"
+            " structures)\n\nNo params."
+        ),
+    )
+
+    DeleteLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Remove the actor from the overworld actor list (in"
+            " GROUND_STATE_PTRS)\n\nr0: the index of the actor in the live actor list"
+        ),
+    )
+
+    InitPartnerFollowData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the partner follow data structure, without allocating it (in"
+            " GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
     SprintfStatic = Symbol(
         None,
         None,
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -17081,14 +17160,55 @@
         None,
         (
             "Zeroes the damage data struct, which is output by the damage calculation"
             " function.\n\nr0: damage data pointer"
         ),
     )
 
+    FreeLoadedAttackSpriteAndMore = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Among other things, free another data structure in the attack sprite"
+            " storage area/data\n\nNo params."
+        ),
+    )
+
+    SetAndLoadCurrentAttackAnimation = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load given sprite into the currently loaded attack sprite structure,"
+            " replacing the previous one if already loaded.\n\nr0: pack id\nr1: file"
+            " index\nreturn: sprite id in the loaded wan list"
+        ),
+    )
+
+    ClearLoadedAttackSprite = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Delete the data of the currently loaded attack sprite, if any.\nDoesn’t"
+            " free the structure, which can continue to be used.\n\nNo params."
+        ),
+    )
+
+    GetLoadedAttackSpriteId = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Get the sprite ID (in the loaded WAN list) of the currently loaded attack"
+            " sprite, or 0 if none.\n\nreturn: sprite ID"
+        ),
+    )
+
     DungeonGetTotalSpriteFileSize = Symbol(
         None,
         None,
         None,
         (
             "Checks Castform and Cherrim\n\nNote: unverified, ported from Irdkwia's"
             " notes\n\nr0: monster ID\nreturn: sprite file size"
@@ -23612,15 +23732,15 @@
     MAP_COLOR_TABLE = Symbol(
         None,
         None,
         None,
         (
             "In order: white, black, red, green, blue, magenta, dark pink, chartreuse,"
             " light orange\n\nNote: unverified, ported from Irdkwia's notes\n\ntype:"
-            " struct rgb[9]"
+            " struct rgba[9]"
         ),
     )
 
     CORNER_CARDINAL_NEIGHBOR_IS_OPEN = Symbol(
         None,
         None,
         None,
@@ -23722,14 +23842,34 @@
         (
             "[Runtime] An array of 5 integers corresponding to the last value generated"
             " for each secondary LCG sequence.\n\nBased on the assembly, this appears"
             " to be its own global array, separate from DUNGEON_PRNG_STATE."
         ),
     )
 
+    LOADED_ATTACK_SPRITE_FILE_INDEX = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] The file index of the currently loaded attack sprite.\n\ntype:"
+            " uint16_t"
+        ),
+    )
+
+    LOADED_ATTACK_SPRITE_PACK_ID = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] The pack id of the currently loaded attack sprite. Should"
+            " correspond to the id of m_attack.bin\n\ntype: enum pack_file_id"
+        ),
+    )
+
     EXCL_ITEM_EFFECTS_WEATHER_ATK_SPEED_BOOST = Symbol(
         None,
         None,
         None,
         (
             "Array of IDs for exclusive item effects that increase attack speed with"
             " certain weather conditions."
@@ -24691,14 +24831,25 @@
     TURNING_ON_THE_SPOT_FLAG = Symbol(
         None,
         None,
         None,
         "[Runtime] Flag for whether the player is turning on the spot (pressing Y).",
     )
 
+    LOADED_ATTACK_SPRITE_DATA = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] Pointer to the dynamically allocated structure relating to the"
+            " currently loaded attack sprite, in dungeon mode.\n\ntype: struct"
+            " loaded_attack_sprite_data*"
+        ),
+    )
+
     ROLLOUT_ICE_BALL_MISSED = Symbol(
         None,
         None,
         None,
         (
             "[Runtime] Appears to be set to true whenever a hit from Rollout or Ice"
             " Ball fails to deal damage."
```

## pmdsky_debug_py/na.py

```diff
@@ -2746,18 +2746,17 @@
     )
 
     FindWanTableEntry = Symbol(
         [0x1D2D4],
         [0x201D2D4],
         None,
         (
-            "Search in the given table (in practice always seems to be"
-            " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
-            " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
-            " if not found"
+            "Search in the given table (in practice always seems to be WAN_TABLE) for"
+            " an entry with the given file name.\n\nr0: table pointer\nr1: file"
+            " name\nreturn: index of the found file, if found, or -1 if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         [0x1D334],
         [0x201D334],
         None,
@@ -2833,14 +2832,49 @@
         (
             "Likely a linker-generated veneer for DeleteWanTableEntry.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
             " wan_table_ptr\nr1: wan_id"
         ),
     )
 
+    WanHasAnimationGroup = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Check if the input WAN file loaded in memory has an animation group with"
+            " this ID\nValid means that the animation group is in the range of existing"
+            " animation, and that it has at least one animation.\n\nr0: pointer to the"
+            " header of the WAN\nr1: id of the animation group\nreturn: whether the WAN"
+            " file has the given animation group"
+        ),
+    )
+
+    WanTableSpriteHasAnimationGroup = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Check if the sprite in the global WAN table has the given animation"
+            " group\nsee WanHasAnimationGroup for more detail\n\nr0: sprite id in the"
+            " WAN table\nr1: animation group id\nreturn: whether the associated sprite"
+            " has the given animation group"
+        ),
+    )
+
+    SpriteTypeInWanTable = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Look up the sprite in the WAN table, and return its type\n\nr0: sprite id"
+            " in the WAN table\nreturn: sprite type"
+        ),
+    )
+
     LoadWteFromRom = Symbol(
         [0x1DE4C],
         [0x201DE4C],
         None,
         (
             "Loads a SIR0-wrapped WTE file from ROM, and returns a handle to it\n\nr0:"
             " [output] pointer to wte handle\nr1: file path string\nr2: load file flags"
@@ -5112,15 +5146,19 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: name",
     )
 
     GetSpriteIndex = Symbol(
         [0x526EC, 0x52708, 0x52724],
         [0x20526EC, 0x2052708, 0x2052724],
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: sprite index",
+        (
+            "Return the sprite index for this monster (inside m_attack.bin,"
+            " m_ground.bin and monster.bin)\nAll three sprites have the same"
+            " index\n\nr0: monster id\nreturn: sprite index"
+        ),
     )
 
     GetDexNumber = Symbol(
         [0x52740],
         [0x2052740],
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: dex number",
@@ -8201,19 +8239,19 @@
         0x4,
         (
             "[Runtime] Points to the contents of the move data table loaded from"
             " waza_p.bin\n\ntype: struct move_data_table*"
         ),
     )
 
-    LOADED_WAN_TABLE_PTR = Symbol(
+    WAN_TABLE = Symbol(
         [0xAFC68],
         [0x20AFC68],
         0x4,
-        "pointer to a wan table\n\nNote: unverified, ported from Irdkwia's notes",
+        "pointer to the list of wan sprite loaded in RAM\n\nstruct wan_table*",
     )
 
     LANGUAGE_INFO_DATA = Symbol([0xAFCE8], [0x20AFCE8], None, "[Runtime]")
 
     TBL_TALK_GROUP_STRING_ID_START = Symbol(
         [0xAFCF8],
         [0x20AFCF8],
@@ -14098,14 +14136,55 @@
         None,
         (
             "Does more stuff related to animations...probably?\n\nr0: animation"
             " pointer?\nothers: ?"
         ),
     )
 
+    AllocAndInitPartnerFollowDataAndLiveActorList = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Allocate and initialize the partner follow data and the live actor list"
+            " (in GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
+    InitPartnerFollowDataAndLiveActorList = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the partner follow data and the live actor list (in"
+            " GROUND_STATE_PTRS, doesn’t perform the allocation of the"
+            " structures)\n\nNo params."
+        ),
+    )
+
+    DeleteLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Remove the actor from the overworld actor list (in"
+            " GROUND_STATE_PTRS)\n\nr0: the index of the actor in the live actor list"
+        ),
+    )
+
+    InitPartnerFollowData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the partner follow data structure, without allocating it (in"
+            " GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
     SprintfStatic = Symbol(
         [0x2CC8C],
         [0x2308ECC],
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -17606,14 +17685,55 @@
         None,
         (
             "Zeroes the damage data struct, which is output by the damage calculation"
             " function.\n\nr0: damage data pointer"
         ),
     )
 
+    FreeLoadedAttackSpriteAndMore = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Among other things, free another data structure in the attack sprite"
+            " storage area/data\n\nNo params."
+        ),
+    )
+
+    SetAndLoadCurrentAttackAnimation = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load given sprite into the currently loaded attack sprite structure,"
+            " replacing the previous one if already loaded.\n\nr0: pack id\nr1: file"
+            " index\nreturn: sprite id in the loaded wan list"
+        ),
+    )
+
+    ClearLoadedAttackSprite = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Delete the data of the currently loaded attack sprite, if any.\nDoesn’t"
+            " free the structure, which can continue to be used.\n\nNo params."
+        ),
+    )
+
+    GetLoadedAttackSpriteId = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Get the sprite ID (in the loaded WAN list) of the currently loaded attack"
+            " sprite, or 0 if none.\n\nreturn: sprite ID"
+        ),
+    )
+
     DungeonGetTotalSpriteFileSize = Symbol(
         [0x1AE28],
         [0x22F7068],
         None,
         (
             "Checks Castform and Cherrim\n\nNote: unverified, ported from Irdkwia's"
             " notes\n\nr0: monster ID\nreturn: sprite file size"
@@ -24322,15 +24442,15 @@
     MAP_COLOR_TABLE = Symbol(
         [0x76D90],
         [0x2352FD0],
         0x24,
         (
             "In order: white, black, red, green, blue, magenta, dark pink, chartreuse,"
             " light orange\n\nNote: unverified, ported from Irdkwia's notes\n\ntype:"
-            " struct rgb[9]"
+            " struct rgba[9]"
         ),
     )
 
     CORNER_CARDINAL_NEIGHBOR_IS_OPEN = Symbol(
         [0x76DD0],
         [0x2353010],
         0x20,
@@ -24432,14 +24552,34 @@
         (
             "[Runtime] An array of 5 integers corresponding to the last value generated"
             " for each secondary LCG sequence.\n\nBased on the assembly, this appears"
             " to be its own global array, separate from DUNGEON_PRNG_STATE."
         ),
     )
 
+    LOADED_ATTACK_SPRITE_FILE_INDEX = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] The file index of the currently loaded attack sprite.\n\ntype:"
+            " uint16_t"
+        ),
+    )
+
+    LOADED_ATTACK_SPRITE_PACK_ID = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] The pack id of the currently loaded attack sprite. Should"
+            " correspond to the id of m_attack.bin\n\ntype: enum pack_file_id"
+        ),
+    )
+
     EXCL_ITEM_EFFECTS_WEATHER_ATK_SPEED_BOOST = Symbol(
         [0x77370],
         [0x23535B0],
         0x8,
         (
             "Array of IDs for exclusive item effects that increase attack speed with"
             " certain weather conditions."
@@ -25413,14 +25553,25 @@
     TURNING_ON_THE_SPOT_FLAG = Symbol(
         [0x37C9A6],
         [0x237C9A6],
         0x1,
         "[Runtime] Flag for whether the player is turning on the spot (pressing Y).",
     )
 
+    LOADED_ATTACK_SPRITE_DATA = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] Pointer to the dynamically allocated structure relating to the"
+            " currently loaded attack sprite, in dungeon mode.\n\ntype: struct"
+            " loaded_attack_sprite_data*"
+        ),
+    )
+
     ROLLOUT_ICE_BALL_MISSED = Symbol(
         [0x37CA69],
         [0x237CA69],
         0x1,
         (
             "[Runtime] Appears to be set to true whenever a hit from Rollout or Ice"
             " Ball fails to deal damage."
```

## pmdsky_debug_py/na_itcm.py

```diff
@@ -2659,18 +2659,17 @@
     )
 
     FindWanTableEntry = Symbol(
         None,
         None,
         None,
         (
-            "Search in the given table (in practice always seems to be"
-            " LOADED_WAN_TABLE_PTR) for an entry with the given file name.\n\nr0: table"
-            " pointer\nr1: file name\nreturn: index of the found file, if found, or -1"
-            " if not found"
+            "Search in the given table (in practice always seems to be WAN_TABLE) for"
+            " an entry with the given file name.\n\nr0: table pointer\nr1: file"
+            " name\nreturn: index of the found file, if found, or -1 if not found"
         ),
     )
 
     GetLoadedWanTableEntry = Symbol(
         None,
         None,
         None,
@@ -2746,14 +2745,49 @@
         (
             "Likely a linker-generated veneer for DeleteWanTableEntry.\n\nSee"
             " https://developer.arm.com/documentation/dui0474/k/image-structure-and-generation/linker-generated-veneers/what-is-a-veneer-\n\nr0:"
             " wan_table_ptr\nr1: wan_id"
         ),
     )
 
+    WanHasAnimationGroup = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Check if the input WAN file loaded in memory has an animation group with"
+            " this ID\nValid means that the animation group is in the range of existing"
+            " animation, and that it has at least one animation.\n\nr0: pointer to the"
+            " header of the WAN\nr1: id of the animation group\nreturn: whether the WAN"
+            " file has the given animation group"
+        ),
+    )
+
+    WanTableSpriteHasAnimationGroup = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Check if the sprite in the global WAN table has the given animation"
+            " group\nsee WanHasAnimationGroup for more detail\n\nr0: sprite id in the"
+            " WAN table\nr1: animation group id\nreturn: whether the associated sprite"
+            " has the given animation group"
+        ),
+    )
+
+    SpriteTypeInWanTable = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Look up the sprite in the WAN table, and return its type\n\nr0: sprite id"
+            " in the WAN table\nreturn: sprite type"
+        ),
+    )
+
     LoadWteFromRom = Symbol(
         None,
         None,
         None,
         (
             "Loads a SIR0-wrapped WTE file from ROM, and returns a handle to it\n\nr0:"
             " [output] pointer to wte handle\nr1: file path string\nr2: load file flags"
@@ -4944,15 +4978,19 @@
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: name",
     )
 
     GetSpriteIndex = Symbol(
         None,
         None,
         None,
-        "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: sprite index",
+        (
+            "Return the sprite index for this monster (inside m_attack.bin,"
+            " m_ground.bin and monster.bin)\nAll three sprites have the same"
+            " index\n\nr0: monster id\nreturn: sprite index"
+        ),
     )
 
     GetDexNumber = Symbol(
         None,
         None,
         None,
         "Note: unverified, ported from Irdkwia's notes\n\nr0: id\nreturn: dex number",
@@ -7957,19 +7995,19 @@
         None,
         (
             "[Runtime] Points to the contents of the move data table loaded from"
             " waza_p.bin\n\ntype: struct move_data_table*"
         ),
     )
 
-    LOADED_WAN_TABLE_PTR = Symbol(
+    WAN_TABLE = Symbol(
         None,
         None,
         None,
-        "pointer to a wan table\n\nNote: unverified, ported from Irdkwia's notes",
+        "pointer to the list of wan sprite loaded in RAM\n\nstruct wan_table*",
     )
 
     LANGUAGE_INFO_DATA = Symbol(None, None, None, "[Runtime]")
 
     TBL_TALK_GROUP_STRING_ID_START = Symbol(
         None,
         None,
@@ -13747,14 +13785,55 @@
         None,
         (
             "Does more stuff related to animations...probably?\n\nr0: animation"
             " pointer?\nothers: ?"
         ),
     )
 
+    AllocAndInitPartnerFollowDataAndLiveActorList = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Allocate and initialize the partner follow data and the live actor list"
+            " (in GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
+    InitPartnerFollowDataAndLiveActorList = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the partner follow data and the live actor list (in"
+            " GROUND_STATE_PTRS, doesn’t perform the allocation of the"
+            " structures)\n\nNo params."
+        ),
+    )
+
+    DeleteLiveActor = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Remove the actor from the overworld actor list (in"
+            " GROUND_STATE_PTRS)\n\nr0: the index of the actor in the live actor list"
+        ),
+    )
+
+    InitPartnerFollowData = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Initialize the partner follow data structure, without allocating it (in"
+            " GROUND_STATE_PTRS)\n\nNo params."
+        ),
+    )
+
     SprintfStatic = Symbol(
         None,
         None,
         None,
         (
             "Statically defined copy of sprintf(3) in overlay 11. See arm9.yml for more"
             " information.\n\nr0: str\nr1: format\n...: variadic\nreturn: number of"
@@ -17081,14 +17160,55 @@
         None,
         (
             "Zeroes the damage data struct, which is output by the damage calculation"
             " function.\n\nr0: damage data pointer"
         ),
     )
 
+    FreeLoadedAttackSpriteAndMore = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Among other things, free another data structure in the attack sprite"
+            " storage area/data\n\nNo params."
+        ),
+    )
+
+    SetAndLoadCurrentAttackAnimation = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Load given sprite into the currently loaded attack sprite structure,"
+            " replacing the previous one if already loaded.\n\nr0: pack id\nr1: file"
+            " index\nreturn: sprite id in the loaded wan list"
+        ),
+    )
+
+    ClearLoadedAttackSprite = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Delete the data of the currently loaded attack sprite, if any.\nDoesn’t"
+            " free the structure, which can continue to be used.\n\nNo params."
+        ),
+    )
+
+    GetLoadedAttackSpriteId = Symbol(
+        None,
+        None,
+        None,
+        (
+            "Get the sprite ID (in the loaded WAN list) of the currently loaded attack"
+            " sprite, or 0 if none.\n\nreturn: sprite ID"
+        ),
+    )
+
     DungeonGetTotalSpriteFileSize = Symbol(
         None,
         None,
         None,
         (
             "Checks Castform and Cherrim\n\nNote: unverified, ported from Irdkwia's"
             " notes\n\nr0: monster ID\nreturn: sprite file size"
@@ -23612,15 +23732,15 @@
     MAP_COLOR_TABLE = Symbol(
         None,
         None,
         None,
         (
             "In order: white, black, red, green, blue, magenta, dark pink, chartreuse,"
             " light orange\n\nNote: unverified, ported from Irdkwia's notes\n\ntype:"
-            " struct rgb[9]"
+            " struct rgba[9]"
         ),
     )
 
     CORNER_CARDINAL_NEIGHBOR_IS_OPEN = Symbol(
         None,
         None,
         None,
@@ -23722,14 +23842,34 @@
         (
             "[Runtime] An array of 5 integers corresponding to the last value generated"
             " for each secondary LCG sequence.\n\nBased on the assembly, this appears"
             " to be its own global array, separate from DUNGEON_PRNG_STATE."
         ),
     )
 
+    LOADED_ATTACK_SPRITE_FILE_INDEX = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] The file index of the currently loaded attack sprite.\n\ntype:"
+            " uint16_t"
+        ),
+    )
+
+    LOADED_ATTACK_SPRITE_PACK_ID = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] The pack id of the currently loaded attack sprite. Should"
+            " correspond to the id of m_attack.bin\n\ntype: enum pack_file_id"
+        ),
+    )
+
     EXCL_ITEM_EFFECTS_WEATHER_ATK_SPEED_BOOST = Symbol(
         None,
         None,
         None,
         (
             "Array of IDs for exclusive item effects that increase attack speed with"
             " certain weather conditions."
@@ -24691,14 +24831,25 @@
     TURNING_ON_THE_SPOT_FLAG = Symbol(
         None,
         None,
         None,
         "[Runtime] Flag for whether the player is turning on the spot (pressing Y).",
     )
 
+    LOADED_ATTACK_SPRITE_DATA = Symbol(
+        None,
+        None,
+        None,
+        (
+            "[Runtime] Pointer to the dynamically allocated structure relating to the"
+            " currently loaded attack sprite, in dungeon mode.\n\ntype: struct"
+            " loaded_attack_sprite_data*"
+        ),
+    )
+
     ROLLOUT_ICE_BALL_MISSED = Symbol(
         None,
         None,
         None,
         (
             "[Runtime] Appears to be set to true whenever a hit from Rollout or Ice"
             " Ball fails to deal damage."
```

## pmdsky_debug_py/protocol.py

```diff
@@ -1552,14 +1552,29 @@
     ]
 
     DeleteWanTableEntryVeneer: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    WanHasAnimationGroup: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    WanTableSpriteHasAnimationGroup: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    SpriteTypeInWanTable: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     LoadWteFromRom: Symbol[
         Optional[List[int]],
         None,
     ]
 
     LoadWteFromFileDirectory: Symbol[
         Optional[List[int]],
@@ -4509,15 +4524,15 @@
     ]
 
     MOVE_DATA_TABLE_PTR: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
-    LOADED_WAN_TABLE_PTR: Symbol[
+    WAN_TABLE: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     LANGUAGE_INFO_DATA: Symbol[
         Optional[List[int]],
         None,
@@ -7590,14 +7605,34 @@
     ]
 
     AnimRelatedFunction: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    AllocAndInitPartnerFollowDataAndLiveActorList: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    InitPartnerFollowDataAndLiveActorList: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    DeleteLiveActor: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    InitPartnerFollowData: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     SprintfStatic: Symbol[
         Optional[List[int]],
         None,
     ]
 
     GetExclusiveItemRequirements: Symbol[
         Optional[List[int]],
@@ -10170,14 +10205,34 @@
     ]
 
     ResetDamageData: Symbol[
         Optional[List[int]],
         None,
     ]
 
+    FreeLoadedAttackSpriteAndMore: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    SetAndLoadCurrentAttackAnimation: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    ClearLoadedAttackSprite: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
+    GetLoadedAttackSpriteId: Symbol[
+        Optional[List[int]],
+        None,
+    ]
+
     DungeonGetTotalSpriteFileSize: Symbol[
         Optional[List[int]],
         None,
     ]
 
     DungeonGetSpriteIndex: Symbol[
         Optional[List[int]],
@@ -13142,14 +13197,24 @@
     ]
 
     DUNGEON_PRNG_STATE_SECONDARY_VALUES: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    LOADED_ATTACK_SPRITE_FILE_INDEX: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
+    LOADED_ATTACK_SPRITE_PACK_ID: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     EXCL_ITEM_EFFECTS_WEATHER_ATK_SPEED_BOOST: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     EXCL_ITEM_EFFECTS_WEATHER_MOVE_SPEED_BOOST: Symbol[
         Optional[List[int]],
@@ -13936,14 +14001,19 @@
     ]
 
     TURNING_ON_THE_SPOT_FLAG: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
+    LOADED_ATTACK_SPRITE_DATA: Symbol[
+        Optional[List[int]],
+        Optional[int],
+    ]
+
     ROLLOUT_ICE_BALL_MISSED: Symbol[
         Optional[List[int]],
         Optional[int],
     ]
 
     ROLLOUT_ICE_BALL_SUCCESSIVE_HITS: Symbol[
         Optional[List[int]],
```

## Comparing `pmdsky_debug_py-7.0.0.dist-info/METADATA` & `pmdsky_debug_py-7.0.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmdsky-debug-py
-Version: 7.0.0
+Version: 7.0.1
 Summary: pmdsky-debug symbols for Python.
 Author-email: Marco 'Capypara' Köpcke <hello@capypara.de>
 License: MIT
 Project-URL: repository, https://github.com/SkyTemple/pmdsky-debug-py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

