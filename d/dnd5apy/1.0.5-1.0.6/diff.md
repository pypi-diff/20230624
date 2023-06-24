# Comparing `tmp/dnd5apy-1.0.5.tar.gz` & `tmp/dnd5apy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnd5apy-1.0.5.tar", max compression
+gzip compressed data, was "dnd5apy-1.0.6.tar", max compression
```

## Comparing `dnd5apy-1.0.5.tar` & `dnd5apy-1.0.6.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rwxr-xr-x   0        0        0    25494 2023-06-24 08:39:59.755627 dnd5apy-1.0.5/README.md
--rwxr-xr-x   0        0        0    15003 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/__init__.py
--rwxr-xr-x   0        0        0      892 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/api/__init__.py
--rwxr-xr-x   0        0        0    36882 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/character_data_api.py
--rwxr-xr-x   0        0        0    22406 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/class_api.py
--rwxr-xr-x   0        0        0    27898 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/class_levels_api.py
--rwxr-xr-x   0        0        0    25406 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/class_resource_lists_api.py
--rwxr-xr-x   0        0        0    17884 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/common_api.py
--rwxr-xr-x   0        0        0    26704 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/equipment_api.py
--rwxr-xr-x   0        0        0    14353 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/feats_api.py
--rwxr-xr-x   0        0        0    14976 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/features_api.py
--rwxr-xr-x   0        0        0    23195 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/game_mechanics_api.py
--rwxr-xr-x   0        0        0    17611 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/monsters_api.py
--rwxr-xr-x   0        0        0    25350 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/races_api.py
--rwxr-xr-x   0        0        0    18567 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/rules_api.py
--rwxr-xr-x   0        0        0    17972 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/spells_api.py
--rwxr-xr-x   0        0        0    30987 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/subclasses_api.py
--rwxr-xr-x   0        0        0    21777 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/subraces_api.py
--rwxr-xr-x   0        0        0    14126 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/traits_api.py
--rwxr-xr-x   0        0        0    34838 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api_client.py
--rwxr-xr-x   0        0        0    17789 2023-06-24 08:18:33.317241 dnd5apy-1.0.5/dnd5apy/configuration.py
--rwxr-xr-x   0        0        0    14060 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/__init__.py
--rwxr-xr-x   0        0        0    13741 2023-06-24 08:18:31.705233 dnd5apy-1.0.5/dnd5apy/models/ability_bonus.py
--rwxr-xr-x   0        0        0    14869 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/ability_score.py
--rwxr-xr-x   0        0        0    14127 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/alignment.py
--rwxr-xr-x   0        0        0    12663 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/all_of_prerequisite_ability_score.py
--rwxr-xr-x   0        0        0    12691 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/all_of_spellcasting_spellcasting_ability.py
--rwxr-xr-x   0        0        0    12302 2023-06-24 08:18:31.865234 dnd5apy-1.0.5/dnd5apy/models/any_of_class_level_class_specific.py
--rwxr-xr-x   0        0        0    14309 2023-06-24 08:18:31.601232 dnd5apy-1.0.5/dnd5apy/models/api_reference.py
--rwxr-xr-x   0        0        0    13687 2023-06-24 08:18:31.661233 dnd5apy-1.0.5/dnd5apy/models/api_reference_list.py
--rwxr-xr-x   0        0        0    13694 2023-06-24 08:18:31.889234 dnd5apy-1.0.5/dnd5apy/models/area_of_effect.py
--rwxr-xr-x   0        0        0    18897 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/armor.py
--rwxr-xr-x   0        0        0    20120 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/background.py
--rwxr-xr-x   0        0        0    13468 2023-06-24 08:18:31.961234 dnd5apy-1.0.5/dnd5apy/models/background_feature.py
--rwxr-xr-x   0        0        0    14869 2023-06-24 08:18:31.981234 dnd5apy-1.0.5/dnd5apy/models/choice.py
--rwxr-xr-x   0        0        0    18996 2023-06-24 08:18:31.997234 dnd5apy-1.0.5/dnd5apy/models/class_level.py
--rwxr-xr-x   0        0        0    13723 2023-06-24 08:18:32.017234 dnd5apy-1.0.5/dnd5apy/models/class_starting_equipment.py
--rwxr-xr-x   0        0        0    13266 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/condition.py
--rwxr-xr-x   0        0        0    13556 2023-06-24 08:18:32.065235 dnd5apy-1.0.5/dnd5apy/models/cost.py
--rwxr-xr-x   0        0        0    13625 2023-06-24 08:18:32.125235 dnd5apy-1.0.5/dnd5apy/models/damage.py
--rwxr-xr-x   0        0        0    14139 2023-06-24 08:18:32.149235 dnd5apy-1.0.5/dnd5apy/models/damage_at_character_level.py
--rwxr-xr-x   0        0        0    13979 2023-06-24 08:18:32.165235 dnd5apy-1.0.5/dnd5apy/models/damage_at_slot_level.py
--rwxr-xr-x   0        0        0    13274 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/damage_type.py
--rwxr-xr-x   0        0        0    14418 2023-06-24 08:18:32.093235 dnd5apy-1.0.5/dnd5apy/models/dc.py
--rwxr-xr-x   0        0        0    12226 2023-06-24 08:18:32.201235 dnd5apy-1.0.5/dnd5apy/models/equipment.py
--rwxr-xr-x   0        0        0    13509 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/equipment_category.py
--rwxr-xr-x   0        0        0    16392 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/equipment_pack.py
--rwxr-xr-x   0        0        0    12925 2023-06-24 08:18:32.257236 dnd5apy-1.0.5/dnd5apy/models/error_response.py
--rwxr-xr-x   0        0        0    14170 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/feat.py
--rwxr-xr-x   0        0        0    17695 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/feature.py
--rwxr-xr-x   0        0        0    16075 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/gear.py
--rwxr-xr-x   0        0        0    15771 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/language.py
--rwxr-xr-x   0        0        0    16207 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/magic_item.py
--rwxr-xr-x   0        0        0    13259 2023-06-24 08:18:32.361236 dnd5apy-1.0.5/dnd5apy/models/magic_item_rarity.py
--rwxr-xr-x   0        0        0    13276 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/magic_school.py
--rwxr-xr-x   0        0        0    22603 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/model_class.py
--rwxr-xr-x   0        0        0    41205 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/monster.py
--rwxr-xr-x   0        0        0    17204 2023-06-24 08:18:32.449237 dnd5apy-1.0.5/dnd5apy/models/monster_ability.py
--rwxr-xr-x   0        0        0    19007 2023-06-24 08:18:32.465237 dnd5apy-1.0.5/dnd5apy/models/monster_action.py
--rwxr-xr-x   0        0        0    12258 2023-06-24 08:18:32.481237 dnd5apy-1.0.5/dnd5apy/models/monster_armor_class.py
--rwxr-xr-x   0        0        0    13989 2023-06-24 08:18:32.493237 dnd5apy-1.0.5/dnd5apy/models/monster_attack.py
--rwxr-xr-x   0        0        0    14616 2023-06-24 08:18:32.505237 dnd5apy-1.0.5/dnd5apy/models/monster_multi_attack_action.py
--rwxr-xr-x   0        0        0    13655 2023-06-24 08:18:32.517237 dnd5apy-1.0.5/dnd5apy/models/monster_proficiency.py
--rwxr-xr-x   0        0        0    17751 2023-06-24 08:18:32.529237 dnd5apy-1.0.5/dnd5apy/models/monster_sense.py
--rwxr-xr-x   0        0        0    16990 2023-06-24 08:18:32.541237 dnd5apy-1.0.5/dnd5apy/models/monster_special_ability.py
--rwxr-xr-x   0        0        0    16745 2023-06-24 08:18:32.557237 dnd5apy-1.0.5/dnd5apy/models/monster_speed.py
--rwxr-xr-x   0        0        0    14597 2023-06-24 08:18:32.569237 dnd5apy-1.0.5/dnd5apy/models/monster_spell.py
--rwxr-xr-x   0        0        0    17140 2023-06-24 08:18:32.581237 dnd5apy-1.0.5/dnd5apy/models/monster_spellcasting.py
--rwxr-xr-x   0        0        0    14448 2023-06-24 08:18:32.593237 dnd5apy-1.0.5/dnd5apy/models/monster_usage.py
--rwxr-xr-x   0        0        0    16276 2023-06-24 08:18:32.601237 dnd5apy-1.0.5/dnd5apy/models/multiclassing.py
--rwxr-xr-x   0        0        0    12214 2023-06-24 08:18:32.613237 dnd5apy-1.0.5/dnd5apy/models/option.py
--rwxr-xr-x   0        0        0    12226 2023-06-24 08:18:32.625238 dnd5apy-1.0.5/dnd5apy/models/option_set.py
--rwxr-xr-x   0        0        0    13958 2023-06-24 08:18:32.633237 dnd5apy-1.0.5/dnd5apy/models/prerequisite.py
--rwxr-xr-x   0        0        0    15712 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/proficiency.py
--rwxr-xr-x   0        0        0    22707 2023-06-24 08:38:46.131261 dnd5apy-1.0.5/dnd5apy/models/race.py
--rwxr-xr-x   0        0        0    12989 2023-06-24 08:18:32.677238 dnd5apy-1.0.5/dnd5apy/models/resource_description.py
--rwxr-xr-x   0        0        0    14112 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/rule.py
--rwxr-xr-x   0        0        0    13256 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/rule_section.py
--rwxr-xr-x   0        0        0    13990 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/skill.py
--rwxr-xr-x   0        0        0    25243 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/spell.py
--rwxr-xr-x   0        0        0    13306 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/spell_prerequisite.py
--rwxr-xr-x   0        0        0    14977 2023-06-24 08:18:32.753238 dnd5apy-1.0.5/dnd5apy/models/spellcasting.py
--rwxr-xr-x   0        0        0    13614 2023-06-24 08:18:32.765238 dnd5apy-1.0.5/dnd5apy/models/spellcasting_info.py
--rwxr-xr-x   0        0        0    16421 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/subclass.py
--rwxr-xr-x   0        0        0    19031 2023-06-24 08:18:32.785238 dnd5apy-1.0.5/dnd5apy/models/subclass_level.py
--rwxr-xr-x   0        0        0    16274 2023-06-24 08:18:32.793238 dnd5apy-1.0.5/dnd5apy/models/subclass_level_resource.py
--rwxr-xr-x   0        0        0    22333 2023-06-24 08:18:32.805238 dnd5apy-1.0.5/dnd5apy/models/subclass_level_spellcasting.py
--rwxr-xr-x   0        0        0    13701 2023-06-24 08:18:32.813238 dnd5apy-1.0.5/dnd5apy/models/subclass_spells.py
--rwxr-xr-x   0        0        0    18550 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/subrace.py
--rwxr-xr-x   0        0        0    18236 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/trait.py
--rwxr-xr-x   0        0        0    20867 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/weapon.py
--rwxr-xr-x   0        0        0    13306 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/weapon_property.py
--rwxr-xr-x   0        0        0    13654 2023-06-24 08:18:32.861239 dnd5apy-1.0.5/dnd5apy/models/weapon_range.py
--rwxr-xr-x   0        0        0    22818 2023-06-24 08:18:33.345241 dnd5apy-1.0.5/dnd5apy/rest.py
--rwxr-xr-x   0        0        0      691 2023-06-24 08:42:10.180274 dnd5apy-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    26368 1970-01-01 00:00:00.000000 dnd5apy-1.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0    25494 2023-06-24 08:39:59.755627 dnd5apy-1.0.6/README.md
+-rwxr-xr-x   0        0        0    15003 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/__init__.py
+-rwxr-xr-x   0        0        0      892 2023-06-24 08:38:46.123261 dnd5apy-1.0.6/dnd5apy/api/__init__.py
+-rwxr-xr-x   0        0        0    36882 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/character_data_api.py
+-rwxr-xr-x   0        0        0    22406 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/class_api.py
+-rwxr-xr-x   0        0        0    27898 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/class_levels_api.py
+-rwxr-xr-x   0        0        0    25406 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/class_resource_lists_api.py
+-rwxr-xr-x   0        0        0    17884 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/common_api.py
+-rwxr-xr-x   0        0        0    26704 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/equipment_api.py
+-rwxr-xr-x   0        0        0    14353 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/feats_api.py
+-rwxr-xr-x   0        0        0    14976 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/features_api.py
+-rwxr-xr-x   0        0        0    23195 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/game_mechanics_api.py
+-rwxr-xr-x   0        0        0    17611 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/monsters_api.py
+-rwxr-xr-x   0        0        0    25350 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/races_api.py
+-rwxr-xr-x   0        0        0    18567 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/rules_api.py
+-rwxr-xr-x   0        0        0    17972 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/spells_api.py
+-rwxr-xr-x   0        0        0    30987 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/subclasses_api.py
+-rwxr-xr-x   0        0        0    21777 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/subraces_api.py
+-rwxr-xr-x   0        0        0    14126 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api/traits_api.py
+-rwxr-xr-x   0        0        0    34838 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/api_client.py
+-rwxr-xr-x   0        0        0    17789 2023-06-24 08:18:33.317241 dnd5apy-1.0.6/dnd5apy/configuration.py
+-rwxr-xr-x   0        0        0    14060 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/__init__.py
+-rwxr-xr-x   0        0        0    13741 2023-06-24 08:18:31.705233 dnd5apy-1.0.6/dnd5apy/models/ability_bonus.py
+-rwxr-xr-x   0        0        0    14869 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/ability_score.py
+-rwxr-xr-x   0        0        0    14127 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/alignment.py
+-rwxr-xr-x   0        0        0    12663 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/all_of_prerequisite_ability_score.py
+-rwxr-xr-x   0        0        0    12691 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/all_of_spellcasting_spellcasting_ability.py
+-rwxr-xr-x   0        0        0    12302 2023-06-24 08:18:31.865234 dnd5apy-1.0.6/dnd5apy/models/any_of_class_level_class_specific.py
+-rwxr-xr-x   0        0        0    14309 2023-06-24 08:18:31.601232 dnd5apy-1.0.6/dnd5apy/models/api_reference.py
+-rwxr-xr-x   0        0        0    13687 2023-06-24 08:18:31.661233 dnd5apy-1.0.6/dnd5apy/models/api_reference_list.py
+-rwxr-xr-x   0        0        0    13694 2023-06-24 08:18:31.889234 dnd5apy-1.0.6/dnd5apy/models/area_of_effect.py
+-rwxr-xr-x   0        0        0    18897 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/armor.py
+-rwxr-xr-x   0        0        0    20120 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/background.py
+-rwxr-xr-x   0        0        0    13468 2023-06-24 08:18:31.961234 dnd5apy-1.0.6/dnd5apy/models/background_feature.py
+-rwxr-xr-x   0        0        0    14869 2023-06-24 08:18:31.981234 dnd5apy-1.0.6/dnd5apy/models/choice.py
+-rwxr-xr-x   0        0        0    18996 2023-06-24 08:18:31.997234 dnd5apy-1.0.6/dnd5apy/models/class_level.py
+-rwxr-xr-x   0        0        0    13723 2023-06-24 08:18:32.017234 dnd5apy-1.0.6/dnd5apy/models/class_starting_equipment.py
+-rwxr-xr-x   0        0        0    13266 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/condition.py
+-rwxr-xr-x   0        0        0    13556 2023-06-24 08:18:32.065235 dnd5apy-1.0.6/dnd5apy/models/cost.py
+-rwxr-xr-x   0        0        0    13625 2023-06-24 08:18:32.125235 dnd5apy-1.0.6/dnd5apy/models/damage.py
+-rwxr-xr-x   0        0        0    14139 2023-06-24 08:18:32.149235 dnd5apy-1.0.6/dnd5apy/models/damage_at_character_level.py
+-rwxr-xr-x   0        0        0    13979 2023-06-24 08:18:32.165235 dnd5apy-1.0.6/dnd5apy/models/damage_at_slot_level.py
+-rwxr-xr-x   0        0        0    13274 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/damage_type.py
+-rwxr-xr-x   0        0        0    14418 2023-06-24 08:18:32.093235 dnd5apy-1.0.6/dnd5apy/models/dc.py
+-rwxr-xr-x   0        0        0    12226 2023-06-24 08:18:32.201235 dnd5apy-1.0.6/dnd5apy/models/equipment.py
+-rwxr-xr-x   0        0        0    13509 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/equipment_category.py
+-rwxr-xr-x   0        0        0    16392 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/equipment_pack.py
+-rwxr-xr-x   0        0        0    12925 2023-06-24 08:18:32.257236 dnd5apy-1.0.6/dnd5apy/models/error_response.py
+-rwxr-xr-x   0        0        0    14170 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/feat.py
+-rwxr-xr-x   0        0        0    17695 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/feature.py
+-rwxr-xr-x   0        0        0    16075 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/gear.py
+-rwxr-xr-x   0        0        0    15771 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/language.py
+-rwxr-xr-x   0        0        0    16207 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/magic_item.py
+-rwxr-xr-x   0        0        0    13259 2023-06-24 08:18:32.361236 dnd5apy-1.0.6/dnd5apy/models/magic_item_rarity.py
+-rwxr-xr-x   0        0        0    13276 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/magic_school.py
+-rwxr-xr-x   0        0        0    22603 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/model_class.py
+-rwxr-xr-x   0        0        0    41205 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/monster.py
+-rwxr-xr-x   0        0        0    17204 2023-06-24 08:18:32.449237 dnd5apy-1.0.6/dnd5apy/models/monster_ability.py
+-rwxr-xr-x   0        0        0    19007 2023-06-24 08:18:32.465237 dnd5apy-1.0.6/dnd5apy/models/monster_action.py
+-rwxr-xr-x   0        0        0    12258 2023-06-24 08:18:32.481237 dnd5apy-1.0.6/dnd5apy/models/monster_armor_class.py
+-rwxr-xr-x   0        0        0    13989 2023-06-24 08:18:32.493237 dnd5apy-1.0.6/dnd5apy/models/monster_attack.py
+-rwxr-xr-x   0        0        0    14616 2023-06-24 08:18:32.505237 dnd5apy-1.0.6/dnd5apy/models/monster_multi_attack_action.py
+-rwxr-xr-x   0        0        0    13655 2023-06-24 08:18:32.517237 dnd5apy-1.0.6/dnd5apy/models/monster_proficiency.py
+-rwxr-xr-x   0        0        0    17751 2023-06-24 08:18:32.529237 dnd5apy-1.0.6/dnd5apy/models/monster_sense.py
+-rwxr-xr-x   0        0        0    16990 2023-06-24 08:18:32.541237 dnd5apy-1.0.6/dnd5apy/models/monster_special_ability.py
+-rwxr-xr-x   0        0        0    16745 2023-06-24 08:18:32.557237 dnd5apy-1.0.6/dnd5apy/models/monster_speed.py
+-rwxr-xr-x   0        0        0    14597 2023-06-24 08:18:32.569237 dnd5apy-1.0.6/dnd5apy/models/monster_spell.py
+-rwxr-xr-x   0        0        0    17140 2023-06-24 08:18:32.581237 dnd5apy-1.0.6/dnd5apy/models/monster_spellcasting.py
+-rwxr-xr-x   0        0        0    14448 2023-06-24 08:18:32.593237 dnd5apy-1.0.6/dnd5apy/models/monster_usage.py
+-rwxr-xr-x   0        0        0    16276 2023-06-24 08:18:32.601237 dnd5apy-1.0.6/dnd5apy/models/multiclassing.py
+-rwxr-xr-x   0        0        0    12214 2023-06-24 08:18:32.613237 dnd5apy-1.0.6/dnd5apy/models/option.py
+-rwxr-xr-x   0        0        0    12226 2023-06-24 08:18:32.625238 dnd5apy-1.0.6/dnd5apy/models/option_set.py
+-rwxr-xr-x   0        0        0    13958 2023-06-24 08:18:32.633237 dnd5apy-1.0.6/dnd5apy/models/prerequisite.py
+-rwxr-xr-x   0        0        0    15712 2023-06-24 08:38:46.139261 dnd5apy-1.0.6/dnd5apy/models/proficiency.py
+-rwxr-xr-x   0        0        0    22707 2023-06-24 08:38:46.131261 dnd5apy-1.0.6/dnd5apy/models/race.py
+-rwxr-xr-x   0        0        0    12989 2023-06-24 08:18:32.677238 dnd5apy-1.0.6/dnd5apy/models/resource_description.py
+-rwxr-xr-x   0        0        0    14112 2023-06-24 08:38:46.123261 dnd5apy-1.0.6/dnd5apy/models/rule.py
+-rwxr-xr-x   0        0        0    13256 2023-06-24 08:38:46.123261 dnd5apy-1.0.6/dnd5apy/models/rule_section.py
+-rwxr-xr-x   0        0        0    13990 2023-06-24 08:38:46.123261 dnd5apy-1.0.6/dnd5apy/models/skill.py
+-rwxr-xr-x   0        0        0    25243 2023-06-24 08:38:46.123261 dnd5apy-1.0.6/dnd5apy/models/spell.py
+-rwxr-xr-x   0        0        0    13306 2023-06-24 08:38:46.123261 dnd5apy-1.0.6/dnd5apy/models/spell_prerequisite.py
+-rwxr-xr-x   0        0        0    14977 2023-06-24 08:18:32.753238 dnd5apy-1.0.6/dnd5apy/models/spellcasting.py
+-rwxr-xr-x   0        0        0    13614 2023-06-24 08:18:32.765238 dnd5apy-1.0.6/dnd5apy/models/spellcasting_info.py
+-rwxr-xr-x   0        0        0    16421 2023-06-24 08:38:46.123261 dnd5apy-1.0.6/dnd5apy/models/subclass.py
+-rwxr-xr-x   0        0        0    19031 2023-06-24 08:18:32.785238 dnd5apy-1.0.6/dnd5apy/models/subclass_level.py
+-rwxr-xr-x   0        0        0    16274 2023-06-24 08:18:32.793238 dnd5apy-1.0.6/dnd5apy/models/subclass_level_resource.py
+-rwxr-xr-x   0        0        0    22333 2023-06-24 08:18:32.805238 dnd5apy-1.0.6/dnd5apy/models/subclass_level_spellcasting.py
+-rwxr-xr-x   0        0        0    13701 2023-06-24 08:18:32.813238 dnd5apy-1.0.6/dnd5apy/models/subclass_spells.py
+-rwxr-xr-x   0        0        0    18550 2023-06-24 08:38:46.123261 dnd5apy-1.0.6/dnd5apy/models/subrace.py
+-rwxr-xr-x   0        0        0    18236 2023-06-24 08:38:46.123261 dnd5apy-1.0.6/dnd5apy/models/trait.py
+-rwxr-xr-x   0        0        0    20867 2023-06-24 08:38:46.123261 dnd5apy-1.0.6/dnd5apy/models/weapon.py
+-rwxr-xr-x   0        0        0    13306 2023-06-24 08:38:46.123261 dnd5apy-1.0.6/dnd5apy/models/weapon_property.py
+-rwxr-xr-x   0        0        0    13654 2023-06-24 08:18:32.861239 dnd5apy-1.0.6/dnd5apy/models/weapon_range.py
+-rwxr-xr-x   0        0        0    22818 2023-06-24 08:18:33.345241 dnd5apy-1.0.6/dnd5apy/rest.py
+-rwxr-xr-x   0        0        0      691 2023-06-24 09:07:11.618164 dnd5apy-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    26368 1970-01-01 00:00:00.000000 dnd5apy-1.0.6/PKG-INFO
```

### Comparing `dnd5apy-1.0.5/README.md` & `dnd5apy-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/__init__.py` & `dnd5apy-1.0.6/dnd5apy/__init__.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/__init__.py` & `dnd5apy-1.0.6/dnd5apy/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/character_data_api.py` & `dnd5apy-1.0.6/dnd5apy/api/character_data_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/class_api.py` & `dnd5apy-1.0.6/dnd5apy/api/class_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/class_levels_api.py` & `dnd5apy-1.0.6/dnd5apy/api/class_levels_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/class_resource_lists_api.py` & `dnd5apy-1.0.6/dnd5apy/api/class_resource_lists_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/common_api.py` & `dnd5apy-1.0.6/dnd5apy/api/common_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/equipment_api.py` & `dnd5apy-1.0.6/dnd5apy/api/equipment_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/feats_api.py` & `dnd5apy-1.0.6/dnd5apy/api/feats_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/features_api.py` & `dnd5apy-1.0.6/dnd5apy/api/features_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/game_mechanics_api.py` & `dnd5apy-1.0.6/dnd5apy/api/game_mechanics_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/monsters_api.py` & `dnd5apy-1.0.6/dnd5apy/api/monsters_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/races_api.py` & `dnd5apy-1.0.6/dnd5apy/api/races_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/rules_api.py` & `dnd5apy-1.0.6/dnd5apy/api/rules_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/spells_api.py` & `dnd5apy-1.0.6/dnd5apy/api/spells_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/subclasses_api.py` & `dnd5apy-1.0.6/dnd5apy/api/subclasses_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/subraces_api.py` & `dnd5apy-1.0.6/dnd5apy/api/subraces_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api/traits_api.py` & `dnd5apy-1.0.6/dnd5apy/api/traits_api.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/api_client.py` & `dnd5apy-1.0.6/dnd5apy/api_client.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/configuration.py` & `dnd5apy-1.0.6/dnd5apy/configuration.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/__init__.py` & `dnd5apy-1.0.6/dnd5apy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/ability_bonus.py` & `dnd5apy-1.0.6/dnd5apy/models/ability_bonus.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/ability_score.py` & `dnd5apy-1.0.6/dnd5apy/models/ability_score.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/alignment.py` & `dnd5apy-1.0.6/dnd5apy/models/alignment.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/all_of_prerequisite_ability_score.py` & `dnd5apy-1.0.6/dnd5apy/models/all_of_prerequisite_ability_score.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/all_of_spellcasting_spellcasting_ability.py` & `dnd5apy-1.0.6/dnd5apy/models/all_of_spellcasting_spellcasting_ability.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/any_of_class_level_class_specific.py` & `dnd5apy-1.0.6/dnd5apy/models/any_of_class_level_class_specific.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/api_reference.py` & `dnd5apy-1.0.6/dnd5apy/models/api_reference.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/api_reference_list.py` & `dnd5apy-1.0.6/dnd5apy/models/api_reference_list.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/area_of_effect.py` & `dnd5apy-1.0.6/dnd5apy/models/area_of_effect.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/armor.py` & `dnd5apy-1.0.6/dnd5apy/models/armor.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/background.py` & `dnd5apy-1.0.6/dnd5apy/models/background.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/background_feature.py` & `dnd5apy-1.0.6/dnd5apy/models/background_feature.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/choice.py` & `dnd5apy-1.0.6/dnd5apy/models/choice.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/class_level.py` & `dnd5apy-1.0.6/dnd5apy/models/class_level.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/class_starting_equipment.py` & `dnd5apy-1.0.6/dnd5apy/models/class_starting_equipment.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/condition.py` & `dnd5apy-1.0.6/dnd5apy/models/condition.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/cost.py` & `dnd5apy-1.0.6/dnd5apy/models/cost.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/damage.py` & `dnd5apy-1.0.6/dnd5apy/models/damage.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/damage_at_character_level.py` & `dnd5apy-1.0.6/dnd5apy/models/damage_at_character_level.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/damage_at_slot_level.py` & `dnd5apy-1.0.6/dnd5apy/models/damage_at_slot_level.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/damage_type.py` & `dnd5apy-1.0.6/dnd5apy/models/damage_type.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/dc.py` & `dnd5apy-1.0.6/dnd5apy/models/dc.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/equipment.py` & `dnd5apy-1.0.6/dnd5apy/models/equipment.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/equipment_category.py` & `dnd5apy-1.0.6/dnd5apy/models/equipment_category.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/equipment_pack.py` & `dnd5apy-1.0.6/dnd5apy/models/equipment_pack.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/error_response.py` & `dnd5apy-1.0.6/dnd5apy/models/error_response.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/feat.py` & `dnd5apy-1.0.6/dnd5apy/models/feat.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/feature.py` & `dnd5apy-1.0.6/dnd5apy/models/feature.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/gear.py` & `dnd5apy-1.0.6/dnd5apy/models/gear.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/language.py` & `dnd5apy-1.0.6/dnd5apy/models/language.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/magic_item.py` & `dnd5apy-1.0.6/dnd5apy/models/magic_item.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/magic_item_rarity.py` & `dnd5apy-1.0.6/dnd5apy/models/magic_item_rarity.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/magic_school.py` & `dnd5apy-1.0.6/dnd5apy/models/magic_school.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/model_class.py` & `dnd5apy-1.0.6/dnd5apy/models/model_class.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster.py` & `dnd5apy-1.0.6/dnd5apy/models/monster.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_ability.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_ability.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_action.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_action.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_armor_class.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_armor_class.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_attack.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_attack.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_multi_attack_action.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_multi_attack_action.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_proficiency.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_proficiency.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_sense.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_sense.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_special_ability.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_special_ability.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_speed.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_speed.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_spell.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_spell.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_spellcasting.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_spellcasting.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/monster_usage.py` & `dnd5apy-1.0.6/dnd5apy/models/monster_usage.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/multiclassing.py` & `dnd5apy-1.0.6/dnd5apy/models/multiclassing.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/option.py` & `dnd5apy-1.0.6/dnd5apy/models/option.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/option_set.py` & `dnd5apy-1.0.6/dnd5apy/models/option_set.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/prerequisite.py` & `dnd5apy-1.0.6/dnd5apy/models/prerequisite.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/proficiency.py` & `dnd5apy-1.0.6/dnd5apy/models/proficiency.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/race.py` & `dnd5apy-1.0.6/dnd5apy/models/race.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/resource_description.py` & `dnd5apy-1.0.6/dnd5apy/models/resource_description.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/rule.py` & `dnd5apy-1.0.6/dnd5apy/models/rule.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/rule_section.py` & `dnd5apy-1.0.6/dnd5apy/models/rule_section.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/skill.py` & `dnd5apy-1.0.6/dnd5apy/models/skill.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/spell.py` & `dnd5apy-1.0.6/dnd5apy/models/spell.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/spell_prerequisite.py` & `dnd5apy-1.0.6/dnd5apy/models/spell_prerequisite.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/spellcasting.py` & `dnd5apy-1.0.6/dnd5apy/models/spellcasting.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/spellcasting_info.py` & `dnd5apy-1.0.6/dnd5apy/models/spellcasting_info.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/subclass.py` & `dnd5apy-1.0.6/dnd5apy/models/subclass.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/subclass_level.py` & `dnd5apy-1.0.6/dnd5apy/models/subclass_level.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/subclass_level_resource.py` & `dnd5apy-1.0.6/dnd5apy/models/subclass_level_resource.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/subclass_level_spellcasting.py` & `dnd5apy-1.0.6/dnd5apy/models/subclass_level_spellcasting.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/subclass_spells.py` & `dnd5apy-1.0.6/dnd5apy/models/subclass_spells.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/subrace.py` & `dnd5apy-1.0.6/dnd5apy/models/subrace.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/trait.py` & `dnd5apy-1.0.6/dnd5apy/models/trait.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/weapon.py` & `dnd5apy-1.0.6/dnd5apy/models/weapon.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/weapon_property.py` & `dnd5apy-1.0.6/dnd5apy/models/weapon_property.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/models/weapon_range.py` & `dnd5apy-1.0.6/dnd5apy/models/weapon_range.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/dnd5apy/rest.py` & `dnd5apy-1.0.6/dnd5apy/rest.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.5/pyproject.toml` & `dnd5apy-1.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dnd5apy"
-version = "1.0.5"
+version = "1.0.6"
 description = "D&D 5e API"
 authors = ["5eBits <team@openapitools.org>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "D&D 5e API"]
 include = ["dnd5epy/py.typed"]
```

### Comparing `dnd5apy-1.0.5/PKG-INFO` & `dnd5apy-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnd5apy
-Version: 1.0.5
+Version: 1.0.6
 Summary: D&D 5e API
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,D&D 5e API
 Author: 5eBits
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
```

