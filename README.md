# Rotoblin-AZMod-Changes
Collection of requested configuration changes to AZMod (https://github.com/fbef0102/Rotoblin-AZMod) for ease of distribution to server owners in our discord community.

NOTE: This is a collection of CHANGES to the base configuration. YOU MUST INSTALL THE BASE CONFIGURATION FIRST.

CHANGES TO FILE LOCATIONS (NOT INCLUDED IN REPO, DO THIS YOURSELF IF YOU WANT THESE CHANGES:
- all4dead.smx (admin spawning items, hordes, infected, etc.) moved to plugins/optional and thereby disabled.
- l4d_QuadCaps.smx - Can't move this to plugins/optional without implementing native KEEP_SI_STARTING somewhere else or using an old version of ready up

----MISSION FILES----
- "Versus Modifers" normalized to 1.0 map multiplier.

----SHARED CONVARS----
- Witch personal space reverted to 100.
- Spec listener (specs can listen to team voice chats) disabled.
- Vocalize spam blocker disabled.
- Stock tank lottery restored (tank_control_disable 1). Need confirmation that tank will still not pass.
- Smoker-pulled survivors blocked by common again (collision_smoker_common 0)
- Car alarm back to default (sm_cvar car_alarm_distance commented out)
- Damage Pounce 50 -> 35

----4v4 HARDCORE----
- Hunting Rifle removed (still gives ammo).
- Shotgun reserve ammo restored to 128.
- Uzi changes reverted to stock.
- Tank speed 205 -> 210 (z_tank_speed_vs 210)
- Tank slowdown from bullets restored (l4d_si_slowdown_tank 0)
- No extra pills (rotoblin_health_style 3).
- Team order 0 (leading team plays Survivor first); ABABA seems buggy? Teams tend to end up swapped.
- Hunter claw damage 3
- All shoves disabled on hunters
- Smoker tongue recharge reverted to 15 seconds.
- Hunter pounce ticks back to normal (z_pounce_damage 5; z_pounce_damage_interval 0.5)

----WITCH PARTY----
- Tank speed 205 -> 210 (z_tank_speed_vs 210)
- Tank slowdown from bullets restored (l4d_si_slowdown_tank 0)
- Tickrate Fixes plugin added.
- No hunter deadstops. (versus_shove_hunter_fov_pouncing 0)
- No medkits or extra pills (rotoblin_health_style 3).

----cfg/Sourcemod----
- cannounce.cfg - turned off detailed connect/disconnect messages, turned off sounds
- l4d_QuadCpas.cfg - disabled random chance to get 4 hunters
- l4d_si_slowdown_remove.cfg - Commented out the cvar changes here so that they'll be handled by configs instead.

----cfg/Reloadables/server_custom_convars.cfg----
- Advertisements/Tips disabled
- Pill bonus disabled

----addons/stripper/Roto-AZMod/maps----
- l4d_vs_airport03_garage: re-added fence blocker at start, re-added baggage cart to block starting event from far away
- l4d_vs_airport04_terminal: metal detector event is forced again
- l4d_vs_smalltown01_caves: removed bus and fences near start

----addons/sourcemod/plugins----
- l4dscores.smx modified by Harry Potter to remove pill bonus (still shows visually, is removed on round end)
- l4d_boss_percent.smx modified by me to reflect survivor progress rather than boss location
- l4d_current_survivor_progress.smx modified by me to reflect survivor progress rather than nearest potential boss spawn location
- linux_auto_restart.smx automatically restarts server when all human players disconnect