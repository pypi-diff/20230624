# Comparing `tmp/dnd5apy-1.0.4.tar.gz` & `tmp/dnd5apy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnd5apy-1.0.4.tar", max compression
+gzip compressed data, was "dnd5apy-1.0.5.tar", max compression
```

## Comparing `dnd5apy-1.0.4.tar` & `dnd5apy-1.0.5.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rwxr-xr-x   0        0        0    25501 2023-06-24 08:18:33.313241 dnd5apy-1.0.4/README.md
--rwxr-xr-x   0        0        0    15626 2023-06-24 08:18:33.321241 dnd5apy-1.0.4/dnd5apy/__init__.py
--rwxr-xr-x   0        0        0     1004 2023-06-24 08:18:33.337241 dnd5apy-1.0.4/dnd5apy/api/__init__.py
--rwxr-xr-x   0        0        0    36889 2023-06-24 08:18:33.005239 dnd5apy-1.0.4/dnd5apy/api/character_data_api.py
--rwxr-xr-x   0        0        0    22413 2023-06-24 08:18:33.029240 dnd5apy-1.0.4/dnd5apy/api/class_api.py
--rwxr-xr-x   0        0        0    27905 2023-06-24 08:18:33.053240 dnd5apy-1.0.4/dnd5apy/api/class_levels_api.py
--rwxr-xr-x   0        0        0    25413 2023-06-24 08:18:33.073240 dnd5apy-1.0.4/dnd5apy/api/class_resource_lists_api.py
--rwxr-xr-x   0        0        0    17891 2023-06-24 08:18:33.089240 dnd5apy-1.0.4/dnd5apy/api/common_api.py
--rwxr-xr-x   0        0        0    26711 2023-06-24 08:18:33.109240 dnd5apy-1.0.4/dnd5apy/api/equipment_api.py
--rwxr-xr-x   0        0        0    14360 2023-06-24 08:18:33.121240 dnd5apy-1.0.4/dnd5apy/api/feats_api.py
--rwxr-xr-x   0        0        0    14983 2023-06-24 08:18:33.137240 dnd5apy-1.0.4/dnd5apy/api/features_api.py
--rwxr-xr-x   0        0        0    23202 2023-06-24 08:18:33.157240 dnd5apy-1.0.4/dnd5apy/api/game_mechanics_api.py
--rwxr-xr-x   0        0        0    17618 2023-06-24 08:18:33.169240 dnd5apy-1.0.4/dnd5apy/api/monsters_api.py
--rwxr-xr-x   0        0        0    25357 2023-06-24 08:18:33.185240 dnd5apy-1.0.4/dnd5apy/api/races_api.py
--rwxr-xr-x   0        0        0    18574 2023-06-24 08:18:33.205240 dnd5apy-1.0.4/dnd5apy/api/rules_api.py
--rwxr-xr-x   0        0        0    17979 2023-06-24 08:18:33.229241 dnd5apy-1.0.4/dnd5apy/api/spells_api.py
--rwxr-xr-x   0        0        0    30994 2023-06-24 08:18:33.249241 dnd5apy-1.0.4/dnd5apy/api/subclasses_api.py
--rwxr-xr-x   0        0        0    21784 2023-06-24 08:18:33.273241 dnd5apy-1.0.4/dnd5apy/api/subraces_api.py
--rwxr-xr-x   0        0        0    14133 2023-06-24 08:18:33.293241 dnd5apy-1.0.4/dnd5apy/api/traits_api.py
--rwxr-xr-x   0        0        0    34866 2023-06-24 08:18:33.345241 dnd5apy-1.0.4/dnd5apy/api_client.py
--rwxr-xr-x   0        0        0    17789 2023-06-24 08:18:33.317241 dnd5apy-1.0.4/dnd5apy/configuration.py
--rwxr-xr-x   0        0        0    14557 2023-06-24 08:18:33.333241 dnd5apy-1.0.4/dnd5apy/models/__init__.py
--rwxr-xr-x   0        0        0    13741 2023-06-24 08:18:31.705233 dnd5apy-1.0.4/dnd5apy/models/ability_bonus.py
--rwxr-xr-x   0        0        0    14876 2023-06-24 08:18:31.745233 dnd5apy-1.0.4/dnd5apy/models/ability_score.py
--rwxr-xr-x   0        0        0    14134 2023-06-24 08:18:31.777233 dnd5apy-1.0.4/dnd5apy/models/alignment.py
--rwxr-xr-x   0        0        0    12670 2023-06-24 08:18:31.809234 dnd5apy-1.0.4/dnd5apy/models/all_of_prerequisite_ability_score.py
--rwxr-xr-x   0        0        0    12698 2023-06-24 08:18:31.837234 dnd5apy-1.0.4/dnd5apy/models/all_of_spellcasting_spellcasting_ability.py
--rwxr-xr-x   0        0        0    12302 2023-06-24 08:18:31.865234 dnd5apy-1.0.4/dnd5apy/models/any_of_class_level_class_specific.py
--rwxr-xr-x   0        0        0    14309 2023-06-24 08:18:31.601232 dnd5apy-1.0.4/dnd5apy/models/api_reference.py
--rwxr-xr-x   0        0        0    13687 2023-06-24 08:18:31.661233 dnd5apy-1.0.4/dnd5apy/models/api_reference_list.py
--rwxr-xr-x   0        0        0    13694 2023-06-24 08:18:31.889234 dnd5apy-1.0.4/dnd5apy/models/area_of_effect.py
--rwxr-xr-x   0        0        0    18904 2023-06-24 08:18:31.913234 dnd5apy-1.0.4/dnd5apy/models/armor.py
--rwxr-xr-x   0        0        0    20127 2023-06-24 08:18:31.941234 dnd5apy-1.0.4/dnd5apy/models/background.py
--rwxr-xr-x   0        0        0    13468 2023-06-24 08:18:31.961234 dnd5apy-1.0.4/dnd5apy/models/background_feature.py
--rwxr-xr-x   0        0        0    14869 2023-06-24 08:18:31.981234 dnd5apy-1.0.4/dnd5apy/models/choice.py
--rwxr-xr-x   0        0        0    18996 2023-06-24 08:18:31.997234 dnd5apy-1.0.4/dnd5apy/models/class_level.py
--rwxr-xr-x   0        0        0    13723 2023-06-24 08:18:32.017234 dnd5apy-1.0.4/dnd5apy/models/class_starting_equipment.py
--rwxr-xr-x   0        0        0    13273 2023-06-24 08:18:32.045235 dnd5apy-1.0.4/dnd5apy/models/condition.py
--rwxr-xr-x   0        0        0    13556 2023-06-24 08:18:32.065235 dnd5apy-1.0.4/dnd5apy/models/cost.py
--rwxr-xr-x   0        0        0    13625 2023-06-24 08:18:32.125235 dnd5apy-1.0.4/dnd5apy/models/damage.py
--rwxr-xr-x   0        0        0    14139 2023-06-24 08:18:32.149235 dnd5apy-1.0.4/dnd5apy/models/damage_at_character_level.py
--rwxr-xr-x   0        0        0    13979 2023-06-24 08:18:32.165235 dnd5apy-1.0.4/dnd5apy/models/damage_at_slot_level.py
--rwxr-xr-x   0        0        0    13281 2023-06-24 08:18:32.181235 dnd5apy-1.0.4/dnd5apy/models/damage_type.py
--rwxr-xr-x   0        0        0    14418 2023-06-24 08:18:32.093235 dnd5apy-1.0.4/dnd5apy/models/dc.py
--rwxr-xr-x   0        0        0    12226 2023-06-24 08:18:32.201235 dnd5apy-1.0.4/dnd5apy/models/equipment.py
--rwxr-xr-x   0        0        0    13516 2023-06-24 08:18:32.221236 dnd5apy-1.0.4/dnd5apy/models/equipment_category.py
--rwxr-xr-x   0        0        0    16399 2023-06-24 08:18:32.241236 dnd5apy-1.0.4/dnd5apy/models/equipment_pack.py
--rwxr-xr-x   0        0        0    12925 2023-06-24 08:18:32.257236 dnd5apy-1.0.4/dnd5apy/models/error_response.py
--rwxr-xr-x   0        0        0    14177 2023-06-24 08:18:32.277236 dnd5apy-1.0.4/dnd5apy/models/feat.py
--rwxr-xr-x   0        0        0    17702 2023-06-24 08:18:32.293236 dnd5apy-1.0.4/dnd5apy/models/feature.py
--rwxr-xr-x   0        0        0    16082 2023-06-24 08:18:32.309236 dnd5apy-1.0.4/dnd5apy/models/gear.py
--rwxr-xr-x   0        0        0    15778 2023-06-24 08:18:32.329236 dnd5apy-1.0.4/dnd5apy/models/language.py
--rwxr-xr-x   0        0        0    16214 2023-06-24 08:18:32.345236 dnd5apy-1.0.4/dnd5apy/models/magic_item.py
--rwxr-xr-x   0        0        0    13259 2023-06-24 08:18:32.361236 dnd5apy-1.0.4/dnd5apy/models/magic_item_rarity.py
--rwxr-xr-x   0        0        0    13283 2023-06-24 08:18:32.381236 dnd5apy-1.0.4/dnd5apy/models/magic_school.py
--rwxr-xr-x   0        0        0    22610 2023-06-24 08:18:32.405236 dnd5apy-1.0.4/dnd5apy/models/model_class.py
--rwxr-xr-x   0        0        0    41212 2023-06-24 08:18:32.433236 dnd5apy-1.0.4/dnd5apy/models/monster.py
--rwxr-xr-x   0        0        0    17204 2023-06-24 08:18:32.449237 dnd5apy-1.0.4/dnd5apy/models/monster_ability.py
--rwxr-xr-x   0        0        0    19007 2023-06-24 08:18:32.465237 dnd5apy-1.0.4/dnd5apy/models/monster_action.py
--rwxr-xr-x   0        0        0    12258 2023-06-24 08:18:32.481237 dnd5apy-1.0.4/dnd5apy/models/monster_armor_class.py
--rwxr-xr-x   0        0        0    13989 2023-06-24 08:18:32.493237 dnd5apy-1.0.4/dnd5apy/models/monster_attack.py
--rwxr-xr-x   0        0        0    14616 2023-06-24 08:18:32.505237 dnd5apy-1.0.4/dnd5apy/models/monster_multi_attack_action.py
--rwxr-xr-x   0        0        0    13655 2023-06-24 08:18:32.517237 dnd5apy-1.0.4/dnd5apy/models/monster_proficiency.py
--rwxr-xr-x   0        0        0    17751 2023-06-24 08:18:32.529237 dnd5apy-1.0.4/dnd5apy/models/monster_sense.py
--rwxr-xr-x   0        0        0    16990 2023-06-24 08:18:32.541237 dnd5apy-1.0.4/dnd5apy/models/monster_special_ability.py
--rwxr-xr-x   0        0        0    16745 2023-06-24 08:18:32.557237 dnd5apy-1.0.4/dnd5apy/models/monster_speed.py
--rwxr-xr-x   0        0        0    14597 2023-06-24 08:18:32.569237 dnd5apy-1.0.4/dnd5apy/models/monster_spell.py
--rwxr-xr-x   0        0        0    17140 2023-06-24 08:18:32.581237 dnd5apy-1.0.4/dnd5apy/models/monster_spellcasting.py
--rwxr-xr-x   0        0        0    14448 2023-06-24 08:18:32.593237 dnd5apy-1.0.4/dnd5apy/models/monster_usage.py
--rwxr-xr-x   0        0        0    16276 2023-06-24 08:18:32.601237 dnd5apy-1.0.4/dnd5apy/models/multiclassing.py
--rwxr-xr-x   0        0        0    12214 2023-06-24 08:18:32.613237 dnd5apy-1.0.4/dnd5apy/models/option.py
--rwxr-xr-x   0        0        0    12226 2023-06-24 08:18:32.625238 dnd5apy-1.0.4/dnd5apy/models/option_set.py
--rwxr-xr-x   0        0        0    13958 2023-06-24 08:18:32.633237 dnd5apy-1.0.4/dnd5apy/models/prerequisite.py
--rwxr-xr-x   0        0        0    15719 2023-06-24 08:18:32.649238 dnd5apy-1.0.4/dnd5apy/models/proficiency.py
--rwxr-xr-x   0        0        0    22714 2023-06-24 08:18:32.665238 dnd5apy-1.0.4/dnd5apy/models/race.py
--rwxr-xr-x   0        0        0    12989 2023-06-24 08:18:32.677238 dnd5apy-1.0.4/dnd5apy/models/resource_description.py
--rwxr-xr-x   0        0        0    14119 2023-06-24 08:18:32.697238 dnd5apy-1.0.4/dnd5apy/models/rule.py
--rwxr-xr-x   0        0        0    13263 2023-06-24 08:18:32.713238 dnd5apy-1.0.4/dnd5apy/models/rule_section.py
--rwxr-xr-x   0        0        0    13997 2023-06-24 08:18:32.725238 dnd5apy-1.0.4/dnd5apy/models/skill.py
--rwxr-xr-x   0        0        0    25250 2023-06-24 08:18:32.733238 dnd5apy-1.0.4/dnd5apy/models/spell.py
--rwxr-xr-x   0        0        0    13313 2023-06-24 08:18:32.745238 dnd5apy-1.0.4/dnd5apy/models/spell_prerequisite.py
--rwxr-xr-x   0        0        0    14977 2023-06-24 08:18:32.753238 dnd5apy-1.0.4/dnd5apy/models/spellcasting.py
--rwxr-xr-x   0        0        0    13614 2023-06-24 08:18:32.765238 dnd5apy-1.0.4/dnd5apy/models/spellcasting_info.py
--rwxr-xr-x   0        0        0    16428 2023-06-24 08:18:32.773238 dnd5apy-1.0.4/dnd5apy/models/subclass.py
--rwxr-xr-x   0        0        0    19031 2023-06-24 08:18:32.785238 dnd5apy-1.0.4/dnd5apy/models/subclass_level.py
--rwxr-xr-x   0        0        0    16274 2023-06-24 08:18:32.793238 dnd5apy-1.0.4/dnd5apy/models/subclass_level_resource.py
--rwxr-xr-x   0        0        0    22333 2023-06-24 08:18:32.805238 dnd5apy-1.0.4/dnd5apy/models/subclass_level_spellcasting.py
--rwxr-xr-x   0        0        0    13701 2023-06-24 08:18:32.813238 dnd5apy-1.0.4/dnd5apy/models/subclass_spells.py
--rwxr-xr-x   0        0        0    18557 2023-06-24 08:18:32.825239 dnd5apy-1.0.4/dnd5apy/models/subrace.py
--rwxr-xr-x   0        0        0    18243 2023-06-24 08:18:32.833238 dnd5apy-1.0.4/dnd5apy/models/trait.py
--rwxr-xr-x   0        0        0    20874 2023-06-24 08:18:32.845239 dnd5apy-1.0.4/dnd5apy/models/weapon.py
--rwxr-xr-x   0        0        0    13313 2023-06-24 08:18:32.853239 dnd5apy-1.0.4/dnd5apy/models/weapon_property.py
--rwxr-xr-x   0        0        0    13654 2023-06-24 08:18:32.861239 dnd5apy-1.0.4/dnd5apy/models/weapon_range.py
--rwxr-xr-x   0        0        0    22818 2023-06-24 08:18:33.345241 dnd5apy-1.0.4/dnd5apy/rest.py
--rwxr-xr-x   0        0        0      691 2023-06-24 08:27:50.332006 dnd5apy-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    26375 1970-01-01 00:00:00.000000 dnd5apy-1.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0    25494 2023-06-24 08:39:59.755627 dnd5apy-1.0.5/README.md
+-rwxr-xr-x   0        0        0    15003 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/__init__.py
+-rwxr-xr-x   0        0        0      892 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/api/__init__.py
+-rwxr-xr-x   0        0        0    36882 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/character_data_api.py
+-rwxr-xr-x   0        0        0    22406 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/class_api.py
+-rwxr-xr-x   0        0        0    27898 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/class_levels_api.py
+-rwxr-xr-x   0        0        0    25406 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/class_resource_lists_api.py
+-rwxr-xr-x   0        0        0    17884 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/common_api.py
+-rwxr-xr-x   0        0        0    26704 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/equipment_api.py
+-rwxr-xr-x   0        0        0    14353 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/feats_api.py
+-rwxr-xr-x   0        0        0    14976 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/features_api.py
+-rwxr-xr-x   0        0        0    23195 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/game_mechanics_api.py
+-rwxr-xr-x   0        0        0    17611 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/monsters_api.py
+-rwxr-xr-x   0        0        0    25350 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/races_api.py
+-rwxr-xr-x   0        0        0    18567 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/rules_api.py
+-rwxr-xr-x   0        0        0    17972 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/spells_api.py
+-rwxr-xr-x   0        0        0    30987 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/subclasses_api.py
+-rwxr-xr-x   0        0        0    21777 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/subraces_api.py
+-rwxr-xr-x   0        0        0    14126 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api/traits_api.py
+-rwxr-xr-x   0        0        0    34838 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/api_client.py
+-rwxr-xr-x   0        0        0    17789 2023-06-24 08:18:33.317241 dnd5apy-1.0.5/dnd5apy/configuration.py
+-rwxr-xr-x   0        0        0    14060 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/__init__.py
+-rwxr-xr-x   0        0        0    13741 2023-06-24 08:18:31.705233 dnd5apy-1.0.5/dnd5apy/models/ability_bonus.py
+-rwxr-xr-x   0        0        0    14869 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/ability_score.py
+-rwxr-xr-x   0        0        0    14127 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/alignment.py
+-rwxr-xr-x   0        0        0    12663 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/all_of_prerequisite_ability_score.py
+-rwxr-xr-x   0        0        0    12691 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/all_of_spellcasting_spellcasting_ability.py
+-rwxr-xr-x   0        0        0    12302 2023-06-24 08:18:31.865234 dnd5apy-1.0.5/dnd5apy/models/any_of_class_level_class_specific.py
+-rwxr-xr-x   0        0        0    14309 2023-06-24 08:18:31.601232 dnd5apy-1.0.5/dnd5apy/models/api_reference.py
+-rwxr-xr-x   0        0        0    13687 2023-06-24 08:18:31.661233 dnd5apy-1.0.5/dnd5apy/models/api_reference_list.py
+-rwxr-xr-x   0        0        0    13694 2023-06-24 08:18:31.889234 dnd5apy-1.0.5/dnd5apy/models/area_of_effect.py
+-rwxr-xr-x   0        0        0    18897 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/armor.py
+-rwxr-xr-x   0        0        0    20120 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/background.py
+-rwxr-xr-x   0        0        0    13468 2023-06-24 08:18:31.961234 dnd5apy-1.0.5/dnd5apy/models/background_feature.py
+-rwxr-xr-x   0        0        0    14869 2023-06-24 08:18:31.981234 dnd5apy-1.0.5/dnd5apy/models/choice.py
+-rwxr-xr-x   0        0        0    18996 2023-06-24 08:18:31.997234 dnd5apy-1.0.5/dnd5apy/models/class_level.py
+-rwxr-xr-x   0        0        0    13723 2023-06-24 08:18:32.017234 dnd5apy-1.0.5/dnd5apy/models/class_starting_equipment.py
+-rwxr-xr-x   0        0        0    13266 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/condition.py
+-rwxr-xr-x   0        0        0    13556 2023-06-24 08:18:32.065235 dnd5apy-1.0.5/dnd5apy/models/cost.py
+-rwxr-xr-x   0        0        0    13625 2023-06-24 08:18:32.125235 dnd5apy-1.0.5/dnd5apy/models/damage.py
+-rwxr-xr-x   0        0        0    14139 2023-06-24 08:18:32.149235 dnd5apy-1.0.5/dnd5apy/models/damage_at_character_level.py
+-rwxr-xr-x   0        0        0    13979 2023-06-24 08:18:32.165235 dnd5apy-1.0.5/dnd5apy/models/damage_at_slot_level.py
+-rwxr-xr-x   0        0        0    13274 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/damage_type.py
+-rwxr-xr-x   0        0        0    14418 2023-06-24 08:18:32.093235 dnd5apy-1.0.5/dnd5apy/models/dc.py
+-rwxr-xr-x   0        0        0    12226 2023-06-24 08:18:32.201235 dnd5apy-1.0.5/dnd5apy/models/equipment.py
+-rwxr-xr-x   0        0        0    13509 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/equipment_category.py
+-rwxr-xr-x   0        0        0    16392 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/equipment_pack.py
+-rwxr-xr-x   0        0        0    12925 2023-06-24 08:18:32.257236 dnd5apy-1.0.5/dnd5apy/models/error_response.py
+-rwxr-xr-x   0        0        0    14170 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/feat.py
+-rwxr-xr-x   0        0        0    17695 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/feature.py
+-rwxr-xr-x   0        0        0    16075 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/gear.py
+-rwxr-xr-x   0        0        0    15771 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/language.py
+-rwxr-xr-x   0        0        0    16207 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/magic_item.py
+-rwxr-xr-x   0        0        0    13259 2023-06-24 08:18:32.361236 dnd5apy-1.0.5/dnd5apy/models/magic_item_rarity.py
+-rwxr-xr-x   0        0        0    13276 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/magic_school.py
+-rwxr-xr-x   0        0        0    22603 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/model_class.py
+-rwxr-xr-x   0        0        0    41205 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/monster.py
+-rwxr-xr-x   0        0        0    17204 2023-06-24 08:18:32.449237 dnd5apy-1.0.5/dnd5apy/models/monster_ability.py
+-rwxr-xr-x   0        0        0    19007 2023-06-24 08:18:32.465237 dnd5apy-1.0.5/dnd5apy/models/monster_action.py
+-rwxr-xr-x   0        0        0    12258 2023-06-24 08:18:32.481237 dnd5apy-1.0.5/dnd5apy/models/monster_armor_class.py
+-rwxr-xr-x   0        0        0    13989 2023-06-24 08:18:32.493237 dnd5apy-1.0.5/dnd5apy/models/monster_attack.py
+-rwxr-xr-x   0        0        0    14616 2023-06-24 08:18:32.505237 dnd5apy-1.0.5/dnd5apy/models/monster_multi_attack_action.py
+-rwxr-xr-x   0        0        0    13655 2023-06-24 08:18:32.517237 dnd5apy-1.0.5/dnd5apy/models/monster_proficiency.py
+-rwxr-xr-x   0        0        0    17751 2023-06-24 08:18:32.529237 dnd5apy-1.0.5/dnd5apy/models/monster_sense.py
+-rwxr-xr-x   0        0        0    16990 2023-06-24 08:18:32.541237 dnd5apy-1.0.5/dnd5apy/models/monster_special_ability.py
+-rwxr-xr-x   0        0        0    16745 2023-06-24 08:18:32.557237 dnd5apy-1.0.5/dnd5apy/models/monster_speed.py
+-rwxr-xr-x   0        0        0    14597 2023-06-24 08:18:32.569237 dnd5apy-1.0.5/dnd5apy/models/monster_spell.py
+-rwxr-xr-x   0        0        0    17140 2023-06-24 08:18:32.581237 dnd5apy-1.0.5/dnd5apy/models/monster_spellcasting.py
+-rwxr-xr-x   0        0        0    14448 2023-06-24 08:18:32.593237 dnd5apy-1.0.5/dnd5apy/models/monster_usage.py
+-rwxr-xr-x   0        0        0    16276 2023-06-24 08:18:32.601237 dnd5apy-1.0.5/dnd5apy/models/multiclassing.py
+-rwxr-xr-x   0        0        0    12214 2023-06-24 08:18:32.613237 dnd5apy-1.0.5/dnd5apy/models/option.py
+-rwxr-xr-x   0        0        0    12226 2023-06-24 08:18:32.625238 dnd5apy-1.0.5/dnd5apy/models/option_set.py
+-rwxr-xr-x   0        0        0    13958 2023-06-24 08:18:32.633237 dnd5apy-1.0.5/dnd5apy/models/prerequisite.py
+-rwxr-xr-x   0        0        0    15712 2023-06-24 08:38:46.139261 dnd5apy-1.0.5/dnd5apy/models/proficiency.py
+-rwxr-xr-x   0        0        0    22707 2023-06-24 08:38:46.131261 dnd5apy-1.0.5/dnd5apy/models/race.py
+-rwxr-xr-x   0        0        0    12989 2023-06-24 08:18:32.677238 dnd5apy-1.0.5/dnd5apy/models/resource_description.py
+-rwxr-xr-x   0        0        0    14112 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/rule.py
+-rwxr-xr-x   0        0        0    13256 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/rule_section.py
+-rwxr-xr-x   0        0        0    13990 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/skill.py
+-rwxr-xr-x   0        0        0    25243 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/spell.py
+-rwxr-xr-x   0        0        0    13306 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/spell_prerequisite.py
+-rwxr-xr-x   0        0        0    14977 2023-06-24 08:18:32.753238 dnd5apy-1.0.5/dnd5apy/models/spellcasting.py
+-rwxr-xr-x   0        0        0    13614 2023-06-24 08:18:32.765238 dnd5apy-1.0.5/dnd5apy/models/spellcasting_info.py
+-rwxr-xr-x   0        0        0    16421 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/subclass.py
+-rwxr-xr-x   0        0        0    19031 2023-06-24 08:18:32.785238 dnd5apy-1.0.5/dnd5apy/models/subclass_level.py
+-rwxr-xr-x   0        0        0    16274 2023-06-24 08:18:32.793238 dnd5apy-1.0.5/dnd5apy/models/subclass_level_resource.py
+-rwxr-xr-x   0        0        0    22333 2023-06-24 08:18:32.805238 dnd5apy-1.0.5/dnd5apy/models/subclass_level_spellcasting.py
+-rwxr-xr-x   0        0        0    13701 2023-06-24 08:18:32.813238 dnd5apy-1.0.5/dnd5apy/models/subclass_spells.py
+-rwxr-xr-x   0        0        0    18550 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/subrace.py
+-rwxr-xr-x   0        0        0    18236 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/trait.py
+-rwxr-xr-x   0        0        0    20867 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/weapon.py
+-rwxr-xr-x   0        0        0    13306 2023-06-24 08:38:46.123261 dnd5apy-1.0.5/dnd5apy/models/weapon_property.py
+-rwxr-xr-x   0        0        0    13654 2023-06-24 08:18:32.861239 dnd5apy-1.0.5/dnd5apy/models/weapon_range.py
+-rwxr-xr-x   0        0        0    22818 2023-06-24 08:18:33.345241 dnd5apy-1.0.5/dnd5apy/rest.py
+-rwxr-xr-x   0        0        0      691 2023-06-24 08:42:10.180274 dnd5apy-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    26368 1970-01-01 00:00:00.000000 dnd5apy-1.0.5/PKG-INFO
```

### Comparing `dnd5apy-1.0.4/README.md` & `dnd5apy-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# swagger-client
+# dnd5apy
 # Introduction  Welcome to the dnd5eapi, the Dungeons & Dragons 5th Edition API! This documentation should help you familiarize yourself with the resources available and how to consume them with HTTP requests. Read through the getting started section before you dive in. Most of your problems should be solved just by reading through it.  ## Getting Started  Let's make our first API request to the D&D 5th Edition API!  Open up a terminal and use [curl](http://curl.haxx.se/) or [httpie](http://httpie.org/) to make an API request for a resource. You can also scroll through the definitions below and send requests directly from the endpoint documentation!  For example, if you paste and run this `curl` command: ```bash curl -X GET \"https://www.dnd5eapi.co/api/ability-scores/cha\" -H \"Accept: application/json\" ```  We should see a result containing details about the Charisma ability score: ```bash {   \"index\": \"cha\",   \"name\": \"CHA\",   \"full_name\": \"Charisma\",   \"desc\": [     \"Charisma measures your ability to interact effectively with others. It       includes such factors as confidence and eloquence, and it can represent       a charming or commanding personality.\",     \"A Charisma check might arise when you try to influence or entertain       others, when you try to make an impression or tell a convincing lie,       or when you are navigating a tricky social situation. The Deception,       Intimidation, Performance, and Persuasion skills reflect aptitude in       certain kinds of Charisma checks.\"   ],   \"skills\": [     {       \"name\": \"Deception\",       \"index\": \"deception\",       \"url\": \"/api/skills/deception\"     },     {       \"name\": \"Intimidation\",       \"index\": \"intimidation\",       \"url\": \"/api/skills/intimidation\"     },     {       \"name\": \"Performance\",       \"index\": \"performance\",       \"url\": \"/api/skills/performance\"     },     {       \"name\": \"Persuasion\",       \"index\": \"persuasion\",       \"url\": \"/api/skills/persuasion\"     }   ],   \"url\": \"/api/ability-scores/cha\" } ```  ## Authentication  The dnd5eapi is a completely open API. No authentication is required to query and get data. This also means that we've limited what you can do to just `GET`-ing the data. If you find a mistake in the data, feel free to [message us](https://discord.gg/TQuYTv7).  ## GraphQL  This API supports [GraphQL](https://graphql.org/). The GraphQL URL for this API is `https://www.dnd5eapi.co/graphql`. Most of your questions regarding the GraphQL schema can be answered by querying the endpoint with the Apollo sandbox explorer.  ## Schemas  Definitions of all schemas will be accessible in a future update. Two of the most common schemas are described here.  ### `APIReference` Represents a minimal representation of a resource. The detailed representation of the referenced resource can be retrieved by making a request to the referenced `URL`. ``` APIReference {   index     string   name      string   url       string } ``` <hr>  ### `DC` Represents a difficulty check. ``` DC {   dc_type       APIReference   dc_value      number   success_type  \"none\" | \"half\" | \"other\" } ``` <hr>  ### `Damage` Represents damage. ``` Damage {   damage_type     APIReference   damage_dice     string } ``` <hr>  ### `Choice` Represents a choice made by a player. Commonly seen related to decisions made during character creation or combat (e.g.: the description of the cleric class, under **Proficiencies**, states \"Skills: Choose two from History, Insight, Medicine, Persuasion, and Religion\" [[SRD p15]](https://media.wizards.com/2016/downloads/DND/SRD-OGL_V5.1.pdf#page=15)) ``` Choice {   desc      string   choose    number   type      string   from      OptionSet } ``` <hr>  ### `OptionSet` The OptionSet structure provides the options to be chosen from, or sufficient data to fetch and interpret the options. All OptionSets have an `option_set_type` attribute that indicates the structure of the object that contains the options. The possible values are `options_array`, `equipment_category`, and `reference_list`. Other attributes on the OptionSet depend on the value of this attribute. - `options_array`   - `options` (array): An array of Option objects. Each item in the array represents an option that can be chosen. - `equipment_category`   - `equipment_category` (APIReference): A reference to an EquipmentCategory. Each item in the EquipmentCategory's `equipment` array represents one option that can be chosen. - `resource_list`   - `resource_list_url` (string): A reference (by URL) to a collection in the database. The URL may include query parameters. Each item in the resulting ResourceList's `results` array represents one option that can be chosen. <hr>  ### `Option` When the options are given in an `options_array`, each item in the array inherits from the Option structure. All Options have an `option_type` attribute that indicates the structure of the option. The value of this attribute indicates how the option should be handled, and each type has different attributes. The possible values and their corresponding attributes are listed below. - `reference` - A terminal option. Contains a reference to a Document that can be added to the list of options chosen.   - `item` (APIReference): A reference to the chosen item. - `action` - A terminal option. Contains information describing an action, for use within Multiattack actions.   - `action_name` (string): The name of the action, according to its `name` attribute.   - `count` (number | string): The number of times this action can be repeated if this option is chosen.   - `type` (string = `\"melee\" | \"ranged\" | \"ability\" | \"magic\"`, optional): For attack actions that can be either melee, ranged, abilities, or magic. - `multiple` - When this option is chosen, all of its child options are chosen, and must be resolved the same way as a normal option.   - `items` (array): An array of Option objects. All of them must be taken if the option is chosen. - `choice` - A nested choice. If this option is chosen, the Choice structure contained within must be resolved like a normal Choice structure, and the results are the chosen options.   - `choice` (Choice): The Choice to resolve. - `string` - A terminal option. Contains a reference to a string.   - `string` (string): The string. - `ideal` - A terminal option. Contains information about an ideal.   - `desc` (string): A description of the ideal.   - `alignments` (ApiReference[]): A list of alignments of those who might follow the ideal. - `counted_reference` - A terminal option. Contains a reference to something else in the API along with a count.   - `count` (number): Count.   - `of` (ApiReference): Thing being referenced. - `score_prerequisite` - A terminal option. Contains a reference to an ability score and a minimum score.   - `ability_score` (ApiReference): Ability score being referenced.   - `minimum_score` (number): The minimum score required to satisfy the prerequisite. - `ability_bonus` - A terminal option. Contains a reference to an ability score and a bonus   - `ability_score` (ApiReference): Ability score being referenced   - `bonus` (number): The bonus being applied to the ability score - `breath` - A terminal option: Contains a reference to information about a breath attack.   - `name` (string): Name of the breath.   - `dc` (DC): Difficulty check of the breath attack.   - `damage` ([Damage]): Damage dealt by the breath attack, if any. - `damage` - A terminal option. Contains information about damage.   - `damage_type` (ApiReference): Reference to type of damage.   - `damage_dice` (string): Damage expressed in dice (e.g. \"13d6\").   - `notes` (string): Information regarding the damage.  ## FAQ  ### What is the SRD? The SRD, or Systems Reference Document, contains guidelines for publishing content under the OGL. This allows for some of the data for D&D 5e to be open source. The API only covers data that can be found in the SRD. [Here's a link to the full text of the SRD.](https://media.wizards.com/2016/downloads/DND/SRD-OGL_V5.1.pdf)  ### What is the OGL? The Open Game License (OGL) is a public copyright license by Wizards of the Coast that may be used by tabletop role-playing game developers to grant permission to modify, copy, and redistribute some of the content designed for their games, notably game mechanics. However, they must share-alike copies and derivative works. [More information about the OGL can be found here.](https://en.wikipedia.org/wiki/Open_Game_License)  ### A monster, spell, subclass, etc. is missing from the API / Database. Can I add it? Please check if the data is within the SRD. If it is, feel free to open an issue or PR to add it yourself. Otherwise, due to legal reasons, we cannot add it.  ### Can this API be self hosted? Yes it can! You can also host the data yourself if you don't want to use the API at all. You can also make changes and add extra data if you like. However, it is up to you to merge in new changes to the data and API.  #### Can I publish is on <insert platform>? Is this free use? Yes, you can. The API itself is under the [MIT license](https://opensource.org/licenses/MIT), and the underlying data accessible via the API is supported under the SRD and OGL.  # Status Page  The status page for the API can be found here: https://5e-bits.github.io/dnd-uptime/  # Chat  Come hang out with us [on Discord](https://discord.gg/TQuYTv7)!  # Contribute  This API is built from two repositories.   - The repo containing the data lives here: https://github.com/bagelbits/5e-database   - The repo with the API implementation lives here: https://github.com/bagelbits/5e-srd-api  This is a evolving API and having fresh ideas are always welcome! You can open an issue in either repo, open a PR for changes, or just discuss with other users in this discord. 
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 0.1
 - Package version: 1.0.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/__init__.py` & `dnd5apy-1.0.5/dnd5apy/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,98 +11,98 @@
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
-from swagger_client.api.character_data_api import CharacterDataApi
-from swagger_client.api.class_api import ClassApi
-from swagger_client.api.class_levels_api import ClassLevelsApi
-from swagger_client.api.class_resource_lists_api import ClassResourceListsApi
-from swagger_client.api.common_api import CommonApi
-from swagger_client.api.equipment_api import EquipmentApi
-from swagger_client.api.feats_api import FeatsApi
-from swagger_client.api.features_api import FeaturesApi
-from swagger_client.api.game_mechanics_api import GameMechanicsApi
-from swagger_client.api.monsters_api import MonstersApi
-from swagger_client.api.races_api import RacesApi
-from swagger_client.api.rules_api import RulesApi
-from swagger_client.api.spells_api import SpellsApi
-from swagger_client.api.subclasses_api import SubclassesApi
-from swagger_client.api.subraces_api import SubracesApi
-from swagger_client.api.traits_api import TraitsApi
+from dnd5apy.api.character_data_api import CharacterDataApi
+from dnd5apy.api.class_api import ClassApi
+from dnd5apy.api.class_levels_api import ClassLevelsApi
+from dnd5apy.api.class_resource_lists_api import ClassResourceListsApi
+from dnd5apy.api.common_api import CommonApi
+from dnd5apy.api.equipment_api import EquipmentApi
+from dnd5apy.api.feats_api import FeatsApi
+from dnd5apy.api.features_api import FeaturesApi
+from dnd5apy.api.game_mechanics_api import GameMechanicsApi
+from dnd5apy.api.monsters_api import MonstersApi
+from dnd5apy.api.races_api import RacesApi
+from dnd5apy.api.rules_api import RulesApi
+from dnd5apy.api.spells_api import SpellsApi
+from dnd5apy.api.subclasses_api import SubclassesApi
+from dnd5apy.api.subraces_api import SubracesApi
+from dnd5apy.api.traits_api import TraitsApi
 # import ApiClient
