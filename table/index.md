
* Never use null
* Always have sane default values
* Use snake_case field names
* Singular form table names, singular form field names
* Table names scope large_to_small

## aa_action

primary: aa_id, rank

old_field|context|new_field|notes
---|---|---|---
aaid|content|aa_id|
rank|content||
reuse_time|content||
spell_id|content||
target|content||
nonspell_action|content||
nonspell_mana|content||
nonspell_duration|content||
redux_aa|content||
redux_rate|content||
redux_aa2|content||
redux_rate2|content||

## aa_effect

primary: id
unique: (aa_id, slot)

old_field|context|new_field|notes
---|---|---|---
id|content||
aaid|content|aa_id|
slot|content||
effectid|content|effect_id|
base1|content||
base2|content||

## account

primary: id
unique: name, ls_account_id

old_field|context|new_field|notes
---|---|---|---
id|data||
name|data||
charname|data|char_name|
sharedplat|data|shared_plat|
password|data||
status|data||
lsaccount_id|data|ls_account_id|
forum_id|data|forum_id|
gmspeed|data||
revoked|data||
karma|data||
minilogin_ip|data||
hideme|data||
rulesflag|data||
suspendeduntil|data||
time_creation|data||
expansion|data||
ban_reason|data||
suspend_reason|data||
active|data||
ip_exemption_multiplier|data||
gminvul|data||
flymode|data||
ignore_tells|data||
mule|data||

## account_flag

primary: account_id, flag

old_field|context|new_field|notes
---|---|---|---
p_accid|data|account_id|
flag|data|flag|
value|data|value|

## account_ip

primary: account_id, ip

old_field|context|new_field|notes
---|---|---|---
accid|data|account_id
ip|data|ip
count|data|count
lastused|data|lastused

## account_rewards > account_reward

unique: account_id, reward_id
key: account_id

old_field|context|new_field|notes
---|---|---|---
account_id|data||
reward_id|data||
amount|data||

## altadv_vars > aa_var

primary: skill_id

old_field|context|new_field|notes
---|---|---|---
skill_id|data||
name|data||
cost|data||
max_level|data||
type|data||
spellid|data||
prereq_skill|data||
prereq_minpoints|data||
spell_type|data||
spell_refresh|data||
classes|data||
class_type|data||
cost_inc|data||
aa_expansion|data||
special_category|data||
account_time_required|data||
level_inc|data||
eqmacid|data||

## banned_ips > banned_ip

primary: ip_address

old_field|context|new_field|notes
---|---|---|---
ip_address|data||
notes|data||

## base_data

primary: level, class

old_field|context|new_field|notes
---|---|---|---
level|content||
class|content||
hp|content||
mana|content||
end|content||
unk1|content||
unk2|content||
hp_fac|content||
mana_fac|content||
end_fac|content||

## blocked_spells > blocked_spell
## books > book
## bugs > bug
## character_alternate_abilities > character_aa
## character_bind
## character_buffs > character_buff
## character_consent
## character_corpses > character_corpse
## character_corpses_backup > character_corpse_backup
## character_corpse_items > character_corpse_item
## character_corpse_items_backup > character_corpse_item_backup
## character_currency
## character_data > character
## character_faction_values > character_faction_value
## character_inspect_messages > character_inspect_message
## character_inventory
## character_keyring
## character_languages > character_language
## character_lookup
## character_memmed_spells > character_memmed_spell
## character_pet_buffs > character_pet_buff
## character_pet_info
## character_pet_inventory
## character_skills > character_skill
## character_soulmarks > character_soulmark
## character_spells > character_spell
## character_timers > character_timer
## character_zone_flags > character_zone_flag
## char_create_combinations > char_create_combination
## char_create_point_allocations > char_create_point_allocation
## chatchannels > chatchannel
## client_version
## commands_log
## command_settings > command_setting
## damageshieldtypes
## discovered_items
## doors > door
## eqtime
## eventlog
## faction_list
## faction_list_mod
## fishing
## forage
## friends
## gm_ips
## goallists
## graveyard
## grid
## grid_entries
## ground_spawns
## group_id > group

primary: id, character_id

old_field|context|new_field|notes
---|---|---|---
groupid|data|id|
charid|data|character_id
accountid|data|account_id

## group_leaders
## guilds > guild
## guild_members
## guild_ranks
## hackers
## horses
## items
## item_tick
## keyring_data
## launcher
## launcher_zones
## level_exp_mods
## logsys_categories
## lootdrop
## lootdrop_entries
## loottable
## loottable_entries
## mail
## merchantlist
## merchantlist_temp
## name_filter
## npc_emotes
## npc_faction
## npc_faction_entries
## npc_spells
## npc_spells_effects
## npc_spells_effects_entries
## npc_spells_entries
## npc_types
## npc_types_metadata
## npc_types_tint
## object
## object_contents
## petitions
## pets
## player_titlesets
## proximities
## qs_merchant_transaction_log
## qs_player_aa_purchase_log
## qs_player_aa_rate_hourly
## qs_player_coin_move_log
## qs_player_events
## qs_player_ground_spawns_log
## qs_player_handin_log
## qs_player_item_delete_log
## qs_player_item_desyncs_log
## qs_player_item_move_log
## qs_player_killed_by_log
## qs_player_loot_records_log
## qs_player_npc_kill_log
## qs_player_qglobal_updates_log
## qs_player_speech
## qs_player_trade_items_log
## qs_player_trade_log
## qs_player_ts_event_log
## qs_trader_audit
## quest_globals
## races
## raid_details
## raid_members
## reports
## respawn_times
## rule_sets
## rule_values
## saylink
## skill_caps
## skill_difficulty
## spawn2
## spawnentry
## spawngroup
## spawn_conditions
## spawn_condition_values
## spawn_events
## spells_en
## spells_new
## spell_globals
## starting_items
## start_zones
## tblaccountaccesslog
## tblloginserveraccounts
## tblserveradminregistration
## tblserverlisttype
## tblworldserverregistration
## titles
## trader
## tradeskill_recipe
## tradeskill_recipe_entries
## traps
## variables
## webdata_character
## webdata_servers
## zone
## zoneserver_auth
## zone_points
## zone_server
## zone_state_dump