# Rotoblin-AZMod-Changes
Collection of requested configuration changes to AZMod (https://github.com/fbef0102/Rotoblin-AZMod) for ease of distribution to server owners in our discord community.

NOTE: This is a collection of CHANGES to the base configuration. YOU MUST INSTALL THE BASE CONFIGURATION FIRST.

CHANGES TO FILE LOCATIONS (NOT INCLUDED IN REPO, DO THIS YOURSELF IF YOU WANT THESE CHANGES:
- all4dead.smx (admin spawning items, hordes, infected, etc.) moved to plugins/optional and thereby disabled.
- l4d_quadcaps.smx (guaranteed quad when boomer dies last) moved to plugins/optional and thereby disabled. - NVM WHY CAN'T THIS THING BE REMOVED LOL

----MISSION FILES----

*"Versus Modifers" normalized to 1.0 map multiplier.

----SHARED CONVARS----

*Witch personal space reverted to 100.
*Spec listener (specs can listen to team voice chats) disabled.
*Vocalize spam blocker disabled.
*Stock tank lottery restored (tank_control_disable 1). Need confirmation that tank will still not pass.

----4v4 HARDCORE----

*Hunting Rifle removed.
*Shotgun reserve ammo restored to 128.
*Uzi changes reverted to stock.
*Tank speed 205 -> 210 (z_tank_speed_vs 210)
*Tank slowdown from bullets restored (l4d_si_slowdown_tank 0)
*No extra pills (rotoblin_health_style 3).
*Team order 0 (leading team plays Survivor first); ABABA seems buggy? Teams tend to end up swapped.

----WITCH PARTY----

*Tank speed 205 -> 210 (z_tank_speed_vs 210)
*Tank slowdown from bullets restored (l4d_si_slowdown_tank 0)
*Tickrate Fixes plugin added.
*No hunter deadstops. (versus_shove_hunter_fov_pouncing 0)
*No medkits or extra pills (rotoblin_health_style 3).

----cfg/Sourcemod----

*cannounce.cfg - turned off detailed connect/disconnect messages
*l4d_QuadCpas.cfg - disabled random chance to get 4 hunters
*l4d_si_slowdown_remove.cfg - Commented out the cvar changes here so that they'll be handled by configs instead.

----cfg/Reloadables----

*Advertisements/Tips disabled