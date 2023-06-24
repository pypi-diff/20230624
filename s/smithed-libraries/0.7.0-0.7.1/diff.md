# Comparing `tmp/smithed_libraries-0.7.0.tar.gz` & `tmp/smithed_libraries-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smithed_libraries-0.7.0.tar", max compression
+gzip compressed data, was "smithed_libraries-0.7.1.tar", max compression
```

## Comparing `smithed_libraries-0.7.0.tar` & `smithed_libraries-0.7.1.tar`

### file list

```diff
@@ -1,1152 +1,1152 @@
--rw-r--r--   0        0        0     1064 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/LICENSE
--rw-r--r--   0        0        0      654 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/README.md
--rw-r--r--   0        0        0      980 2023-06-19 00:23:50.835553 smithed_libraries-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      571 2023-06-19 00:23:50.823553 smithed_libraries-0.7.0/smithed_libraries/__init__.py
--rw-r--r--   0        0        0     2219 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/common.yaml
--rw-r--r--   0        0        0      939 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/README.md
--rw-r--r--   0        0        0      223 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/beet.yaml
--rw-r--r--   0        0        0     3808 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/advancements/impl/vanilla/bed/clicked_bed.json
--rw-r--r--   0        0        0      323 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/advancements/impl/vanilla/bed/slept_in_bed.json
--rw-r--r--   0        0        0     1467 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/advancements/impl/vanilla/container/clicked_lockable_block.json
--rw-r--r--   0        0        0     1215 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/display.mcfunction
--rw-r--r--   0        0        0     2167 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/message.mcfunction
--rw-r--r--   0        0        0      263 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/reset.mcfunction
--rw-r--r--   0        0        0      924 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/technical/load.mcfunction
--rw-r--r--   0        0        0      754 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/technical/tick.mcfunction
--rw-r--r--   0        0        0      855 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/check_sleep_status.mcfunction
--rw-r--r--   0        0        0     1124 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/clicked_bed.mcfunction
--rw-r--r--   0        0        0      329 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/get_server_status.mcfunction
--rw-r--r--   0        0        0      576 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/send_sleep_status.mcfunction
--rw-r--r--   0        0        0     2053 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/show_sleep_percentage.mcfunction
--rw-r--r--   0        0        0     1203 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/track_leave_bed.mcfunction
--rw-r--r--   0        0        0      927 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/east.mcfunction
--rw-r--r--   0        0        0      927 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/north.mcfunction
--rw-r--r--   0        0        0      927 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/south.mcfunction
--rw-r--r--   0        0        0      927 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/west.mcfunction
--rw-r--r--   0        0        0     1096 2023-06-19 00:23:34.059520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock.mcfunction
--rw-r--r--   0        0        0      853 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_lock.mcfunction
--rw-r--r--   0        0        0      469 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/clicked_lockable_block.mcfunction
--rw-r--r--   0        0        0      651 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/raycast.mcfunction
--rw-r--r--   0        0        0     1799 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/send_message.mcfunction
--rw-r--r--   0        0        0     1183 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/predicates/impl/is_day.json
--rw-r--r--   0        0        0       87 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/tags/blocks/impl/chests.json
--rw-r--r--   0        0        0      394 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/tags/blocks/impl/lockable.json
--rw-r--r--   0        0        0       21 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/tags/functions/event/player/on_click_locked_container.json
--rw-r--r--   0        0        0    88530 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/pack.png
--rw-r--r--   0        0        0      280 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/README.md
--rw-r--r--   0        0        0      203 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/minecraft/models/item/furnace.json
--rw-r--r--   0        0        0      319 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/font/gui.json
--rw-r--r--   0        0        0      106 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/lang/en_us.json
--rw-r--r--   0        0        0     1361 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/models/block/table.json
--rw-r--r--   0        0        0      897 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/heavy_workbench.png
--rw-r--r--   0        0        0      287 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/table_front.png
--rw-r--r--   0        0        0      511 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/table_legacy.png
--rw-r--r--   0        0        0      299 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/table_side.png
--rw-r--r--   0        0        0      224 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/table_top.png
--rw-r--r--   0        0        0      336 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/gui/negative_space.png
--rw-r--r--   0        0        0      556 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/gui/table.png
--rw-r--r--   0        0        0      566 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/beet.yaml
--rw-r--r--   0        0        0      302 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/advancements/technical/craft_table.json
--rw-r--r--   0        0        0      496 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/advancements/technical/enter_gui.json
--rw-r--r--   0        0        0      147 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/place.mcfunction
--rw-r--r--   0        0        0      287 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/break/delete_output.mcfunction
--rw-r--r--   0        0        0      278 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/break/drop_item.mcfunction
--rw-r--r--   0        0        0      581 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/break.mcfunction
--rw-r--r--   0        0        0      139 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/craft.mcfunction
--rw-r--r--   0        0        0     2974 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/handle_tags.mcfunction
--rw-r--r--   0        0        0     3547 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/mirror.mcfunction
--rw-r--r--   0        0        0     6352 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/process.mcfunction
--rw-r--r--   0        0        0    11765 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/query_tags.mcfunction
--rw-r--r--   0        0        0     4476 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/read_barrel.mcfunction
--rw-r--r--   0        0        0     2119 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/export.mcfunction
--rw-r--r--   0        0        0     1397 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/export_output.mcfunction
--rw-r--r--   0        0        0     2061 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/move.mcfunction
--rw-r--r--   0        0        0      699 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/spawn_loop.mcfunction
--rw-r--r--   0        0        0      412 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/check.mcfunction
--rw-r--r--   0        0        0      161 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/advanced/buckets.mcfunction
--rw-r--r--   0        0        0      603 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/advanced.mcfunction
--rw-r--r--   0        0        0      127 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/delete_tool/sub.mcfunction
--rw-r--r--   0        0        0     6295 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/delete_tool.mcfunction
--rw-r--r--   0        0        0      637 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/handle_tools.mcfunction
--rw-r--r--   0        0        0     4715 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/test.mcfunction
--rw-r--r--   0        0        0      632 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input.mcfunction
--rw-r--r--   0        0        0      505 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/cursor_check/loop.mcfunction
--rw-r--r--   0        0        0      622 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/cursor_check/main.mcfunction
--rw-r--r--   0        0        0     3077 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/calculate_extras.mcfunction
--rw-r--r--   0        0        0     2678 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/main.mcfunction
--rw-r--r--   0        0        0      714 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/spawn_extra_items.mcfunction
--rw-r--r--   0        0        0      327 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/recipes.mcfunction
--rw-r--r--   0        0        0      200 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/append.mcfunction
--rw-r--r--   0        0        0      598 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/0.mcfunction
--rw-r--r--   0        0        0      539 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/1.mcfunction
--rw-r--r--   0        0        0      540 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/2.mcfunction
--rw-r--r--   0        0        0      540 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/3.mcfunction
--rw-r--r--   0        0        0      540 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/4.mcfunction
--rw-r--r--   0        0        0      540 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/5.mcfunction
--rw-r--r--   0        0        0      540 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/6.mcfunction
--rw-r--r--   0        0        0      540 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/7.mcfunction
--rw-r--r--   0        0        0      540 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/8.mcfunction
--rw-r--r--   0        0        0     2421 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/loop.mcfunction
--rw-r--r--   0        0        0      452 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/main.mcfunction
--rw-r--r--   0        0        0      593 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/simplify.mcfunction
--rw-r--r--   0        0        0      558 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes.mcfunction
--rw-r--r--   0        0        0      141 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/interact/enter_gui.mcfunction
--rw-r--r--   0        0        0     1583 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/open_tick.mcfunction
--rw-r--r--   0        0        0     1557 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/place.mcfunction
--rw-r--r--   0        0        0       73 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/reset.mcfunction
--rw-r--r--   0        0        0      393 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/tick.mcfunction
--rw-r--r--   0        0        0      157 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/entity/player/slow_tick.mcfunction
--rw-r--r--   0        0        0      574 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/recipes/shaped.mcfunction
--rw-r--r--   0        0        0      104 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/technical/armor_stand.mcfunction
--rw-r--r--   0        0        0      248 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/technical/load.mcfunction
--rw-r--r--   0        0        0      148 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/technical/slow_tick.mcfunction
--rw-r--r--   0        0        0      158 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/technical/tick.mcfunction
--rw-r--r--   0        0        0       43 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/zint/technical/craft_table.mcfunction
--rw-r--r--   0        0        0       57 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/zint/technical/enter_gui.mcfunction
--rw-r--r--   0        0        0      559 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/loot_tables/blocks/table.json
--rw-r--r--   0        0        0     3448 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/invalid_items.json
--rw-r--r--   0        0        0     1110 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/special_clear/buckets.json
--rw-r--r--   0        0        0     2198 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/special_clear/tools.json
--rw-r--r--   0        0        0      218 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/acacia_logs.json
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/anvil.json
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/arrows.json
--rw-r--r--   0        0        0      226 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/axolotl_tempt_items.json
--rw-r--r--   0        0        0      214 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/banners.json
--rw-r--r--   0        0        0      227 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/beacon_payment_items.json
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/beds.json
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/birch_logs.json
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/boats.json
--rw-r--r--   0        0        0      214 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/buttons.json
--rw-r--r--   0        0        0      214 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/candles.json
--rw-r--r--   0        0        0      214 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/carpets.json
--rw-r--r--   0        0        0      231 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/cluster_max_harvestables.json
--rw-r--r--   0        0        0      216 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/coal_ores.json
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/coals.json
--rw-r--r--   0        0        0      218 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/copper_ores.json
--rw-r--r--   0        0        0      231 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/creeper_drop_music_discs.json
--rw-r--r--   0        0        0      220 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/crimson_stems.json
--rw-r--r--   0        0        0      220 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/dark_oak_logs.json
--rw-r--r--   0        0        0      219 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/diamond_ores.json
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/doors.json
--rw-r--r--   0        0        0      219 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/emerald_ores.json
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/fences.json
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/fishes.json
--rw-r--r--   0        0        0      214 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/flowers.json
--rw-r--r--   0        0        0      215 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/fox_food.json
--rw-r--r--   0        0        0      230 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/freeze_immune_wearables.json
--rw-r--r--   0        0        0      216 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/gold_ores.json
--rw-r--r--   0        0        0      231 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/ignored_by_piglin_babies.json
--rw-r--r--   0        0        0      216 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/iron_ores.json
--rw-r--r--   0        0        0      218 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/jungle_logs.json
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/lapis_ores.json
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/leaves.json
--rw-r--r--   0        0        0      220 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/lectern_books.json
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/logs.json
--rw-r--r--   0        0        0      221 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/logs_that_burn.json
--rw-r--r--   0        0        0      218 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/music_discs.json
--rw-r--r--   0        0        0      225 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/non_flammable_wood.json
--rw-r--r--   0        0        0      215 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/oak_logs.json
--rw-r--r--   0        0        0      233 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/occludes_vibration_signals.json
--rw-r--r--   0        0        0      218 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/piglin_food.json
--rw-r--r--   0        0        0      219 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/piglin_loved.json
--rw-r--r--   0        0        0      224 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/piglin_repellents.json
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/planks.json
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/rails.json
--rw-r--r--   0        0        0      220 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/redstone_ores.json
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/sand.json
--rw-r--r--   0        0        0      215 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/saplings.json
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/signs.json
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/slabs.json
--rw-r--r--   0        0        0      220 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/small_flowers.json
--rw-r--r--   0        0        0      228 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/soul_fire_base_blocks.json
--rw-r--r--   0        0        0      218 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/spruce_logs.json
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/stairs.json
--rw-r--r--   0        0        0      219 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/stone_bricks.json
--rw-r--r--   0        0        0      231 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/stone_crafting_materials.json
--rw-r--r--   0        0        0      227 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/stone_tool_materials.json
--rw-r--r--   0        0        0      219 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/tall_flowers.json
--rw-r--r--   0        0        0      216 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/trapdoors.json
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/walls.json
--rw-r--r--   0        0        0      219 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/warped_stems.json
--rw-r--r--   0        0        0      221 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_buttons.json
--rw-r--r--   0        0        0      219 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_doors.json
--rw-r--r--   0        0        0      220 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_fences.json
--rw-r--r--   0        0        0      229 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_pressure_plates.json
--rw-r--r--   0        0        0      219 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_slabs.json
--rw-r--r--   0        0        0      220 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_stairs.json
--rw-r--r--   0        0        0      223 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_trapdoors.json
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wool.json
--rw-r--r--   0        0        0      422 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/recipes/table.json
--rw-r--r--   0        0        0       33 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/tags/functions/event/advanced_remove.json
--rw-r--r--   0        0        0       33 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/tags/functions/event/break.json
--rw-r--r--   0        0        0       33 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/tags/functions/event/query_tags.json
--rw-r--r--   0        0        0       66 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/tags/functions/event/recipes.json
--rw-r--r--   0        0        0       33 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/tags/functions/event/shapeless_recipes.json
--rw-r--r--   0        0        0    39527 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/tags/items/all.json
--rw-r--r--   0        0        0       63 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.custom_block/tags/functions/event/on_place.json
--rw-r--r--   0        0        0    88568 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter/pack.png
--rw-r--r--   0        0        0      311 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/beet.yaml
--rw-r--r--   0        0        0       72 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter/tags/functions/event/query_tags.json
--rw-r--r--   0        0        0       82 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter/tags/functions/event/recipes.json
--rw-r--r--   0        0        0       85 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter/tags/functions/event/shapeless_recipes.json
--rw-r--r--   0        0        0     1069 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_1.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_135.mcfunction
--rw-r--r--   0        0        0      204 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_16.mcfunction
--rw-r--r--   0        0        0      203 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_2.mcfunction
--rw-r--r--   0        0        0      209 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_271.mcfunction
--rw-r--r--   0        0        0      206 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_33.mcfunction
--rw-r--r--   0        0        0      203 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_4.mcfunction
--rw-r--r--   0        0        0      209 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_542.mcfunction
--rw-r--r--   0        0        0      206 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_67.mcfunction
--rw-r--r--   0        0        0      203 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_8.mcfunction
--rw-r--r--   0        0        0      977 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/100_101.mcfunction
--rw-r--r--   0        0        0     1092 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_103.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_104.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_106.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_110.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_118.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_135.mcfunction
--rw-r--r--   0        0        0      557 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/104_104.mcfunction
--rw-r--r--   0        0        0     1025 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/105_106.mcfunction
--rw-r--r--   0        0        0      924 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/107_108.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/107_110.mcfunction
--rw-r--r--   0        0        0      976 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/109_110.mcfunction
--rw-r--r--   0        0        0     1099 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/111_112.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/111_114.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/111_118.mcfunction
--rw-r--r--   0        0        0     1020 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/113_114.mcfunction
--rw-r--r--   0        0        0      946 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/115_116.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/115_118.mcfunction
--rw-r--r--   0        0        0      951 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/117_118.mcfunction
--rw-r--r--   0        0        0      915 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_120.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_121.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_123.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_127.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_135.mcfunction
--rw-r--r--   0        0        0      916 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/11_12.mcfunction
--rw-r--r--   0        0        0      528 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/121_121.mcfunction
--rw-r--r--   0        0        0      915 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/122_123.mcfunction
--rw-r--r--   0        0        0     1085 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/124_125.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/124_127.mcfunction
--rw-r--r--   0        0        0     1135 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/126_127.mcfunction
--rw-r--r--   0        0        0     1086 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/128_129.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/128_131.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/128_135.mcfunction
--rw-r--r--   0        0        0     1088 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/130_131.mcfunction
--rw-r--r--   0        0        0      928 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/132_133.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/132_135.mcfunction
--rw-r--r--   0        0        0      987 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/134_135.mcfunction
--rw-r--r--   0        0        0     1113 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_137.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_138.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_140.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_144.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_152.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_169.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_203.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_271.mcfunction
--rw-r--r--   0        0        0      507 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/138_138.mcfunction
--rw-r--r--   0        0        0     1032 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/139_140.mcfunction
--rw-r--r--   0        0        0     1025 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/13_14.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/13_16.mcfunction
--rw-r--r--   0        0        0     1138 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/141_142.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/141_144.mcfunction
--rw-r--r--   0        0        0      965 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/143_144.mcfunction
--rw-r--r--   0        0        0     1135 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/145_146.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/145_148.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/145_152.mcfunction
--rw-r--r--   0        0        0      952 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/147_148.mcfunction
--rw-r--r--   0        0        0     1121 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/149_150.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/149_152.mcfunction
--rw-r--r--   0        0        0     1062 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/151_152.mcfunction
--rw-r--r--   0        0        0     1015 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_154.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_155.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_157.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_161.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_169.mcfunction
--rw-r--r--   0        0        0      529 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/155_155.mcfunction
--rw-r--r--   0        0        0      994 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/156_157.mcfunction
--rw-r--r--   0        0        0     1033 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/158_159.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/158_161.mcfunction
--rw-r--r--   0        0        0     1049 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/15_16.mcfunction
--rw-r--r--   0        0        0     1003 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/160_161.mcfunction
--rw-r--r--   0        0        0      883 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/162_163.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/162_165.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/162_169.mcfunction
--rw-r--r--   0        0        0     1011 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/164_165.mcfunction
--rw-r--r--   0        0        0     1107 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/166_167.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/166_169.mcfunction
--rw-r--r--   0        0        0     1076 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/168_169.mcfunction
--rw-r--r--   0        0        0     1052 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_171.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_172.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_174.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_178.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_186.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_203.mcfunction
--rw-r--r--   0        0        0      536 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/172_172.mcfunction
--rw-r--r--   0        0        0     1004 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/173_174.mcfunction
--rw-r--r--   0        0        0      929 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/175_176.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/175_178.mcfunction
--rw-r--r--   0        0        0     1135 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/177_178.mcfunction
--rw-r--r--   0        0        0      960 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/179_180.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/179_182.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/179_186.mcfunction
--rw-r--r--   0        0        0     1085 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_18.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_19.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_21.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_25.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_33.mcfunction
--rw-r--r--   0        0        0     1096 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/181_182.mcfunction
--rw-r--r--   0        0        0     1020 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/183_184.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/183_186.mcfunction
--rw-r--r--   0        0        0     1209 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/185_186.mcfunction
--rw-r--r--   0        0        0      957 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_188.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_189.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.063520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_191.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_195.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_203.mcfunction
--rw-r--r--   0        0        0      573 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/189_189.mcfunction
--rw-r--r--   0        0        0     1060 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/190_191.mcfunction
--rw-r--r--   0        0        0     1012 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/192_193.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/192_195.mcfunction
--rw-r--r--   0        0        0     1111 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/194_195.mcfunction
--rw-r--r--   0        0        0     1013 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/196_197.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/196_199.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/196_203.mcfunction
--rw-r--r--   0        0        0     1061 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/198_199.mcfunction
--rw-r--r--   0        0        0      518 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/19_19.mcfunction
--rw-r--r--   0        0        0     1010 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/200_201.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/200_203.mcfunction
--rw-r--r--   0        0        0     1113 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/202_203.mcfunction
--rw-r--r--   0        0        0      913 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_205.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_206.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_208.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_212.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_220.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_237.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_271.mcfunction
--rw-r--r--   0        0        0      494 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/206_206.mcfunction
--rw-r--r--   0        0        0     1048 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/207_208.mcfunction
--rw-r--r--   0        0        0      962 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/209_210.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/209_212.mcfunction
--rw-r--r--   0        0        0     1089 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/20_21.mcfunction
--rw-r--r--   0        0        0     1090 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/211_212.mcfunction
--rw-r--r--   0        0        0     1118 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/213_214.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/213_216.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/213_220.mcfunction
--rw-r--r--   0        0        0     1059 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/215_216.mcfunction
--rw-r--r--   0        0        0      967 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/217_218.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/217_220.mcfunction
--rw-r--r--   0        0        0     1099 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/219_220.mcfunction
--rw-r--r--   0        0        0     1122 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_222.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_223.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_225.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_229.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_237.mcfunction
--rw-r--r--   0        0        0      503 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/223_223.mcfunction
--rw-r--r--   0        0        0      921 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/224_225.mcfunction
--rw-r--r--   0        0        0     1002 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/226_227.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/226_229.mcfunction
--rw-r--r--   0        0        0     1003 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/228_229.mcfunction
--rw-r--r--   0        0        0     1052 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/22_23.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/22_25.mcfunction
--rw-r--r--   0        0        0     1022 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/230_231.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/230_233.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/230_237.mcfunction
--rw-r--r--   0        0        0     1048 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/232_233.mcfunction
--rw-r--r--   0        0        0     1080 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/234_235.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/234_237.mcfunction
--rw-r--r--   0        0        0     1009 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/236_237.mcfunction
--rw-r--r--   0        0        0     1102 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_239.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_240.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_242.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_246.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_254.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_271.mcfunction
--rw-r--r--   0        0        0      516 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/240_240.mcfunction
--rw-r--r--   0        0        0     1006 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/241_242.mcfunction
--rw-r--r--   0        0        0     1008 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/243_244.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/243_246.mcfunction
--rw-r--r--   0        0        0     1071 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/245_246.mcfunction
--rw-r--r--   0        0        0     1069 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/247_248.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/247_250.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/247_254.mcfunction
--rw-r--r--   0        0        0     1017 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/249_250.mcfunction
--rw-r--r--   0        0        0      910 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/24_25.mcfunction
--rw-r--r--   0        0        0      965 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/251_252.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/251_254.mcfunction
--rw-r--r--   0        0        0      965 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/253_254.mcfunction
--rw-r--r--   0        0        0     1030 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_256.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_257.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_259.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_263.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_271.mcfunction
--rw-r--r--   0        0        0      499 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/257_257.mcfunction
--rw-r--r--   0        0        0     1123 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/258_259.mcfunction
--rw-r--r--   0        0        0      999 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/260_261.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/260_263.mcfunction
--rw-r--r--   0        0        0     1016 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/262_263.mcfunction
--rw-r--r--   0        0        0     1018 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/264_265.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/264_267.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/264_271.mcfunction
--rw-r--r--   0        0        0     1087 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/266_267.mcfunction
--rw-r--r--   0        0        0      992 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/268_269.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/268_271.mcfunction
--rw-r--r--   0        0        0      954 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/26_27.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/26_29.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/26_33.mcfunction
--rw-r--r--   0        0        0     1114 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/270_271.mcfunction
--rw-r--r--   0        0        0      992 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_273.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_274.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_276.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_280.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_288.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_305.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_339.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_407.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_542.mcfunction
--rw-r--r--   0        0        0      530 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/274_274.mcfunction
--rw-r--r--   0        0        0     1189 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/275_276.mcfunction
--rw-r--r--   0        0        0     1137 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/277_278.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/277_280.mcfunction
--rw-r--r--   0        0        0      957 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/279_280.mcfunction
--rw-r--r--   0        0        0     1109 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/281_282.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/281_284.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/281_288.mcfunction
--rw-r--r--   0        0        0     1189 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/283_284.mcfunction
--rw-r--r--   0        0        0      982 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/285_286.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/285_288.mcfunction
--rw-r--r--   0        0        0     1048 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/287_288.mcfunction
--rw-r--r--   0        0        0      962 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_290.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_291.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_293.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_297.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_305.mcfunction
--rw-r--r--   0        0        0     1071 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/28_29.mcfunction
--rw-r--r--   0        0        0      518 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/291_291.mcfunction
--rw-r--r--   0        0        0     1135 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/292_293.mcfunction
--rw-r--r--   0        0        0     1199 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/294_295.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/294_297.mcfunction
--rw-r--r--   0        0        0     1041 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/296_297.mcfunction
--rw-r--r--   0        0        0      936 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/298_299.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/298_301.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/298_305.mcfunction
--rw-r--r--   0        0        0      514 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/2_2.mcfunction
--rw-r--r--   0        0        0     1097 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/300_301.mcfunction
--rw-r--r--   0        0        0     1162 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/302_303.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/302_305.mcfunction
--rw-r--r--   0        0        0     1062 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/304_305.mcfunction
--rw-r--r--   0        0        0     1058 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_307.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_308.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_310.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_314.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_322.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_339.mcfunction
--rw-r--r--   0        0        0      501 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/308_308.mcfunction
--rw-r--r--   0        0        0     1023 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/309_310.mcfunction
--rw-r--r--   0        0        0      900 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/30_31.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/30_33.mcfunction
--rw-r--r--   0        0        0     1003 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/311_312.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/311_314.mcfunction
--rw-r--r--   0        0        0     1163 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/313_314.mcfunction
--rw-r--r--   0        0        0      999 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/315_316.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/315_318.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/315_322.mcfunction
--rw-r--r--   0        0        0     1041 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/317_318.mcfunction
--rw-r--r--   0        0        0      977 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/319_320.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/319_322.mcfunction
--rw-r--r--   0        0        0     1103 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/321_322.mcfunction
--rw-r--r--   0        0        0     1091 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_324.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_325.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_327.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_331.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_339.mcfunction
--rw-r--r--   0        0        0      529 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/325_325.mcfunction
--rw-r--r--   0        0        0      993 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/326_327.mcfunction
--rw-r--r--   0        0        0      935 2023-06-19 00:23:34.067520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/328_329.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/328_331.mcfunction
--rw-r--r--   0        0        0     1053 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/32_33.mcfunction
--rw-r--r--   0        0        0      932 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/330_331.mcfunction
--rw-r--r--   0        0        0      994 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/332_333.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/332_335.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/332_339.mcfunction
--rw-r--r--   0        0        0     1090 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/334_335.mcfunction
--rw-r--r--   0        0        0      929 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/336_337.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/336_339.mcfunction
--rw-r--r--   0        0        0     1093 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/338_339.mcfunction
--rw-r--r--   0        0        0     1153 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_341.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_342.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_344.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_348.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_356.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_373.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_407.mcfunction
--rw-r--r--   0        0        0      559 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/342_342.mcfunction
--rw-r--r--   0        0        0      969 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/343_344.mcfunction
--rw-r--r--   0        0        0     1114 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/345_346.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/345_348.mcfunction
--rw-r--r--   0        0        0      926 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/347_348.mcfunction
--rw-r--r--   0        0        0      915 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/349_350.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/349_352.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/349_356.mcfunction
--rw-r--r--   0        0        0     1059 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_35.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_36.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_38.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_42.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_50.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_67.mcfunction
--rw-r--r--   0        0        0     1085 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/351_352.mcfunction
--rw-r--r--   0        0        0     1135 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/353_354.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/353_356.mcfunction
--rw-r--r--   0        0        0     1120 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/355_356.mcfunction
--rw-r--r--   0        0        0      931 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_358.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_359.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_361.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_365.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_373.mcfunction
--rw-r--r--   0        0        0      587 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/359_359.mcfunction
--rw-r--r--   0        0        0      990 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/360_361.mcfunction
--rw-r--r--   0        0        0     1019 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/362_363.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/362_365.mcfunction
--rw-r--r--   0        0        0     1275 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/364_365.mcfunction
--rw-r--r--   0        0        0      882 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/366_367.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/366_369.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/366_373.mcfunction
--rw-r--r--   0        0        0     1179 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/368_369.mcfunction
--rw-r--r--   0        0        0      398 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/36_36.mcfunction
--rw-r--r--   0        0        0      972 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/370_371.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/370_373.mcfunction
--rw-r--r--   0        0        0     1165 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/372_373.mcfunction
--rw-r--r--   0        0        0      922 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_375.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_376.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_378.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_382.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_390.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_407.mcfunction
--rw-r--r--   0        0        0      580 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/376_376.mcfunction
--rw-r--r--   0        0        0      922 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/377_378.mcfunction
--rw-r--r--   0        0        0     1120 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/379_380.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/379_382.mcfunction
--rw-r--r--   0        0        0     1089 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/37_38.mcfunction
--rw-r--r--   0        0        0     1133 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/381_382.mcfunction
--rw-r--r--   0        0        0     1021 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/383_384.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/383_386.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/383_390.mcfunction
--rw-r--r--   0        0        0      946 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/385_386.mcfunction
--rw-r--r--   0        0        0     1057 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/387_388.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/387_390.mcfunction
--rw-r--r--   0        0        0      929 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/389_390.mcfunction
--rw-r--r--   0        0        0     1093 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_392.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_393.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_395.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_399.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_407.mcfunction
--rw-r--r--   0        0        0      586 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/393_393.mcfunction
--rw-r--r--   0        0        0     1126 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/394_395.mcfunction
--rw-r--r--   0        0        0     1021 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/396_397.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/396_399.mcfunction
--rw-r--r--   0        0        0     1064 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/398_399.mcfunction
--rw-r--r--   0        0        0     1144 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/39_40.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/39_42.mcfunction
--rw-r--r--   0        0        0      916 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/3_4.mcfunction
--rw-r--r--   0        0        0      989 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/400_401.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/400_403.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/400_407.mcfunction
--rw-r--r--   0        0        0      935 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/402_403.mcfunction
--rw-r--r--   0        0        0     1146 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/404_405.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/404_407.mcfunction
--rw-r--r--   0        0        0     1096 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/406_407.mcfunction
--rw-r--r--   0        0        0     1076 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_409.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_410.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_412.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_416.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_424.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_441.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_475.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_542.mcfunction
--rw-r--r--   0        0        0      518 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/410_410.mcfunction
--rw-r--r--   0        0        0     1000 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/411_412.mcfunction
--rw-r--r--   0        0        0      908 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/413_414.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/413_416.mcfunction
--rw-r--r--   0        0        0     1074 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/415_416.mcfunction
--rw-r--r--   0        0        0     1021 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/417_418.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/417_420.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/417_424.mcfunction
--rw-r--r--   0        0        0     1054 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/419_420.mcfunction
--rw-r--r--   0        0        0     1115 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/41_42.mcfunction
--rw-r--r--   0        0        0     1090 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/421_422.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/421_424.mcfunction
--rw-r--r--   0        0        0     1052 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/423_424.mcfunction
--rw-r--r--   0        0        0     1126 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_426.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_427.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_429.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_433.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_441.mcfunction
--rw-r--r--   0        0        0      553 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/427_427.mcfunction
--rw-r--r--   0        0        0     1082 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/428_429.mcfunction
--rw-r--r--   0        0        0      896 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/430_431.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/430_433.mcfunction
--rw-r--r--   0        0        0     1129 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/432_433.mcfunction
--rw-r--r--   0        0        0     1133 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/434_435.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/434_437.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/434_441.mcfunction
--rw-r--r--   0        0        0     1042 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/436_437.mcfunction
--rw-r--r--   0        0        0     1065 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/438_439.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/438_441.mcfunction
--rw-r--r--   0        0        0     1048 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/43_44.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/43_46.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/43_50.mcfunction
--rw-r--r--   0        0        0     1084 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/440_441.mcfunction
--rw-r--r--   0        0        0      979 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_443.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_444.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_446.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_450.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_458.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_475.mcfunction
--rw-r--r--   0        0        0      448 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/444_444.mcfunction
--rw-r--r--   0        0        0     1040 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/445_446.mcfunction
--rw-r--r--   0        0        0      996 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/447_448.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/447_450.mcfunction
--rw-r--r--   0        0        0      885 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/449_450.mcfunction
--rw-r--r--   0        0        0     1117 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/451_452.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/451_454.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/451_458.mcfunction
--rw-r--r--   0        0        0     1074 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/453_454.mcfunction
--rw-r--r--   0        0        0     1069 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/455_456.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/455_458.mcfunction
--rw-r--r--   0        0        0     1017 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/457_458.mcfunction
--rw-r--r--   0        0        0      965 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_460.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_461.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_463.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_467.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_475.mcfunction
--rw-r--r--   0        0        0      962 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/45_46.mcfunction
--rw-r--r--   0        0        0      413 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/461_461.mcfunction
--rw-r--r--   0        0        0     1085 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/462_463.mcfunction
--rw-r--r--   0        0        0     1013 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/464_465.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/464_467.mcfunction
--rw-r--r--   0        0        0      968 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/466_467.mcfunction
--rw-r--r--   0        0        0      951 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/468_469.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.071520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/468_471.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/468_475.mcfunction
--rw-r--r--   0        0        0     1048 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/470_471.mcfunction
--rw-r--r--   0        0        0      966 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/472_473.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/472_475.mcfunction
--rw-r--r--   0        0        0     1072 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/474_475.mcfunction
--rw-r--r--   0        0        0      970 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_477.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_478.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_480.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_484.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_492.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_509.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_542.mcfunction
--rw-r--r--   0        0        0      521 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/478_478.mcfunction
--rw-r--r--   0        0        0      891 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/479_480.mcfunction
--rw-r--r--   0        0        0     1068 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/47_48.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/47_50.mcfunction
--rw-r--r--   0        0        0     1086 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/481_482.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/481_484.mcfunction
--rw-r--r--   0        0        0     1090 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/483_484.mcfunction
--rw-r--r--   0        0        0     1094 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/485_486.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/485_488.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/485_492.mcfunction
--rw-r--r--   0        0        0     1069 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/487_488.mcfunction
--rw-r--r--   0        0        0     1059 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/489_490.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/489_492.mcfunction
--rw-r--r--   0        0        0     1133 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/491_492.mcfunction
--rw-r--r--   0        0        0      957 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_494.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_495.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_497.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_501.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_509.mcfunction
--rw-r--r--   0        0        0      513 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/495_495.mcfunction
--rw-r--r--   0        0        0     1031 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/496_497.mcfunction
--rw-r--r--   0        0        0     1017 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/498_499.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/498_501.mcfunction
--rw-r--r--   0        0        0     1135 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/49_50.mcfunction
--rw-r--r--   0        0        0     1003 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/500_501.mcfunction
--rw-r--r--   0        0        0      965 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/502_503.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/502_505.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/502_509.mcfunction
--rw-r--r--   0        0        0      965 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/504_505.mcfunction
--rw-r--r--   0        0        0     1067 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/506_507.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/506_509.mcfunction
--rw-r--r--   0        0        0     1012 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/508_509.mcfunction
--rw-r--r--   0        0        0     1014 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_511.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_512.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_514.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_518.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_526.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_542.mcfunction
--rw-r--r--   0        0        0      636 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/512_512.mcfunction
--rw-r--r--   0        0        0     1023 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/513_514.mcfunction
--rw-r--r--   0        0        0     1203 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/515_516.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/515_518.mcfunction
--rw-r--r--   0        0        0     1122 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/517_518.mcfunction
--rw-r--r--   0        0        0      978 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/519_520.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/519_522.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/519_526.mcfunction
--rw-r--r--   0        0        0     1098 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_52.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_53.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_55.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_59.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_67.mcfunction
--rw-r--r--   0        0        0     1143 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/521_522.mcfunction
--rw-r--r--   0        0        0      922 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/523_524.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/523_526.mcfunction
--rw-r--r--   0        0        0     1099 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/525_526.mcfunction
--rw-r--r--   0        0        0     1122 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/527_528.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/527_530.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/527_534.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/527_542.mcfunction
--rw-r--r--   0        0        0     1009 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/529_530.mcfunction
--rw-r--r--   0        0        0     1050 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/531_532.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/531_534.mcfunction
--rw-r--r--   0        0        0     1025 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/533_534.mcfunction
--rw-r--r--   0        0        0     1070 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/535_536.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/535_538.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/535_542.mcfunction
--rw-r--r--   0        0        0      972 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/537_538.mcfunction
--rw-r--r--   0        0        0     1108 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/539_540.mcfunction
--rw-r--r--   0        0        0      211 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/539_542.mcfunction
--rw-r--r--   0        0        0      563 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/53_53.mcfunction
--rw-r--r--   0        0        0     1126 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/541_542.mcfunction
--rw-r--r--   0        0        0      995 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/54_55.mcfunction
--rw-r--r--   0        0        0      950 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/56_57.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/56_59.mcfunction
--rw-r--r--   0        0        0      863 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/58_59.mcfunction
--rw-r--r--   0        0        0      965 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/5_6.mcfunction
--rw-r--r--   0        0        0      203 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/5_8.mcfunction
--rw-r--r--   0        0        0      995 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/60_61.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/60_63.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/60_67.mcfunction
--rw-r--r--   0        0        0     1059 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/62_63.mcfunction
--rw-r--r--   0        0        0      967 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/64_65.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/64_67.mcfunction
--rw-r--r--   0        0        0     1099 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/66_67.mcfunction
--rw-r--r--   0        0        0      208 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_101.mcfunction
--rw-r--r--   0        0        0      210 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_135.mcfunction
--rw-r--r--   0        0        0     1122 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_69.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_70.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_72.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_76.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_84.mcfunction
--rw-r--r--   0        0        0      485 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/70_70.mcfunction
--rw-r--r--   0        0        0     1051 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/71_72.mcfunction
--rw-r--r--   0        0        0      959 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/73_74.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/73_76.mcfunction
--rw-r--r--   0        0        0     1084 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/75_76.mcfunction
--rw-r--r--   0        0        0     1087 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/77_78.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/77_80.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/77_84.mcfunction
--rw-r--r--   0        0        0      993 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/79_80.mcfunction
--rw-r--r--   0        0        0     1085 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/7_8.mcfunction
--rw-r--r--   0        0        0     1036 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/81_82.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/81_84.mcfunction
--rw-r--r--   0        0        0     1005 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/83_84.mcfunction
--rw-r--r--   0        0        0      208 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_101.mcfunction
--rw-r--r--   0        0        0     1003 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_86.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_87.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_89.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_93.mcfunction
--rw-r--r--   0        0        0      486 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/87_87.mcfunction
--rw-r--r--   0        0        0     1015 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/88_89.mcfunction
--rw-r--r--   0        0        0      913 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/90_91.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/90_93.mcfunction
--rw-r--r--   0        0        0     1151 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/92_93.mcfunction
--rw-r--r--   0        0        0      208 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/94_101.mcfunction
--rw-r--r--   0        0        0      957 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/94_95.mcfunction
--rw-r--r--   0        0        0      207 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/94_97.mcfunction
--rw-r--r--   0        0        0     1053 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/96_97.mcfunction
--rw-r--r--   0        0        0      209 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/98_101.mcfunction
--rw-r--r--   0        0        0     1133 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/98_99.mcfunction
--rw-r--r--   0        0        0     1047 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/9_10.mcfunction
--rw-r--r--   0        0        0      206 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/9_12.mcfunction
--rw-r--r--   0        0        0      206 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/9_16.mcfunction
--rw-r--r--   0        0        0      603 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_1.mcfunction
--rw-r--r--   0        0        0      210 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_11.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_182.mcfunction
--rw-r--r--   0        0        0      209 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_2.mcfunction
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_22.mcfunction
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_45.mcfunction
--rw-r--r--   0        0        0      209 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_5.mcfunction
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_91.mcfunction
--rw-r--r--   0        0        0      328 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/100_100.mcfunction
--rw-r--r--   0        0        0      652 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/101_102.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/101_103.mcfunction
--rw-r--r--   0        0        0      324 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/103_103.mcfunction
--rw-r--r--   0        0        0      699 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/104_105.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/104_106.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/104_109.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/104_114.mcfunction
--rw-r--r--   0        0        0      302 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/106_106.mcfunction
--rw-r--r--   0        0        0      591 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/107_108.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/107_109.mcfunction
--rw-r--r--   0        0        0      319 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/109_109.mcfunction
--rw-r--r--   0        0        0      687 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/110_111.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/110_112.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/110_114.mcfunction
--rw-r--r--   0        0        0      294 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/112_112.mcfunction
--rw-r--r--   0        0        0      638 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/113_114.mcfunction
--rw-r--r--   0        0        0      609 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_116.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_117.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_120.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_126.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.075520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_137.mcfunction
--rw-r--r--   0        0        0      315 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/117_117.mcfunction
--rw-r--r--   0        0        0      649 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/118_119.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/118_120.mcfunction
--rw-r--r--   0        0        0      319 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/11_11.mcfunction
--rw-r--r--   0        0        0      290 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/120_120.mcfunction
--rw-r--r--   0        0        0      631 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/121_122.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/121_123.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/121_126.mcfunction
--rw-r--r--   0        0        0      317 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/123_123.mcfunction
--rw-r--r--   0        0        0      626 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/124_125.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/124_126.mcfunction
--rw-r--r--   0        0        0      319 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/126_126.mcfunction
--rw-r--r--   0        0        0      687 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/127_128.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/127_129.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/127_132.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/127_137.mcfunction
--rw-r--r--   0        0        0      315 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/129_129.mcfunction
--rw-r--r--   0        0        0      608 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/12_13.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/12_14.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/12_17.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/12_22.mcfunction
--rw-r--r--   0        0        0      725 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/130_131.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/130_132.mcfunction
--rw-r--r--   0        0        0      402 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/132_132.mcfunction
--rw-r--r--   0        0        0      592 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/133_134.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/133_135.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/133_137.mcfunction
--rw-r--r--   0        0        0      294 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/135_135.mcfunction
--rw-r--r--   0        0        0      607 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/136_137.mcfunction
--rw-r--r--   0        0        0      675 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_139.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_140.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_143.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_149.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_160.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_182.mcfunction
--rw-r--r--   0        0        0      287 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/140_140.mcfunction
--rw-r--r--   0        0        0      572 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/141_142.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/141_143.mcfunction
--rw-r--r--   0        0        0      288 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/143_143.mcfunction
--rw-r--r--   0        0        0      651 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/144_145.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/144_146.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/144_149.mcfunction
--rw-r--r--   0        0        0      293 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/146_146.mcfunction
--rw-r--r--   0        0        0      603 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/147_148.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/147_149.mcfunction
--rw-r--r--   0        0        0      289 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/149_149.mcfunction
--rw-r--r--   0        0        0      315 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/14_14.mcfunction
--rw-r--r--   0        0        0      576 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/150_151.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/150_152.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/150_155.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/150_160.mcfunction
--rw-r--r--   0        0        0      321 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/152_152.mcfunction
--rw-r--r--   0        0        0      604 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/153_154.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/153_155.mcfunction
--rw-r--r--   0        0        0      329 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/155_155.mcfunction
--rw-r--r--   0        0        0      660 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/156_157.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/156_158.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/156_160.mcfunction
--rw-r--r--   0        0        0      339 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/158_158.mcfunction
--rw-r--r--   0        0        0      674 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/159_160.mcfunction
--rw-r--r--   0        0        0      656 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/15_16.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/15_17.mcfunction
--rw-r--r--   0        0        0      706 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_162.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_163.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_166.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_171.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_182.mcfunction
--rw-r--r--   0        0        0      335 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/163_163.mcfunction
--rw-r--r--   0        0        0      696 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/164_165.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/164_166.mcfunction
--rw-r--r--   0        0        0      357 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/166_166.mcfunction
--rw-r--r--   0        0        0      682 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/167_168.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/167_169.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/167_171.mcfunction
--rw-r--r--   0        0        0      355 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/169_169.mcfunction
--rw-r--r--   0        0        0      645 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/170_171.mcfunction
--rw-r--r--   0        0        0      683 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/172_173.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/172_174.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/172_177.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/172_182.mcfunction
--rw-r--r--   0        0        0      290 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/174_174.mcfunction
--rw-r--r--   0        0        0      638 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/175_176.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/175_177.mcfunction
--rw-r--r--   0        0        0      319 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/177_177.mcfunction
--rw-r--r--   0        0        0      687 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/178_179.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/178_180.mcfunction
--rw-r--r--   0        0        0      217 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/178_182.mcfunction
--rw-r--r--   0        0        0      290 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/17_17.mcfunction
--rw-r--r--   0        0        0      291 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/180_180.mcfunction
--rw-r--r--   0        0        0      612 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/181_182.mcfunction
--rw-r--r--   0        0        0      602 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/18_19.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/18_20.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/18_22.mcfunction
--rw-r--r--   0        0        0      291 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/20_20.mcfunction
--rw-r--r--   0        0        0      632 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/21_22.mcfunction
--rw-r--r--   0        0        0      683 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_24.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_25.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_28.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_34.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_45.mcfunction
--rw-r--r--   0        0        0      292 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/25_25.mcfunction
--rw-r--r--   0        0        0      605 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/26_27.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/26_28.mcfunction
--rw-r--r--   0        0        0      296 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/28_28.mcfunction
--rw-r--r--   0        0        0      631 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/29_30.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/29_31.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/29_34.mcfunction
--rw-r--r--   0        0        0      316 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/2_2.mcfunction
--rw-r--r--   0        0        0      300 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/31_31.mcfunction
--rw-r--r--   0        0        0      623 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/32_33.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/32_34.mcfunction
--rw-r--r--   0        0        0      315 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/34_34.mcfunction
--rw-r--r--   0        0        0      679 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/35_36.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/35_37.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/35_40.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/35_45.mcfunction
--rw-r--r--   0        0        0      317 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/37_37.mcfunction
--rw-r--r--   0        0        0      611 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/38_39.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/38_40.mcfunction
--rw-r--r--   0        0        0      620 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/3_4.mcfunction
--rw-r--r--   0        0        0      209 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/3_5.mcfunction
--rw-r--r--   0        0        0      292 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/40_40.mcfunction
--rw-r--r--   0        0        0      590 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/41_42.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/41_43.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/41_45.mcfunction
--rw-r--r--   0        0        0      322 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/43_43.mcfunction
--rw-r--r--   0        0        0      676 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/44_45.mcfunction
--rw-r--r--   0        0        0      680 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_47.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_48.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_51.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_57.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_68.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_91.mcfunction
--rw-r--r--   0        0        0      327 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/48_48.mcfunction
--rw-r--r--   0        0        0      619 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/49_50.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/49_51.mcfunction
--rw-r--r--   0        0        0      293 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/51_51.mcfunction
--rw-r--r--   0        0        0      625 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/52_53.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/52_54.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/52_57.mcfunction
--rw-r--r--   0        0        0      315 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/54_54.mcfunction
--rw-r--r--   0        0        0      680 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/55_56.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/55_57.mcfunction
--rw-r--r--   0        0        0      317 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/57_57.mcfunction
--rw-r--r--   0        0        0      634 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/58_59.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/58_60.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/58_63.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/58_68.mcfunction
--rw-r--r--   0        0        0      303 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/5_5.mcfunction
--rw-r--r--   0        0        0      486 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/60_60.mcfunction
--rw-r--r--   0        0        0      653 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/61_62.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/61_63.mcfunction
--rw-r--r--   0        0        0      292 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/63_63.mcfunction
--rw-r--r--   0        0        0      591 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/64_65.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/64_66.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/64_68.mcfunction
--rw-r--r--   0        0        0      305 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/66_66.mcfunction
--rw-r--r--   0        0        0      622 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/67_68.mcfunction
--rw-r--r--   0        0        0      703 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_70.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_71.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_74.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_80.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_91.mcfunction
--rw-r--r--   0        0        0      210 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/6_11.mcfunction
--rw-r--r--   0        0        0      634 2023-06-19 00:23:34.079520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/6_7.mcfunction
--rw-r--r--   0        0        0      209 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/6_8.mcfunction
--rw-r--r--   0        0        0      297 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/71_71.mcfunction
--rw-r--r--   0        0        0      650 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/72_73.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/72_74.mcfunction
--rw-r--r--   0        0        0      327 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/74_74.mcfunction
--rw-r--r--   0        0        0      703 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/75_76.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/75_77.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/75_80.mcfunction
--rw-r--r--   0        0        0      297 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/77_77.mcfunction
--rw-r--r--   0        0        0      652 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/78_79.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/78_80.mcfunction
--rw-r--r--   0        0        0      297 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/80_80.mcfunction
--rw-r--r--   0        0        0      626 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/81_82.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/81_83.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/81_86.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/81_91.mcfunction
--rw-r--r--   0        0        0      315 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/83_83.mcfunction
--rw-r--r--   0        0        0      679 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/84_85.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/84_86.mcfunction
--rw-r--r--   0        0        0      316 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/86_86.mcfunction
--rw-r--r--   0        0        0      638 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/87_88.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/87_89.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/87_91.mcfunction
--rw-r--r--   0        0        0      321 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/89_89.mcfunction
--rw-r--r--   0        0        0      375 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/8_8.mcfunction
--rw-r--r--   0        0        0      659 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/90_91.mcfunction
--rw-r--r--   0        0        0      214 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_103.mcfunction
--rw-r--r--   0        0        0      216 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_114.mcfunction
--rw-r--r--   0        0        0      216 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_137.mcfunction
--rw-r--r--   0        0        0      216 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_182.mcfunction
--rw-r--r--   0        0        0      694 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_93.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_94.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_97.mcfunction
--rw-r--r--   0        0        0      288 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/94_94.mcfunction
--rw-r--r--   0        0        0      642 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/95_96.mcfunction
--rw-r--r--   0        0        0      213 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/95_97.mcfunction
--rw-r--r--   0        0        0      323 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/97_97.mcfunction
--rw-r--r--   0        0        0      215 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/98_100.mcfunction
--rw-r--r--   0        0        0      216 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/98_103.mcfunction
--rw-r--r--   0        0        0      632 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/98_99.mcfunction
--rw-r--r--   0        0        0      580 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/9_10.mcfunction
--rw-r--r--   0        0        0      212 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/9_11.mcfunction
--rw-r--r--   0        0        0     1376 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/tags/query.mcfunction
--rw-r--r--   0        0        0      260 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/coal_charcoal.json
--rw-r--r--   0        0        0      273 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/purpur_decoration.json
--rw-r--r--   0        0        0      320 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/quartz_decoration.json
--rw-r--r--   0        0        0      283 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/red_sandstone.json
--rw-r--r--   0        0        0      326 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/red_sandstone_and_cut.json
--rw-r--r--   0        0        0      260 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/sand_and_red_sand.json
--rw-r--r--   0        0        0      275 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/sandstone.json
--rw-r--r--   0        0        0      314 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/sandstone_and_cut.json
--rw-r--r--   0        0        0    80541 2023-06-19 00:23:34.083520 smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/pack.png
--rw-r--r--   0        0        0      509 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/README.md
--rw-r--r--   0        0        0      319 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/beet.yaml
--rw-r--r--   0        0        0      543 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/advancements/impl/technical/place_custom_block.json
--rw-r--r--   0        0        0      240 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place/block_unchanged.mcfunction
--rw-r--r--   0        0        0      357 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place/found.mcfunction
--rw-r--r--   0        0        0    27546 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place/layer.mcfunction
--rw-r--r--   0        0        0      205 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place/throw_warning.mcfunction
--rw-r--r--   0        0        0     1420 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place.mcfunction
--rw-r--r--   0        0        0     1280 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/technical/def_const.mcfunction
--rw-r--r--   0        0        0     1065 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/technical/load.mcfunction
--rw-r--r--   0        0        0      264 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/technical/tick.mcfunction
--rw-r--r--   0        0        0      269 2023-06-19 00:23:34.087520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/tags/blocks/placeable.json
--rw-r--r--   0        0        0    88530 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/pack.png
--rw-r--r--   0        0        0      509 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/README.md
--rw-r--r--   0        0        0      232 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/beet.yaml
--rw-r--r--   0        0        0     1636 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/advancements/impl/player/event.json
--rw-r--r--   0        0        0     2050 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/armor.mcfunction
--rw-r--r--   0        0        0     2163 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/explosion.mcfunction
--rw-r--r--   0        0        0     2161 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/projectile.mcfunction
--rw-r--r--   0        0        0     1304 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply.mcfunction
--rw-r--r--   0        0        0     1744 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/blast_protection.mcfunction
--rw-r--r--   0        0        0     1764 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/proj_protection.mcfunction
--rw-r--r--   0        0        0     2062 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/protection.mcfunction
--rw-r--r--   0        0        0     1393 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/resistance.mcfunction
--rw-r--r--   0        0        0     3290 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/toughness.mcfunction
--rw-r--r--   0        0        0      142 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/1.mcfunction
--rw-r--r--   0        0        0      148 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/1024.mcfunction
--rw-r--r--   0        0        0      146 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/128.mcfunction
--rw-r--r--   0        0        0      144 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/16.mcfunction
--rw-r--r--   0        0        0      142 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/2.mcfunction
--rw-r--r--   0        0        0      146 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/256.mcfunction
--rw-r--r--   0        0        0      144 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/32.mcfunction
--rw-r--r--   0        0        0      142 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/4.mcfunction
--rw-r--r--   0        0        0      146 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/512.mcfunction
--rw-r--r--   0        0        0      144 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/64.mcfunction
--rw-r--r--   0        0        0      142 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/8.mcfunction
--rw-r--r--   0        0        0     1166 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/give.mcfunction
--rw-r--r--   0        0        0      979 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/remove.mcfunction
--rw-r--r--   0        0        0      107 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/schedule.mcfunction
--rw-r--r--   0        0        0     1358 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/death_message.mcfunction
--rw-r--r--   0        0        0      344 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/calculate_modifier.mcfunction
--rw-r--r--   0        0        0       87 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/get_entity_health.mcfunction
--rw-r--r--   0        0        0      191 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/update.mcfunction
--rw-r--r--   0        0        0      743 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/update_entity.mcfunction
--rw-r--r--   0        0        0      160 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/update_player.mcfunction
--rw-r--r--   0        0        0     1471 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/on_death.mcfunction
--rw-r--r--   0        0        0     2469 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/player/event.mcfunction
--rw-r--r--   0        0        0     1321 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/technical/def_const.mcfunction
--rw-r--r--   0        0        0      143 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/technical/load.mcfunction
--rw-r--r--   0        0        0      425 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/tags/entity_types/undead.json
--rw-r--r--   0        0        0       21 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/tags/functions/event/entity/on_death.json
--rw-r--r--   0        0        0       20 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/tags/functions/event/player/on_damage.json
--rw-r--r--   0        0        0       20 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/tags/functions/event/player/on_death_message.json
--rw-r--r--   0        0        0    88530 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/damage/pack.png
--rw-r--r--   0        0        0      363 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/assets/smithed.enchanter/font/gui.json
--rw-r--r--   0        0        0      102 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/assets/smithed.enchanter/lang/en_us.json
--rw-r--r--   0        0        0      444 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/assets/smithed.enchanter/textures/gui/table.png
--rw-r--r--   0        0        0      410 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/beet.yaml
--rw-r--r--   0        0        0      299 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/advancements/impl/test.json
--rw-r--r--   0        0        0     1348 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_bookshelves.mcfunction
--rw-r--r--   0        0        0      938 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_levels.mcfunction
--rw-r--r--   0        0        0      627 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_modified_level.mcfunction
--rw-r--r--   0        0        0     1128 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/place.mcfunction
--rw-r--r--   0        0        0       44 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/tick.mcfunction
--rw-r--r--   0        0        0     1557 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/binomial_random.mcfunction
--rw-r--r--   0        0        0      356 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/load.mcfunction
--rw-r--r--   0        0        0       95 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/path.mcfunction
--rw-r--r--   0        0        0      132 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/tick.mcfunction
--rw-r--r--   0        0        0      469 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/uniform_random.mcfunction
--rw-r--r--   0        0        0      604 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/test.mcfunction
--rw-r--r--   0        0        0      507 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/README.md
--rw-r--r--   0        0        0      288 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/beet.yaml
--rw-r--r--   0        0        0      340 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/advancements/impl/technical/inventory_changed.json
--rw-r--r--   0        0        0     3762 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_durability.mcfunction
--rw-r--r--   0        0        0     1838 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_mending/clamp.mcfunction
--rw-r--r--   0        0        0      228 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_mending/return_overflow.mcfunction
--rw-r--r--   0        0        0      323 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_mending.mcfunction
--rw-r--r--   0        0        0      414 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/boots.mcfunction
--rw-r--r--   0        0        0      416 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/chestplate.mcfunction
--rw-r--r--   0        0        0      336 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/force/sub.mcfunction
--rw-r--r--   0        0        0     1668 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/force.mcfunction
--rw-r--r--   0        0        0      414 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/helmet.mcfunction
--rw-r--r--   0        0        0      414 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/leggings.mcfunction
--rw-r--r--   0        0        0      414 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/mainhand.mcfunction
--rw-r--r--   0        0        0      423 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/offhand.mcfunction
--rw-r--r--   0        0        0      498 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage.mcfunction
--rw-r--r--   0        0        0      774 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/detect.mcfunction
--rw-r--r--   0        0        0     8770 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/get_max.mcfunction
--rw-r--r--   0        0        0      221 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/init.mcfunction
--rw-r--r--   0        0        0      404 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/boots.mcfunction
--rw-r--r--   0        0        0      406 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/chestplate.mcfunction
--rw-r--r--   0        0        0      439 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/handle.mcfunction
--rw-r--r--   0        0        0      404 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/helmet.mcfunction
--rw-r--r--   0        0        0      404 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/leggings.mcfunction
--rw-r--r--   0        0        0      405 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/mainhand.mcfunction
--rw-r--r--   0        0        0      413 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/offhand.mcfunction
--rw-r--r--   0        0        0     8473 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/attributes.mcfunction
--rw-r--r--   0        0        0    13178 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/base_attributes.mcfunction
--rw-r--r--   0        0        0     2218 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/build.mcfunction
--rw-r--r--   0        0        0      675 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/custom.mcfunction
--rw-r--r--   0        0        0      405 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/durability.mcfunction
--rw-r--r--   0        0        0     3259 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/enchantments.mcfunction
--rw-r--r--   0        0        0        0 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/update_inventory.mcfunction
--rw-r--r--   0        0        0      171 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/technical/load.mcfunction
--rw-r--r--   0        0        0      110 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/technical/player.mcfunction
--rw-r--r--   0        0        0      124 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/technical/tick.mcfunction
--rw-r--r--   0        0        0      282 2023-06-19 00:23:34.091520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/item_modifiers/update_nbt.json
--rw-r--r--   0        0        0       86 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/predicates/chance/10.json
--rw-r--r--   0        0        0       94 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/predicates/chance/11.json
--rw-r--r--   0        0        0       88 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/predicates/chance/12.json
--rw-r--r--   0        0        0       93 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/predicates/chance/14.json
--rw-r--r--   0        0        0       94 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/predicates/chance/16.json
--rw-r--r--   0        0        0       87 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/predicates/chance/20.json
--rw-r--r--   0        0        0       87 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/predicates/chance/25.json
--rw-r--r--   0        0        0       94 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/predicates/chance/33.json
--rw-r--r--   0        0        0       86 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/predicates/chance/50.json
--rw-r--r--   0        0        0       95 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/predicates/chance/9.json
--rw-r--r--   0        0        0       20 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/tags/functions/event/build_custom.json
--rw-r--r--   0        0        0    88530 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/item/pack.png
--rw-r--r--   0        0        0       19 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/prevent-aggression/README.md
--rw-r--r--   0        0        0      257 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/prevent-aggression/beet.yaml
--rw-r--r--   0        0        0     2399 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/prevent-aggression/data/smithed.prevent_aggression/functions/impl/technical/10_tick.mcfunction
--rw-r--r--   0        0        0      175 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/prevent-aggression/data/smithed.prevent_aggression/functions/impl/technical/load.mcfunction
--rw-r--r--   0        0        0      359 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/prevent-aggression/data/smithed.prevent_aggression/tags/entity_types/mobs.json
--rw-r--r--   0        0        0    13663 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/packs/prevent-aggression/pack.png
--rw-r--r--   0        0        0        0 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/__init__.py
--rw-r--r--   0        0        0      553 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/companion_mod.py
--rw-r--r--   0        0        0     4105 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/documentation.py
--rw-r--r--   0        0        0      729 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/manifest.py
--rw-r--r--   0        0        0     1050 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/misc.py
--rw-r--r--   0        0        0     2158 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/nbt_literals.py
--rw-r--r--   0        0        0      129 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/README.md
--rw-r--r--   0        0        0       61 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/__init__.py
--rw-r--r--   0        0        0     1304 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/api.py
--rw-r--r--   0        0        0     8097 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/load.py
--rw-r--r--   0        0        0     3985 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/models.py
--rw-r--r--   0        0        0     1478 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/plugin.py
--rw-r--r--   0        0        0      112 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/types.py
--rw-r--r--   0        0        0      483 2023-06-19 00:23:34.095520 smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/utils.py
--rw-r--r--   0        0        0     9653 1970-01-01 00:00:00.000000 smithed_libraries-0.7.0/setup.py
--rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 smithed_libraries-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/LICENSE
+-rw-r--r--   0        0        0      654 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/README.md
+-rw-r--r--   0        0        0      980 2023-06-24 17:52:04.810249 smithed_libraries-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      571 2023-06-24 17:52:04.794249 smithed_libraries-0.7.1/smithed_libraries/__init__.py
+-rw-r--r--   0        0        0     2219 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/common.yaml
+-rw-r--r--   0        0        0      939 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/README.md
+-rw-r--r--   0        0        0      223 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/beet.yaml
+-rw-r--r--   0        0        0     3808 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/advancements/impl/vanilla/bed/clicked_bed.json
+-rw-r--r--   0        0        0      323 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/advancements/impl/vanilla/bed/slept_in_bed.json
+-rw-r--r--   0        0        0     1467 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/advancements/impl/vanilla/container/clicked_lockable_block.json
+-rw-r--r--   0        0        0     1215 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/display.mcfunction
+-rw-r--r--   0        0        0     2167 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/message.mcfunction
+-rw-r--r--   0        0        0      264 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/reset.mcfunction
+-rw-r--r--   0        0        0      924 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/technical/load.mcfunction
+-rw-r--r--   0        0        0      754 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/technical/tick.mcfunction
+-rw-r--r--   0        0        0      855 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/check_sleep_status.mcfunction
+-rw-r--r--   0        0        0     1124 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/clicked_bed.mcfunction
+-rw-r--r--   0        0        0      329 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/get_server_status.mcfunction
+-rw-r--r--   0        0        0      576 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/send_sleep_status.mcfunction
+-rw-r--r--   0        0        0     2053 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/show_sleep_percentage.mcfunction
+-rw-r--r--   0        0        0     1203 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/track_leave_bed.mcfunction
+-rw-r--r--   0        0        0      927 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/east.mcfunction
+-rw-r--r--   0        0        0      927 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/north.mcfunction
+-rw-r--r--   0        0        0      927 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/south.mcfunction
+-rw-r--r--   0        0        0      927 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/west.mcfunction
+-rw-r--r--   0        0        0     1096 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock.mcfunction
+-rw-r--r--   0        0        0      853 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_lock.mcfunction
+-rw-r--r--   0        0        0      469 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/clicked_lockable_block.mcfunction
+-rw-r--r--   0        0        0      651 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/raycast.mcfunction
+-rw-r--r--   0        0        0     1799 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/send_message.mcfunction
+-rw-r--r--   0        0        0     1183 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/predicates/impl/is_day.json
+-rw-r--r--   0        0        0       87 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/tags/blocks/impl/chests.json
+-rw-r--r--   0        0        0      394 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/tags/blocks/impl/lockable.json
+-rw-r--r--   0        0        0       21 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/tags/functions/event/player/on_click_locked_container.json
+-rw-r--r--   0        0        0    88530 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/pack.png
+-rw-r--r--   0        0        0      280 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/README.md
+-rw-r--r--   0        0        0      203 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/minecraft/models/item/furnace.json
+-rw-r--r--   0        0        0      319 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/font/gui.json
+-rw-r--r--   0        0        0      106 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/lang/en_us.json
+-rw-r--r--   0        0        0     1361 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/models/block/table.json
+-rw-r--r--   0        0        0      897 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/heavy_workbench.png
+-rw-r--r--   0        0        0      287 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/table_front.png
+-rw-r--r--   0        0        0      511 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/table_legacy.png
+-rw-r--r--   0        0        0      299 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/table_side.png
+-rw-r--r--   0        0        0      224 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/table_top.png
+-rw-r--r--   0        0        0      336 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/gui/negative_space.png
+-rw-r--r--   0        0        0      556 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/gui/table.png
+-rw-r--r--   0        0        0      566 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/beet.yaml
+-rw-r--r--   0        0        0      302 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/advancements/technical/craft_table.json
+-rw-r--r--   0        0        0      496 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/advancements/technical/enter_gui.json
+-rw-r--r--   0        0        0      147 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/place.mcfunction
+-rw-r--r--   0        0        0      287 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/break/delete_output.mcfunction
+-rw-r--r--   0        0        0      278 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/break/drop_item.mcfunction
+-rw-r--r--   0        0        0      581 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/break.mcfunction
+-rw-r--r--   0        0        0      139 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/craft.mcfunction
+-rw-r--r--   0        0        0     2974 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/handle_tags.mcfunction
+-rw-r--r--   0        0        0     3547 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/mirror.mcfunction
+-rw-r--r--   0        0        0     6352 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/process.mcfunction
+-rw-r--r--   0        0        0    11765 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/query_tags.mcfunction
+-rw-r--r--   0        0        0     4476 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/read_barrel.mcfunction
+-rw-r--r--   0        0        0     2119 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/export.mcfunction
+-rw-r--r--   0        0        0     1397 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/export_output.mcfunction
+-rw-r--r--   0        0        0     2061 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/move.mcfunction
+-rw-r--r--   0        0        0      699 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/spawn_loop.mcfunction
+-rw-r--r--   0        0        0      412 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/check.mcfunction
+-rw-r--r--   0        0        0      161 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/advanced/buckets.mcfunction
+-rw-r--r--   0        0        0      603 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/advanced.mcfunction
+-rw-r--r--   0        0        0      127 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/delete_tool/sub.mcfunction
+-rw-r--r--   0        0        0     6295 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/delete_tool.mcfunction
+-rw-r--r--   0        0        0      637 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/handle_tools.mcfunction
+-rw-r--r--   0        0        0     4715 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/test.mcfunction
+-rw-r--r--   0        0        0      632 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input.mcfunction
+-rw-r--r--   0        0        0      505 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/cursor_check/loop.mcfunction
+-rw-r--r--   0        0        0      622 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/cursor_check/main.mcfunction
+-rw-r--r--   0        0        0     3077 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/calculate_extras.mcfunction
+-rw-r--r--   0        0        0     2678 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/main.mcfunction
+-rw-r--r--   0        0        0      714 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/spawn_extra_items.mcfunction
+-rw-r--r--   0        0        0      327 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/recipes.mcfunction
+-rw-r--r--   0        0        0      200 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/append.mcfunction
+-rw-r--r--   0        0        0      598 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/0.mcfunction
+-rw-r--r--   0        0        0      539 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/1.mcfunction
+-rw-r--r--   0        0        0      540 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/2.mcfunction
+-rw-r--r--   0        0        0      540 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/3.mcfunction
+-rw-r--r--   0        0        0      540 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/4.mcfunction
+-rw-r--r--   0        0        0      540 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/5.mcfunction
+-rw-r--r--   0        0        0      540 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/6.mcfunction
+-rw-r--r--   0        0        0      540 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/7.mcfunction
+-rw-r--r--   0        0        0      540 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/8.mcfunction
+-rw-r--r--   0        0        0     2421 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/loop.mcfunction
+-rw-r--r--   0        0        0      452 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/main.mcfunction
+-rw-r--r--   0        0        0      593 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/simplify.mcfunction
+-rw-r--r--   0        0        0      558 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes.mcfunction
+-rw-r--r--   0        0        0      141 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/interact/enter_gui.mcfunction
+-rw-r--r--   0        0        0     1583 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/open_tick.mcfunction
+-rw-r--r--   0        0        0     1557 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/place.mcfunction
+-rw-r--r--   0        0        0       73 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/reset.mcfunction
+-rw-r--r--   0        0        0      393 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/tick.mcfunction
+-rw-r--r--   0        0        0      157 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/entity/player/slow_tick.mcfunction
+-rw-r--r--   0        0        0      574 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/recipes/shaped.mcfunction
+-rw-r--r--   0        0        0      104 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/technical/armor_stand.mcfunction
+-rw-r--r--   0        0        0      248 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/technical/load.mcfunction
+-rw-r--r--   0        0        0      148 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/technical/slow_tick.mcfunction
+-rw-r--r--   0        0        0      158 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/technical/tick.mcfunction
+-rw-r--r--   0        0        0       43 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/zint/technical/craft_table.mcfunction
+-rw-r--r--   0        0        0       57 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/zint/technical/enter_gui.mcfunction
+-rw-r--r--   0        0        0      559 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/loot_tables/blocks/table.json
+-rw-r--r--   0        0        0     3448 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/invalid_items.json
+-rw-r--r--   0        0        0     1110 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/special_clear/buckets.json
+-rw-r--r--   0        0        0     2198 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/special_clear/tools.json
+-rw-r--r--   0        0        0      218 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/acacia_logs.json
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/anvil.json
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/arrows.json
+-rw-r--r--   0        0        0      226 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/axolotl_tempt_items.json
+-rw-r--r--   0        0        0      214 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/banners.json
+-rw-r--r--   0        0        0      227 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/beacon_payment_items.json
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/beds.json
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/birch_logs.json
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/boats.json
+-rw-r--r--   0        0        0      214 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/buttons.json
+-rw-r--r--   0        0        0      214 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/candles.json
+-rw-r--r--   0        0        0      214 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/carpets.json
+-rw-r--r--   0        0        0      231 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/cluster_max_harvestables.json
+-rw-r--r--   0        0        0      216 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/coal_ores.json
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/coals.json
+-rw-r--r--   0        0        0      218 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/copper_ores.json
+-rw-r--r--   0        0        0      231 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/creeper_drop_music_discs.json
+-rw-r--r--   0        0        0      220 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/crimson_stems.json
+-rw-r--r--   0        0        0      220 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/dark_oak_logs.json
+-rw-r--r--   0        0        0      219 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/diamond_ores.json
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/doors.json
+-rw-r--r--   0        0        0      219 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/emerald_ores.json
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/fences.json
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/fishes.json
+-rw-r--r--   0        0        0      214 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/flowers.json
+-rw-r--r--   0        0        0      215 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/fox_food.json
+-rw-r--r--   0        0        0      230 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/freeze_immune_wearables.json
+-rw-r--r--   0        0        0      216 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/gold_ores.json
+-rw-r--r--   0        0        0      231 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/ignored_by_piglin_babies.json
+-rw-r--r--   0        0        0      216 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/iron_ores.json
+-rw-r--r--   0        0        0      218 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/jungle_logs.json
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/lapis_ores.json
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/leaves.json
+-rw-r--r--   0        0        0      220 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/lectern_books.json
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/logs.json
+-rw-r--r--   0        0        0      221 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/logs_that_burn.json
+-rw-r--r--   0        0        0      218 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/music_discs.json
+-rw-r--r--   0        0        0      225 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/non_flammable_wood.json
+-rw-r--r--   0        0        0      215 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/oak_logs.json
+-rw-r--r--   0        0        0      233 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/occludes_vibration_signals.json
+-rw-r--r--   0        0        0      218 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/piglin_food.json
+-rw-r--r--   0        0        0      219 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/piglin_loved.json
+-rw-r--r--   0        0        0      224 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/piglin_repellents.json
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/planks.json
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/rails.json
+-rw-r--r--   0        0        0      220 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/redstone_ores.json
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/sand.json
+-rw-r--r--   0        0        0      215 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/saplings.json
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/signs.json
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/slabs.json
+-rw-r--r--   0        0        0      220 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/small_flowers.json
+-rw-r--r--   0        0        0      228 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/soul_fire_base_blocks.json
+-rw-r--r--   0        0        0      218 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/spruce_logs.json
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/stairs.json
+-rw-r--r--   0        0        0      219 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/stone_bricks.json
+-rw-r--r--   0        0        0      231 2023-06-24 17:51:48.906154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/stone_crafting_materials.json
+-rw-r--r--   0        0        0      227 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/stone_tool_materials.json
+-rw-r--r--   0        0        0      219 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/tall_flowers.json
+-rw-r--r--   0        0        0      216 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/trapdoors.json
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/walls.json
+-rw-r--r--   0        0        0      219 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/warped_stems.json
+-rw-r--r--   0        0        0      221 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_buttons.json
+-rw-r--r--   0        0        0      219 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_doors.json
+-rw-r--r--   0        0        0      220 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_fences.json
+-rw-r--r--   0        0        0      229 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_pressure_plates.json
+-rw-r--r--   0        0        0      219 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_slabs.json
+-rw-r--r--   0        0        0      220 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_stairs.json
+-rw-r--r--   0        0        0      223 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wooden_trapdoors.json
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/tags/wool.json
+-rw-r--r--   0        0        0      422 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/recipes/table.json
+-rw-r--r--   0        0        0       33 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/tags/functions/event/advanced_remove.json
+-rw-r--r--   0        0        0       33 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/tags/functions/event/break.json
+-rw-r--r--   0        0        0       33 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/tags/functions/event/query_tags.json
+-rw-r--r--   0        0        0       66 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/tags/functions/event/recipes.json
+-rw-r--r--   0        0        0       33 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/tags/functions/event/shapeless_recipes.json
+-rw-r--r--   0        0        0    43577 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/tags/items/all.json
+-rw-r--r--   0        0        0       63 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.custom_block/tags/functions/event/on_place.json
+-rw-r--r--   0        0        0    88568 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/crafter/pack.png
+-rw-r--r--   0        0        0      311 2023-06-24 17:51:48.878157 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/beet.yaml
+-rw-r--r--   0        0        0       72 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter/tags/functions/event/query_tags.json
+-rw-r--r--   0        0        0       82 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter/tags/functions/event/recipes.json
+-rw-r--r--   0        0        0       85 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter/tags/functions/event/shapeless_recipes.json
+-rw-r--r--   0        0        0     1069 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_1.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_135.mcfunction
+-rw-r--r--   0        0        0      204 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_16.mcfunction
+-rw-r--r--   0        0        0      203 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_2.mcfunction
+-rw-r--r--   0        0        0      209 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_271.mcfunction
+-rw-r--r--   0        0        0      206 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_33.mcfunction
+-rw-r--r--   0        0        0      203 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_4.mcfunction
+-rw-r--r--   0        0        0      209 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_542.mcfunction
+-rw-r--r--   0        0        0      206 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_67.mcfunction
+-rw-r--r--   0        0        0      203 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_8.mcfunction
+-rw-r--r--   0        0        0      977 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/100_101.mcfunction
+-rw-r--r--   0        0        0     1092 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_103.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_104.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_106.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_110.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_118.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_135.mcfunction
+-rw-r--r--   0        0        0      557 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/104_104.mcfunction
+-rw-r--r--   0        0        0     1025 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/105_106.mcfunction
+-rw-r--r--   0        0        0      924 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/107_108.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/107_110.mcfunction
+-rw-r--r--   0        0        0      976 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/109_110.mcfunction
+-rw-r--r--   0        0        0     1099 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/111_112.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/111_114.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/111_118.mcfunction
+-rw-r--r--   0        0        0     1020 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/113_114.mcfunction
+-rw-r--r--   0        0        0      946 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/115_116.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/115_118.mcfunction
+-rw-r--r--   0        0        0      951 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/117_118.mcfunction
+-rw-r--r--   0        0        0      915 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_120.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_121.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_123.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_127.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_135.mcfunction
+-rw-r--r--   0        0        0      916 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/11_12.mcfunction
+-rw-r--r--   0        0        0      528 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/121_121.mcfunction
+-rw-r--r--   0        0        0      915 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/122_123.mcfunction
+-rw-r--r--   0        0        0     1085 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/124_125.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/124_127.mcfunction
+-rw-r--r--   0        0        0     1135 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/126_127.mcfunction
+-rw-r--r--   0        0        0     1086 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/128_129.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/128_131.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/128_135.mcfunction
+-rw-r--r--   0        0        0     1088 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/130_131.mcfunction
+-rw-r--r--   0        0        0      928 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/132_133.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/132_135.mcfunction
+-rw-r--r--   0        0        0      987 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/134_135.mcfunction
+-rw-r--r--   0        0        0     1113 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_137.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_138.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_140.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_144.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_152.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_169.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_203.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_271.mcfunction
+-rw-r--r--   0        0        0      507 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/138_138.mcfunction
+-rw-r--r--   0        0        0     1032 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/139_140.mcfunction
+-rw-r--r--   0        0        0     1025 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/13_14.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/13_16.mcfunction
+-rw-r--r--   0        0        0     1138 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/141_142.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/141_144.mcfunction
+-rw-r--r--   0        0        0      965 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/143_144.mcfunction
+-rw-r--r--   0        0        0     1135 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/145_146.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/145_148.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/145_152.mcfunction
+-rw-r--r--   0        0        0      952 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/147_148.mcfunction
+-rw-r--r--   0        0        0     1121 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/149_150.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/149_152.mcfunction
+-rw-r--r--   0        0        0     1062 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/151_152.mcfunction
+-rw-r--r--   0        0        0     1015 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_154.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_155.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_157.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_161.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_169.mcfunction
+-rw-r--r--   0        0        0      529 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/155_155.mcfunction
+-rw-r--r--   0        0        0      994 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/156_157.mcfunction
+-rw-r--r--   0        0        0     1033 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/158_159.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/158_161.mcfunction
+-rw-r--r--   0        0        0     1049 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/15_16.mcfunction
+-rw-r--r--   0        0        0     1003 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/160_161.mcfunction
+-rw-r--r--   0        0        0      883 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/162_163.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/162_165.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/162_169.mcfunction
+-rw-r--r--   0        0        0     1011 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/164_165.mcfunction
+-rw-r--r--   0        0        0     1107 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/166_167.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/166_169.mcfunction
+-rw-r--r--   0        0        0     1076 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/168_169.mcfunction
+-rw-r--r--   0        0        0     1052 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_171.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_172.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_174.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_178.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_186.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_203.mcfunction
+-rw-r--r--   0        0        0      536 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/172_172.mcfunction
+-rw-r--r--   0        0        0     1004 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/173_174.mcfunction
+-rw-r--r--   0        0        0      929 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/175_176.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/175_178.mcfunction
+-rw-r--r--   0        0        0     1135 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/177_178.mcfunction
+-rw-r--r--   0        0        0      960 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/179_180.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/179_182.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/179_186.mcfunction
+-rw-r--r--   0        0        0     1085 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_18.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_19.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_21.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_25.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_33.mcfunction
+-rw-r--r--   0        0        0     1096 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/181_182.mcfunction
+-rw-r--r--   0        0        0     1020 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/183_184.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/183_186.mcfunction
+-rw-r--r--   0        0        0     1209 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/185_186.mcfunction
+-rw-r--r--   0        0        0      957 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_188.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_189.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_191.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_195.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_203.mcfunction
+-rw-r--r--   0        0        0      573 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/189_189.mcfunction
+-rw-r--r--   0        0        0     1060 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/190_191.mcfunction
+-rw-r--r--   0        0        0     1012 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/192_193.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/192_195.mcfunction
+-rw-r--r--   0        0        0     1111 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/194_195.mcfunction
+-rw-r--r--   0        0        0     1013 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/196_197.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/196_199.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/196_203.mcfunction
+-rw-r--r--   0        0        0     1061 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/198_199.mcfunction
+-rw-r--r--   0        0        0      518 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/19_19.mcfunction
+-rw-r--r--   0        0        0     1010 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/200_201.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/200_203.mcfunction
+-rw-r--r--   0        0        0     1113 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/202_203.mcfunction
+-rw-r--r--   0        0        0      913 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_205.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_206.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_208.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_212.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_220.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_237.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_271.mcfunction
+-rw-r--r--   0        0        0      494 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/206_206.mcfunction
+-rw-r--r--   0        0        0     1048 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/207_208.mcfunction
+-rw-r--r--   0        0        0      962 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/209_210.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/209_212.mcfunction
+-rw-r--r--   0        0        0     1089 2023-06-24 17:51:48.882156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/20_21.mcfunction
+-rw-r--r--   0        0        0     1090 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/211_212.mcfunction
+-rw-r--r--   0        0        0     1118 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/213_214.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/213_216.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/213_220.mcfunction
+-rw-r--r--   0        0        0     1059 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/215_216.mcfunction
+-rw-r--r--   0        0        0      967 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/217_218.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/217_220.mcfunction
+-rw-r--r--   0        0        0     1099 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/219_220.mcfunction
+-rw-r--r--   0        0        0     1122 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_222.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_223.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_225.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_229.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_237.mcfunction
+-rw-r--r--   0        0        0      503 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/223_223.mcfunction
+-rw-r--r--   0        0        0      921 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/224_225.mcfunction
+-rw-r--r--   0        0        0     1002 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/226_227.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/226_229.mcfunction
+-rw-r--r--   0        0        0     1003 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/228_229.mcfunction
+-rw-r--r--   0        0        0     1052 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/22_23.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/22_25.mcfunction
+-rw-r--r--   0        0        0     1022 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/230_231.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/230_233.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/230_237.mcfunction
+-rw-r--r--   0        0        0     1048 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/232_233.mcfunction
+-rw-r--r--   0        0        0     1080 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/234_235.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/234_237.mcfunction
+-rw-r--r--   0        0        0     1009 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/236_237.mcfunction
+-rw-r--r--   0        0        0     1102 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_239.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_240.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_242.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_246.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_254.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_271.mcfunction
+-rw-r--r--   0        0        0      516 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/240_240.mcfunction
+-rw-r--r--   0        0        0     1006 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/241_242.mcfunction
+-rw-r--r--   0        0        0     1008 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/243_244.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/243_246.mcfunction
+-rw-r--r--   0        0        0     1071 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/245_246.mcfunction
+-rw-r--r--   0        0        0     1069 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/247_248.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/247_250.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/247_254.mcfunction
+-rw-r--r--   0        0        0     1017 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/249_250.mcfunction
+-rw-r--r--   0        0        0      910 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/24_25.mcfunction
+-rw-r--r--   0        0        0      965 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/251_252.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/251_254.mcfunction
+-rw-r--r--   0        0        0      965 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/253_254.mcfunction
+-rw-r--r--   0        0        0     1030 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_256.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_257.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_259.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_263.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_271.mcfunction
+-rw-r--r--   0        0        0      499 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/257_257.mcfunction
+-rw-r--r--   0        0        0     1123 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/258_259.mcfunction
+-rw-r--r--   0        0        0      999 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/260_261.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/260_263.mcfunction
+-rw-r--r--   0        0        0     1016 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/262_263.mcfunction
+-rw-r--r--   0        0        0     1018 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/264_265.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/264_267.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/264_271.mcfunction
+-rw-r--r--   0        0        0     1087 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/266_267.mcfunction
+-rw-r--r--   0        0        0      992 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/268_269.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/268_271.mcfunction
+-rw-r--r--   0        0        0      954 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/26_27.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/26_29.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/26_33.mcfunction
+-rw-r--r--   0        0        0     1114 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/270_271.mcfunction
+-rw-r--r--   0        0        0      992 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_273.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_274.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_276.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_280.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_288.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_305.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_339.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_407.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_542.mcfunction
+-rw-r--r--   0        0        0      530 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/274_274.mcfunction
+-rw-r--r--   0        0        0     1189 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/275_276.mcfunction
+-rw-r--r--   0        0        0     1137 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/277_278.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/277_280.mcfunction
+-rw-r--r--   0        0        0      957 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/279_280.mcfunction
+-rw-r--r--   0        0        0     1109 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/281_282.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/281_284.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/281_288.mcfunction
+-rw-r--r--   0        0        0     1189 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/283_284.mcfunction
+-rw-r--r--   0        0        0      982 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/285_286.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/285_288.mcfunction
+-rw-r--r--   0        0        0     1048 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/287_288.mcfunction
+-rw-r--r--   0        0        0      962 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_290.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_291.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_293.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_297.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_305.mcfunction
+-rw-r--r--   0        0        0     1071 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/28_29.mcfunction
+-rw-r--r--   0        0        0      518 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/291_291.mcfunction
+-rw-r--r--   0        0        0     1135 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/292_293.mcfunction
+-rw-r--r--   0        0        0     1199 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/294_295.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/294_297.mcfunction
+-rw-r--r--   0        0        0     1041 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/296_297.mcfunction
+-rw-r--r--   0        0        0      936 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/298_299.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/298_301.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/298_305.mcfunction
+-rw-r--r--   0        0        0      514 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/2_2.mcfunction
+-rw-r--r--   0        0        0     1097 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/300_301.mcfunction
+-rw-r--r--   0        0        0     1162 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/302_303.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/302_305.mcfunction
+-rw-r--r--   0        0        0     1062 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/304_305.mcfunction
+-rw-r--r--   0        0        0     1058 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_307.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_308.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_310.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_314.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_322.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_339.mcfunction
+-rw-r--r--   0        0        0      501 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/308_308.mcfunction
+-rw-r--r--   0        0        0     1023 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/309_310.mcfunction
+-rw-r--r--   0        0        0      900 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/30_31.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/30_33.mcfunction
+-rw-r--r--   0        0        0     1003 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/311_312.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/311_314.mcfunction
+-rw-r--r--   0        0        0     1163 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/313_314.mcfunction
+-rw-r--r--   0        0        0      999 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/315_316.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/315_318.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/315_322.mcfunction
+-rw-r--r--   0        0        0     1041 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/317_318.mcfunction
+-rw-r--r--   0        0        0      977 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/319_320.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/319_322.mcfunction
+-rw-r--r--   0        0        0     1103 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/321_322.mcfunction
+-rw-r--r--   0        0        0     1091 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_324.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_325.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_327.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_331.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_339.mcfunction
+-rw-r--r--   0        0        0      529 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/325_325.mcfunction
+-rw-r--r--   0        0        0      993 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/326_327.mcfunction
+-rw-r--r--   0        0        0      935 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/328_329.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/328_331.mcfunction
+-rw-r--r--   0        0        0     1053 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/32_33.mcfunction
+-rw-r--r--   0        0        0      932 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/330_331.mcfunction
+-rw-r--r--   0        0        0      994 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/332_333.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/332_335.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/332_339.mcfunction
+-rw-r--r--   0        0        0     1090 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/334_335.mcfunction
+-rw-r--r--   0        0        0      929 2023-06-24 17:51:48.886156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/336_337.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/336_339.mcfunction
+-rw-r--r--   0        0        0     1093 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/338_339.mcfunction
+-rw-r--r--   0        0        0     1153 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_341.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_342.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_344.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_348.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_356.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_373.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_407.mcfunction
+-rw-r--r--   0        0        0      559 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/342_342.mcfunction
+-rw-r--r--   0        0        0      969 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/343_344.mcfunction
+-rw-r--r--   0        0        0     1114 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/345_346.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/345_348.mcfunction
+-rw-r--r--   0        0        0      926 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/347_348.mcfunction
+-rw-r--r--   0        0        0      915 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/349_350.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/349_352.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/349_356.mcfunction
+-rw-r--r--   0        0        0     1059 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_35.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_36.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_38.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_42.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_50.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_67.mcfunction
+-rw-r--r--   0        0        0     1085 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/351_352.mcfunction
+-rw-r--r--   0        0        0     1135 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/353_354.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/353_356.mcfunction
+-rw-r--r--   0        0        0     1120 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/355_356.mcfunction
+-rw-r--r--   0        0        0      931 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_358.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_359.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_361.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_365.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_373.mcfunction
+-rw-r--r--   0        0        0      587 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/359_359.mcfunction
+-rw-r--r--   0        0        0      990 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/360_361.mcfunction
+-rw-r--r--   0        0        0     1019 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/362_363.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/362_365.mcfunction
+-rw-r--r--   0        0        0     1275 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/364_365.mcfunction
+-rw-r--r--   0        0        0      882 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/366_367.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/366_369.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/366_373.mcfunction
+-rw-r--r--   0        0        0     1179 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/368_369.mcfunction
+-rw-r--r--   0        0        0      398 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/36_36.mcfunction
+-rw-r--r--   0        0        0      972 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/370_371.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/370_373.mcfunction
+-rw-r--r--   0        0        0     1165 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/372_373.mcfunction
+-rw-r--r--   0        0        0      922 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_375.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_376.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_378.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_382.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_390.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_407.mcfunction
+-rw-r--r--   0        0        0      580 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/376_376.mcfunction
+-rw-r--r--   0        0        0      922 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/377_378.mcfunction
+-rw-r--r--   0        0        0     1120 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/379_380.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/379_382.mcfunction
+-rw-r--r--   0        0        0     1089 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/37_38.mcfunction
+-rw-r--r--   0        0        0     1133 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/381_382.mcfunction
+-rw-r--r--   0        0        0     1021 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/383_384.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/383_386.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/383_390.mcfunction
+-rw-r--r--   0        0        0      946 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/385_386.mcfunction
+-rw-r--r--   0        0        0     1057 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/387_388.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/387_390.mcfunction
+-rw-r--r--   0        0        0      929 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/389_390.mcfunction
+-rw-r--r--   0        0        0     1093 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_392.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_393.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_395.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_399.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_407.mcfunction
+-rw-r--r--   0        0        0      586 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/393_393.mcfunction
+-rw-r--r--   0        0        0     1126 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/394_395.mcfunction
+-rw-r--r--   0        0        0     1021 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/396_397.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/396_399.mcfunction
+-rw-r--r--   0        0        0     1064 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/398_399.mcfunction
+-rw-r--r--   0        0        0     1144 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/39_40.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/39_42.mcfunction
+-rw-r--r--   0        0        0      916 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/3_4.mcfunction
+-rw-r--r--   0        0        0      989 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/400_401.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/400_403.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/400_407.mcfunction
+-rw-r--r--   0        0        0      935 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/402_403.mcfunction
+-rw-r--r--   0        0        0     1146 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/404_405.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/404_407.mcfunction
+-rw-r--r--   0        0        0     1096 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/406_407.mcfunction
+-rw-r--r--   0        0        0     1076 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_409.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_410.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_412.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_416.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_424.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_441.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_475.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_542.mcfunction
+-rw-r--r--   0        0        0      518 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/410_410.mcfunction
+-rw-r--r--   0        0        0     1000 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/411_412.mcfunction
+-rw-r--r--   0        0        0      908 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/413_414.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/413_416.mcfunction
+-rw-r--r--   0        0        0     1074 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/415_416.mcfunction
+-rw-r--r--   0        0        0     1021 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/417_418.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/417_420.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/417_424.mcfunction
+-rw-r--r--   0        0        0     1054 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/419_420.mcfunction
+-rw-r--r--   0        0        0     1115 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/41_42.mcfunction
+-rw-r--r--   0        0        0     1090 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/421_422.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/421_424.mcfunction
+-rw-r--r--   0        0        0     1052 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/423_424.mcfunction
+-rw-r--r--   0        0        0     1126 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_426.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_427.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_429.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_433.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_441.mcfunction
+-rw-r--r--   0        0        0      553 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/427_427.mcfunction
+-rw-r--r--   0        0        0     1082 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/428_429.mcfunction
+-rw-r--r--   0        0        0      896 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/430_431.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/430_433.mcfunction
+-rw-r--r--   0        0        0     1129 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/432_433.mcfunction
+-rw-r--r--   0        0        0     1133 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/434_435.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/434_437.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/434_441.mcfunction
+-rw-r--r--   0        0        0     1042 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/436_437.mcfunction
+-rw-r--r--   0        0        0     1065 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/438_439.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/438_441.mcfunction
+-rw-r--r--   0        0        0     1048 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/43_44.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/43_46.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/43_50.mcfunction
+-rw-r--r--   0        0        0     1084 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/440_441.mcfunction
+-rw-r--r--   0        0        0      979 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_443.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_444.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_446.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_450.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_458.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_475.mcfunction
+-rw-r--r--   0        0        0      448 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/444_444.mcfunction
+-rw-r--r--   0        0        0     1040 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/445_446.mcfunction
+-rw-r--r--   0        0        0      996 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/447_448.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/447_450.mcfunction
+-rw-r--r--   0        0        0      885 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/449_450.mcfunction
+-rw-r--r--   0        0        0     1117 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/451_452.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/451_454.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/451_458.mcfunction
+-rw-r--r--   0        0        0     1074 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/453_454.mcfunction
+-rw-r--r--   0        0        0     1069 2023-06-24 17:51:48.890156 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/455_456.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/455_458.mcfunction
+-rw-r--r--   0        0        0     1017 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/457_458.mcfunction
+-rw-r--r--   0        0        0      965 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_460.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_461.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_463.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_467.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_475.mcfunction
+-rw-r--r--   0        0        0      962 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/45_46.mcfunction
+-rw-r--r--   0        0        0      413 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/461_461.mcfunction
+-rw-r--r--   0        0        0     1085 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/462_463.mcfunction
+-rw-r--r--   0        0        0     1013 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/464_465.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/464_467.mcfunction
+-rw-r--r--   0        0        0      968 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/466_467.mcfunction
+-rw-r--r--   0        0        0      951 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/468_469.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/468_471.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/468_475.mcfunction
+-rw-r--r--   0        0        0     1048 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/470_471.mcfunction
+-rw-r--r--   0        0        0      966 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/472_473.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/472_475.mcfunction
+-rw-r--r--   0        0        0     1072 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/474_475.mcfunction
+-rw-r--r--   0        0        0      970 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_477.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_478.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_480.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_484.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_492.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_509.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_542.mcfunction
+-rw-r--r--   0        0        0      521 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/478_478.mcfunction
+-rw-r--r--   0        0        0      891 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/479_480.mcfunction
+-rw-r--r--   0        0        0     1068 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/47_48.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/47_50.mcfunction
+-rw-r--r--   0        0        0     1086 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/481_482.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/481_484.mcfunction
+-rw-r--r--   0        0        0     1090 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/483_484.mcfunction
+-rw-r--r--   0        0        0     1094 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/485_486.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/485_488.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/485_492.mcfunction
+-rw-r--r--   0        0        0     1069 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/487_488.mcfunction
+-rw-r--r--   0        0        0     1059 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/489_490.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/489_492.mcfunction
+-rw-r--r--   0        0        0     1133 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/491_492.mcfunction
+-rw-r--r--   0        0        0      957 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_494.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_495.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_497.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_501.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_509.mcfunction
+-rw-r--r--   0        0        0      513 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/495_495.mcfunction
+-rw-r--r--   0        0        0     1031 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/496_497.mcfunction
+-rw-r--r--   0        0        0     1017 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/498_499.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/498_501.mcfunction
+-rw-r--r--   0        0        0     1135 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/49_50.mcfunction
+-rw-r--r--   0        0        0     1003 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/500_501.mcfunction
+-rw-r--r--   0        0        0      965 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/502_503.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/502_505.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/502_509.mcfunction
+-rw-r--r--   0        0        0      965 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/504_505.mcfunction
+-rw-r--r--   0        0        0     1067 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/506_507.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/506_509.mcfunction
+-rw-r--r--   0        0        0     1012 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/508_509.mcfunction
+-rw-r--r--   0        0        0     1014 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_511.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_512.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_514.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_518.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_526.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_542.mcfunction
+-rw-r--r--   0        0        0      636 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/512_512.mcfunction
+-rw-r--r--   0        0        0     1023 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/513_514.mcfunction
+-rw-r--r--   0        0        0     1203 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/515_516.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/515_518.mcfunction
+-rw-r--r--   0        0        0     1122 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/517_518.mcfunction
+-rw-r--r--   0        0        0      978 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/519_520.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/519_522.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/519_526.mcfunction
+-rw-r--r--   0        0        0     1098 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_52.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_53.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_55.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_59.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_67.mcfunction
+-rw-r--r--   0        0        0     1143 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/521_522.mcfunction
+-rw-r--r--   0        0        0      922 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/523_524.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/523_526.mcfunction
+-rw-r--r--   0        0        0     1099 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/525_526.mcfunction
+-rw-r--r--   0        0        0     1122 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/527_528.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/527_530.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/527_534.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/527_542.mcfunction
+-rw-r--r--   0        0        0     1009 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/529_530.mcfunction
+-rw-r--r--   0        0        0     1050 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/531_532.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/531_534.mcfunction
+-rw-r--r--   0        0        0     1025 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/533_534.mcfunction
+-rw-r--r--   0        0        0     1070 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/535_536.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/535_538.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/535_542.mcfunction
+-rw-r--r--   0        0        0      972 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/537_538.mcfunction
+-rw-r--r--   0        0        0     1108 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/539_540.mcfunction
+-rw-r--r--   0        0        0      211 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/539_542.mcfunction
+-rw-r--r--   0        0        0      563 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/53_53.mcfunction
+-rw-r--r--   0        0        0     1126 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/541_542.mcfunction
+-rw-r--r--   0        0        0      995 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/54_55.mcfunction
+-rw-r--r--   0        0        0      950 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/56_57.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/56_59.mcfunction
+-rw-r--r--   0        0        0      863 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/58_59.mcfunction
+-rw-r--r--   0        0        0      965 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/5_6.mcfunction
+-rw-r--r--   0        0        0      203 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/5_8.mcfunction
+-rw-r--r--   0        0        0      995 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/60_61.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/60_63.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/60_67.mcfunction
+-rw-r--r--   0        0        0     1059 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/62_63.mcfunction
+-rw-r--r--   0        0        0      967 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/64_65.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/64_67.mcfunction
+-rw-r--r--   0        0        0     1099 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/66_67.mcfunction
+-rw-r--r--   0        0        0      208 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_101.mcfunction
+-rw-r--r--   0        0        0      210 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_135.mcfunction
+-rw-r--r--   0        0        0     1122 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_69.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_70.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_72.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_76.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_84.mcfunction
+-rw-r--r--   0        0        0      485 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/70_70.mcfunction
+-rw-r--r--   0        0        0     1051 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/71_72.mcfunction
+-rw-r--r--   0        0        0      959 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/73_74.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/73_76.mcfunction
+-rw-r--r--   0        0        0     1084 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/75_76.mcfunction
+-rw-r--r--   0        0        0     1087 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/77_78.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/77_80.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/77_84.mcfunction
+-rw-r--r--   0        0        0      993 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/79_80.mcfunction
+-rw-r--r--   0        0        0     1085 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/7_8.mcfunction
+-rw-r--r--   0        0        0     1036 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/81_82.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/81_84.mcfunction
+-rw-r--r--   0        0        0     1005 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/83_84.mcfunction
+-rw-r--r--   0        0        0      208 2023-06-24 17:51:48.894155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_101.mcfunction
+-rw-r--r--   0        0        0     1003 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_86.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_87.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_89.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_93.mcfunction
+-rw-r--r--   0        0        0      486 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/87_87.mcfunction
+-rw-r--r--   0        0        0     1015 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/88_89.mcfunction
+-rw-r--r--   0        0        0      913 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/90_91.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/90_93.mcfunction
+-rw-r--r--   0        0        0     1151 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/92_93.mcfunction
+-rw-r--r--   0        0        0      208 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/94_101.mcfunction
+-rw-r--r--   0        0        0      957 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/94_95.mcfunction
+-rw-r--r--   0        0        0      207 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/94_97.mcfunction
+-rw-r--r--   0        0        0     1053 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/96_97.mcfunction
+-rw-r--r--   0        0        0      209 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/98_101.mcfunction
+-rw-r--r--   0        0        0     1133 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/98_99.mcfunction
+-rw-r--r--   0        0        0     1047 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/9_10.mcfunction
+-rw-r--r--   0        0        0      206 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/9_12.mcfunction
+-rw-r--r--   0        0        0      206 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/9_16.mcfunction
+-rw-r--r--   0        0        0      603 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_1.mcfunction
+-rw-r--r--   0        0        0      210 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_11.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_182.mcfunction
+-rw-r--r--   0        0        0      209 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_2.mcfunction
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_22.mcfunction
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_45.mcfunction
+-rw-r--r--   0        0        0      209 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_5.mcfunction
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_91.mcfunction
+-rw-r--r--   0        0        0      328 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/100_100.mcfunction
+-rw-r--r--   0        0        0      652 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/101_102.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/101_103.mcfunction
+-rw-r--r--   0        0        0      324 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/103_103.mcfunction
+-rw-r--r--   0        0        0      699 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/104_105.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/104_106.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/104_109.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/104_114.mcfunction
+-rw-r--r--   0        0        0      302 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/106_106.mcfunction
+-rw-r--r--   0        0        0      591 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/107_108.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/107_109.mcfunction
+-rw-r--r--   0        0        0      319 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/109_109.mcfunction
+-rw-r--r--   0        0        0      687 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/110_111.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/110_112.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/110_114.mcfunction
+-rw-r--r--   0        0        0      294 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/112_112.mcfunction
+-rw-r--r--   0        0        0      638 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/113_114.mcfunction
+-rw-r--r--   0        0        0      609 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_116.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_117.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_120.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_126.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_137.mcfunction
+-rw-r--r--   0        0        0      315 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/117_117.mcfunction
+-rw-r--r--   0        0        0      649 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/118_119.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/118_120.mcfunction
+-rw-r--r--   0        0        0      319 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/11_11.mcfunction
+-rw-r--r--   0        0        0      290 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/120_120.mcfunction
+-rw-r--r--   0        0        0      631 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/121_122.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/121_123.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/121_126.mcfunction
+-rw-r--r--   0        0        0      317 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/123_123.mcfunction
+-rw-r--r--   0        0        0      626 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/124_125.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/124_126.mcfunction
+-rw-r--r--   0        0        0      319 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/126_126.mcfunction
+-rw-r--r--   0        0        0      687 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/127_128.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/127_129.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/127_132.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/127_137.mcfunction
+-rw-r--r--   0        0        0      315 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/129_129.mcfunction
+-rw-r--r--   0        0        0      608 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/12_13.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/12_14.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/12_17.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/12_22.mcfunction
+-rw-r--r--   0        0        0      725 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/130_131.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/130_132.mcfunction
+-rw-r--r--   0        0        0      402 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/132_132.mcfunction
+-rw-r--r--   0        0        0      592 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/133_134.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/133_135.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/133_137.mcfunction
+-rw-r--r--   0        0        0      294 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/135_135.mcfunction
+-rw-r--r--   0        0        0      607 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/136_137.mcfunction
+-rw-r--r--   0        0        0      675 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_139.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_140.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_143.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_149.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_160.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_182.mcfunction
+-rw-r--r--   0        0        0      287 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/140_140.mcfunction
+-rw-r--r--   0        0        0      572 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/141_142.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/141_143.mcfunction
+-rw-r--r--   0        0        0      288 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/143_143.mcfunction
+-rw-r--r--   0        0        0      651 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/144_145.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/144_146.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/144_149.mcfunction
+-rw-r--r--   0        0        0      293 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/146_146.mcfunction
+-rw-r--r--   0        0        0      603 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/147_148.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/147_149.mcfunction
+-rw-r--r--   0        0        0      289 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/149_149.mcfunction
+-rw-r--r--   0        0        0      315 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/14_14.mcfunction
+-rw-r--r--   0        0        0      576 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/150_151.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/150_152.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/150_155.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/150_160.mcfunction
+-rw-r--r--   0        0        0      321 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/152_152.mcfunction
+-rw-r--r--   0        0        0      604 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/153_154.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/153_155.mcfunction
+-rw-r--r--   0        0        0      329 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/155_155.mcfunction
+-rw-r--r--   0        0        0      660 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/156_157.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/156_158.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/156_160.mcfunction
+-rw-r--r--   0        0        0      339 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/158_158.mcfunction
+-rw-r--r--   0        0        0      674 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/159_160.mcfunction
+-rw-r--r--   0        0        0      656 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/15_16.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/15_17.mcfunction
+-rw-r--r--   0        0        0      706 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_162.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_163.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_166.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_171.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_182.mcfunction
+-rw-r--r--   0        0        0      335 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/163_163.mcfunction
+-rw-r--r--   0        0        0      696 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/164_165.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/164_166.mcfunction
+-rw-r--r--   0        0        0      357 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/166_166.mcfunction
+-rw-r--r--   0        0        0      682 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/167_168.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/167_169.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/167_171.mcfunction
+-rw-r--r--   0        0        0      355 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/169_169.mcfunction
+-rw-r--r--   0        0        0      645 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/170_171.mcfunction
+-rw-r--r--   0        0        0      683 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/172_173.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/172_174.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/172_177.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/172_182.mcfunction
+-rw-r--r--   0        0        0      290 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/174_174.mcfunction
+-rw-r--r--   0        0        0      638 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/175_176.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/175_177.mcfunction
+-rw-r--r--   0        0        0      319 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/177_177.mcfunction
+-rw-r--r--   0        0        0      687 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/178_179.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/178_180.mcfunction
+-rw-r--r--   0        0        0      217 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/178_182.mcfunction
+-rw-r--r--   0        0        0      290 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/17_17.mcfunction
+-rw-r--r--   0        0        0      291 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/180_180.mcfunction
+-rw-r--r--   0        0        0      612 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/181_182.mcfunction
+-rw-r--r--   0        0        0      602 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/18_19.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/18_20.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/18_22.mcfunction
+-rw-r--r--   0        0        0      291 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/20_20.mcfunction
+-rw-r--r--   0        0        0      632 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/21_22.mcfunction
+-rw-r--r--   0        0        0      683 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_24.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_25.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_28.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_34.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_45.mcfunction
+-rw-r--r--   0        0        0      292 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/25_25.mcfunction
+-rw-r--r--   0        0        0      605 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/26_27.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/26_28.mcfunction
+-rw-r--r--   0        0        0      296 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/28_28.mcfunction
+-rw-r--r--   0        0        0      631 2023-06-24 17:51:48.898155 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/29_30.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/29_31.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/29_34.mcfunction
+-rw-r--r--   0        0        0      316 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/2_2.mcfunction
+-rw-r--r--   0        0        0      300 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/31_31.mcfunction
+-rw-r--r--   0        0        0      623 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/32_33.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/32_34.mcfunction
+-rw-r--r--   0        0        0      315 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/34_34.mcfunction
+-rw-r--r--   0        0        0      679 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/35_36.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/35_37.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/35_40.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/35_45.mcfunction
+-rw-r--r--   0        0        0      317 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/37_37.mcfunction
+-rw-r--r--   0        0        0      611 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/38_39.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/38_40.mcfunction
+-rw-r--r--   0        0        0      620 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/3_4.mcfunction
+-rw-r--r--   0        0        0      209 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/3_5.mcfunction
+-rw-r--r--   0        0        0      292 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/40_40.mcfunction
+-rw-r--r--   0        0        0      590 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/41_42.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/41_43.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/41_45.mcfunction
+-rw-r--r--   0        0        0      322 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/43_43.mcfunction
+-rw-r--r--   0        0        0      676 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/44_45.mcfunction
+-rw-r--r--   0        0        0      680 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_47.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_48.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_51.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_57.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_68.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_91.mcfunction
+-rw-r--r--   0        0        0      327 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/48_48.mcfunction
+-rw-r--r--   0        0        0      619 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/49_50.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/49_51.mcfunction
+-rw-r--r--   0        0        0      293 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/51_51.mcfunction
+-rw-r--r--   0        0        0      625 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/52_53.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/52_54.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/52_57.mcfunction
+-rw-r--r--   0        0        0      315 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/54_54.mcfunction
+-rw-r--r--   0        0        0      680 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/55_56.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/55_57.mcfunction
+-rw-r--r--   0        0        0      317 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/57_57.mcfunction
+-rw-r--r--   0        0        0      634 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/58_59.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/58_60.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/58_63.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/58_68.mcfunction
+-rw-r--r--   0        0        0      303 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/5_5.mcfunction
+-rw-r--r--   0        0        0      486 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/60_60.mcfunction
+-rw-r--r--   0        0        0      653 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/61_62.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/61_63.mcfunction
+-rw-r--r--   0        0        0      292 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/63_63.mcfunction
+-rw-r--r--   0        0        0      591 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/64_65.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/64_66.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/64_68.mcfunction
+-rw-r--r--   0        0        0      305 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/66_66.mcfunction
+-rw-r--r--   0        0        0      622 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/67_68.mcfunction
+-rw-r--r--   0        0        0      703 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_70.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_71.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_74.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_80.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_91.mcfunction
+-rw-r--r--   0        0        0      210 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/6_11.mcfunction
+-rw-r--r--   0        0        0      634 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/6_7.mcfunction
+-rw-r--r--   0        0        0      209 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/6_8.mcfunction
+-rw-r--r--   0        0        0      297 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/71_71.mcfunction
+-rw-r--r--   0        0        0      650 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/72_73.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/72_74.mcfunction
+-rw-r--r--   0        0        0      327 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/74_74.mcfunction
+-rw-r--r--   0        0        0      703 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/75_76.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/75_77.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/75_80.mcfunction
+-rw-r--r--   0        0        0      297 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/77_77.mcfunction
+-rw-r--r--   0        0        0      652 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/78_79.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/78_80.mcfunction
+-rw-r--r--   0        0        0      297 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/80_80.mcfunction
+-rw-r--r--   0        0        0      626 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/81_82.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/81_83.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/81_86.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/81_91.mcfunction
+-rw-r--r--   0        0        0      315 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/83_83.mcfunction
+-rw-r--r--   0        0        0      679 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/84_85.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/84_86.mcfunction
+-rw-r--r--   0        0        0      316 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/86_86.mcfunction
+-rw-r--r--   0        0        0      638 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/87_88.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/87_89.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/87_91.mcfunction
+-rw-r--r--   0        0        0      321 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/89_89.mcfunction
+-rw-r--r--   0        0        0      375 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/8_8.mcfunction
+-rw-r--r--   0        0        0      659 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/90_91.mcfunction
+-rw-r--r--   0        0        0      214 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_103.mcfunction
+-rw-r--r--   0        0        0      216 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_114.mcfunction
+-rw-r--r--   0        0        0      216 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_137.mcfunction
+-rw-r--r--   0        0        0      216 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_182.mcfunction
+-rw-r--r--   0        0        0      694 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_93.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_94.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_97.mcfunction
+-rw-r--r--   0        0        0      288 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/94_94.mcfunction
+-rw-r--r--   0        0        0      642 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/95_96.mcfunction
+-rw-r--r--   0        0        0      213 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/95_97.mcfunction
+-rw-r--r--   0        0        0      323 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/97_97.mcfunction
+-rw-r--r--   0        0        0      215 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/98_100.mcfunction
+-rw-r--r--   0        0        0      216 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/98_103.mcfunction
+-rw-r--r--   0        0        0      632 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/98_99.mcfunction
+-rw-r--r--   0        0        0      580 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/9_10.mcfunction
+-rw-r--r--   0        0        0      212 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/9_11.mcfunction
+-rw-r--r--   0        0        0     1376 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/tags/query.mcfunction
+-rw-r--r--   0        0        0      260 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/coal_charcoal.json
+-rw-r--r--   0        0        0      273 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/purpur_decoration.json
+-rw-r--r--   0        0        0      320 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/quartz_decoration.json
+-rw-r--r--   0        0        0      283 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/red_sandstone.json
+-rw-r--r--   0        0        0      326 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/red_sandstone_and_cut.json
+-rw-r--r--   0        0        0      260 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/sand_and_red_sand.json
+-rw-r--r--   0        0        0      275 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/sandstone.json
+-rw-r--r--   0        0        0      314 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/predicates/recipes/sandstone_and_cut.json
+-rw-r--r--   0        0        0    80541 2023-06-24 17:51:48.902154 smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/pack.png
+-rw-r--r--   0        0        0      509 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/README.md
+-rw-r--r--   0        0        0      319 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/beet.yaml
+-rw-r--r--   0        0        0      543 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/advancements/impl/technical/place_custom_block.json
+-rw-r--r--   0        0        0      240 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place/block_unchanged.mcfunction
+-rw-r--r--   0        0        0      357 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place/found.mcfunction
+-rw-r--r--   0        0        0    27546 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place/layer.mcfunction
+-rw-r--r--   0        0        0      205 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place/throw_warning.mcfunction
+-rw-r--r--   0        0        0     1420 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place.mcfunction
+-rw-r--r--   0        0        0     1280 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/technical/def_const.mcfunction
+-rw-r--r--   0        0        0     1065 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/technical/load.mcfunction
+-rw-r--r--   0        0        0      264 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/technical/tick.mcfunction
+-rw-r--r--   0        0        0      269 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/tags/blocks/placeable.json
+-rw-r--r--   0        0        0    88530 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/pack.png
+-rw-r--r--   0        0        0      509 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/README.md
+-rw-r--r--   0        0        0      232 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/beet.yaml
+-rw-r--r--   0        0        0     1636 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/advancements/impl/player/event.json
+-rw-r--r--   0        0        0     2050 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/armor.mcfunction
+-rw-r--r--   0        0        0     2163 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/explosion.mcfunction
+-rw-r--r--   0        0        0     2161 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/projectile.mcfunction
+-rw-r--r--   0        0        0     1304 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply.mcfunction
+-rw-r--r--   0        0        0     1744 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/blast_protection.mcfunction
+-rw-r--r--   0        0        0     1764 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/proj_protection.mcfunction
+-rw-r--r--   0        0        0     2062 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/protection.mcfunction
+-rw-r--r--   0        0        0     1393 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/resistance.mcfunction
+-rw-r--r--   0        0        0     3290 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/toughness.mcfunction
+-rw-r--r--   0        0        0      142 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/1.mcfunction
+-rw-r--r--   0        0        0      148 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/1024.mcfunction
+-rw-r--r--   0        0        0      146 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/128.mcfunction
+-rw-r--r--   0        0        0      144 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/16.mcfunction
+-rw-r--r--   0        0        0      142 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/2.mcfunction
+-rw-r--r--   0        0        0      146 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/256.mcfunction
+-rw-r--r--   0        0        0      144 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/32.mcfunction
+-rw-r--r--   0        0        0      142 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/4.mcfunction
+-rw-r--r--   0        0        0      146 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/512.mcfunction
+-rw-r--r--   0        0        0      144 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/64.mcfunction
+-rw-r--r--   0        0        0      142 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/8.mcfunction
+-rw-r--r--   0        0        0     1166 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/give.mcfunction
+-rw-r--r--   0        0        0      979 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/remove.mcfunction
+-rw-r--r--   0        0        0      107 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/schedule.mcfunction
+-rw-r--r--   0        0        0     1358 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/death_message.mcfunction
+-rw-r--r--   0        0        0      344 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/calculate_modifier.mcfunction
+-rw-r--r--   0        0        0       87 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/get_entity_health.mcfunction
+-rw-r--r--   0        0        0      191 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/update.mcfunction
+-rw-r--r--   0        0        0      743 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/update_entity.mcfunction
+-rw-r--r--   0        0        0      160 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/update_player.mcfunction
+-rw-r--r--   0        0        0     1471 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/on_death.mcfunction
+-rw-r--r--   0        0        0     2469 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/player/event.mcfunction
+-rw-r--r--   0        0        0     1321 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/technical/def_const.mcfunction
+-rw-r--r--   0        0        0      143 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/technical/load.mcfunction
+-rw-r--r--   0        0        0      425 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/tags/entity_types/undead.json
+-rw-r--r--   0        0        0       21 2023-06-24 17:51:48.910153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/tags/functions/event/entity/on_death.json
+-rw-r--r--   0        0        0       20 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/tags/functions/event/player/on_damage.json
+-rw-r--r--   0        0        0       20 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/tags/functions/event/player/on_death_message.json
+-rw-r--r--   0        0        0    88530 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/damage/pack.png
+-rw-r--r--   0        0        0      363 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/assets/smithed.enchanter/font/gui.json
+-rw-r--r--   0        0        0      102 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/assets/smithed.enchanter/lang/en_us.json
+-rw-r--r--   0        0        0      444 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/assets/smithed.enchanter/textures/gui/table.png
+-rw-r--r--   0        0        0      410 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/beet.yaml
+-rw-r--r--   0        0        0      299 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/advancements/impl/test.json
+-rw-r--r--   0        0        0     1348 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_bookshelves.mcfunction
+-rw-r--r--   0        0        0      938 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_levels.mcfunction
+-rw-r--r--   0        0        0      627 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_modified_level.mcfunction
+-rw-r--r--   0        0        0     1128 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/place.mcfunction
+-rw-r--r--   0        0        0       44 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/tick.mcfunction
+-rw-r--r--   0        0        0     1557 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/binomial_random.mcfunction
+-rw-r--r--   0        0        0      356 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/load.mcfunction
+-rw-r--r--   0        0        0       95 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/path.mcfunction
+-rw-r--r--   0        0        0      132 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/tick.mcfunction
+-rw-r--r--   0        0        0      469 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/uniform_random.mcfunction
+-rw-r--r--   0        0        0      604 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/test.mcfunction
+-rw-r--r--   0        0        0      507 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/README.md
+-rw-r--r--   0        0        0      288 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/beet.yaml
+-rw-r--r--   0        0        0      340 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/advancements/impl/technical/inventory_changed.json
+-rw-r--r--   0        0        0     3762 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_durability.mcfunction
+-rw-r--r--   0        0        0     1838 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_mending/clamp.mcfunction
+-rw-r--r--   0        0        0      228 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_mending/return_overflow.mcfunction
+-rw-r--r--   0        0        0      323 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_mending.mcfunction
+-rw-r--r--   0        0        0      414 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/boots.mcfunction
+-rw-r--r--   0        0        0      416 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/chestplate.mcfunction
+-rw-r--r--   0        0        0      336 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/force/sub.mcfunction
+-rw-r--r--   0        0        0     1668 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/force.mcfunction
+-rw-r--r--   0        0        0      414 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/helmet.mcfunction
+-rw-r--r--   0        0        0      414 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/leggings.mcfunction
+-rw-r--r--   0        0        0      414 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/mainhand.mcfunction
+-rw-r--r--   0        0        0      423 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/offhand.mcfunction
+-rw-r--r--   0        0        0      498 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage.mcfunction
+-rw-r--r--   0        0        0      774 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/detect.mcfunction
+-rw-r--r--   0        0        0     8770 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/get_max.mcfunction
+-rw-r--r--   0        0        0      221 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/init.mcfunction
+-rw-r--r--   0        0        0      404 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/boots.mcfunction
+-rw-r--r--   0        0        0      406 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/chestplate.mcfunction
+-rw-r--r--   0        0        0      439 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/handle.mcfunction
+-rw-r--r--   0        0        0      404 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/helmet.mcfunction
+-rw-r--r--   0        0        0      404 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/leggings.mcfunction
+-rw-r--r--   0        0        0      405 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/mainhand.mcfunction
+-rw-r--r--   0        0        0      413 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/process/offhand.mcfunction
+-rw-r--r--   0        0        0     8473 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/attributes.mcfunction
+-rw-r--r--   0        0        0    13178 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/base_attributes.mcfunction
+-rw-r--r--   0        0        0     2218 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/build.mcfunction
+-rw-r--r--   0        0        0      675 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/custom.mcfunction
+-rw-r--r--   0        0        0      405 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/durability.mcfunction
+-rw-r--r--   0        0        0     3259 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/enchantments.mcfunction
+-rw-r--r--   0        0        0        0 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/update_inventory.mcfunction
+-rw-r--r--   0        0        0      171 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/technical/load.mcfunction
+-rw-r--r--   0        0        0      110 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/technical/player.mcfunction
+-rw-r--r--   0        0        0      124 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/technical/tick.mcfunction
+-rw-r--r--   0        0        0      282 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/item_modifiers/update_nbt.json
+-rw-r--r--   0        0        0       86 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/predicates/chance/10.json
+-rw-r--r--   0        0        0       94 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/predicates/chance/11.json
+-rw-r--r--   0        0        0       88 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/predicates/chance/12.json
+-rw-r--r--   0        0        0       93 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/predicates/chance/14.json
+-rw-r--r--   0        0        0       94 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/predicates/chance/16.json
+-rw-r--r--   0        0        0       87 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/predicates/chance/20.json
+-rw-r--r--   0        0        0       87 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/predicates/chance/25.json
+-rw-r--r--   0        0        0       94 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/predicates/chance/33.json
+-rw-r--r--   0        0        0       86 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/predicates/chance/50.json
+-rw-r--r--   0        0        0       95 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/predicates/chance/9.json
+-rw-r--r--   0        0        0       20 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/tags/functions/event/build_custom.json
+-rw-r--r--   0        0        0    88530 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/item/pack.png
+-rw-r--r--   0        0        0       19 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/prevent-aggression/README.md
+-rw-r--r--   0        0        0      257 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/prevent-aggression/beet.yaml
+-rw-r--r--   0        0        0     2399 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/prevent-aggression/data/smithed.prevent_aggression/functions/impl/technical/10_tick.mcfunction
+-rw-r--r--   0        0        0      175 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/prevent-aggression/data/smithed.prevent_aggression/functions/impl/technical/load.mcfunction
+-rw-r--r--   0        0        0      359 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/prevent-aggression/data/smithed.prevent_aggression/tags/entity_types/mobs.json
+-rw-r--r--   0        0        0    13663 2023-06-24 17:51:48.914153 smithed_libraries-0.7.1/smithed_libraries/packs/prevent-aggression/pack.png
+-rw-r--r--   0        0        0        0 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/__init__.py
+-rw-r--r--   0        0        0      553 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/companion_mod.py
+-rw-r--r--   0        0        0     4105 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/documentation.py
+-rw-r--r--   0        0        0      729 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/manifest.py
+-rw-r--r--   0        0        0     1050 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/misc.py
+-rw-r--r--   0        0        0     2158 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/nbt_literals.py
+-rw-r--r--   0        0        0      129 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/README.md
+-rw-r--r--   0        0        0       61 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/__init__.py
+-rw-r--r--   0        0        0     1304 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/api.py
+-rw-r--r--   0        0        0     8097 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/load.py
+-rw-r--r--   0        0        0     3985 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/models.py
+-rw-r--r--   0        0        0     1478 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/plugin.py
+-rw-r--r--   0        0        0      112 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/types.py
+-rw-r--r--   0        0        0      483 2023-06-24 17:51:48.918152 smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/utils.py
+-rw-r--r--   0        0        0     9653 1970-01-01 00:00:00.000000 smithed_libraries-0.7.1/setup.py
+-rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 smithed_libraries-0.7.1/PKG-INFO
```

### Comparing `smithed_libraries-0.7.0/LICENSE` & `smithed_libraries-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/README.md` & `smithed_libraries-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/pyproject.toml` & `smithed_libraries-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smithed-libraries"
-version = "0.7.0"
+version = "0.7.1"
 description = "All of the Smithed Libraries"
 authors = ["Smithed Council <team@smithed.dev>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `smithed_libraries-0.7.0/smithed_libraries/__init__.py` & `smithed_libraries-0.7.1/smithed_libraries/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pyright: reportUnsupportedDunderAll=false
 
 from beet import subproject
 
 from . import plugins
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 __all__ = [
     "actionbar",
     "crafter",
     "crafter-addon",
     "custom-block",
     "damage",
```

### Comparing `smithed_libraries-0.7.0/smithed_libraries/common.yaml` & `smithed_libraries-0.7.1/smithed_libraries/common.yaml`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/README.md` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/README.md`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/advancements/impl/vanilla/bed/clicked_bed.json` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/advancements/impl/vanilla/bed/clicked_bed.json`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/advancements/impl/vanilla/container/clicked_lockable_block.json` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/advancements/impl/vanilla/container/clicked_lockable_block.json`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/display.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/display.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/message.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/message.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/technical/load.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/technical/load.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/technical/tick.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/technical/tick.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/check_sleep_status.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/check_sleep_status.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/clicked_bed.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/clicked_bed.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/send_sleep_status.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/send_sleep_status.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/show_sleep_percentage.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/show_sleep_percentage.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/track_leave_bed.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/bed/track_leave_bed.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/east.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/east.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/north.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/north.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/south.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/south.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/west.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock/west.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_double_chest_lock.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_lock.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/check_lock.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/raycast.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/raycast.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/send_message.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/functions/impl/vanilla/container/send_message.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/data/smithed.actionbar/predicates/impl/is_day.json` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/data/smithed.actionbar/predicates/impl/is_day.json`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/actionbar/pack.png` & `smithed_libraries-0.7.1/smithed_libraries/packs/actionbar/pack.png`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/models/block/table.json` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/models/block/table.json`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/heavy_workbench.png` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/block/heavy_workbench.png`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/gui/table.png` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/assets/smithed.crafter/textures/gui/table.png`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/beet.yaml` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/beet.yaml`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/break.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/break.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/handle_tags.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/handle_tags.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/mirror.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/mirror.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/process.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/process.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/query_tags.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/query_tags.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/read_barrel.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/input/read_barrel.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/export.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/export.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/export_output.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/export_output.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/move.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/move.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/spawn_loop.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/manage_invalids/spawn_loop.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/advanced.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/advanced.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/delete_tool.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/delete_tool.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/handle_tools.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/handle_tools.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/test.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input/test.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/clear_input.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/cursor_check/main.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/cursor_check/main.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/calculate_extras.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/calculate_extras.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/main.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/main.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/spawn_extra_items.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/output/shift_click/spawn_extra_items.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/0.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/0.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/1.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/1.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/2.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/2.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/3.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/3.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/4.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/4.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/5.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/5.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/6.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/6.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/7.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/7.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/8.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/checks/8.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/loop.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/loop.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/simplify.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes/simplify.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/crafting/shapeless_recipes.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/open_tick.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/open_tick.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/place.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/block/table/place.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/recipes/shaped.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/functions/impl/recipes/shaped.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/loot_tables/blocks/table.json` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/loot_tables/blocks/table.json`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/invalid_items.json` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/invalid_items.json`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/special_clear/buckets.json` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/special_clear/buckets.json`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/special_clear/tools.json` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/predicates/block/table/special_clear/tools.json`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/data/smithed.crafter/tags/items/all.json` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/data/smithed.crafter/tags/items/all.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9152091254752852%*

 * *Differences: {"'values'": "{insert: [(6, 'minecraft:acacia_hanging_sign'), (29, "*

 * *             "'minecraft:angler_pottery_sherd'), (32, 'minecraft:archer_pottery_sherd'), (34, "*

 * *             "'minecraft:arms_up_pottery_sherd'), (43, 'minecraft:bamboo_block'), (44, "*

 * *             "'minecraft:bamboo_button'), (45, 'minecraft:bamboo_chest_raft'), (46, "*

 * *             "'minecraft:bamboo_door'), (47, 'minecraft:bamboo_fence'), (48, "*

 * *             "'minecraft:bamboo_fence_gate'), (49, 'minecraft:bamboo_hanging_sign'), (50, "*

 * *  […]*

```diff
@@ -2,14 +2,15 @@
     "values": [
         "minecraft:acacia_boat",
         "minecraft:acacia_button",
         "minecraft:acacia_chest_boat",
         "minecraft:acacia_door",
         "minecraft:acacia_fence",
         "minecraft:acacia_fence_gate",
+        "minecraft:acacia_hanging_sign",
         "minecraft:acacia_leaves",
         "minecraft:acacia_log",
         "minecraft:acacia_planks",
         "minecraft:acacia_pressure_plate",
         "minecraft:acacia_sapling",
         "minecraft:acacia_sign",
         "minecraft:acacia_slab",
@@ -24,73 +25,95 @@
         "minecraft:amethyst_cluster",
         "minecraft:amethyst_shard",
         "minecraft:ancient_debris",
         "minecraft:andesite",
         "minecraft:andesite_slab",
         "minecraft:andesite_stairs",
         "minecraft:andesite_wall",
+        "minecraft:angler_pottery_sherd",
         "minecraft:anvil",
         "minecraft:apple",
+        "minecraft:archer_pottery_sherd",
         "minecraft:armor_stand",
+        "minecraft:arms_up_pottery_sherd",
         "minecraft:arrow",
         "minecraft:axolotl_bucket",
         "minecraft:axolotl_spawn_egg",
         "minecraft:azalea",
         "minecraft:azalea_leaves",
         "minecraft:azure_bluet",
         "minecraft:baked_potato",
         "minecraft:bamboo",
+        "minecraft:bamboo_block",
+        "minecraft:bamboo_button",
+        "minecraft:bamboo_chest_raft",
+        "minecraft:bamboo_door",
+        "minecraft:bamboo_fence",
+        "minecraft:bamboo_fence_gate",
+        "minecraft:bamboo_hanging_sign",
+        "minecraft:bamboo_mosaic",
+        "minecraft:bamboo_mosaic_slab",
+        "minecraft:bamboo_mosaic_stairs",
+        "minecraft:bamboo_planks",
+        "minecraft:bamboo_pressure_plate",
+        "minecraft:bamboo_raft",
+        "minecraft:bamboo_sign",
+        "minecraft:bamboo_slab",
+        "minecraft:bamboo_stairs",
+        "minecraft:bamboo_trapdoor",
         "minecraft:barrel",
         "minecraft:barrier",
         "minecraft:basalt",
         "minecraft:bat_spawn_egg",
         "minecraft:beacon",
         "minecraft:bedrock",
+        "minecraft:bee_nest",
+        "minecraft:bee_spawn_egg",
         "minecraft:beef",
         "minecraft:beehive",
         "minecraft:beetroot",
         "minecraft:beetroot_seeds",
         "minecraft:beetroot_soup",
-        "minecraft:bee_nest",
-        "minecraft:bee_spawn_egg",
         "minecraft:bell",
         "minecraft:big_dripleaf",
         "minecraft:birch_boat",
         "minecraft:birch_button",
         "minecraft:birch_chest_boat",
         "minecraft:birch_door",
         "minecraft:birch_fence",
         "minecraft:birch_fence_gate",
+        "minecraft:birch_hanging_sign",
         "minecraft:birch_leaves",
         "minecraft:birch_log",
         "minecraft:birch_planks",
         "minecraft:birch_pressure_plate",
         "minecraft:birch_sapling",
         "minecraft:birch_sign",
         "minecraft:birch_slab",
         "minecraft:birch_stairs",
         "minecraft:birch_trapdoor",
         "minecraft:birch_wood",
-        "minecraft:blackstone",
-        "minecraft:blackstone_slab",
-        "minecraft:blackstone_stairs",
-        "minecraft:blackstone_wall",
         "minecraft:black_banner",
         "minecraft:black_bed",
         "minecraft:black_candle",
         "minecraft:black_carpet",
         "minecraft:black_concrete",
         "minecraft:black_concrete_powder",
         "minecraft:black_dye",
         "minecraft:black_glazed_terracotta",
         "minecraft:black_shulker_box",
         "minecraft:black_stained_glass",
         "minecraft:black_stained_glass_pane",
         "minecraft:black_terracotta",
         "minecraft:black_wool",
+        "minecraft:blackstone",
+        "minecraft:blackstone_slab",
+        "minecraft:blackstone_stairs",
+        "minecraft:blackstone_wall",
+        "minecraft:blade_pottery_sherd",
         "minecraft:blast_furnace",
         "minecraft:blaze_powder",
         "minecraft:blaze_rod",
         "minecraft:blaze_spawn_egg",
         "minecraft:blue_banner",
         "minecraft:blue_bed",
         "minecraft:blue_candle",
@@ -113,20 +136,21 @@
         "minecraft:bookshelf",
         "minecraft:bow",
         "minecraft:bowl",
         "minecraft:brain_coral",
         "minecraft:brain_coral_block",
         "minecraft:brain_coral_fan",
         "minecraft:bread",
+        "minecraft:brewer_pottery_sherd",
         "minecraft:brewing_stand",
         "minecraft:brick",
-        "minecraft:bricks",
         "minecraft:brick_slab",
         "minecraft:brick_stairs",
         "minecraft:brick_wall",
+        "minecraft:bricks",
         "minecraft:brown_banner",
         "minecraft:brown_bed",
         "minecraft:brown_candle",
         "minecraft:brown_carpet",
         "minecraft:brown_concrete",
         "minecraft:brown_concrete_powder",
         "minecraft:brown_dye",
@@ -134,44 +158,66 @@
         "minecraft:brown_mushroom",
         "minecraft:brown_mushroom_block",
         "minecraft:brown_shulker_box",
         "minecraft:brown_stained_glass",
         "minecraft:brown_stained_glass_pane",
         "minecraft:brown_terracotta",
         "minecraft:brown_wool",
+        "minecraft:brush",
         "minecraft:bubble_coral",
         "minecraft:bubble_coral_block",
         "minecraft:bubble_coral_fan",
         "minecraft:bucket",
         "minecraft:budding_amethyst",
         "minecraft:bundle",
+        "minecraft:burn_pottery_sherd",
         "minecraft:cactus",
         "minecraft:cake",
         "minecraft:calcite",
+        "minecraft:calibrated_sculk_sensor",
+        "minecraft:camel_spawn_egg",
         "minecraft:campfire",
         "minecraft:candle",
         "minecraft:carrot",
         "minecraft:carrot_on_a_stick",
         "minecraft:cartography_table",
         "minecraft:carved_pumpkin",
         "minecraft:cat_spawn_egg",
         "minecraft:cauldron",
         "minecraft:cave_spider_spawn_egg",
         "minecraft:chain",
+        "minecraft:chain_command_block",
         "minecraft:chainmail_boots",
         "minecraft:chainmail_chestplate",
         "minecraft:chainmail_helmet",
         "minecraft:chainmail_leggings",
-        "minecraft:chain_command_block",
         "minecraft:charcoal",
+        "minecraft:cherry_boat",
+        "minecraft:cherry_button",
+        "minecraft:cherry_chest_boat",
+        "minecraft:cherry_door",
+        "minecraft:cherry_fence",
+        "minecraft:cherry_fence_gate",
+        "minecraft:cherry_hanging_sign",
+        "minecraft:cherry_leaves",
+        "minecraft:cherry_log",
+        "minecraft:cherry_planks",
+        "minecraft:cherry_pressure_plate",
+        "minecraft:cherry_sapling",
+        "minecraft:cherry_sign",
+        "minecraft:cherry_slab",
+        "minecraft:cherry_stairs",
+        "minecraft:cherry_trapdoor",
+        "minecraft:cherry_wood",
         "minecraft:chest",
         "minecraft:chest_minecart",
         "minecraft:chicken",
         "minecraft:chicken_spawn_egg",
         "minecraft:chipped_anvil",
+        "minecraft:chiseled_bookshelf",
         "minecraft:chiseled_deepslate",
         "minecraft:chiseled_nether_bricks",
         "minecraft:chiseled_polished_blackstone",
         "minecraft:chiseled_quartz_block",
         "minecraft:chiseled_red_sandstone",
         "minecraft:chiseled_sandstone",
         "minecraft:chiseled_stone_bricks",
@@ -181,14 +227,15 @@
         "minecraft:clay",
         "minecraft:clay_ball",
         "minecraft:clock",
         "minecraft:coal",
         "minecraft:coal_block",
         "minecraft:coal_ore",
         "minecraft:coarse_dirt",
+        "minecraft:coast_armor_trim_smithing_template",
         "minecraft:cobbled_deepslate",
         "minecraft:cobbled_deepslate_slab",
         "minecraft:cobbled_deepslate_stairs",
         "minecraft:cobbled_deepslate_wall",
         "minecraft:cobblestone",
         "minecraft:cobblestone_slab",
         "minecraft:cobblestone_stairs",
@@ -227,14 +274,15 @@
         "minecraft:creeper_head",
         "minecraft:creeper_spawn_egg",
         "minecraft:crimson_button",
         "minecraft:crimson_door",
         "minecraft:crimson_fence",
         "minecraft:crimson_fence_gate",
         "minecraft:crimson_fungus",
+        "minecraft:crimson_hanging_sign",
         "minecraft:crimson_hyphae",
         "minecraft:crimson_nylium",
         "minecraft:crimson_planks",
         "minecraft:crimson_pressure_plate",
         "minecraft:crimson_roots",
         "minecraft:crimson_sign",
         "minecraft:crimson_slab",
@@ -261,20 +309,22 @@
         "minecraft:cyan_shulker_box",
         "minecraft:cyan_stained_glass",
         "minecraft:cyan_stained_glass_pane",
         "minecraft:cyan_terracotta",
         "minecraft:cyan_wool",
         "minecraft:damaged_anvil",
         "minecraft:dandelion",
+        "minecraft:danger_pottery_sherd",
         "minecraft:dark_oak_boat",
         "minecraft:dark_oak_button",
         "minecraft:dark_oak_chest_boat",
         "minecraft:dark_oak_door",
         "minecraft:dark_oak_fence",
         "minecraft:dark_oak_fence_gate",
+        "minecraft:dark_oak_hanging_sign",
         "minecraft:dark_oak_leaves",
         "minecraft:dark_oak_log",
         "minecraft:dark_oak_planks",
         "minecraft:dark_oak_pressure_plate",
         "minecraft:dark_oak_sapling",
         "minecraft:dark_oak_sign",
         "minecraft:dark_oak_slab",
@@ -298,31 +348,32 @@
         "minecraft:dead_horn_coral",
         "minecraft:dead_horn_coral_block",
         "minecraft:dead_horn_coral_fan",
         "minecraft:dead_tube_coral",
         "minecraft:dead_tube_coral_block",
         "minecraft:dead_tube_coral_fan",
         "minecraft:debug_stick",
+        "minecraft:decorated_pot",
         "minecraft:deepslate",
-        "minecraft:deepslate_bricks",
         "minecraft:deepslate_brick_slab",
         "minecraft:deepslate_brick_stairs",
         "minecraft:deepslate_brick_wall",
+        "minecraft:deepslate_bricks",
         "minecraft:deepslate_coal_ore",
         "minecraft:deepslate_copper_ore",
         "minecraft:deepslate_diamond_ore",
         "minecraft:deepslate_emerald_ore",
         "minecraft:deepslate_gold_ore",
         "minecraft:deepslate_iron_ore",
         "minecraft:deepslate_lapis_ore",
         "minecraft:deepslate_redstone_ore",
-        "minecraft:deepslate_tiles",
         "minecraft:deepslate_tile_slab",
         "minecraft:deepslate_tile_stairs",
         "minecraft:deepslate_tile_wall",
+        "minecraft:deepslate_tiles",
         "minecraft:detector_rail",
         "minecraft:diamond",
         "minecraft:diamond_axe",
         "minecraft:diamond_block",
         "minecraft:diamond_boots",
         "minecraft:diamond_chestplate",
         "minecraft:diamond_helmet",
@@ -347,100 +398,105 @@
         "minecraft:dragon_egg",
         "minecraft:dragon_head",
         "minecraft:dried_kelp",
         "minecraft:dried_kelp_block",
         "minecraft:dripstone_block",
         "minecraft:dropper",
         "minecraft:drowned_spawn_egg",
+        "minecraft:dune_armor_trim_smithing_template",
         "minecraft:echo_shard",
         "minecraft:egg",
         "minecraft:elder_guardian_spawn_egg",
         "minecraft:elytra",
         "minecraft:emerald",
         "minecraft:emerald_block",
         "minecraft:emerald_ore",
         "minecraft:enchanted_book",
         "minecraft:enchanted_golden_apple",
         "minecraft:enchanting_table",
-        "minecraft:enderman_spawn_egg",
-        "minecraft:endermite_spawn_egg",
-        "minecraft:ender_chest",
-        "minecraft:ender_eye",
-        "minecraft:ender_pearl",
         "minecraft:end_crystal",
         "minecraft:end_portal_frame",
         "minecraft:end_rod",
         "minecraft:end_stone",
-        "minecraft:end_stone_bricks",
         "minecraft:end_stone_brick_slab",
         "minecraft:end_stone_brick_stairs",
         "minecraft:end_stone_brick_wall",
+        "minecraft:end_stone_bricks",
+        "minecraft:ender_chest",
+        "minecraft:ender_dragon_spawn_egg",
+        "minecraft:ender_eye",
+        "minecraft:ender_pearl",
+        "minecraft:enderman_spawn_egg",
+        "minecraft:endermite_spawn_egg",
         "minecraft:evoker_spawn_egg",
         "minecraft:experience_bottle",
+        "minecraft:explorer_pottery_sherd",
         "minecraft:exposed_copper",
         "minecraft:exposed_cut_copper",
         "minecraft:exposed_cut_copper_slab",
         "minecraft:exposed_cut_copper_stairs",
+        "minecraft:eye_armor_trim_smithing_template",
         "minecraft:farmland",
         "minecraft:feather",
         "minecraft:fermented_spider_eye",
         "minecraft:fern",
         "minecraft:filled_map",
-        "minecraft:firework_rocket",
-        "minecraft:firework_star",
         "minecraft:fire_charge",
         "minecraft:fire_coral",
         "minecraft:fire_coral_block",
         "minecraft:fire_coral_fan",
+        "minecraft:firework_rocket",
+        "minecraft:firework_star",
         "minecraft:fishing_rod",
         "minecraft:fletching_table",
         "minecraft:flint",
         "minecraft:flint_and_steel",
-        "minecraft:flowering_azalea",
-        "minecraft:flowering_azalea_leaves",
         "minecraft:flower_banner_pattern",
         "minecraft:flower_pot",
+        "minecraft:flowering_azalea",
+        "minecraft:flowering_azalea_leaves",
         "minecraft:fox_spawn_egg",
-        "minecraft:frogspawn",
+        "minecraft:friend_pottery_sherd",
         "minecraft:frog_spawn_egg",
+        "minecraft:frogspawn",
         "minecraft:furnace",
         "minecraft:furnace_minecart",
         "minecraft:ghast_spawn_egg",
         "minecraft:ghast_tear",
         "minecraft:gilded_blackstone",
         "minecraft:glass",
         "minecraft:glass_bottle",
         "minecraft:glass_pane",
         "minecraft:glistering_melon_slice",
         "minecraft:globe_banner_pattern",
-        "minecraft:glowstone",
-        "minecraft:glowstone_dust",
         "minecraft:glow_berries",
         "minecraft:glow_ink_sac",
         "minecraft:glow_item_frame",
         "minecraft:glow_lichen",
         "minecraft:glow_squid_spawn_egg",
+        "minecraft:glowstone",
+        "minecraft:glowstone_dust",
         "minecraft:goat_horn",
         "minecraft:goat_spawn_egg",
+        "minecraft:gold_block",
+        "minecraft:gold_ingot",
+        "minecraft:gold_nugget",
+        "minecraft:gold_ore",
         "minecraft:golden_apple",
         "minecraft:golden_axe",
         "minecraft:golden_boots",
         "minecraft:golden_carrot",
         "minecraft:golden_chestplate",
         "minecraft:golden_helmet",
         "minecraft:golden_hoe",
         "minecraft:golden_horse_armor",
         "minecraft:golden_leggings",
         "minecraft:golden_pickaxe",
         "minecraft:golden_shovel",
         "minecraft:golden_sword",
-        "minecraft:gold_block",
-        "minecraft:gold_ingot",
-        "minecraft:gold_nugget",
-        "minecraft:gold_ore",
         "minecraft:granite",
         "minecraft:granite_slab",
         "minecraft:granite_stairs",
         "minecraft:granite_wall",
         "minecraft:grass",
         "minecraft:grass_block",
         "minecraft:gravel",
@@ -472,26 +528,30 @@
         "minecraft:green_wool",
         "minecraft:grindstone",
         "minecraft:guardian_spawn_egg",
         "minecraft:gunpowder",
         "minecraft:hanging_roots",
         "minecraft:hay_block",
         "minecraft:heart_of_the_sea",
+        "minecraft:heart_pottery_sherd",
+        "minecraft:heartbreak_pottery_sherd",
         "minecraft:heavy_weighted_pressure_plate",
         "minecraft:hoglin_spawn_egg",
-        "minecraft:honeycomb",
-        "minecraft:honeycomb_block",
         "minecraft:honey_block",
         "minecraft:honey_bottle",
+        "minecraft:honeycomb",
+        "minecraft:honeycomb_block",
         "minecraft:hopper",
         "minecraft:hopper_minecart",
         "minecraft:horn_coral",
         "minecraft:horn_coral_block",
         "minecraft:horn_coral_fan",
         "minecraft:horse_spawn_egg",
+        "minecraft:host_armor_trim_smithing_template",
+        "minecraft:howl_pottery_sherd",
         "minecraft:husk_spawn_egg",
         "minecraft:ice",
         "minecraft:infested_chiseled_stone_bricks",
         "minecraft:infested_cobblestone",
         "minecraft:infested_cracked_stone_bricks",
         "minecraft:infested_deepslate",
         "minecraft:infested_mossy_stone_bricks",
@@ -500,14 +560,15 @@
         "minecraft:ink_sac",
         "minecraft:iron_axe",
         "minecraft:iron_bars",
         "minecraft:iron_block",
         "minecraft:iron_boots",
         "minecraft:iron_chestplate",
         "minecraft:iron_door",
+        "minecraft:iron_golem_spawn_egg",
         "minecraft:iron_helmet",
         "minecraft:iron_hoe",
         "minecraft:iron_horse_armor",
         "minecraft:iron_ingot",
         "minecraft:iron_leggings",
         "minecraft:iron_nugget",
         "minecraft:iron_ore",
@@ -521,14 +582,15 @@
         "minecraft:jukebox",
         "minecraft:jungle_boat",
         "minecraft:jungle_button",
         "minecraft:jungle_chest_boat",
         "minecraft:jungle_door",
         "minecraft:jungle_fence",
         "minecraft:jungle_fence_gate",
+        "minecraft:jungle_hanging_sign",
         "minecraft:jungle_leaves",
         "minecraft:jungle_log",
         "minecraft:jungle_planks",
         "minecraft:jungle_pressure_plate",
         "minecraft:jungle_sapling",
         "minecraft:jungle_sign",
         "minecraft:jungle_slab",
@@ -551,15 +613,14 @@
         "minecraft:leather_chestplate",
         "minecraft:leather_helmet",
         "minecraft:leather_horse_armor",
         "minecraft:leather_leggings",
         "minecraft:lectern",
         "minecraft:lever",
         "minecraft:light",
-        "minecraft:lightning_rod",
         "minecraft:light_blue_banner",
         "minecraft:light_blue_bed",
         "minecraft:light_blue_candle",
         "minecraft:light_blue_carpet",
         "minecraft:light_blue_concrete",
         "minecraft:light_blue_concrete_powder",
         "minecraft:light_blue_dye",
@@ -579,14 +640,15 @@
         "minecraft:light_gray_glazed_terracotta",
         "minecraft:light_gray_shulker_box",
         "minecraft:light_gray_stained_glass",
         "minecraft:light_gray_stained_glass_pane",
         "minecraft:light_gray_terracotta",
         "minecraft:light_gray_wool",
         "minecraft:light_weighted_pressure_plate",
+        "minecraft:lightning_rod",
         "minecraft:lilac",
         "minecraft:lily_of_the_valley",
         "minecraft:lily_pad",
         "minecraft:lime_banner",
         "minecraft:lime_bed",
         "minecraft:lime_candle",
         "minecraft:lime_carpet",
@@ -621,14 +683,15 @@
         "minecraft:magma_cube_spawn_egg",
         "minecraft:mangrove_boat",
         "minecraft:mangrove_button",
         "minecraft:mangrove_chest_boat",
         "minecraft:mangrove_door",
         "minecraft:mangrove_fence",
         "minecraft:mangrove_fence_gate",
+        "minecraft:mangrove_hanging_sign",
         "minecraft:mangrove_leaves",
         "minecraft:mangrove_log",
         "minecraft:mangrove_planks",
         "minecraft:mangrove_pressure_plate",
         "minecraft:mangrove_propagule",
         "minecraft:mangrove_roots",
         "minecraft:mangrove_sign",
@@ -639,86 +702,91 @@
         "minecraft:map",
         "minecraft:medium_amethyst_bud",
         "minecraft:melon",
         "minecraft:melon_seeds",
         "minecraft:melon_slice",
         "minecraft:milk_bucket",
         "minecraft:minecart",
+        "minecraft:miner_pottery_sherd",
         "minecraft:mojang_banner_pattern",
         "minecraft:mooshroom_spawn_egg",
+        "minecraft:moss_block",
+        "minecraft:moss_carpet",
         "minecraft:mossy_cobblestone",
         "minecraft:mossy_cobblestone_slab",
         "minecraft:mossy_cobblestone_stairs",
         "minecraft:mossy_cobblestone_wall",
-        "minecraft:mossy_stone_bricks",
         "minecraft:mossy_stone_brick_slab",
         "minecraft:mossy_stone_brick_stairs",
         "minecraft:mossy_stone_brick_wall",
-        "minecraft:moss_block",
-        "minecraft:moss_carpet",
+        "minecraft:mossy_stone_bricks",
+        "minecraft:mourner_pottery_sherd",
         "minecraft:mud",
-        "minecraft:muddy_mangrove_roots",
-        "minecraft:mud_bricks",
         "minecraft:mud_brick_slab",
         "minecraft:mud_brick_stairs",
         "minecraft:mud_brick_wall",
+        "minecraft:mud_bricks",
+        "minecraft:muddy_mangrove_roots",
         "minecraft:mule_spawn_egg",
         "minecraft:mushroom_stem",
         "minecraft:mushroom_stew",
         "minecraft:music_disc_11",
         "minecraft:music_disc_13",
         "minecraft:music_disc_5",
         "minecraft:music_disc_blocks",
         "minecraft:music_disc_cat",
         "minecraft:music_disc_chirp",
         "minecraft:music_disc_far",
         "minecraft:music_disc_mall",
         "minecraft:music_disc_mellohi",
         "minecraft:music_disc_otherside",
         "minecraft:music_disc_pigstep",
+        "minecraft:music_disc_relic",
         "minecraft:music_disc_stal",
         "minecraft:music_disc_strad",
         "minecraft:music_disc_wait",
         "minecraft:music_disc_ward",
         "minecraft:mutton",
         "minecraft:mycelium",
         "minecraft:name_tag",
         "minecraft:nautilus_shell",
+        "minecraft:nether_brick",
+        "minecraft:nether_brick_fence",
+        "minecraft:nether_brick_slab",
+        "minecraft:nether_brick_stairs",
+        "minecraft:nether_brick_wall",
+        "minecraft:nether_bricks",
+        "minecraft:nether_gold_ore",
+        "minecraft:nether_quartz_ore",
+        "minecraft:nether_sprouts",
+        "minecraft:nether_star",
+        "minecraft:nether_wart",
+        "minecraft:nether_wart_block",
         "minecraft:netherite_axe",
         "minecraft:netherite_block",
         "minecraft:netherite_boots",
         "minecraft:netherite_chestplate",
         "minecraft:netherite_helmet",
         "minecraft:netherite_hoe",
         "minecraft:netherite_ingot",
         "minecraft:netherite_leggings",
         "minecraft:netherite_pickaxe",
         "minecraft:netherite_scrap",
         "minecraft:netherite_shovel",
         "minecraft:netherite_sword",
+        "minecraft:netherite_upgrade_smithing_template",
         "minecraft:netherrack",
-        "minecraft:nether_brick",
-        "minecraft:nether_bricks",
-        "minecraft:nether_brick_fence",
-        "minecraft:nether_brick_slab",
-        "minecraft:nether_brick_stairs",
-        "minecraft:nether_brick_wall",
-        "minecraft:nether_gold_ore",
-        "minecraft:nether_quartz_ore",
-        "minecraft:nether_sprouts",
-        "minecraft:nether_star",
-        "minecraft:nether_wart",
-        "minecraft:nether_wart_block",
         "minecraft:note_block",
         "minecraft:oak_boat",
         "minecraft:oak_button",
         "minecraft:oak_chest_boat",
         "minecraft:oak_door",
         "minecraft:oak_fence",
         "minecraft:oak_fence_gate",
+        "minecraft:oak_hanging_sign",
         "minecraft:oak_leaves",
         "minecraft:oak_log",
         "minecraft:oak_planks",
         "minecraft:oak_pressure_plate",
         "minecraft:oak_sapling",
         "minecraft:oak_sign",
         "minecraft:oak_slab",
@@ -755,48 +823,53 @@
         "minecraft:paper",
         "minecraft:parrot_spawn_egg",
         "minecraft:pearlescent_froglight",
         "minecraft:peony",
         "minecraft:petrified_oak_slab",
         "minecraft:phantom_membrane",
         "minecraft:phantom_spawn_egg",
+        "minecraft:pig_spawn_egg",
         "minecraft:piglin_banner_pattern",
         "minecraft:piglin_brute_spawn_egg",
+        "minecraft:piglin_head",
         "minecraft:piglin_spawn_egg",
-        "minecraft:pig_spawn_egg",
         "minecraft:pillager_spawn_egg",
         "minecraft:pink_banner",
         "minecraft:pink_bed",
         "minecraft:pink_candle",
         "minecraft:pink_carpet",
         "minecraft:pink_concrete",
         "minecraft:pink_concrete_powder",
         "minecraft:pink_dye",
         "minecraft:pink_glazed_terracotta",
+        "minecraft:pink_petals",
         "minecraft:pink_shulker_box",
         "minecraft:pink_stained_glass",
         "minecraft:pink_stained_glass_pane",
         "minecraft:pink_terracotta",
         "minecraft:pink_tulip",
         "minecraft:pink_wool",
         "minecraft:piston",
+        "minecraft:pitcher_plant",
+        "minecraft:pitcher_pod",
         "minecraft:player_head",
+        "minecraft:plenty_pottery_sherd",
         "minecraft:podzol",
         "minecraft:pointed_dripstone",
         "minecraft:poisonous_potato",
         "minecraft:polar_bear_spawn_egg",
         "minecraft:polished_andesite",
         "minecraft:polished_andesite_slab",
         "minecraft:polished_andesite_stairs",
         "minecraft:polished_basalt",
         "minecraft:polished_blackstone",
-        "minecraft:polished_blackstone_bricks",
         "minecraft:polished_blackstone_brick_slab",
         "minecraft:polished_blackstone_brick_stairs",
         "minecraft:polished_blackstone_brick_wall",
+        "minecraft:polished_blackstone_bricks",
         "minecraft:polished_blackstone_button",
         "minecraft:polished_blackstone_pressure_plate",
         "minecraft:polished_blackstone_slab",
         "minecraft:polished_blackstone_stairs",
         "minecraft:polished_blackstone_wall",
         "minecraft:polished_deepslate",
         "minecraft:polished_deepslate_slab",
@@ -812,22 +885,23 @@
         "minecraft:poppy",
         "minecraft:porkchop",
         "minecraft:potato",
         "minecraft:potion",
         "minecraft:powder_snow_bucket",
         "minecraft:powered_rail",
         "minecraft:prismarine",
-        "minecraft:prismarine_bricks",
         "minecraft:prismarine_brick_slab",
         "minecraft:prismarine_brick_stairs",
+        "minecraft:prismarine_bricks",
         "minecraft:prismarine_crystals",
         "minecraft:prismarine_shard",
         "minecraft:prismarine_slab",
         "minecraft:prismarine_stairs",
         "minecraft:prismarine_wall",
+        "minecraft:prize_pottery_sherd",
         "minecraft:pufferfish",
         "minecraft:pufferfish_bucket",
         "minecraft:pufferfish_spawn_egg",
         "minecraft:pumpkin",
         "minecraft:pumpkin_pie",
         "minecraft:pumpkin_seeds",
         "minecraft:purple_banner",
@@ -855,56 +929,58 @@
         "minecraft:quartz_stairs",
         "minecraft:rabbit",
         "minecraft:rabbit_foot",
         "minecraft:rabbit_hide",
         "minecraft:rabbit_spawn_egg",
         "minecraft:rabbit_stew",
         "minecraft:rail",
+        "minecraft:raiser_armor_trim_smithing_template",
         "minecraft:ravager_spawn_egg",
         "minecraft:raw_copper",
         "minecraft:raw_copper_block",
         "minecraft:raw_gold",
         "minecraft:raw_gold_block",
         "minecraft:raw_iron",
         "minecraft:raw_iron_block",
         "minecraft:recovery_compass",
-        "minecraft:redstone",
-        "minecraft:redstone_block",
-        "minecraft:redstone_lamp",
-        "minecraft:redstone_ore",
-        "minecraft:redstone_torch",
         "minecraft:red_banner",
         "minecraft:red_bed",
         "minecraft:red_candle",
         "minecraft:red_carpet",
         "minecraft:red_concrete",
         "minecraft:red_concrete_powder",
         "minecraft:red_dye",
         "minecraft:red_glazed_terracotta",
         "minecraft:red_mushroom",
         "minecraft:red_mushroom_block",
-        "minecraft:red_nether_bricks",
         "minecraft:red_nether_brick_slab",
         "minecraft:red_nether_brick_stairs",
         "minecraft:red_nether_brick_wall",
+        "minecraft:red_nether_bricks",
         "minecraft:red_sand",
         "minecraft:red_sandstone",
         "minecraft:red_sandstone_slab",
         "minecraft:red_sandstone_stairs",
         "minecraft:red_sandstone_wall",
         "minecraft:red_shulker_box",
         "minecraft:red_stained_glass",
         "minecraft:red_stained_glass_pane",
         "minecraft:red_terracotta",
         "minecraft:red_tulip",
         "minecraft:red_wool",
+        "minecraft:redstone",
+        "minecraft:redstone_block",
+        "minecraft:redstone_lamp",
+        "minecraft:redstone_ore",
+        "minecraft:redstone_torch",
         "minecraft:reinforced_deepslate",
         "minecraft:repeater",
         "minecraft:repeating_command_block",
         "minecraft:respawn_anchor",
+        "minecraft:rib_armor_trim_smithing_template",
         "minecraft:rooted_dirt",
         "minecraft:rose_bush",
         "minecraft:rotten_flesh",
         "minecraft:saddle",
         "minecraft:salmon",
         "minecraft:salmon_bucket",
         "minecraft:salmon_spawn_egg",
@@ -916,29 +992,35 @@
         "minecraft:scaffolding",
         "minecraft:sculk",
         "minecraft:sculk_catalyst",
         "minecraft:sculk_sensor",
         "minecraft:sculk_shrieker",
         "minecraft:sculk_vein",
         "minecraft:scute",
-        "minecraft:seagrass",
         "minecraft:sea_lantern",
         "minecraft:sea_pickle",
+        "minecraft:seagrass",
+        "minecraft:sentry_armor_trim_smithing_template",
+        "minecraft:shaper_armor_trim_smithing_template",
+        "minecraft:sheaf_pottery_sherd",
         "minecraft:shears",
         "minecraft:sheep_spawn_egg",
+        "minecraft:shelter_pottery_sherd",
         "minecraft:shield",
         "minecraft:shroomlight",
         "minecraft:shulker_box",
         "minecraft:shulker_shell",
         "minecraft:shulker_spawn_egg",
+        "minecraft:silence_armor_trim_smithing_template",
         "minecraft:silverfish_spawn_egg",
         "minecraft:skeleton_horse_spawn_egg",
         "minecraft:skeleton_skull",
         "minecraft:skeleton_spawn_egg",
         "minecraft:skull_banner_pattern",
+        "minecraft:skull_pottery_sherd",
         "minecraft:slime_ball",
         "minecraft:slime_block",
         "minecraft:slime_spawn_egg",
         "minecraft:small_amethyst_bud",
         "minecraft:small_dripleaf",
         "minecraft:smithing_table",
         "minecraft:smoker",
@@ -950,35 +1032,42 @@
         "minecraft:smooth_red_sandstone_slab",
         "minecraft:smooth_red_sandstone_stairs",
         "minecraft:smooth_sandstone",
         "minecraft:smooth_sandstone_slab",
         "minecraft:smooth_sandstone_stairs",
         "minecraft:smooth_stone",
         "minecraft:smooth_stone_slab",
+        "minecraft:sniffer_egg",
+        "minecraft:sniffer_spawn_egg",
+        "minecraft:snort_pottery_sherd",
+        "minecraft:snout_armor_trim_smithing_template",
         "minecraft:snow",
-        "minecraft:snowball",
         "minecraft:snow_block",
+        "minecraft:snow_golem_spawn_egg",
+        "minecraft:snowball",
         "minecraft:soul_campfire",
         "minecraft:soul_lantern",
         "minecraft:soul_sand",
         "minecraft:soul_soil",
         "minecraft:soul_torch",
         "minecraft:spawner",
         "minecraft:spectral_arrow",
         "minecraft:spider_eye",
         "minecraft:spider_spawn_egg",
+        "minecraft:spire_armor_trim_smithing_template",
         "minecraft:splash_potion",
         "minecraft:sponge",
         "minecraft:spore_blossom",
         "minecraft:spruce_boat",
         "minecraft:spruce_button",
         "minecraft:spruce_chest_boat",
         "minecraft:spruce_door",
         "minecraft:spruce_fence",
         "minecraft:spruce_fence_gate",
+        "minecraft:spruce_hanging_sign",
         "minecraft:spruce_leaves",
         "minecraft:spruce_log",
         "minecraft:spruce_planks",
         "minecraft:spruce_pressure_plate",
         "minecraft:spruce_sapling",
         "minecraft:spruce_sign",
         "minecraft:spruce_slab",
@@ -986,35 +1075,38 @@
         "minecraft:spruce_trapdoor",
         "minecraft:spruce_wood",
         "minecraft:spyglass",
         "minecraft:squid_spawn_egg",
         "minecraft:stick",
         "minecraft:sticky_piston",
         "minecraft:stone",
-        "minecraft:stonecutter",
         "minecraft:stone_axe",
-        "minecraft:stone_bricks",
         "minecraft:stone_brick_slab",
         "minecraft:stone_brick_stairs",
         "minecraft:stone_brick_wall",
+        "minecraft:stone_bricks",
         "minecraft:stone_button",
         "minecraft:stone_hoe",
         "minecraft:stone_pickaxe",
         "minecraft:stone_pressure_plate",
         "minecraft:stone_shovel",
         "minecraft:stone_slab",
         "minecraft:stone_stairs",
         "minecraft:stone_sword",
+        "minecraft:stonecutter",
         "minecraft:stray_spawn_egg",
         "minecraft:strider_spawn_egg",
         "minecraft:string",
         "minecraft:stripped_acacia_log",
         "minecraft:stripped_acacia_wood",
+        "minecraft:stripped_bamboo_block",
         "minecraft:stripped_birch_log",
         "minecraft:stripped_birch_wood",
+        "minecraft:stripped_cherry_log",
+        "minecraft:stripped_cherry_wood",
         "minecraft:stripped_crimson_hyphae",
         "minecraft:stripped_crimson_stem",
         "minecraft:stripped_dark_oak_log",
         "minecraft:stripped_dark_oak_wood",
         "minecraft:stripped_jungle_log",
         "minecraft:stripped_jungle_wood",
         "minecraft:stripped_mangrove_log",
@@ -1026,26 +1118,31 @@
         "minecraft:stripped_warped_hyphae",
         "minecraft:stripped_warped_stem",
         "minecraft:structure_block",
         "minecraft:structure_void",
         "minecraft:sugar",
         "minecraft:sugar_cane",
         "minecraft:sunflower",
+        "minecraft:suspicious_gravel",
+        "minecraft:suspicious_sand",
         "minecraft:suspicious_stew",
         "minecraft:sweet_berries",
         "minecraft:tadpole_bucket",
         "minecraft:tadpole_spawn_egg",
         "minecraft:tall_grass",
         "minecraft:target",
         "minecraft:terracotta",
+        "minecraft:tide_armor_trim_smithing_template",
         "minecraft:tinted_glass",
         "minecraft:tipped_arrow",
         "minecraft:tnt",
         "minecraft:tnt_minecart",
         "minecraft:torch",
+        "minecraft:torchflower",
+        "minecraft:torchflower_seeds",
         "minecraft:totem_of_undying",
         "minecraft:trader_llama_spawn_egg",
         "minecraft:trapped_chest",
         "minecraft:trident",
         "minecraft:tripwire_hook",
         "minecraft:tropical_fish",
         "minecraft:tropical_fish_bucket",
@@ -1055,26 +1152,29 @@
         "minecraft:tube_coral_fan",
         "minecraft:tuff",
         "minecraft:turtle_egg",
         "minecraft:turtle_helmet",
         "minecraft:turtle_spawn_egg",
         "minecraft:twisting_vines",
         "minecraft:verdant_froglight",
+        "minecraft:vex_armor_trim_smithing_template",
         "minecraft:vex_spawn_egg",
         "minecraft:villager_spawn_egg",
         "minecraft:vindicator_spawn_egg",
         "minecraft:vine",
         "minecraft:wandering_trader_spawn_egg",
+        "minecraft:ward_armor_trim_smithing_template",
         "minecraft:warden_spawn_egg",
         "minecraft:warped_button",
         "minecraft:warped_door",
         "minecraft:warped_fence",
         "minecraft:warped_fence_gate",
         "minecraft:warped_fungus",
         "minecraft:warped_fungus_on_a_stick",
+        "minecraft:warped_hanging_sign",
         "minecraft:warped_hyphae",
         "minecraft:warped_nylium",
         "minecraft:warped_planks",
         "minecraft:warped_pressure_plate",
         "minecraft:warped_roots",
         "minecraft:warped_sign",
         "minecraft:warped_slab",
@@ -1095,14 +1195,15 @@
         "minecraft:waxed_oxidized_cut_copper",
         "minecraft:waxed_oxidized_cut_copper_slab",
         "minecraft:waxed_oxidized_cut_copper_stairs",
         "minecraft:waxed_weathered_copper",
         "minecraft:waxed_weathered_cut_copper",
         "minecraft:waxed_weathered_cut_copper_slab",
         "minecraft:waxed_weathered_cut_copper_stairs",
+        "minecraft:wayfinder_armor_trim_smithing_template",
         "minecraft:weathered_copper",
         "minecraft:weathered_cut_copper",
         "minecraft:weathered_cut_copper_slab",
         "minecraft:weathered_cut_copper_stairs",
         "minecraft:weeping_vines",
         "minecraft:wet_sponge",
         "minecraft:wheat",
@@ -1117,18 +1218,20 @@
         "minecraft:white_glazed_terracotta",
         "minecraft:white_shulker_box",
         "minecraft:white_stained_glass",
         "minecraft:white_stained_glass_pane",
         "minecraft:white_terracotta",
         "minecraft:white_tulip",
         "minecraft:white_wool",
+        "minecraft:wild_armor_trim_smithing_template",
         "minecraft:witch_spawn_egg",
         "minecraft:wither_rose",
         "minecraft:wither_skeleton_skull",
         "minecraft:wither_skeleton_spawn_egg",
+        "minecraft:wither_spawn_egg",
         "minecraft:wolf_spawn_egg",
         "minecraft:wooden_axe",
         "minecraft:wooden_hoe",
         "minecraft:wooden_pickaxe",
         "minecraft:wooden_shovel",
         "minecraft:wooden_sword",
         "minecraft:writable_book",
```

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter/pack.png` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter/pack.png`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_1.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/0_1.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/100_101.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/100_101.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_103.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/102_103.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/104_104.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/104_104.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/105_106.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/105_106.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/107_108.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/107_108.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/109_110.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/109_110.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/111_112.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/111_112.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/113_114.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/113_114.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/115_116.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/115_116.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/117_118.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/117_118.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_120.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/119_120.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/11_12.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/11_12.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/121_121.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/121_121.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/122_123.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/122_123.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/124_125.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/124_125.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/126_127.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/126_127.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/128_129.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/128_129.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/130_131.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/130_131.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/132_133.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/132_133.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/134_135.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/134_135.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_137.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/136_137.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/139_140.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/139_140.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/13_14.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/13_14.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/141_142.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/141_142.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/143_144.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/143_144.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/145_146.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/145_146.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/147_148.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/147_148.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/149_150.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/149_150.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/151_152.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/151_152.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_154.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/153_154.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/155_155.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/155_155.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/156_157.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/156_157.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/158_159.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/158_159.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/15_16.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/15_16.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/160_161.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/160_161.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/162_163.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/162_163.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/164_165.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/164_165.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/166_167.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/166_167.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/168_169.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/168_169.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_171.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/170_171.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/172_172.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/172_172.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/173_174.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/173_174.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/175_176.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/175_176.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/177_178.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/177_178.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/179_180.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/179_180.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_18.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/17_18.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/181_182.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/181_182.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/183_184.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/183_184.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/185_186.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/185_186.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_188.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/187_188.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/189_189.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/189_189.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/190_191.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/190_191.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/192_193.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/192_193.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/194_195.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/194_195.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/196_197.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/196_197.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/198_199.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/198_199.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/19_19.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/19_19.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/200_201.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/200_201.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/202_203.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/202_203.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_205.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/204_205.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/207_208.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/207_208.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/209_210.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/209_210.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/20_21.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/20_21.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/211_212.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/211_212.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/213_214.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/213_214.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/215_216.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/215_216.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/217_218.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/217_218.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/219_220.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/219_220.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_222.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/221_222.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/224_225.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/224_225.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/226_227.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/226_227.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/228_229.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/228_229.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/22_23.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/22_23.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/230_231.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/230_231.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/232_233.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/232_233.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/234_235.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/234_235.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/236_237.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/236_237.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_239.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/238_239.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/240_240.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/240_240.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/241_242.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/241_242.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/243_244.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/243_244.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/245_246.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/245_246.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/247_248.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/247_248.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/249_250.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/249_250.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/24_25.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/24_25.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/251_252.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/251_252.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/253_254.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/253_254.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_256.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/255_256.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/258_259.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/258_259.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/260_261.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/260_261.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/262_263.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/262_263.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/264_265.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/264_265.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/266_267.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/266_267.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/268_269.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/268_269.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/26_27.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/26_27.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/270_271.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/270_271.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_273.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/272_273.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/274_274.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/274_274.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/275_276.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/275_276.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/277_278.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/277_278.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/279_280.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/279_280.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/281_282.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/281_282.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/283_284.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/283_284.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/285_286.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/285_286.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/287_288.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/287_288.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_290.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/289_290.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/28_29.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/28_29.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/291_291.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/291_291.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/292_293.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/292_293.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/294_295.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/294_295.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/296_297.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/296_297.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/298_299.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/298_299.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/2_2.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/2_2.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/300_301.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/300_301.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/302_303.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/302_303.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/304_305.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/304_305.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_307.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/306_307.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/309_310.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/309_310.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/30_31.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/30_31.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/311_312.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/311_312.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/313_314.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/313_314.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/315_316.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/315_316.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/317_318.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/317_318.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/319_320.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/319_320.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/321_322.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/321_322.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_324.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/323_324.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/325_325.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/325_325.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/326_327.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/326_327.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/328_329.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/328_329.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/32_33.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/32_33.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/330_331.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/330_331.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/332_333.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/332_333.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/334_335.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/334_335.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/336_337.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/336_337.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/338_339.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/338_339.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_341.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/340_341.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/342_342.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/342_342.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/343_344.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/343_344.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/345_346.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/345_346.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/347_348.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/347_348.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/349_350.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/349_350.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_35.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/34_35.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/351_352.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/351_352.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/353_354.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/353_354.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/355_356.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/355_356.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_358.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/357_358.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/359_359.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/359_359.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/360_361.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/360_361.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/362_363.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/362_363.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/364_365.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/364_365.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/366_367.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/366_367.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/368_369.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/368_369.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/370_371.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/370_371.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/372_373.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/372_373.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_375.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/374_375.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/376_376.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/376_376.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/377_378.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/377_378.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/379_380.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/379_380.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/37_38.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/37_38.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/381_382.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/381_382.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/383_384.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/383_384.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/385_386.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/385_386.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/387_388.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/387_388.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/389_390.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/389_390.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_392.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/391_392.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/393_393.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/393_393.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/394_395.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/394_395.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/396_397.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/396_397.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/398_399.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/398_399.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/39_40.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/39_40.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/3_4.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/3_4.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/400_401.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/400_401.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/402_403.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/402_403.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/404_405.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/404_405.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/406_407.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/406_407.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_409.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/408_409.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/410_410.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/410_410.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/411_412.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/411_412.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/413_414.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/413_414.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/415_416.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/415_416.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/417_418.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/417_418.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/419_420.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/419_420.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/41_42.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/41_42.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/421_422.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/421_422.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/423_424.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/423_424.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_426.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/425_426.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/427_427.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/427_427.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/428_429.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/428_429.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/430_431.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/430_431.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/432_433.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/432_433.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/434_435.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/434_435.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/436_437.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/436_437.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/438_439.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/438_439.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/43_44.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/43_44.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/440_441.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/440_441.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_443.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/442_443.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/445_446.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/445_446.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/447_448.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/447_448.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/449_450.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/449_450.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/451_452.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/451_452.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/453_454.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/453_454.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/455_456.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/455_456.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/457_458.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/457_458.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_460.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/459_460.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/45_46.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/45_46.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/462_463.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/462_463.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/464_465.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/464_465.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/466_467.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/466_467.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/468_469.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/468_469.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/470_471.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/470_471.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/472_473.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/472_473.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/474_475.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/474_475.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_477.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/476_477.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/478_478.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/478_478.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/479_480.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/479_480.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/47_48.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/47_48.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/481_482.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/481_482.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/483_484.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/483_484.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/485_486.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/485_486.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/487_488.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/487_488.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/489_490.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/489_490.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/491_492.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/491_492.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_494.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/493_494.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/495_495.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/495_495.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/496_497.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/496_497.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/498_499.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/498_499.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/49_50.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/49_50.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/500_501.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/500_501.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/502_503.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/502_503.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/504_505.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/504_505.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/506_507.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/506_507.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/508_509.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/508_509.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_511.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/510_511.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/512_512.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/512_512.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/513_514.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/513_514.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/515_516.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/515_516.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/517_518.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/517_518.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/519_520.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/519_520.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_52.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/51_52.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/521_522.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/521_522.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/523_524.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/523_524.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/525_526.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/525_526.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/527_528.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/527_528.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/529_530.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/529_530.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/531_532.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/531_532.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/533_534.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/533_534.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/535_536.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/535_536.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/537_538.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/537_538.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/539_540.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/539_540.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/53_53.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/53_53.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/541_542.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/541_542.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/54_55.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/54_55.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/56_57.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/56_57.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/58_59.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/58_59.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/5_6.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/5_6.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/60_61.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/60_61.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/62_63.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/62_63.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/64_65.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/64_65.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/66_67.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/66_67.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_69.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/68_69.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/71_72.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/71_72.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/73_74.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/73_74.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/75_76.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/75_76.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/77_78.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/77_78.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/79_80.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/79_80.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/7_8.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/7_8.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/81_82.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/81_82.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/83_84.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/83_84.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_86.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/85_86.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/88_89.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/88_89.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/90_91.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/90_91.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/92_93.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/92_93.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/94_95.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/94_95.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/96_97.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/96_97.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/98_99.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/98_99.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/9_10.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shaped/9_10.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_1.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/0_1.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/101_102.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/101_102.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/104_105.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/104_105.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/107_108.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/107_108.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/110_111.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/110_111.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/113_114.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/113_114.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_116.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/115_116.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/118_119.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/118_119.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/121_122.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/121_122.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/124_125.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/124_125.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/127_128.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/127_128.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/12_13.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/12_13.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/130_131.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/130_131.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/133_134.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/133_134.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/136_137.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/136_137.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_139.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/138_139.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/141_142.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/141_142.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/144_145.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/144_145.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/147_148.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/147_148.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/150_151.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/150_151.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/153_154.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/153_154.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/156_157.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/156_157.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/159_160.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/159_160.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/15_16.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/15_16.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_162.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/161_162.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/164_165.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/164_165.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/167_168.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/167_168.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/170_171.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/170_171.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/172_173.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/172_173.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/175_176.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/175_176.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/178_179.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/178_179.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/181_182.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/181_182.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/18_19.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/18_19.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/21_22.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/21_22.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_24.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/23_24.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/26_27.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/26_27.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/29_30.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/29_30.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/32_33.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/32_33.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/35_36.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/35_36.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/38_39.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/38_39.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/3_4.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/3_4.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/41_42.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/41_42.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/44_45.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/44_45.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_47.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/46_47.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/49_50.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/49_50.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/52_53.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/52_53.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/55_56.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/55_56.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/58_59.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/58_59.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/61_62.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/61_62.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/64_65.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/64_65.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/67_68.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/67_68.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_70.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/69_70.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/6_7.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/6_7.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/72_73.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/72_73.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/75_76.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/75_76.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/78_79.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/78_79.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/81_82.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/81_82.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/84_85.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/84_85.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/87_88.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/87_88.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/90_91.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/90_91.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_93.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/92_93.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/95_96.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/95_96.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/98_99.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/98_99.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/9_10.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/recipes/shapeless/9_10.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/tags/query.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/data/smithed.crafter_addon/functions/impl/tags/query.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/crafter-addon/pack.png` & `smithed_libraries-0.7.1/smithed_libraries/packs/crafter-addon/pack.png`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/advancements/impl/technical/place_custom_block.json` & `smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/advancements/impl/technical/place_custom_block.json`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place/layer.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place/layer.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/place.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/technical/def_const.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/technical/def_const.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/technical/load.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/data/smithed.custom_block/functions/impl/technical/load.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/custom-block/pack.png` & `smithed_libraries-0.7.1/smithed_libraries/packs/custom-block/pack.png`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/advancements/impl/player/event.json` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/advancements/impl/player/event.json`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/armor.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/armor.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/explosion.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/explosion.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/projectile.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply/projectile.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/apply.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/blast_protection.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/blast_protection.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/proj_protection.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/proj_protection.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/protection.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/protection.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/resistance.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/resistance.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/toughness.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/armor/toughness.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/give.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/give.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/remove.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/attributes/remove.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/death_message.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/death_message.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/update_entity.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/health/update_entity.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/on_death.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/entity/on_death.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/player/event.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/player/event.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/technical/def_const.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/data/smithed.damage/functions/impl/technical/def_const.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/damage/pack.png` & `smithed_libraries-0.7.1/smithed_libraries/packs/damage/pack.png`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_bookshelves.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_bookshelves.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_levels.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_levels.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_modified_level.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/get_modified_level.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/place.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/block/enchanter/place.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/binomial_random.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/technical/binomial_random.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/test.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/enchanter/data/smithed.enchanter/functions/impl/test.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_durability.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_durability.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_mending/clamp.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/calc_mending/clamp.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/force.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/damage/force.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/detect.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/detect.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/get_max.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/durability/get_max.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/attributes.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/attributes.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/base_attributes.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/base_attributes.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/build.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/build.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/custom.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/custom.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/enchantments.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/item/data/smithed.item/functions/impl/lore/enchantments.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/item/pack.png` & `smithed_libraries-0.7.1/smithed_libraries/packs/item/pack.png`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/prevent-aggression/data/smithed.prevent_aggression/functions/impl/technical/10_tick.mcfunction` & `smithed_libraries-0.7.1/smithed_libraries/packs/prevent-aggression/data/smithed.prevent_aggression/functions/impl/technical/10_tick.mcfunction`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/packs/prevent-aggression/pack.png` & `smithed_libraries-0.7.1/smithed_libraries/packs/prevent-aggression/pack.png`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/plugins/companion_mod.py` & `smithed_libraries-0.7.1/smithed_libraries/plugins/companion_mod.py`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/plugins/documentation.py` & `smithed_libraries-0.7.1/smithed_libraries/plugins/documentation.py`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/plugins/manifest.py` & `smithed_libraries-0.7.1/smithed_libraries/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/plugins/misc.py` & `smithed_libraries-0.7.1/smithed_libraries/plugins/misc.py`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/plugins/nbt_literals.py` & `smithed_libraries-0.7.1/smithed_libraries/plugins/nbt_literals.py`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/api.py` & `smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/api.py`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/load.py` & `smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/load.py`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/models.py` & `smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/models.py`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/smithed_libraries/plugins/versioning/plugin.py` & `smithed_libraries-0.7.1/smithed_libraries/plugins/versioning/plugin.py`

 * *Files identical despite different names*

### Comparing `smithed_libraries-0.7.0/setup.py` & `smithed_libraries-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
  'bolt-expressions>=0.12.2,<0.13.0',
  'bolt>=0.36.0,<0.37.0',
  'mecha>=0.73.0,<0.74.0',
  'pydantic>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'smithed-libraries',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'All of the Smithed Libraries',
     'long_description': '# Libraries\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Discord](https://img.shields.io/discord/511303648119226382?color=%236d82cc&label=Discord&logo=discord&logoColor=white)](https://discord.gg/gkp6UqEUph)\n\n> Collection of Libraries for the Smithed Ecosystem\n\n## Downloading\n\nYou can download it from [Stable](https://smithed.dev/libraries) | [Nightly](https://nightly.link/Smithed-MC/Libraries/workflows/nightly-build/main/packs.zip)<br/>\nor<br/>\nYou can build it from source using the [beet](https://github.com/mcbeet/beet) via the [Contributing](CONTRIBUTING.md) instructions.\n',
     'author': 'Smithed Council',
     'author_email': 'team@smithed.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `smithed_libraries-0.7.0/PKG-INFO` & `smithed_libraries-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smithed-libraries
-Version: 0.7.0
+Version: 0.7.1
 Summary: All of the Smithed Libraries
 License: MIT
 Author: Smithed Council
 Author-email: team@smithed.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