-from swagger_client.api_client import ApiClient
-from swagger_client.configuration import Configuration
+from dnd5apy.api_client import ApiClient
+from dnd5apy.configuration import Configuration
 # import models into sdk package
-from swagger_client.models.api_reference import APIReference
-from swagger_client.models.api_reference_list import APIReferenceList
-from swagger_client.models.ability_bonus import AbilityBonus
-from swagger_client.models.ability_score import AbilityScore
-from swagger_client.models.alignment import Alignment
-from swagger_client.models.all_of_prerequisite_ability_score import AllOfPrerequisiteAbilityScore
-from swagger_client.models.all_of_spellcasting_spellcasting_ability import AllOfSpellcastingSpellcastingAbility
-from swagger_client.models.any_of_class_level_class_specific import AnyOfClassLevelClassSpecific
-from swagger_client.models.area_of_effect import AreaOfEffect
-from swagger_client.models.armor import Armor
-from swagger_client.models.background import Background
-from swagger_client.models.background_feature import BackgroundFeature
-from swagger_client.models.choice import Choice
-from swagger_client.models.class_level import ClassLevel
-from swagger_client.models.class_starting_equipment import ClassStartingEquipment
-from swagger_client.models.condition import Condition
-from swagger_client.models.cost import Cost
-from swagger_client.models.dc import DC
-from swagger_client.models.damage import Damage
-from swagger_client.models.damage_at_character_level import DamageAtCharacterLevel
-from swagger_client.models.damage_at_slot_level import DamageAtSlotLevel
-from swagger_client.models.damage_type import DamageType
-from swagger_client.models.equipment import Equipment
-from swagger_client.models.equipment_category import EquipmentCategory
-from swagger_client.models.equipment_pack import EquipmentPack
-from swagger_client.models.error_response import ErrorResponse
-from swagger_client.models.feat import Feat
-from swagger_client.models.feature import Feature
-from swagger_client.models.gear import Gear
-from swagger_client.models.language import Language
-from swagger_client.models.magic_item import MagicItem
-from swagger_client.models.magic_item_rarity import MagicItemRarity
-from swagger_client.models.magic_school import MagicSchool
-from swagger_client.models.model_class import ModelClass
-from swagger_client.models.monster import Monster
-from swagger_client.models.monster_ability import MonsterAbility
-from swagger_client.models.monster_action import MonsterAction
-from swagger_client.models.monster_armor_class import MonsterArmorClass
-from swagger_client.models.monster_attack import MonsterAttack
-from swagger_client.models.monster_multi_attack_action import MonsterMultiAttackAction
-from swagger_client.models.monster_proficiency import MonsterProficiency
-from swagger_client.models.monster_sense import MonsterSense
-from swagger_client.models.monster_special_ability import MonsterSpecialAbility
-from swagger_client.models.monster_speed import MonsterSpeed
-from swagger_client.models.monster_spell import MonsterSpell
-from swagger_client.models.monster_spellcasting import MonsterSpellcasting
-from swagger_client.models.monster_usage import MonsterUsage
-from swagger_client.models.multiclassing import Multiclassing
-from swagger_client.models.option import Option
-from swagger_client.models.option_set import OptionSet
-from swagger_client.models.prerequisite import Prerequisite
-from swagger_client.models.proficiency import Proficiency
-from swagger_client.models.race import Race
-from swagger_client.models.resource_description import ResourceDescription
-from swagger_client.models.rule import Rule
-from swagger_client.models.rule_section import RuleSection
-from swagger_client.models.skill import Skill
-from swagger_client.models.spell import Spell
-from swagger_client.models.spell_prerequisite import SpellPrerequisite
-from swagger_client.models.spellcasting import Spellcasting
-from swagger_client.models.spellcasting_info import SpellcastingInfo
-from swagger_client.models.subclass import Subclass
-from swagger_client.models.subclass_level import SubclassLevel
-from swagger_client.models.subclass_level_resource import SubclassLevelResource
-from swagger_client.models.subclass_level_spellcasting import SubclassLevelSpellcasting
-from swagger_client.models.subclass_spells import SubclassSpells
-from swagger_client.models.subrace import Subrace
-from swagger_client.models.trait import Trait
-from swagger_client.models.weapon import Weapon
-from swagger_client.models.weapon_property import WeaponProperty
-from swagger_client.models.weapon_range import WeaponRange
+from dnd5apy.models.api_reference import APIReference
+from dnd5apy.models.api_reference_list import APIReferenceList
+from dnd5apy.models.ability_bonus import AbilityBonus
+from dnd5apy.models.ability_score import AbilityScore
+from dnd5apy.models.alignment import Alignment
+from dnd5apy.models.all_of_prerequisite_ability_score import AllOfPrerequisiteAbilityScore
+from dnd5apy.models.all_of_spellcasting_spellcasting_ability import AllOfSpellcastingSpellcastingAbility
+from dnd5apy.models.any_of_class_level_class_specific import AnyOfClassLevelClassSpecific
+from dnd5apy.models.area_of_effect import AreaOfEffect
+from dnd5apy.models.armor import Armor
+from dnd5apy.models.background import Background
+from dnd5apy.models.background_feature import BackgroundFeature
+from dnd5apy.models.choice import Choice
+from dnd5apy.models.class_level import ClassLevel
+from dnd5apy.models.class_starting_equipment import ClassStartingEquipment
+from dnd5apy.models.condition import Condition
+from dnd5apy.models.cost import Cost
+from dnd5apy.models.dc import DC
+from dnd5apy.models.damage import Damage
+from dnd5apy.models.damage_at_character_level import DamageAtCharacterLevel
+from dnd5apy.models.damage_at_slot_level import DamageAtSlotLevel
+from dnd5apy.models.damage_type import DamageType
+from dnd5apy.models.equipment import Equipment
+from dnd5apy.models.equipment_category import EquipmentCategory
+from dnd5apy.models.equipment_pack import EquipmentPack
+from dnd5apy.models.error_response import ErrorResponse
+from dnd5apy.models.feat import Feat
+from dnd5apy.models.feature import Feature
+from dnd5apy.models.gear import Gear
+from dnd5apy.models.language import Language
+from dnd5apy.models.magic_item import MagicItem
+from dnd5apy.models.magic_item_rarity import MagicItemRarity
+from dnd5apy.models.magic_school import MagicSchool
+from dnd5apy.models.model_class import ModelClass
+from dnd5apy.models.monster import Monster
+from dnd5apy.models.monster_ability import MonsterAbility
+from dnd5apy.models.monster_action import MonsterAction
+from dnd5apy.models.monster_armor_class import MonsterArmorClass
+from dnd5apy.models.monster_attack import MonsterAttack
+from dnd5apy.models.monster_multi_attack_action import MonsterMultiAttackAction
+from dnd5apy.models.monster_proficiency import MonsterProficiency
+from dnd5apy.models.monster_sense import MonsterSense
+from dnd5apy.models.monster_special_ability import MonsterSpecialAbility
+from dnd5apy.models.monster_speed import MonsterSpeed
+from dnd5apy.models.monster_spell import MonsterSpell
+from dnd5apy.models.monster_spellcasting import MonsterSpellcasting
+from dnd5apy.models.monster_usage import MonsterUsage
+from dnd5apy.models.multiclassing import Multiclassing
+from dnd5apy.models.option import Option
+from dnd5apy.models.option_set import OptionSet
+from dnd5apy.models.prerequisite import Prerequisite
+from dnd5apy.models.proficiency import Proficiency
+from dnd5apy.models.race import Race
+from dnd5apy.models.resource_description import ResourceDescription
+from dnd5apy.models.rule import Rule
+from dnd5apy.models.rule_section import RuleSection
+from dnd5apy.models.skill import Skill
+from dnd5apy.models.spell import Spell
+from dnd5apy.models.spell_prerequisite import SpellPrerequisite
+from dnd5apy.models.spellcasting import Spellcasting
+from dnd5apy.models.spellcasting_info import SpellcastingInfo
+from dnd5apy.models.subclass import Subclass
+from dnd5apy.models.subclass_level import SubclassLevel
+from dnd5apy.models.subclass_level_resource import SubclassLevelResource
+from dnd5apy.models.subclass_level_spellcasting import SubclassLevelSpellcasting
+from dnd5apy.models.subclass_spells import SubclassSpells
+from dnd5apy.models.subrace import Subrace
+from dnd5apy.models.trait import Trait
+from dnd5apy.models.weapon import Weapon
+from dnd5apy.models.weapon_property import WeaponProperty
+from dnd5apy.models.weapon_range import WeaponRange
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/character_data_api.py` & `dnd5apy-1.0.5/dnd5apy/api/character_data_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class CharacterDataApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/class_api.py` & `dnd5apy-1.0.5/dnd5apy/api/class_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class ClassApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/class_levels_api.py` & `dnd5apy-1.0.5/dnd5apy/api/class_levels_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class ClassLevelsApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/class_resource_lists_api.py` & `dnd5apy-1.0.5/dnd5apy/api/class_resource_lists_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class ClassResourceListsApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/common_api.py` & `dnd5apy-1.0.5/dnd5apy/api/common_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class CommonApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/equipment_api.py` & `dnd5apy-1.0.5/dnd5apy/api/equipment_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class EquipmentApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/feats_api.py` & `dnd5apy-1.0.5/dnd5apy/api/feats_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class FeatsApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/features_api.py` & `dnd5apy-1.0.5/dnd5apy/api/features_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class FeaturesApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/game_mechanics_api.py` & `dnd5apy-1.0.5/dnd5apy/api/game_mechanics_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class GameMechanicsApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/monsters_api.py` & `dnd5apy-1.0.5/dnd5apy/api/monsters_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class MonstersApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/races_api.py` & `dnd5apy-1.0.5/dnd5apy/api/races_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class RacesApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/rules_api.py` & `dnd5apy-1.0.5/dnd5apy/api/rules_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class RulesApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/spells_api.py` & `dnd5apy-1.0.5/dnd5apy/api/spells_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class SpellsApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/subclasses_api.py` & `dnd5apy-1.0.5/dnd5apy/api/subclasses_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class SubclassesApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/subraces_api.py` & `dnd5apy-1.0.5/dnd5apy/api/subraces_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class SubracesApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api/traits_api.py` & `dnd5apy-1.0.5/dnd5apy/api/traits_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
 
