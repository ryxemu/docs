
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
rank|content|rank|
reuse_time|content|reuse_time|
spell_id|content|spell_id|
target|content|target|
nonspell_action|content|nonspell_action|
nonspell_mana|content|nonspell_mana|
nonspell_duration|content|nonspell_duration|
redux_aa|content|redux_aa|
redux_rate|content|redux_rate|
redux_aa2|content|redux_aa2|
redux_rate2|content|redux_rate2|

## aa_effect

primary: id
unique: (aa_id, slot)

old_field|context|new_field|notes
---|---|---|---
id|content|id|
aaid|content|aa_id|
slot|content|slot|
effectid|content|effect_id|
base1|content|base1|
base2|content|base2|

## account

primary: id
unique: name, ls_account_id

old_field|context|new_field|notes
---|---|---|---
id|data|id|
name|data|name|
charname|data|char_name|
sharedplat|data|shared_plat|
password|data|password|
status|data|status|
lsaccount_id|data|ls_account_id|
forum_id|data|forum_id|
gmspeed|data|gmspeed|
revoked|data|revoked|
karma|data|karma|
minilogin_ip|data|minilogin_ip|
hideme|data|hideme|
rulesflag|data|rulesflag|
suspendeduntil|data|suspendeduntil|
time_creation|data|time_creation|
expansion|data|expansion|
ban_reason|data|ban_reason|
suspend_reason|data|suspend_reason|
active|data|active|
ip_exemption_multiplier|data|ip_exemption_multiplier|
gminvul|data|gminvul|
flymode|data|flymode|
ignore_tells|data|ignore_tells|
mule|data|mule|

## account_flag

primary: account_id, flag

old_field|context|new_field|notes
---|---|---|---
p_accid|data|account_id|
flag|data|flag|
value|data|value|

## account_ip
## account_rewards > account_reward
## altadv_vars > aa_var
## banned_ips > banned_ip
## base_data
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