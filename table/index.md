
* Never use null
* Always have sane default values
* Use snake_case field names
* Plural table names, singular field names
* Table names scope large_to_small

## aa_actions

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

## aa_effects

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

## account -> accounts

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

## account_flags

primary: account_id, flag

old_field|context|new_field|notes
---|---|---|---
p_accid|data|account_id|
flag|data|flag|
value|data|value|