-from swagger_client.api_client import ApiClient
+from dnd5apy.api_client import ApiClient
 
 
 class TraitsApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
```

### Comparing `dnd5apy-1.0.4/dnd5apy/api_client.py` & `dnd5apy-1.0.5/dnd5apy/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import re
 import tempfile
 
 # python 2 and python 3 compatibility library
 import six
 from six.moves.urllib.parse import quote
 
-from swagger_client.configuration import Configuration
-import swagger_client.models
-from swagger_client import rest
+from dnd5apy.configuration import Configuration
+import dnd5apy.models
+from dnd5apy import rest
 
 
 class ApiClient(object):
     """Generic API client for Swagger client library builds.
 
     Swagger generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
@@ -253,15 +253,15 @@
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in six.iteritems(data)}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
-                klass = getattr(swagger_client.models, klass)
+                klass = getattr(dnd5apy.models, klass)
 
         if klass in self.PRIMITIVE_TYPES:
             return self.__deserialize_primitive(data, klass)
         elif klass == object:
             return self.__deserialize_object(data)
         elif klass == datetime.date:
             return self.__deserialize_date(data)
```

### Comparing `dnd5apy-1.0.4/dnd5apy/configuration.py` & `dnd5apy-1.0.5/dnd5apy/configuration.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/__init__.py` & `dnd5apy-1.0.5/dnd5apy/models/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,78 +10,78 @@
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import models into model package
-from swagger_client.models.api_reference import APIReference
-from swagger_client.models.api_reference_list import APIReferenceList
-from swagger_client.models.ability_bonus import AbilityBonus
-from swagger_client.models.ability_score import AbilityScore
-from swagger_client.models.alignment import Alignment
-from swagger_client.models.all_of_prerequisite_ability_score import AllOfPrerequisiteAbilityScore
-from swagger_client.models.all_of_spellcasting_spellcasting_ability import AllOfSpellcastingSpellcastingAbility
-from swagger_client.models.any_of_class_level_class_specific import AnyOfClassLevelClassSpecific
-from swagger_client.models.area_of_effect import AreaOfEffect
-from swagger_client.models.armor import Armor
-from swagger_client.models.background import Background
-from swagger_client.models.background_feature import BackgroundFeature
-from swagger_client.models.choice import Choice
-from swagger_client.models.class_level import ClassLevel
-from swagger_client.models.class_starting_equipment import ClassStartingEquipment
-from swagger_client.models.condition import Condition
-from swagger_client.models.cost import Cost
-from swagger_client.models.dc import DC
-from swagger_client.models.damage import Damage
-from swagger_client.models.damage_at_character_level import DamageAtCharacterLevel
-from swagger_client.models.damage_at_slot_level import DamageAtSlotLevel
-from swagger_client.models.damage_type import DamageType
-from swagger_client.models.equipment import Equipment
-from swagger_client.models.equipment_category import EquipmentCategory
-from swagger_client.models.equipment_pack import EquipmentPack
-from swagger_client.models.error_response import ErrorResponse
-from swagger_client.models.feat import Feat
-from swagger_client.models.feature import Feature
-from swagger_client.models.gear import Gear
-from swagger_client.models.language import Language
-from swagger_client.models.magic_item import MagicItem
-from swagger_client.models.magic_item_rarity import MagicItemRarity
-from swagger_client.models.magic_school import MagicSchool
-from swagger_client.models.model_class import ModelClass
-from swagger_client.models.monster import Monster
-from swagger_client.models.monster_ability import MonsterAbility
-from swagger_client.models.monster_action import MonsterAction
-from swagger_client.models.monster_armor_class import MonsterArmorClass
-from swagger_client.models.monster_attack import MonsterAttack
-from swagger_client.models.monster_multi_attack_action import MonsterMultiAttackAction
-from swagger_client.models.monster_proficiency import MonsterProficiency
-from swagger_client.models.monster_sense import MonsterSense
-from swagger_client.models.monster_special_ability import MonsterSpecialAbility
-from swagger_client.models.monster_speed import MonsterSpeed
-from swagger_client.models.monster_spell import MonsterSpell
-from swagger_client.models.monster_spellcasting import MonsterSpellcasting
-from swagger_client.models.monster_usage import MonsterUsage
-from swagger_client.models.multiclassing import Multiclassing
-from swagger_client.models.option import Option
-from swagger_client.models.option_set import OptionSet
-from swagger_client.models.prerequisite import Prerequisite
-from swagger_client.models.proficiency import Proficiency
-from swagger_client.models.race import Race
-from swagger_client.models.resource_description import ResourceDescription
-from swagger_client.models.rule import Rule
-from swagger_client.models.rule_section import RuleSection
-from swagger_client.models.skill import Skill
-from swagger_client.models.spell import Spell
-from swagger_client.models.spell_prerequisite import SpellPrerequisite
-from swagger_client.models.spellcasting import Spellcasting
-from swagger_client.models.spellcasting_info import SpellcastingInfo
-from swagger_client.models.subclass import Subclass
-from swagger_client.models.subclass_level import SubclassLevel
-from swagger_client.models.subclass_level_resource import SubclassLevelResource
-from swagger_client.models.subclass_level_spellcasting import SubclassLevelSpellcasting
-from swagger_client.models.subclass_spells import SubclassSpells
-from swagger_client.models.subrace import Subrace
-from swagger_client.models.trait import Trait
-from swagger_client.models.weapon import Weapon
-from swagger_client.models.weapon_property import WeaponProperty
-from swagger_client.models.weapon_range import WeaponRange
+from dnd5apy.models.api_reference import APIReference
+from dnd5apy.models.api_reference_list import APIReferenceList
+from dnd5apy.models.ability_bonus import AbilityBonus
+from dnd5apy.models.ability_score import AbilityScore
+from dnd5apy.models.alignment import Alignment
+from dnd5apy.models.all_of_prerequisite_ability_score import AllOfPrerequisiteAbilityScore
+from dnd5apy.models.all_of_spellcasting_spellcasting_ability import AllOfSpellcastingSpellcastingAbility
+from dnd5apy.models.any_of_class_level_class_specific import AnyOfClassLevelClassSpecific
+from dnd5apy.models.area_of_effect import AreaOfEffect
+from dnd5apy.models.armor import Armor
+from dnd5apy.models.background import Background
+from dnd5apy.models.background_feature import BackgroundFeature
+from dnd5apy.models.choice import Choice
+from dnd5apy.models.class_level import ClassLevel
+from dnd5apy.models.class_starting_equipment import ClassStartingEquipment
+from dnd5apy.models.condition import Condition
+from dnd5apy.models.cost import Cost
+from dnd5apy.models.dc import DC
+from dnd5apy.models.damage import Damage
+from dnd5apy.models.damage_at_character_level import DamageAtCharacterLevel
+from dnd5apy.models.damage_at_slot_level import DamageAtSlotLevel
+from dnd5apy.models.damage_type import DamageType
+from dnd5apy.models.equipment import Equipment
+from dnd5apy.models.equipment_category import EquipmentCategory
+from dnd5apy.models.equipment_pack import EquipmentPack
+from dnd5apy.models.error_response import ErrorResponse
+from dnd5apy.models.feat import Feat
+from dnd5apy.models.feature import Feature
+from dnd5apy.models.gear import Gear
+from dnd5apy.models.language import Language
+from dnd5apy.models.magic_item import MagicItem
+from dnd5apy.models.magic_item_rarity import MagicItemRarity
+from dnd5apy.models.magic_school import MagicSchool
+from dnd5apy.models.model_class import ModelClass
+from dnd5apy.models.monster import Monster
+from dnd5apy.models.monster_ability import MonsterAbility
+from dnd5apy.models.monster_action import MonsterAction
+from dnd5apy.models.monster_armor_class import MonsterArmorClass
+from dnd5apy.models.monster_attack import MonsterAttack
+from dnd5apy.models.monster_multi_attack_action import MonsterMultiAttackAction
+from dnd5apy.models.monster_proficiency import MonsterProficiency
+from dnd5apy.models.monster_sense import MonsterSense
+from dnd5apy.models.monster_special_ability import MonsterSpecialAbility
+from dnd5apy.models.monster_speed import MonsterSpeed
+from dnd5apy.models.monster_spell import MonsterSpell
+from dnd5apy.models.monster_spellcasting import MonsterSpellcasting
+from dnd5apy.models.monster_usage import MonsterUsage
+from dnd5apy.models.multiclassing import Multiclassing
+from dnd5apy.models.option import Option
+from dnd5apy.models.option_set import OptionSet
+from dnd5apy.models.prerequisite import Prerequisite
+from dnd5apy.models.proficiency import Proficiency
+from dnd5apy.models.race import Race
+from dnd5apy.models.resource_description import ResourceDescription
+from dnd5apy.models.rule import Rule
+from dnd5apy.models.rule_section import RuleSection
+from dnd5apy.models.skill import Skill
+from dnd5apy.models.spell import Spell
+from dnd5apy.models.spell_prerequisite import SpellPrerequisite
+from dnd5apy.models.spellcasting import Spellcasting
+from dnd5apy.models.spellcasting_info import SpellcastingInfo
+from dnd5apy.models.subclass import Subclass
+from dnd5apy.models.subclass_level import SubclassLevel
+from dnd5apy.models.subclass_level_resource import SubclassLevelResource
+from dnd5apy.models.subclass_level_spellcasting import SubclassLevelSpellcasting
+from dnd5apy.models.subclass_spells import SubclassSpells
+from dnd5apy.models.subrace import Subrace
+from dnd5apy.models.trait import Trait
+from dnd5apy.models.weapon import Weapon
+from dnd5apy.models.weapon_property import WeaponProperty
+from dnd5apy.models.weapon_range import WeaponRange
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/ability_bonus.py` & `dnd5apy-1.0.5/dnd5apy/models/ability_bonus.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/ability_score.py` & `dnd5apy-1.0.5/dnd5apy/models/ability_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class AbilityScore(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/alignment.py` & `dnd5apy-1.0.5/dnd5apy/models/alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Alignment(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/all_of_prerequisite_ability_score.py` & `dnd5apy-1.0.5/dnd5apy/models/all_of_prerequisite_ability_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class AllOfPrerequisiteAbilityScore(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/all_of_spellcasting_spellcasting_ability.py` & `dnd5apy-1.0.5/dnd5apy/models/all_of_spellcasting_spellcasting_ability.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class AllOfSpellcastingSpellcastingAbility(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/any_of_class_level_class_specific.py` & `dnd5apy-1.0.5/dnd5apy/models/any_of_class_level_class_specific.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/api_reference.py` & `dnd5apy-1.0.5/dnd5apy/models/api_reference.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/api_reference_list.py` & `dnd5apy-1.0.5/dnd5apy/models/api_reference_list.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/area_of_effect.py` & `dnd5apy-1.0.5/dnd5apy/models/area_of_effect.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/armor.py` & `dnd5apy-1.0.5/dnd5apy/models/armor.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Armor(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/background.py` & `dnd5apy-1.0.5/dnd5apy/models/background.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Background(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/background_feature.py` & `dnd5apy-1.0.5/dnd5apy/models/background_feature.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/choice.py` & `dnd5apy-1.0.5/dnd5apy/models/choice.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/class_level.py` & `dnd5apy-1.0.5/dnd5apy/models/class_level.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/class_starting_equipment.py` & `dnd5apy-1.0.5/dnd5apy/models/class_starting_equipment.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/condition.py` & `dnd5apy-1.0.5/dnd5apy/models/condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Condition(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/cost.py` & `dnd5apy-1.0.5/dnd5apy/models/cost.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/damage.py` & `dnd5apy-1.0.5/dnd5apy/models/damage.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/damage_at_character_level.py` & `dnd5apy-1.0.5/dnd5apy/models/damage_at_character_level.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/damage_at_slot_level.py` & `dnd5apy-1.0.5/dnd5apy/models/damage_at_slot_level.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/damage_type.py` & `dnd5apy-1.0.5/dnd5apy/models/damage_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class DamageType(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/dc.py` & `dnd5apy-1.0.5/dnd5apy/models/dc.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/equipment.py` & `dnd5apy-1.0.5/dnd5apy/models/equipment.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/equipment_category.py` & `dnd5apy-1.0.5/dnd5apy/models/equipment_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class EquipmentCategory(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/equipment_pack.py` & `dnd5apy-1.0.5/dnd5apy/models/equipment_pack.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class EquipmentPack(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/error_response.py` & `dnd5apy-1.0.5/dnd5apy/models/error_response.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/feat.py` & `dnd5apy-1.0.5/dnd5apy/models/feat.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Feat(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/feature.py` & `dnd5apy-1.0.5/dnd5apy/models/feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Feature(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/gear.py` & `dnd5apy-1.0.5/dnd5apy/models/gear.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Gear(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/language.py` & `dnd5apy-1.0.5/dnd5apy/models/language.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Language(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/magic_item.py` & `dnd5apy-1.0.5/dnd5apy/models/magic_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class MagicItem(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/magic_item_rarity.py` & `dnd5apy-1.0.5/dnd5apy/models/magic_item_rarity.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/magic_school.py` & `dnd5apy-1.0.5/dnd5apy/models/magic_school.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class MagicSchool(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/model_class.py` & `dnd5apy-1.0.5/dnd5apy/models/model_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class ModelClass(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster.py` & `dnd5apy-1.0.5/dnd5apy/models/monster.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Monster(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_ability.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_ability.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_action.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_action.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_armor_class.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_armor_class.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_attack.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_attack.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_multi_attack_action.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_multi_attack_action.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_proficiency.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_proficiency.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_sense.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_sense.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_special_ability.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_special_ability.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_speed.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_speed.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_spell.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_spell.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_spellcasting.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_spellcasting.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/monster_usage.py` & `dnd5apy-1.0.5/dnd5apy/models/monster_usage.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/multiclassing.py` & `dnd5apy-1.0.5/dnd5apy/models/multiclassing.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/option.py` & `dnd5apy-1.0.5/dnd5apy/models/option.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/option_set.py` & `dnd5apy-1.0.5/dnd5apy/models/option_set.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/prerequisite.py` & `dnd5apy-1.0.5/dnd5apy/models/prerequisite.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/proficiency.py` & `dnd5apy-1.0.5/dnd5apy/models/proficiency.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Proficiency(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/race.py` & `dnd5apy-1.0.5/dnd5apy/models/race.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Race(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/resource_description.py` & `dnd5apy-1.0.5/dnd5apy/models/resource_description.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/rule.py` & `dnd5apy-1.0.5/dnd5apy/models/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Rule(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/rule_section.py` & `dnd5apy-1.0.5/dnd5apy/models/rule_section.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class RuleSection(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/skill.py` & `dnd5apy-1.0.5/dnd5apy/models/skill.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Skill(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/spell.py` & `dnd5apy-1.0.5/dnd5apy/models/spell.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Spell(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/spell_prerequisite.py` & `dnd5apy-1.0.5/dnd5apy/models/spell_prerequisite.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class SpellPrerequisite(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/spellcasting.py` & `dnd5apy-1.0.5/dnd5apy/models/spellcasting.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/spellcasting_info.py` & `dnd5apy-1.0.5/dnd5apy/models/spellcasting_info.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/subclass.py` & `dnd5apy-1.0.5/dnd5apy/models/subclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Subclass(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/subclass_level.py` & `dnd5apy-1.0.5/dnd5apy/models/subclass_level.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/subclass_level_resource.py` & `dnd5apy-1.0.5/dnd5apy/models/subclass_level_resource.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/subclass_level_spellcasting.py` & `dnd5apy-1.0.5/dnd5apy/models/subclass_level_spellcasting.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/subclass_spells.py` & `dnd5apy-1.0.5/dnd5apy/models/subclass_spells.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/models/subrace.py` & `dnd5apy-1.0.5/dnd5apy/models/subrace.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Subrace(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/trait.py` & `dnd5apy-1.0.5/dnd5apy/models/trait.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Trait(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/weapon.py` & `dnd5apy-1.0.5/dnd5apy/models/weapon.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class Weapon(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/weapon_property.py` & `dnd5apy-1.0.5/dnd5apy/models/weapon_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
-from swagger_client.models.api_reference import APIReference  # noqa: F401,E501
+from dnd5apy.models.api_reference import APIReference  # noqa: F401,E501
 
 class WeaponProperty(APIReference):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
```

### Comparing `dnd5apy-1.0.4/dnd5apy/models/weapon_range.py` & `dnd5apy-1.0.5/dnd5apy/models/weapon_range.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/dnd5apy/rest.py` & `dnd5apy-1.0.5/dnd5apy/rest.py`

 * *Files identical despite different names*

### Comparing `dnd5apy-1.0.4/pyproject.toml` & `dnd5apy-1.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dnd5apy"
-version = "1.0.4"
+version = "1.0.5"
 description = "D&D 5e API"
 authors = ["5eBits <team@openapitools.org>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "D&D 5e API"]
 include = ["dnd5epy/py.typed"]
```

### Comparing `dnd5apy-1.0.4/PKG-INFO` & `dnd5apy-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnd5apy
-Version: 1.0.4
+Version: 1.0.5
 Summary: D&D 5e API
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,D&D 5e API
 Author: 5eBits
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -18,15 +18,15 @@
 Requires-Dist: aenum (>=3.1.11)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: urllib3 (>=1.25.3)
 Project-URL: Repository, https://github.com/GIT_USER_ID/GIT_REPO_ID
 Description-Content-Type: text/markdown
 
-# swagger-client
+# dnd5apy
 # Introduction  Welcome to the dnd5eapi, the Dungeons & Dragons 5th Edition API! This documentation should help you familiarize yourself with the resources available and how to consume them with HTTP requests. Read through the getting started section before you dive in. Most of your problems should be solved just by reading through it.  ## Getting Started  Let's make our first API request to the D&D 5th Edition API!  Open up a terminal and use [curl](http://curl.haxx.se/) or [httpie](http://httpie.org/) to make an API request for a resource. You can also scroll through the definitions below and send requests directly from the endpoint documentation!  For example, if you paste and run this `curl` command: ```bash curl -X GET \"https://www.dnd5eapi.co/api/ability-scores/cha\" -H \"Accept: application/json\" ```  We should see a result containing details about the Charisma ability score: ```bash {   \"index\": \"cha\",   \"name\": \"CHA\",   \"full_name\": \"Charisma\",   \"desc\": [     \"Charisma measures your ability to interact effectively with others. It       includes such factors as confidence and eloquence, and it can represent       a charming or commanding personality.\",     \"A Charisma check might arise when you try to influence or entertain       others, when you try to make an impression or tell a convincing lie,       or when you are navigating a tricky social situation. The Deception,       Intimidation, Performance, and Persuasion skills reflect aptitude in       certain kinds of Charisma checks.\"   ],   \"skills\": [     {       \"name\": \"Deception\",       \"index\": \"deception\",       \"url\": \"/api/skills/deception\"     },     {       \"name\": \"Intimidation\",       \"index\": \"intimidation\",       \"url\": \"/api/skills/intimidation\"     },     {       \"name\": \"Performance\",       \"index\": \"performance\",       \"url\": \"/api/skills/performance\"     },     {       \"name\": \"Persuasion\",       \"index\": \"persuasion\",       \"url\": \"/api/skills/persuasion\"     }   ],   \"url\": \"/api/ability-scores/cha\" } ```  ## Authentication  The dnd5eapi is a completely open API. No authentication is required to query and get data. This also means that we've limited what you can do to just `GET`-ing the data. If you find a mistake in the data, feel free to [message us](https://discord.gg/TQuYTv7).  ## GraphQL  This API supports [GraphQL](https://graphql.org/). The GraphQL URL for this API is `https://www.dnd5eapi.co/graphql`. Most of your questions regarding the GraphQL schema can be answered by querying the endpoint with the Apollo sandbox explorer.  ## Schemas  Definitions of all schemas will be accessible in a future update. Two of the most common schemas are described here.  ### `APIReference` Represents a minimal representation of a resource. The detailed representation of the referenced resource can be retrieved by making a request to the referenced `URL`. ``` APIReference {   index     string   name      string   url       string } ``` <hr>  ### `DC` Represents a difficulty check. ``` DC {   dc_type       APIReference   dc_value      number   success_type  \"none\" | \"half\" | \"other\" } ``` <hr>  ### `Damage` Represents damage. ``` Damage {   damage_type     APIReference   damage_dice     string } ``` <hr>  ### `Choice` Represents a choice made by a player. Commonly seen related to decisions made during character creation or combat (e.g.: the description of the cleric class, under **Proficiencies**, states \"Skills: Choose two from History, Insight, Medicine, Persuasion, and Religion\" [[SRD p15]](https://media.wizards.com/2016/downloads/DND/SRD-OGL_V5.1.pdf#page=15)) ``` Choice {   desc      string   choose    number   type      string   from      OptionSet } ``` <hr>  ### `OptionSet` The OptionSet structure provides the options to be chosen from, or sufficient data to fetch and interpret the options. All OptionSets have an `option_set_type` attribute that indicates the structure of the object that contains the options. The possible values are `options_array`, `equipment_category`, and `reference_list`. Other attributes on the OptionSet depend on the value of this attribute. - `options_array`   - `options` (array): An array of Option objects. Each item in the array represents an option that can be chosen. - `equipment_category`   - `equipment_category` (APIReference): A reference to an EquipmentCategory. Each item in the EquipmentCategory's `equipment` array represents one option that can be chosen. - `resource_list`   - `resource_list_url` (string): A reference (by URL) to a collection in the database. The URL may include query parameters. Each item in the resulting ResourceList's `results` array represents one option that can be chosen. <hr>  ### `Option` When the options are given in an `options_array`, each item in the array inherits from the Option structure. All Options have an `option_type` attribute that indicates the structure of the option. The value of this attribute indicates how the option should be handled, and each type has different attributes. The possible values and their corresponding attributes are listed below. - `reference` - A terminal option. Contains a reference to a Document that can be added to the list of options chosen.   - `item` (APIReference): A reference to the chosen item. - `action` - A terminal option. Contains information describing an action, for use within Multiattack actions.   - `action_name` (string): The name of the action, according to its `name` attribute.   - `count` (number | string): The number of times this action can be repeated if this option is chosen.   - `type` (string = `\"melee\" | \"ranged\" | \"ability\" | \"magic\"`, optional): For attack actions that can be either melee, ranged, abilities, or magic. - `multiple` - When this option is chosen, all of its child options are chosen, and must be resolved the same way as a normal option.   - `items` (array): An array of Option objects. All of them must be taken if the option is chosen. - `choice` - A nested choice. If this option is chosen, the Choice structure contained within must be resolved like a normal Choice structure, and the results are the chosen options.   - `choice` (Choice): The Choice to resolve. - `string` - A terminal option. Contains a reference to a string.   - `string` (string): The string. - `ideal` - A terminal option. Contains information about an ideal.   - `desc` (string): A description of the ideal.   - `alignments` (ApiReference[]): A list of alignments of those who might follow the ideal. - `counted_reference` - A terminal option. Contains a reference to something else in the API along with a count.   - `count` (number): Count.   - `of` (ApiReference): Thing being referenced. - `score_prerequisite` - A terminal option. Contains a reference to an ability score and a minimum score.   - `ability_score` (ApiReference): Ability score being referenced.   - `minimum_score` (number): The minimum score required to satisfy the prerequisite. - `ability_bonus` - A terminal option. Contains a reference to an ability score and a bonus   - `ability_score` (ApiReference): Ability score being referenced   - `bonus` (number): The bonus being applied to the ability score - `breath` - A terminal option: Contains a reference to information about a breath attack.   - `name` (string): Name of the breath.   - `dc` (DC): Difficulty check of the breath attack.   - `damage` ([Damage]): Damage dealt by the breath attack, if any. - `damage` - A terminal option. Contains information about damage.   - `damage_type` (ApiReference): Reference to type of damage.   - `damage_dice` (string): Damage expressed in dice (e.g. \"13d6\").   - `notes` (string): Information regarding the damage.  ## FAQ  ### What is the SRD? The SRD, or Systems Reference Document, contains guidelines for publishing content under the OGL. This allows for some of the data for D&D 5e to be open source. The API only covers data that can be found in the SRD. [Here's a link to the full text of the SRD.](https://media.wizards.com/2016/downloads/DND/SRD-OGL_V5.1.pdf)  ### What is the OGL? The Open Game License (OGL) is a public copyright license by Wizards of the Coast that may be used by tabletop role-playing game developers to grant permission to modify, copy, and redistribute some of the content designed for their games, notably game mechanics. However, they must share-alike copies and derivative works. [More information about the OGL can be found here.](https://en.wikipedia.org/wiki/Open_Game_License)  ### A monster, spell, subclass, etc. is missing from the API / Database. Can I add it? Please check if the data is within the SRD. If it is, feel free to open an issue or PR to add it yourself. Otherwise, due to legal reasons, we cannot add it.  ### Can this API be self hosted? Yes it can! You can also host the data yourself if you don't want to use the API at all. You can also make changes and add extra data if you like. However, it is up to you to merge in new changes to the data and API.  #### Can I publish is on <insert platform>? Is this free use? Yes, you can. The API itself is under the [MIT license](https://opensource.org/licenses/MIT), and the underlying data accessible via the API is supported under the SRD and OGL.  # Status Page  The status page for the API can be found here: https://5e-bits.github.io/dnd-uptime/  # Chat  Come hang out with us [on Discord](https://discord.gg/TQuYTv7)!  # Contribute  This API is built from two repositories.   - The repo containing the data lives here: https://github.com/bagelbits/5e-database   - The repo with the API implementation lives here: https://github.com/bagelbits/5e-srd-api  This is a evolving API and having fresh ideas are always welcome! You can open an issue in either repo, open a PR for changes, or just discuss with other users in this discord. 
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 0.1
 - Package version: 1.0.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
```

