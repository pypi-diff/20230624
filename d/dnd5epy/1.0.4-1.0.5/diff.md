# Comparing `tmp/dnd5epy-1.0.4.tar.gz` & `tmp/dnd5epy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnd5epy-1.0.4.tar", max compression
+gzip compressed data, was "dnd5epy-1.0.5.tar", max compression
```

## Comparing `dnd5epy-1.0.4.tar` & `dnd5epy-1.0.5.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rwxr-xr-x   0        0        0    26768 2023-06-24 06:48:23.533042 dnd5epy-1.0.4/README.md
--rwxr-xr-x   0        0        0    19310 2023-06-24 06:48:23.677042 dnd5epy-1.0.4/dnd5epy/__init__.py
--rwxr-xr-x   0        0        0      853 2023-06-24 06:48:23.525042 dnd5epy-1.0.4/dnd5epy/api/__init__.py
--rwxr-xr-x   0        0        0    51804 2023-06-24 06:48:23.541042 dnd5epy-1.0.4/dnd5epy/api/character_data_api.py
--rwxr-xr-x   0        0        0    29903 2023-06-24 06:48:23.637042 dnd5epy-1.0.4/dnd5epy/api/class_api.py
--rwxr-xr-x   0        0        0    37732 2023-06-24 06:48:23.621042 dnd5epy-1.0.4/dnd5epy/api/class_levels_api.py
--rwxr-xr-x   0        0        0    35141 2023-06-24 06:48:23.625042 dnd5epy-1.0.4/dnd5epy/api/class_resource_lists_api.py
--rwxr-xr-x   0        0        0    22842 2023-06-24 06:48:23.617042 dnd5epy-1.0.4/dnd5epy/api/common_api.py
--rwxr-xr-x   0        0        0    37138 2023-06-24 06:48:23.585042 dnd5epy-1.0.4/dnd5epy/api/equipment_api.py
--rwxr-xr-x   0        0        0    16984 2023-06-24 06:48:23.589042 dnd5epy-1.0.4/dnd5epy/api/feats_api.py
--rwxr-xr-x   0        0        0    17805 2023-06-24 06:48:23.537042 dnd5epy-1.0.4/dnd5epy/api/features_api.py
--rwxr-xr-x   0        0        0    30690 2023-06-24 06:48:23.661042 dnd5epy-1.0.4/dnd5epy/api/game_mechanics_api.py
--rwxr-xr-x   0        0        0    23257 2023-06-24 06:48:23.561042 dnd5epy-1.0.4/dnd5epy/api/monsters_api.py
--rwxr-xr-x   0        0        0    35121 2023-06-24 06:48:23.617042 dnd5epy-1.0.4/dnd5epy/api/races_api.py
--rwxr-xr-x   0        0        0    23622 2023-06-24 06:48:23.641042 dnd5epy-1.0.4/dnd5epy/api/rules_api.py
--rwxr-xr-x   0        0        0    23958 2023-06-24 06:48:23.521042 dnd5epy-1.0.4/dnd5epy/api/spells_api.py
--rwxr-xr-x   0        0        0    42870 2023-06-24 06:48:23.601042 dnd5epy-1.0.4/dnd5epy/api/subclasses_api.py
--rwxr-xr-x   0        0        0    29206 2023-06-24 06:48:23.629042 dnd5epy-1.0.4/dnd5epy/api/subraces_api.py
--rwxr-xr-x   0        0        0    16763 2023-06-24 06:48:23.625042 dnd5epy-1.0.4/dnd5epy/api/traits_api.py
--rwxr-xr-x   0        0        0    39816 2023-06-24 06:39:49.942599 dnd5epy-1.0.4/dnd5epy/api_client.py
--rwxr-xr-x   0        0        0      844 2023-06-23 10:05:22.279678 dnd5epy-1.0.4/dnd5epy/api_response.py
--rwxr-xr-x   0        0        0    24362 2023-06-24 06:48:23.625042 dnd5epy-1.0.4/dnd5epy/configuration.py
--rwxr-xr-x   0        0        0    15157 2023-06-23 10:05:22.271678 dnd5epy-1.0.4/dnd5epy/exceptions.py
--rwxr-xr-x   0        0        0    18024 2023-06-24 06:48:23.601042 dnd5epy-1.0.4/dnd5epy/models/__init__.py
--rwxr-xr-x   0        0        0    12243 2023-06-24 06:48:23.553042 dnd5epy-1.0.4/dnd5epy/models/ability_bonus.py
--rwxr-xr-x   0        0        0    12964 2023-06-24 06:48:23.593042 dnd5epy-1.0.4/dnd5epy/models/ability_score.py
--rwxr-xr-x   0        0        0    12340 2023-06-23 10:05:20.527685 dnd5epy-1.0.4/dnd5epy/models/alignment.py
--rwxr-xr-x   0        0        0    12040 2023-06-23 10:05:20.471685 dnd5epy-1.0.4/dnd5epy/models/api_reference.py
--rwxr-xr-x   0        0        0    12409 2023-06-24 06:48:23.529042 dnd5epy-1.0.4/dnd5epy/models/api_reference_list.py
--rwxr-xr-x   0        0        0    12187 2023-06-23 10:05:20.539685 dnd5epy-1.0.4/dnd5epy/models/area_of_effect.py
--rwxr-xr-x   0        0        0    13938 2023-06-24 06:48:23.549042 dnd5epy-1.0.4/dnd5epy/models/armor.py
--rwxr-xr-x   0        0        0    15989 2023-06-24 06:48:23.525042 dnd5epy-1.0.4/dnd5epy/models/background.py
--rwxr-xr-x   0        0        0    11920 2023-06-23 10:05:20.571685 dnd5epy-1.0.4/dnd5epy/models/background_all_of_feature.py
--rwxr-xr-x   0        0        0    12399 2023-06-23 10:05:20.579685 dnd5epy-1.0.4/dnd5epy/models/choice.py
--rwxr-xr-x   0        0        0    12273 2023-06-24 06:48:23.573042 dnd5epy-1.0.4/dnd5epy/models/class_all_of_starting_equipment.py
--rwxr-xr-x   0        0        0    14184 2023-06-24 06:48:23.645042 dnd5epy-1.0.4/dnd5epy/models/class_level.py
--rwxr-xr-x   0        0        0    23774 2023-06-24 06:48:23.561042 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific.py
--rwxr-xr-x   0        0        0    12212 2023-06-23 10:05:20.615684 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of.py
--rwxr-xr-x   0        0        0    12606 2023-06-23 10:05:20.627684 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of1.py
--rwxr-xr-x   0        0        0    12627 2023-06-23 10:05:20.635684 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of10.py
--rwxr-xr-x   0        0        0    11947 2023-06-23 10:05:20.643684 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of11.py
--rwxr-xr-x   0        0        0    12106 2023-06-23 10:05:20.651684 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of2.py
--rwxr-xr-x   0        0        0    12185 2023-06-23 10:05:20.659684 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of3.py
--rwxr-xr-x   0        0        0    12197 2023-06-23 10:05:20.667684 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of4.py
--rwxr-xr-x   0        0        0    12595 2023-06-24 06:48:23.537042 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of5.py
--rwxr-xr-x   0        0        0    12109 2023-06-23 10:05:20.683684 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of5_martial_arts.py
--rwxr-xr-x   0        0        0    11897 2023-06-23 10:05:20.691684 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of6.py
--rwxr-xr-x   0        0        0    12061 2023-06-23 10:05:20.699684 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of7.py
--rwxr-xr-x   0        0        0    12284 2023-06-24 06:48:23.481042 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of8.py
--rwxr-xr-x   0        0        0    12913 2023-06-24 06:48:23.537042 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of9.py
--rwxr-xr-x   0        0        0    12261 2023-06-23 10:05:20.723684 dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of9_creating_spell_slots_inner.py
--rwxr-xr-x   0        0        0    12173 2023-06-23 10:05:20.731684 dnd5epy-1.0.4/dnd5epy/models/condition.py
--rwxr-xr-x   0        0        0    11878 2023-06-23 10:05:20.755684 dnd5epy-1.0.4/dnd5epy/models/cost.py
--rwxr-xr-x   0        0        0    12098 2023-06-24 06:48:23.509042 dnd5epy-1.0.4/dnd5epy/models/damage.py
--rwxr-xr-x   0        0        0    12277 2023-06-24 06:48:23.613042 dnd5epy-1.0.4/dnd5epy/models/damage_at_character_level.py
--rwxr-xr-x   0        0        0    12222 2023-06-24 06:48:23.609042 dnd5epy-1.0.4/dnd5epy/models/damage_at_slot_level.py
--rwxr-xr-x   0        0        0    12181 2023-06-23 10:05:20.827684 dnd5epy-1.0.4/dnd5epy/models/damage_type.py
--rwxr-xr-x   0        0        0    12329 2023-06-24 06:48:23.585042 dnd5epy-1.0.4/dnd5epy/models/dc.py
--rwxr-xr-x   0        0        0    15415 2023-06-24 06:48:23.569042 dnd5epy-1.0.4/dnd5epy/models/equipment.py
--rwxr-xr-x   0        0        0    12744 2023-06-24 06:48:23.545042 dnd5epy-1.0.4/dnd5epy/models/equipment_category.py
--rwxr-xr-x   0        0        0    13969 2023-06-24 06:48:23.629042 dnd5epy-1.0.4/dnd5epy/models/equipment_pack.py
--rwxr-xr-x   0        0        0    11683 2023-06-23 10:05:20.859684 dnd5epy-1.0.4/dnd5epy/models/error_response.py
--rwxr-xr-x   0        0        0    12827 2023-06-24 06:48:23.661042 dnd5epy-1.0.4/dnd5epy/models/feat.py
--rwxr-xr-x   0        0        0    14365 2023-06-24 06:39:44.782569 dnd5epy-1.0.4/dnd5epy/models/feature.py
--rwxr-xr-x   0        0        0    16058 2023-06-24 06:48:23.645042 dnd5epy-1.0.4/dnd5epy/models/feature_all_of_prerequisites_inner.py
--rwxr-xr-x   0        0        0    12016 2023-06-23 10:05:20.907683 dnd5epy-1.0.4/dnd5epy/models/feature_all_of_prerequisites_inner_any_of.py
--rwxr-xr-x   0        0        0    11981 2023-06-23 10:05:20.919683 dnd5epy-1.0.4/dnd5epy/models/feature_all_of_prerequisites_inner_any_of1.py
--rwxr-xr-x   0        0        0    11973 2023-06-23 10:05:20.931683 dnd5epy-1.0.4/dnd5epy/models/feature_all_of_prerequisites_inner_any_of2.py
--rwxr-xr-x   0        0        0    13518 2023-06-24 06:48:23.545042 dnd5epy-1.0.4/dnd5epy/models/gear.py
--rwxr-xr-x   0        0        0    12916 2023-06-23 10:05:20.955683 dnd5epy-1.0.4/dnd5epy/models/language.py
--rwxr-xr-x   0        0        0    13737 2023-06-24 06:48:23.617042 dnd5epy-1.0.4/dnd5epy/models/magic_item.py
--rwxr-xr-x   0        0        0    12235 2023-06-23 10:05:20.983683 dnd5epy-1.0.4/dnd5epy/models/magic_item_all_of_rarity.py
--rwxr-xr-x   0        0        0    12171 2023-06-23 10:05:20.999683 dnd5epy-1.0.4/dnd5epy/models/magic_school.py
--rwxr-xr-x   0        0        0    17618 2023-06-24 06:48:23.541042 dnd5epy-1.0.4/dnd5epy/models/model_class.py
--rwxr-xr-x   0        0        0    24034 2023-06-24 06:48:23.545042 dnd5epy-1.0.4/dnd5epy/models/monster.py
--rwxr-xr-x   0        0        0    12793 2023-06-23 10:05:21.039683 dnd5epy-1.0.4/dnd5epy/models/monster_ability.py
--rwxr-xr-x   0        0        0    14879 2023-06-24 06:48:23.553042 dnd5epy-1.0.4/dnd5epy/models/monster_action.py
--rwxr-xr-x   0        0        0    13296 2023-06-23 10:05:21.059683 dnd5epy-1.0.4/dnd5epy/models/monster_all_of_senses.py
--rwxr-xr-x   0        0        0    12914 2023-06-23 10:05:21.071683 dnd5epy-1.0.4/dnd5epy/models/monster_all_of_speed.py
--rwxr-xr-x   0        0        0    17702 2023-06-24 06:48:23.549042 dnd5epy-1.0.4/dnd5epy/models/monster_armor_class.py
--rwxr-xr-x   0        0        0    12359 2023-06-23 10:05:21.091683 dnd5epy-1.0.4/dnd5epy/models/monster_armor_class_one_of.py
--rwxr-xr-x   0        0        0    12291 2023-06-23 10:05:21.103683 dnd5epy-1.0.4/dnd5epy/models/monster_armor_class_one_of1.py
--rwxr-xr-x   0        0        0    12838 2023-06-24 06:48:23.597042 dnd5epy-1.0.4/dnd5epy/models/monster_armor_class_one_of2.py
--rwxr-xr-x   0        0        0    12653 2023-06-24 06:48:23.597042 dnd5epy-1.0.4/dnd5epy/models/monster_armor_class_one_of3.py
--rwxr-xr-x   0        0        0    12697 2023-06-24 06:48:23.597042 dnd5epy-1.0.4/dnd5epy/models/monster_armor_class_one_of4.py
--rwxr-xr-x   0        0        0    12351 2023-06-24 06:48:23.585042 dnd5epy-1.0.4/dnd5epy/models/monster_attack.py
--rwxr-xr-x   0        0        0    12383 2023-06-23 10:05:21.167683 dnd5epy-1.0.4/dnd5epy/models/monster_multi_attack_action.py
--rwxr-xr-x   0        0        0    12207 2023-06-24 06:48:23.573042 dnd5epy-1.0.4/dnd5epy/models/monster_proficiency.py
--rwxr-xr-x   0        0        0    13165 2023-06-23 10:05:21.195682 dnd5epy-1.0.4/dnd5epy/models/monster_sense.py
--rwxr-xr-x   0        0        0    13485 2023-06-24 06:48:23.513042 dnd5epy-1.0.4/dnd5epy/models/monster_special_ability.py
--rwxr-xr-x   0        0        0    12276 2023-06-24 06:48:23.545042 dnd5epy-1.0.4/dnd5epy/models/monster_spell.py
--rwxr-xr-x   0        0        0    13220 2023-06-24 06:48:23.529042 dnd5epy-1.0.4/dnd5epy/models/monster_spellcasting.py
--rwxr-xr-x   0        0        0    12359 2023-06-23 10:05:21.239682 dnd5epy-1.0.4/dnd5epy/models/monster_usage.py
--rwxr-xr-x   0        0        0    14386 2023-06-24 06:48:23.573042 dnd5epy-1.0.4/dnd5epy/models/multiclassing.py
--rwxr-xr-x   0        0        0    20749 2023-06-24 06:48:23.585042 dnd5epy-1.0.4/dnd5epy/models/option.py
--rwxr-xr-x   0        0        0    12146 2023-06-24 06:48:23.553042 dnd5epy-1.0.4/dnd5epy/models/option_one_of.py
--rwxr-xr-x   0        0        0    12688 2023-06-23 10:05:21.271682 dnd5epy-1.0.4/dnd5epy/models/option_one_of1.py
--rwxr-xr-x   0        0        0    12541 2023-06-24 06:48:23.637042 dnd5epy-1.0.4/dnd5epy/models/option_one_of10.py
--rwxr-xr-x   0        0        0    12282 2023-06-23 10:05:21.295682 dnd5epy-1.0.4/dnd5epy/models/option_one_of2.py
--rwxr-xr-x   0        0        0    12106 2023-06-23 10:05:21.303682 dnd5epy-1.0.4/dnd5epy/models/option_one_of3.py
--rwxr-xr-x   0        0        0    11921 2023-06-23 10:05:21.311682 dnd5epy-1.0.4/dnd5epy/models/option_one_of4.py
--rwxr-xr-x   0        0        0    12605 2023-06-24 06:48:23.633042 dnd5epy-1.0.4/dnd5epy/models/option_one_of5.py
--rwxr-xr-x   0        0        0    12301 2023-06-24 06:48:23.633042 dnd5epy-1.0.4/dnd5epy/models/option_one_of6.py
--rwxr-xr-x   0        0        0    12482 2023-06-24 06:48:23.633042 dnd5epy-1.0.4/dnd5epy/models/option_one_of7.py
--rwxr-xr-x   0        0        0    12446 2023-06-23 10:05:21.355682 dnd5epy-1.0.4/dnd5epy/models/option_one_of8.py
--rwxr-xr-x   0        0        0    12818 2023-06-24 06:48:23.637042 dnd5epy-1.0.4/dnd5epy/models/option_one_of9.py
--rwxr-xr-x   0        0        0    15533 2023-06-24 06:48:23.645042 dnd5epy-1.0.4/dnd5epy/models/option_set.py
--rwxr-xr-x   0        0        0    12445 2023-06-23 10:05:21.407682 dnd5epy-1.0.4/dnd5epy/models/option_set_one_of.py
--rwxr-xr-x   0        0        0    12324 2023-06-24 06:48:23.505042 dnd5epy-1.0.4/dnd5epy/models/option_set_one_of1.py
--rwxr-xr-x   0        0        0    12035 2023-06-23 10:05:21.427682 dnd5epy-1.0.4/dnd5epy/models/option_set_one_of2.py
--rwxr-xr-x   0        0        0    12330 2023-06-24 06:48:23.645042 dnd5epy-1.0.4/dnd5epy/models/prerequisite.py
--rwxr-xr-x   0        0        0    12133 2023-06-23 10:05:21.443681 dnd5epy-1.0.4/dnd5epy/models/prerequisite_ability_score.py
--rwxr-xr-x   0        0        0    13810 2023-06-24 06:48:23.517042 dnd5epy-1.0.4/dnd5epy/models/proficiency.py
--rwxr-xr-x   0        0        0    12180 2023-06-23 10:05:21.463681 dnd5epy-1.0.4/dnd5epy/models/proficiency_all_of_reference.py
--rwxr-xr-x   0        0        0    16802 2023-06-24 06:48:23.501042 dnd5epy-1.0.4/dnd5epy/models/race.py
--rwxr-xr-x   0        0        0    11833 2023-06-23 10:05:21.503681 dnd5epy-1.0.4/dnd5epy/models/resource_description.py
--rwxr-xr-x   0        0        0    12801 2023-06-24 06:48:23.589042 dnd5epy-1.0.4/dnd5epy/models/rule.py
--rwxr-xr-x   0        0        0    12161 2023-06-23 10:05:21.523681 dnd5epy-1.0.4/dnd5epy/models/rule_section.py
--rwxr-xr-x   0        0        0    12579 2023-06-24 06:48:23.581042 dnd5epy-1.0.4/dnd5epy/models/skill.py
--rwxr-xr-x   0        0        0    16675 2023-06-24 06:48:23.581042 dnd5epy-1.0.4/dnd5epy/models/spell.py
--rwxr-xr-x   0        0        0    15093 2023-06-24 06:48:23.553042 dnd5epy-1.0.4/dnd5epy/models/spell_all_of_damage.py
--rwxr-xr-x   0        0        0    12210 2023-06-23 10:05:21.563681 dnd5epy-1.0.4/dnd5epy/models/spell_prerequisite.py
--rwxr-xr-x   0        0        0    13070 2023-06-24 06:48:23.501042 dnd5epy-1.0.4/dnd5epy/models/spellcasting.py
--rwxr-xr-x   0        0        0    11959 2023-06-23 10:05:21.579681 dnd5epy-1.0.4/dnd5epy/models/spellcasting_info_inner.py
--rwxr-xr-x   0        0        0    12225 2023-06-23 10:05:21.591681 dnd5epy-1.0.4/dnd5epy/models/spellcasting_spellcasting_ability.py
--rwxr-xr-x   0        0        0    13561 2023-06-24 06:48:23.545042 dnd5epy-1.0.4/dnd5epy/models/subclass.py
--rwxr-xr-x   0        0        0    12667 2023-06-24 06:48:23.505042 dnd5epy-1.0.4/dnd5epy/models/subclass_all_of_spells.py
--rwxr-xr-x   0        0        0    13958 2023-06-24 06:48:23.601042 dnd5epy-1.0.4/dnd5epy/models/subclass_level.py
--rwxr-xr-x   0        0        0    13264 2023-06-24 06:48:23.565042 dnd5epy-1.0.4/dnd5epy/models/subclass_level_resource.py
--rwxr-xr-x   0        0        0    13484 2023-06-23 10:05:21.631681 dnd5epy-1.0.4/dnd5epy/models/subclass_level_spellcasting.py
--rwxr-xr-x   0        0        0    15638 2023-06-24 06:48:23.545042 dnd5epy-1.0.4/dnd5epy/models/subrace.py
--rwxr-xr-x   0        0        0    12081 2023-06-23 10:05:21.651681 dnd5epy-1.0.4/dnd5epy/models/subrace_all_of_race.py
--rwxr-xr-x   0        0        0    15306 2023-06-24 06:48:23.629042 dnd5epy-1.0.4/dnd5epy/models/trait.py
--rwxr-xr-x   0        0        0    15626 2023-06-24 06:48:23.525042 dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific.py
--rwxr-xr-x   0        0        0    12883 2023-06-24 06:48:23.573042 dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific_one_of.py
--rwxr-xr-x   0        0        0    13793 2023-06-24 06:48:23.553042 dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon.py
--rwxr-xr-x   0        0        0    12537 2023-06-24 06:48:23.661042 dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_damage.py
--rwxr-xr-x   0        0        0    12103 2023-06-23 10:05:21.707680 dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_usage.py
--rwxr-xr-x   0        0        0    12248 2023-06-23 10:05:21.715680 dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific_one_of_damage_type.py
--rwxr-xr-x   0        0        0    15444 2023-06-24 06:48:23.625042 dnd5epy-1.0.4/dnd5epy/models/weapon.py
--rwxr-xr-x   0        0        0    11996 2023-06-23 10:05:21.727680 dnd5epy-1.0.4/dnd5epy/models/weapon_all_of_range.py
--rwxr-xr-x   0        0        0    12210 2023-06-23 10:05:21.735680 dnd5epy-1.0.4/dnd5epy/models/weapon_property.py
--rwxr-xr-x   0        0        0        0 2023-06-23 10:05:22.247678 dnd5epy-1.0.4/dnd5epy/py.typed
--rwxr-xr-x   0        0        0    22720 2023-06-24 06:48:23.661042 dnd5epy-1.0.4/dnd5epy/rest.py
--rwxr-xr-x   0        0        0      691 2023-06-24 06:52:28.717248 dnd5epy-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    27642 1970-01-01 00:00:00.000000 dnd5epy-1.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0    26768 2023-06-24 06:48:23.533042 dnd5epy-1.0.5/README.md
+-rwxr-xr-x   0        0        0    19310 2023-06-24 06:48:23.677042 dnd5epy-1.0.5/dnd5epy/__init__.py
+-rwxr-xr-x   0        0        0      853 2023-06-24 06:48:23.525042 dnd5epy-1.0.5/dnd5epy/api/__init__.py
+-rwxr-xr-x   0        0        0    51804 2023-06-24 06:48:23.541042 dnd5epy-1.0.5/dnd5epy/api/character_data_api.py
+-rwxr-xr-x   0        0        0    29903 2023-06-24 06:48:23.637042 dnd5epy-1.0.5/dnd5epy/api/class_api.py
+-rwxr-xr-x   0        0        0    37732 2023-06-24 06:48:23.621042 dnd5epy-1.0.5/dnd5epy/api/class_levels_api.py
+-rwxr-xr-x   0        0        0    35141 2023-06-24 06:48:23.625042 dnd5epy-1.0.5/dnd5epy/api/class_resource_lists_api.py
+-rwxr-xr-x   0        0        0    22842 2023-06-24 06:48:23.617042 dnd5epy-1.0.5/dnd5epy/api/common_api.py
+-rwxr-xr-x   0        0        0    37138 2023-06-24 06:48:23.585042 dnd5epy-1.0.5/dnd5epy/api/equipment_api.py
+-rwxr-xr-x   0        0        0    16984 2023-06-24 06:48:23.589042 dnd5epy-1.0.5/dnd5epy/api/feats_api.py
+-rwxr-xr-x   0        0        0    17805 2023-06-24 06:48:23.537042 dnd5epy-1.0.5/dnd5epy/api/features_api.py
+-rwxr-xr-x   0        0        0    30690 2023-06-24 06:48:23.661042 dnd5epy-1.0.5/dnd5epy/api/game_mechanics_api.py
+-rwxr-xr-x   0        0        0    23257 2023-06-24 06:48:23.561042 dnd5epy-1.0.5/dnd5epy/api/monsters_api.py
+-rwxr-xr-x   0        0        0    35121 2023-06-24 06:48:23.617042 dnd5epy-1.0.5/dnd5epy/api/races_api.py
+-rwxr-xr-x   0        0        0    23622 2023-06-24 06:48:23.641042 dnd5epy-1.0.5/dnd5epy/api/rules_api.py
+-rwxr-xr-x   0        0        0    23958 2023-06-24 06:48:23.521042 dnd5epy-1.0.5/dnd5epy/api/spells_api.py
+-rwxr-xr-x   0        0        0    42870 2023-06-24 06:48:23.601042 dnd5epy-1.0.5/dnd5epy/api/subclasses_api.py
+-rwxr-xr-x   0        0        0    29206 2023-06-24 06:48:23.629042 dnd5epy-1.0.5/dnd5epy/api/subraces_api.py
+-rwxr-xr-x   0        0        0    16763 2023-06-24 06:48:23.625042 dnd5epy-1.0.5/dnd5epy/api/traits_api.py
+-rwxr-xr-x   0        0        0    39816 2023-06-24 06:39:49.942599 dnd5epy-1.0.5/dnd5epy/api_client.py
+-rwxr-xr-x   0        0        0      844 2023-06-23 10:05:22.279678 dnd5epy-1.0.5/dnd5epy/api_response.py
+-rwxr-xr-x   0        0        0    24362 2023-06-24 06:48:23.625042 dnd5epy-1.0.5/dnd5epy/configuration.py
+-rwxr-xr-x   0        0        0    15157 2023-06-23 10:05:22.271678 dnd5epy-1.0.5/dnd5epy/exceptions.py
+-rwxr-xr-x   0        0        0    18024 2023-06-24 06:48:23.601042 dnd5epy-1.0.5/dnd5epy/models/__init__.py
+-rwxr-xr-x   0        0        0    12243 2023-06-24 06:48:23.553042 dnd5epy-1.0.5/dnd5epy/models/ability_bonus.py
+-rwxr-xr-x   0        0        0    12964 2023-06-24 06:48:23.593042 dnd5epy-1.0.5/dnd5epy/models/ability_score.py
+-rwxr-xr-x   0        0        0    12340 2023-06-23 10:05:20.527685 dnd5epy-1.0.5/dnd5epy/models/alignment.py
+-rwxr-xr-x   0        0        0    12040 2023-06-23 10:05:20.471685 dnd5epy-1.0.5/dnd5epy/models/api_reference.py
+-rwxr-xr-x   0        0        0    12409 2023-06-24 06:48:23.529042 dnd5epy-1.0.5/dnd5epy/models/api_reference_list.py
+-rwxr-xr-x   0        0        0    12187 2023-06-23 10:05:20.539685 dnd5epy-1.0.5/dnd5epy/models/area_of_effect.py
+-rwxr-xr-x   0        0        0    13938 2023-06-24 06:48:23.549042 dnd5epy-1.0.5/dnd5epy/models/armor.py
+-rwxr-xr-x   0        0        0    15989 2023-06-24 06:48:23.525042 dnd5epy-1.0.5/dnd5epy/models/background.py
+-rwxr-xr-x   0        0        0    11920 2023-06-23 10:05:20.571685 dnd5epy-1.0.5/dnd5epy/models/background_all_of_feature.py
+-rwxr-xr-x   0        0        0    12399 2023-06-23 10:05:20.579685 dnd5epy-1.0.5/dnd5epy/models/choice.py
+-rwxr-xr-x   0        0        0    12273 2023-06-24 06:48:23.573042 dnd5epy-1.0.5/dnd5epy/models/class_all_of_starting_equipment.py
+-rwxr-xr-x   0        0        0    14184 2023-06-24 06:48:23.645042 dnd5epy-1.0.5/dnd5epy/models/class_level.py
+-rwxr-xr-x   0        0        0    23774 2023-06-24 06:48:23.561042 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific.py
+-rwxr-xr-x   0        0        0    12212 2023-06-23 10:05:20.615684 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of.py
+-rwxr-xr-x   0        0        0    12606 2023-06-23 10:05:20.627684 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of1.py
+-rwxr-xr-x   0        0        0    12627 2023-06-23 10:05:20.635684 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of10.py
+-rwxr-xr-x   0        0        0    11947 2023-06-23 10:05:20.643684 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of11.py
+-rwxr-xr-x   0        0        0    12106 2023-06-23 10:05:20.651684 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of2.py
+-rwxr-xr-x   0        0        0    12185 2023-06-23 10:05:20.659684 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of3.py
+-rwxr-xr-x   0        0        0    12197 2023-06-23 10:05:20.667684 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of4.py
+-rwxr-xr-x   0        0        0    12595 2023-06-24 06:48:23.537042 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of5.py
+-rwxr-xr-x   0        0        0    12109 2023-06-23 10:05:20.683684 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of5_martial_arts.py
+-rwxr-xr-x   0        0        0    11897 2023-06-23 10:05:20.691684 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of6.py
+-rwxr-xr-x   0        0        0    12061 2023-06-23 10:05:20.699684 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of7.py
+-rwxr-xr-x   0        0        0    12284 2023-06-24 06:48:23.481042 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of8.py
+-rwxr-xr-x   0        0        0    12913 2023-06-24 06:48:23.537042 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of9.py
+-rwxr-xr-x   0        0        0    12261 2023-06-23 10:05:20.723684 dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of9_creating_spell_slots_inner.py
+-rwxr-xr-x   0        0        0    12173 2023-06-23 10:05:20.731684 dnd5epy-1.0.5/dnd5epy/models/condition.py
+-rwxr-xr-x   0        0        0    11878 2023-06-23 10:05:20.755684 dnd5epy-1.0.5/dnd5epy/models/cost.py
+-rwxr-xr-x   0        0        0    12098 2023-06-24 06:48:23.509042 dnd5epy-1.0.5/dnd5epy/models/damage.py
+-rwxr-xr-x   0        0        0    12277 2023-06-24 06:48:23.613042 dnd5epy-1.0.5/dnd5epy/models/damage_at_character_level.py
+-rwxr-xr-x   0        0        0    12222 2023-06-24 06:48:23.609042 dnd5epy-1.0.5/dnd5epy/models/damage_at_slot_level.py
+-rwxr-xr-x   0        0        0    12181 2023-06-23 10:05:20.827684 dnd5epy-1.0.5/dnd5epy/models/damage_type.py
+-rwxr-xr-x   0        0        0    12329 2023-06-24 06:48:23.585042 dnd5epy-1.0.5/dnd5epy/models/dc.py
+-rwxr-xr-x   0        0        0    15415 2023-06-24 06:48:23.569042 dnd5epy-1.0.5/dnd5epy/models/equipment.py
+-rwxr-xr-x   0        0        0    12744 2023-06-24 06:48:23.545042 dnd5epy-1.0.5/dnd5epy/models/equipment_category.py
+-rwxr-xr-x   0        0        0    13969 2023-06-24 06:48:23.629042 dnd5epy-1.0.5/dnd5epy/models/equipment_pack.py
+-rwxr-xr-x   0        0        0    11683 2023-06-23 10:05:20.859684 dnd5epy-1.0.5/dnd5epy/models/error_response.py
+-rwxr-xr-x   0        0        0    12827 2023-06-24 06:48:23.661042 dnd5epy-1.0.5/dnd5epy/models/feat.py
+-rwxr-xr-x   0        0        0    14365 2023-06-24 06:39:44.782569 dnd5epy-1.0.5/dnd5epy/models/feature.py
+-rwxr-xr-x   0        0        0    16058 2023-06-24 06:48:23.645042 dnd5epy-1.0.5/dnd5epy/models/feature_all_of_prerequisites_inner.py
+-rwxr-xr-x   0        0        0    12016 2023-06-23 10:05:20.907683 dnd5epy-1.0.5/dnd5epy/models/feature_all_of_prerequisites_inner_any_of.py
+-rwxr-xr-x   0        0        0    11981 2023-06-23 10:05:20.919683 dnd5epy-1.0.5/dnd5epy/models/feature_all_of_prerequisites_inner_any_of1.py
+-rwxr-xr-x   0        0        0    11973 2023-06-23 10:05:20.931683 dnd5epy-1.0.5/dnd5epy/models/feature_all_of_prerequisites_inner_any_of2.py
+-rwxr-xr-x   0        0        0    13518 2023-06-24 06:48:23.545042 dnd5epy-1.0.5/dnd5epy/models/gear.py
+-rwxr-xr-x   0        0        0    12916 2023-06-23 10:05:20.955683 dnd5epy-1.0.5/dnd5epy/models/language.py
+-rwxr-xr-x   0        0        0    13737 2023-06-24 06:48:23.617042 dnd5epy-1.0.5/dnd5epy/models/magic_item.py
+-rwxr-xr-x   0        0        0    12235 2023-06-23 10:05:20.983683 dnd5epy-1.0.5/dnd5epy/models/magic_item_all_of_rarity.py
+-rwxr-xr-x   0        0        0    12171 2023-06-23 10:05:20.999683 dnd5epy-1.0.5/dnd5epy/models/magic_school.py
+-rwxr-xr-x   0        0        0    17618 2023-06-24 06:48:23.541042 dnd5epy-1.0.5/dnd5epy/models/model_class.py
+-rwxr-xr-x   0        0        0    24034 2023-06-24 06:48:23.545042 dnd5epy-1.0.5/dnd5epy/models/monster.py
+-rwxr-xr-x   0        0        0    12793 2023-06-23 10:05:21.039683 dnd5epy-1.0.5/dnd5epy/models/monster_ability.py
+-rwxr-xr-x   0        0        0    14879 2023-06-24 06:48:23.553042 dnd5epy-1.0.5/dnd5epy/models/monster_action.py
+-rwxr-xr-x   0        0        0    13296 2023-06-23 10:05:21.059683 dnd5epy-1.0.5/dnd5epy/models/monster_all_of_senses.py
+-rwxr-xr-x   0        0        0    12914 2023-06-23 10:05:21.071683 dnd5epy-1.0.5/dnd5epy/models/monster_all_of_speed.py
+-rwxr-xr-x   0        0        0    17702 2023-06-24 06:48:23.549042 dnd5epy-1.0.5/dnd5epy/models/monster_armor_class.py
+-rwxr-xr-x   0        0        0    12359 2023-06-23 10:05:21.091683 dnd5epy-1.0.5/dnd5epy/models/monster_armor_class_one_of.py
+-rwxr-xr-x   0        0        0    12291 2023-06-23 10:05:21.103683 dnd5epy-1.0.5/dnd5epy/models/monster_armor_class_one_of1.py
+-rwxr-xr-x   0        0        0    12838 2023-06-24 06:48:23.597042 dnd5epy-1.0.5/dnd5epy/models/monster_armor_class_one_of2.py
+-rwxr-xr-x   0        0        0    12653 2023-06-24 06:48:23.597042 dnd5epy-1.0.5/dnd5epy/models/monster_armor_class_one_of3.py
+-rwxr-xr-x   0        0        0    12697 2023-06-24 06:48:23.597042 dnd5epy-1.0.5/dnd5epy/models/monster_armor_class_one_of4.py
+-rwxr-xr-x   0        0        0    12351 2023-06-24 06:48:23.585042 dnd5epy-1.0.5/dnd5epy/models/monster_attack.py
+-rwxr-xr-x   0        0        0    12383 2023-06-23 10:05:21.167683 dnd5epy-1.0.5/dnd5epy/models/monster_multi_attack_action.py
+-rwxr-xr-x   0        0        0    12207 2023-06-24 06:48:23.573042 dnd5epy-1.0.5/dnd5epy/models/monster_proficiency.py
+-rwxr-xr-x   0        0        0    13165 2023-06-23 10:05:21.195682 dnd5epy-1.0.5/dnd5epy/models/monster_sense.py
+-rwxr-xr-x   0        0        0    13485 2023-06-24 06:48:23.513042 dnd5epy-1.0.5/dnd5epy/models/monster_special_ability.py
+-rwxr-xr-x   0        0        0    12276 2023-06-24 06:48:23.545042 dnd5epy-1.0.5/dnd5epy/models/monster_spell.py
+-rwxr-xr-x   0        0        0    13220 2023-06-24 06:48:23.529042 dnd5epy-1.0.5/dnd5epy/models/monster_spellcasting.py
+-rwxr-xr-x   0        0        0    12359 2023-06-23 10:05:21.239682 dnd5epy-1.0.5/dnd5epy/models/monster_usage.py
+-rwxr-xr-x   0        0        0    14386 2023-06-24 06:48:23.573042 dnd5epy-1.0.5/dnd5epy/models/multiclassing.py
+-rwxr-xr-x   0        0        0    20749 2023-06-24 06:48:23.585042 dnd5epy-1.0.5/dnd5epy/models/option.py
+-rwxr-xr-x   0        0        0    12146 2023-06-24 06:48:23.553042 dnd5epy-1.0.5/dnd5epy/models/option_one_of.py
+-rwxr-xr-x   0        0        0    12688 2023-06-23 10:05:21.271682 dnd5epy-1.0.5/dnd5epy/models/option_one_of1.py
+-rwxr-xr-x   0        0        0    12541 2023-06-24 06:48:23.637042 dnd5epy-1.0.5/dnd5epy/models/option_one_of10.py
+-rwxr-xr-x   0        0        0    12282 2023-06-23 10:05:21.295682 dnd5epy-1.0.5/dnd5epy/models/option_one_of2.py
+-rwxr-xr-x   0        0        0    12106 2023-06-23 10:05:21.303682 dnd5epy-1.0.5/dnd5epy/models/option_one_of3.py
+-rwxr-xr-x   0        0        0    11921 2023-06-23 10:05:21.311682 dnd5epy-1.0.5/dnd5epy/models/option_one_of4.py
+-rwxr-xr-x   0        0        0    12605 2023-06-24 06:48:23.633042 dnd5epy-1.0.5/dnd5epy/models/option_one_of5.py
+-rwxr-xr-x   0        0        0    12301 2023-06-24 06:48:23.633042 dnd5epy-1.0.5/dnd5epy/models/option_one_of6.py
+-rwxr-xr-x   0        0        0    12482 2023-06-24 06:48:23.633042 dnd5epy-1.0.5/dnd5epy/models/option_one_of7.py
+-rwxr-xr-x   0        0        0    12439 2023-06-24 06:56:19.501797 dnd5epy-1.0.5/dnd5epy/models/option_one_of8.py
+-rwxr-xr-x   0        0        0    12818 2023-06-24 06:48:23.637042 dnd5epy-1.0.5/dnd5epy/models/option_one_of9.py
+-rwxr-xr-x   0        0        0    15533 2023-06-24 06:48:23.645042 dnd5epy-1.0.5/dnd5epy/models/option_set.py
+-rwxr-xr-x   0        0        0    12445 2023-06-23 10:05:21.407682 dnd5epy-1.0.5/dnd5epy/models/option_set_one_of.py
+-rwxr-xr-x   0        0        0    12324 2023-06-24 06:48:23.505042 dnd5epy-1.0.5/dnd5epy/models/option_set_one_of1.py
+-rwxr-xr-x   0        0        0    12035 2023-06-23 10:05:21.427682 dnd5epy-1.0.5/dnd5epy/models/option_set_one_of2.py
+-rwxr-xr-x   0        0        0    12330 2023-06-24 06:48:23.645042 dnd5epy-1.0.5/dnd5epy/models/prerequisite.py
+-rwxr-xr-x   0        0        0    12133 2023-06-23 10:05:21.443681 dnd5epy-1.0.5/dnd5epy/models/prerequisite_ability_score.py
+-rwxr-xr-x   0        0        0    13810 2023-06-24 06:48:23.517042 dnd5epy-1.0.5/dnd5epy/models/proficiency.py
+-rwxr-xr-x   0        0        0    12180 2023-06-23 10:05:21.463681 dnd5epy-1.0.5/dnd5epy/models/proficiency_all_of_reference.py
+-rwxr-xr-x   0        0        0    16802 2023-06-24 06:48:23.501042 dnd5epy-1.0.5/dnd5epy/models/race.py
+-rwxr-xr-x   0        0        0    11833 2023-06-23 10:05:21.503681 dnd5epy-1.0.5/dnd5epy/models/resource_description.py
+-rwxr-xr-x   0        0        0    12801 2023-06-24 06:48:23.589042 dnd5epy-1.0.5/dnd5epy/models/rule.py
+-rwxr-xr-x   0        0        0    12161 2023-06-23 10:05:21.523681 dnd5epy-1.0.5/dnd5epy/models/rule_section.py
+-rwxr-xr-x   0        0        0    12579 2023-06-24 06:48:23.581042 dnd5epy-1.0.5/dnd5epy/models/skill.py
+-rwxr-xr-x   0        0        0    16675 2023-06-24 06:48:23.581042 dnd5epy-1.0.5/dnd5epy/models/spell.py
+-rwxr-xr-x   0        0        0    15093 2023-06-24 06:48:23.553042 dnd5epy-1.0.5/dnd5epy/models/spell_all_of_damage.py
+-rwxr-xr-x   0        0        0    12210 2023-06-23 10:05:21.563681 dnd5epy-1.0.5/dnd5epy/models/spell_prerequisite.py
+-rwxr-xr-x   0        0        0    13070 2023-06-24 06:48:23.501042 dnd5epy-1.0.5/dnd5epy/models/spellcasting.py
+-rwxr-xr-x   0        0        0    11959 2023-06-23 10:05:21.579681 dnd5epy-1.0.5/dnd5epy/models/spellcasting_info_inner.py
+-rwxr-xr-x   0        0        0    12225 2023-06-23 10:05:21.591681 dnd5epy-1.0.5/dnd5epy/models/spellcasting_spellcasting_ability.py
+-rwxr-xr-x   0        0        0    13561 2023-06-24 06:48:23.545042 dnd5epy-1.0.5/dnd5epy/models/subclass.py
+-rwxr-xr-x   0        0        0    12667 2023-06-24 06:48:23.505042 dnd5epy-1.0.5/dnd5epy/models/subclass_all_of_spells.py
+-rwxr-xr-x   0        0        0    13958 2023-06-24 06:48:23.601042 dnd5epy-1.0.5/dnd5epy/models/subclass_level.py
+-rwxr-xr-x   0        0        0    13264 2023-06-24 06:48:23.565042 dnd5epy-1.0.5/dnd5epy/models/subclass_level_resource.py
+-rwxr-xr-x   0        0        0    13484 2023-06-23 10:05:21.631681 dnd5epy-1.0.5/dnd5epy/models/subclass_level_spellcasting.py
+-rwxr-xr-x   0        0        0    15638 2023-06-24 06:48:23.545042 dnd5epy-1.0.5/dnd5epy/models/subrace.py
+-rwxr-xr-x   0        0        0    12081 2023-06-23 10:05:21.651681 dnd5epy-1.0.5/dnd5epy/models/subrace_all_of_race.py
+-rwxr-xr-x   0        0        0    15306 2023-06-24 06:48:23.629042 dnd5epy-1.0.5/dnd5epy/models/trait.py
+-rwxr-xr-x   0        0        0    15626 2023-06-24 06:48:23.525042 dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific.py
+-rwxr-xr-x   0        0        0    12883 2023-06-24 06:48:23.573042 dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific_one_of.py
+-rwxr-xr-x   0        0        0    13793 2023-06-24 06:48:23.553042 dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon.py
+-rwxr-xr-x   0        0        0    12537 2023-06-24 06:48:23.661042 dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_damage.py
+-rwxr-xr-x   0        0        0    12103 2023-06-23 10:05:21.707680 dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_usage.py
+-rwxr-xr-x   0        0        0    12248 2023-06-23 10:05:21.715680 dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific_one_of_damage_type.py
+-rwxr-xr-x   0        0        0    15444 2023-06-24 06:48:23.625042 dnd5epy-1.0.5/dnd5epy/models/weapon.py
+-rwxr-xr-x   0        0        0    11996 2023-06-23 10:05:21.727680 dnd5epy-1.0.5/dnd5epy/models/weapon_all_of_range.py
+-rwxr-xr-x   0        0        0    12210 2023-06-23 10:05:21.735680 dnd5epy-1.0.5/dnd5epy/models/weapon_property.py
+-rwxr-xr-x   0        0        0        0 2023-06-23 10:05:22.247678 dnd5epy-1.0.5/dnd5epy/py.typed
+-rwxr-xr-x   0        0        0    22720 2023-06-24 06:48:23.661042 dnd5epy-1.0.5/dnd5epy/rest.py
+-rwxr-xr-x   0        0        0      691 2023-06-24 06:55:25.261644 dnd5epy-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    27642 1970-01-01 00:00:00.000000 dnd5epy-1.0.5/PKG-INFO
```

### Comparing `dnd5epy-1.0.4/README.md` & `dnd5epy-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/__init__.py` & `dnd5epy-1.0.5/dnd5epy/__init__.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/__init__.py` & `dnd5epy-1.0.5/dnd5epy/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/character_data_api.py` & `dnd5epy-1.0.5/dnd5epy/api/character_data_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/class_api.py` & `dnd5epy-1.0.5/dnd5epy/api/class_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/class_levels_api.py` & `dnd5epy-1.0.5/dnd5epy/api/class_levels_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/class_resource_lists_api.py` & `dnd5epy-1.0.5/dnd5epy/api/class_resource_lists_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/common_api.py` & `dnd5epy-1.0.5/dnd5epy/api/common_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/equipment_api.py` & `dnd5epy-1.0.5/dnd5epy/api/equipment_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/feats_api.py` & `dnd5epy-1.0.5/dnd5epy/api/feats_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/features_api.py` & `dnd5epy-1.0.5/dnd5epy/api/features_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/game_mechanics_api.py` & `dnd5epy-1.0.5/dnd5epy/api/game_mechanics_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/monsters_api.py` & `dnd5epy-1.0.5/dnd5epy/api/monsters_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/races_api.py` & `dnd5epy-1.0.5/dnd5epy/api/races_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/rules_api.py` & `dnd5epy-1.0.5/dnd5epy/api/rules_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/spells_api.py` & `dnd5epy-1.0.5/dnd5epy/api/spells_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/subclasses_api.py` & `dnd5epy-1.0.5/dnd5epy/api/subclasses_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/subraces_api.py` & `dnd5epy-1.0.5/dnd5epy/api/subraces_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api/traits_api.py` & `dnd5epy-1.0.5/dnd5epy/api/traits_api.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api_client.py` & `dnd5epy-1.0.5/dnd5epy/api_client.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/api_response.py` & `dnd5epy-1.0.5/dnd5epy/api_response.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/configuration.py` & `dnd5epy-1.0.5/dnd5epy/configuration.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/exceptions.py` & `dnd5epy-1.0.5/dnd5epy/exceptions.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/__init__.py` & `dnd5epy-1.0.5/dnd5epy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/ability_bonus.py` & `dnd5epy-1.0.5/dnd5epy/models/ability_bonus.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/ability_score.py` & `dnd5epy-1.0.5/dnd5epy/models/ability_score.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/alignment.py` & `dnd5epy-1.0.5/dnd5epy/models/alignment.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/api_reference.py` & `dnd5epy-1.0.5/dnd5epy/models/api_reference.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/api_reference_list.py` & `dnd5epy-1.0.5/dnd5epy/models/api_reference_list.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/area_of_effect.py` & `dnd5epy-1.0.5/dnd5epy/models/area_of_effect.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/armor.py` & `dnd5epy-1.0.5/dnd5epy/models/armor.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/background.py` & `dnd5epy-1.0.5/dnd5epy/models/background.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/background_all_of_feature.py` & `dnd5epy-1.0.5/dnd5epy/models/background_all_of_feature.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/choice.py` & `dnd5epy-1.0.5/dnd5epy/models/choice.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_all_of_starting_equipment.py` & `dnd5epy-1.0.5/dnd5epy/models/class_all_of_starting_equipment.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of1.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of1.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of10.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of10.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of11.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of11.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of2.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of2.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of3.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of3.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of4.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of4.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of5.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of5.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of5_martial_arts.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of5_martial_arts.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of6.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of6.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of7.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of7.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of8.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of8.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of9.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of9.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/class_level_class_specific_any_of9_creating_spell_slots_inner.py` & `dnd5epy-1.0.5/dnd5epy/models/class_level_class_specific_any_of9_creating_spell_slots_inner.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/condition.py` & `dnd5epy-1.0.5/dnd5epy/models/condition.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/cost.py` & `dnd5epy-1.0.5/dnd5epy/models/cost.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/damage.py` & `dnd5epy-1.0.5/dnd5epy/models/damage.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/damage_at_character_level.py` & `dnd5epy-1.0.5/dnd5epy/models/damage_at_character_level.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/damage_at_slot_level.py` & `dnd5epy-1.0.5/dnd5epy/models/damage_at_slot_level.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/damage_type.py` & `dnd5epy-1.0.5/dnd5epy/models/damage_type.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/dc.py` & `dnd5epy-1.0.5/dnd5epy/models/dc.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/equipment.py` & `dnd5epy-1.0.5/dnd5epy/models/equipment.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/equipment_category.py` & `dnd5epy-1.0.5/dnd5epy/models/equipment_category.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/equipment_pack.py` & `dnd5epy-1.0.5/dnd5epy/models/equipment_pack.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/error_response.py` & `dnd5epy-1.0.5/dnd5epy/models/error_response.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/feat.py` & `dnd5epy-1.0.5/dnd5epy/models/feat.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/feature.py` & `dnd5epy-1.0.5/dnd5epy/models/feature.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/feature_all_of_prerequisites_inner.py` & `dnd5epy-1.0.5/dnd5epy/models/feature_all_of_prerequisites_inner.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/feature_all_of_prerequisites_inner_any_of.py` & `dnd5epy-1.0.5/dnd5epy/models/feature_all_of_prerequisites_inner_any_of.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/feature_all_of_prerequisites_inner_any_of1.py` & `dnd5epy-1.0.5/dnd5epy/models/feature_all_of_prerequisites_inner_any_of1.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/feature_all_of_prerequisites_inner_any_of2.py` & `dnd5epy-1.0.5/dnd5epy/models/feature_all_of_prerequisites_inner_any_of2.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/gear.py` & `dnd5epy-1.0.5/dnd5epy/models/gear.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/language.py` & `dnd5epy-1.0.5/dnd5epy/models/language.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/magic_item.py` & `dnd5epy-1.0.5/dnd5epy/models/magic_item.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/magic_item_all_of_rarity.py` & `dnd5epy-1.0.5/dnd5epy/models/magic_item_all_of_rarity.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/magic_school.py` & `dnd5epy-1.0.5/dnd5epy/models/magic_school.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/model_class.py` & `dnd5epy-1.0.5/dnd5epy/models/model_class.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster.py` & `dnd5epy-1.0.5/dnd5epy/models/monster.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_ability.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_ability.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_action.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_action.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_all_of_senses.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_all_of_senses.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_all_of_speed.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_all_of_speed.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_armor_class.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_armor_class.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_armor_class_one_of.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_armor_class_one_of.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_armor_class_one_of1.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_armor_class_one_of1.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_armor_class_one_of2.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_armor_class_one_of2.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_armor_class_one_of3.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_armor_class_one_of3.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_armor_class_one_of4.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_armor_class_one_of4.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_attack.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_attack.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_multi_attack_action.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_multi_attack_action.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_proficiency.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_proficiency.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_sense.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_sense.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_special_ability.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_special_ability.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_spell.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_spell.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_spellcasting.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_spellcasting.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/monster_usage.py` & `dnd5epy-1.0.5/dnd5epy/models/monster_usage.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/multiclassing.py` & `dnd5epy-1.0.5/dnd5epy/models/multiclassing.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option.py` & `dnd5epy-1.0.5/dnd5epy/models/option.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_one_of.py` & `dnd5epy-1.0.5/dnd5epy/models/option_one_of.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_one_of1.py` & `dnd5epy-1.0.5/dnd5epy/models/option_one_of1.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_one_of10.py` & `dnd5epy-1.0.5/dnd5epy/models/option_one_of10.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_one_of2.py` & `dnd5epy-1.0.5/dnd5epy/models/option_one_of2.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_one_of3.py` & `dnd5epy-1.0.5/dnd5epy/models/option_one_of3.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_one_of4.py` & `dnd5epy-1.0.5/dnd5epy/models/option_one_of4.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_one_of5.py` & `dnd5epy-1.0.5/dnd5epy/models/option_one_of5.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_one_of6.py` & `dnd5epy-1.0.5/dnd5epy/models/option_one_of6.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_one_of7.py` & `dnd5epy-1.0.5/dnd5epy/models/option_one_of7.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_one_of8.py` & `dnd5epy-1.0.5/dnd5epy/models/option_one_of8.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional, Union
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
-from openapi_client.models.api_reference import APIReference
+from dnd5epy.models.api_reference import APIReference
 
 class OptionOneOf8(BaseModel):
     """
     OptionOneOf8
     """
     option_type: Optional[StrictStr] = Field(None, description="Type of option; determines other attributes.")
     ability_score: Optional[APIReference] = None
