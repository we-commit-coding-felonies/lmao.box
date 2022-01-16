# lmao.box
A Northstar Riff for a silly, server-side, smart pistol gamemode.

- All guns (primary, secondary, anti-titan) are removed, and you are given a smart pistol.
- Cloak is banned, it gets replaced by stim. You can run, but you can't hide!
- Getting a player kill fully restores the smart pistol's ammo reserve (you will still have to reload though).
- Everyone only has 1 HP, meaning any damage is fatal. Additionally, the smart pistol locks on to players as fast as it does grunts!
- Ordinance is replaced with pulse blade. Pulse blade pilots are given grapple.

## Installation
1. On the main page click `Releases`, and download the latest file.
2. Open the file, and extract the folder inside to your mods folder (`/Titanfall2/R2Northstar/mods`).
3. Reload your mods, or restart the game.

If you did all that right, there should be an option in private lobby settings under `Riffs` to enable the mode. Have fun!
It is also entirely server-side, **clients don't need to download or install anything!**

## Configuration
The gamemode has many configuration options, held in ConVars. They are listed here, along with the value type, default value, and a brief description of what they do.

Some of these options use internal weapon names. A list of these can be found [here.](https://noskill.gitbook.io/titanfall2/documentation/file-location/weapon/weapon-config-file-name)

| Name | Internal name | Default Value | Description |
| ---- | ------------- | ------------- | ----------- |
| LMAOBox Mode | `riff_lmaobox` | 0 | Toggles the gamemode off/on |
| Instant Lock | `lmaobox_instant_lock` | 1 | Sets pilot health to 30, massiveley decreasing the ttk by requiring only 1 lock |
| Clip refill on kill | `lmaobox_refill_clip_on_kill` | 0 | Refills the clip on kill |
| Clip refill amount | `lmaobox_refill_clip_amount` | 12 | Amount to add to the clip (will not exceed max clip size) | 
| Reserve refill on kill | `lmaobox_refill_reserve_on_kill` | 1 | Refills the reserve on kill |
| Reserve refill amount | `lmaobox_refill_reserve_amount` | 12 | Amount to add to the reserve | 
| Replace ordinance with | `lmaobox_replace_ordinance_with` | 0(*) | Sets whether to replace the pilots' ordinance, and what to replace it with |
| Ban `<ability>` | `lmaobox_ban_<ability>` | 1 (stim, awall),0 (others) | Sets wheter to remove a given tactical ability |
| Banned tactical replacement | `lmaobox_replace_banned_tacticals_with` | 3(**) | Sets whether to give a pilot using a banned tactical a replacement, and what to replace it with |
| HUD Messages | `lmaobox_hud_messages` | 1 | Toggles hud messages |
| Spawn/respawn message | lmaobox_message_on_spawn | "Get good, get LMAOBox!" | Message shown to players on respawn |
| Kill Message | lmaobox_message_on_kill | "LMAOBox - Way to the top!" | Message shown on kill |
| Death Message | lmaobox_message_on_die | "LMAOBox - Best free TF|2 hacks!" | Message shown on death |
| Banned tactical message | lmaobox_message_on_banned_tactical | "You can run, but you can't hide!" | Overwrites spawn message for users of banned tacticals |

These options are all toggleable in the lobby menu, but for dedicated servers:
* Amounts are just ints, messages are just strings
* Toggles are boolean, using 0 as false and 1 as true
* *For ordinance, the list is an array with the option specifying the index <br>
`[
	"mp_weapon_grenade_sonar",
	"mp_weapon_frag_grenade",
	"mp_weapon_grenade_emp", 
	"mp_weapon_thermite_grenade",
	"mp_weapon_grenade_electric_smoke", 
	"mp_weapon_frag_drone", 
	"mp_weapon_grenade_gravity", 
	"mp_weapon_satchel",
	""
] ` <br>
An option of 0 will supply `"mp_weapon_grenade_sonar"`, giving pulse blade, and so on. 8 will remove ordinance, and 9 will disable this, allowing normal loadout use.
* **For tacticals, the list is also an array with the option specifying the index <br> 
`[
	"mp_ability_cloak",
	"mp_weapon_grenade_sonar", 
	"mp_ability_grapple", 
	"mp_ability_heal", 
	"mp_weapon_deployable_cover", 
	"mp_ability_shifter", 
	"mp_ability_holopilot",
	""
]` <br>
7 will not replace the banned tactical





## FAQ
- Why?

Why not?