```

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_one_of9.py` & `dnd5epy-1.0.5/dnd5epy/models/option_one_of9.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_set.py` & `dnd5epy-1.0.5/dnd5epy/models/option_set.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_set_one_of.py` & `dnd5epy-1.0.5/dnd5epy/models/option_set_one_of.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_set_one_of1.py` & `dnd5epy-1.0.5/dnd5epy/models/option_set_one_of1.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/option_set_one_of2.py` & `dnd5epy-1.0.5/dnd5epy/models/option_set_one_of2.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/prerequisite.py` & `dnd5epy-1.0.5/dnd5epy/models/prerequisite.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/prerequisite_ability_score.py` & `dnd5epy-1.0.5/dnd5epy/models/prerequisite_ability_score.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/proficiency.py` & `dnd5epy-1.0.5/dnd5epy/models/proficiency.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/proficiency_all_of_reference.py` & `dnd5epy-1.0.5/dnd5epy/models/proficiency_all_of_reference.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/race.py` & `dnd5epy-1.0.5/dnd5epy/models/race.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/resource_description.py` & `dnd5epy-1.0.5/dnd5epy/models/resource_description.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/rule.py` & `dnd5epy-1.0.5/dnd5epy/models/rule.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/rule_section.py` & `dnd5epy-1.0.5/dnd5epy/models/rule_section.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/skill.py` & `dnd5epy-1.0.5/dnd5epy/models/skill.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/spell.py` & `dnd5epy-1.0.5/dnd5epy/models/spell.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/spell_all_of_damage.py` & `dnd5epy-1.0.5/dnd5epy/models/spell_all_of_damage.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/spell_prerequisite.py` & `dnd5epy-1.0.5/dnd5epy/models/spell_prerequisite.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/spellcasting.py` & `dnd5epy-1.0.5/dnd5epy/models/spellcasting.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/spellcasting_info_inner.py` & `dnd5epy-1.0.5/dnd5epy/models/spellcasting_info_inner.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/spellcasting_spellcasting_ability.py` & `dnd5epy-1.0.5/dnd5epy/models/spellcasting_spellcasting_ability.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/subclass.py` & `dnd5epy-1.0.5/dnd5epy/models/subclass.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/subclass_all_of_spells.py` & `dnd5epy-1.0.5/dnd5epy/models/subclass_all_of_spells.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/subclass_level.py` & `dnd5epy-1.0.5/dnd5epy/models/subclass_level.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/subclass_level_resource.py` & `dnd5epy-1.0.5/dnd5epy/models/subclass_level_resource.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/subclass_level_spellcasting.py` & `dnd5epy-1.0.5/dnd5epy/models/subclass_level_spellcasting.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/subrace.py` & `dnd5epy-1.0.5/dnd5epy/models/subrace.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/subrace_all_of_race.py` & `dnd5epy-1.0.5/dnd5epy/models/subrace_all_of_race.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/trait.py` & `dnd5epy-1.0.5/dnd5epy/models/trait.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific.py` & `dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific_one_of.py` & `dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific_one_of.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon.py` & `dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_damage.py` & `dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_damage.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_usage.py` & `dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific_one_of_breath_weapon_usage.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/trait_all_of_trait_specific_one_of_damage_type.py` & `dnd5epy-1.0.5/dnd5epy/models/trait_all_of_trait_specific_one_of_damage_type.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/weapon.py` & `dnd5epy-1.0.5/dnd5epy/models/weapon.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/weapon_all_of_range.py` & `dnd5epy-1.0.5/dnd5epy/models/weapon_all_of_range.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/models/weapon_property.py` & `dnd5epy-1.0.5/dnd5epy/models/weapon_property.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/dnd5epy/rest.py` & `dnd5epy-1.0.5/dnd5epy/rest.py`

 * *Files identical despite different names*

### Comparing `dnd5epy-1.0.4/pyproject.toml` & `dnd5epy-1.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dnd5epy"
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

### Comparing `dnd5epy-1.0.4/PKG-INFO` & `dnd5epy-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnd5epy
-Version: 1.0.4
+Version: 1.0.5
 Summary: D&D 5e API
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,D&D 5e API
 Author: 5eBits
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
```

