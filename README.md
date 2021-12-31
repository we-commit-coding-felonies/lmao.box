# lmao.box
A Northstar Riff for a silly smart pistol gamemode.

- All guns (primary, secondary, anti-titan) are removed, and you are given a smart pistol.
- Cloak is banned, it gets replaced by stim. You can run, but you can't hide!
- Getting a kill fully restores the smart pistol's ammo reserve (you will still have to reload though)
- Everyone only has 1 HP, meaning any damage is fatal. Additionally, the smart pistol locks on to players as fast as it does grunts!
- Ordinance is replaced with pulse blade. Pulse blade pilots are given grapple.

## Installation
1. On the main page click `Code`, then `Download ZIP`
2. Open the ZIP file, and extract the folder inside to your mods folder (`/Titanfall2/R2Northstar/mods`)
3. Reload your mods, or restart the game

If you did all that right, there should be an option in private lobby settings under `Riffs` to enable the mode. Have fun!
It is also entirely server-side, clients don't need to download or install anything!

## Configuration
The gamemode has many configuration options, held in ConVars. They are listed here, along with the value type, default value, and a brief description of what they do.

Some of these options use internal weapon names. A list of these can be found [here.](https://noskill.gitbook.io/titanfall2/documentation/file-location/weapon/weapon-config-file-name)

| Name | Value Type | Default Value | Description |
| - | - | - | - |
| `lmao_defaulthealth` | Integer | `1` | Sets the amount of health players have. In normal games, this value is 100. |
| `lmao_replaceordinance` | Boolean | `1` | If 1 (true), will replace all players ordinance (grenades). |
| `lmao_ordinancereplacement` | String | `mp_weapon_grenade_sonar` | Defines what to replace ordinance with when `lmao_replaceordinance` is true. |
| `lmao_bannedtacticals` | String | `mp_ability_cloak,mp_weapon_deployable_cover` | List of tacticals to be replaced. ***MUST*** be in the format `wep1,wep2,wep3,etc`. |
| `lmao_replacebannedtactical` | Boolean | `1` | Turn this off to remove banend tacticals withoput replacing them |
| `lmao_tacticalreplacement` | String | `mp_ability_heal` | Defines what to replace banned tacticals with. |
| `lmao_enablehudmessages` | Boolean | `1` | Turn this off to disable all of the on-screen messages. |
| `lmao_messagerespawn` | String | `Get good, get LMAOBox!` | Defines what message is displayed at the start of a match, and upon player respawn. |
| `lmao_messagebannedtactical` | String | `You can run, but you can't hide!` | Defines what message is displayed at the start of the match, and at player respawn, for players who have a banned tactical equipped. |
| `lmao_refillcliponkill` | Boolean | `0` | If enabled, sets the currently loaded bullets in the smart pistol to a number upon killing another player. |
| `lmao_cliprefillamount` | Integer | `12` | Defines the number of bullets for `lmao_refillcliponkill` |
| `lmao_refillreserveonkill` | Boolean | `1` | If enabled, sets the reserve ammo to a number upon killing another player |
| `lmao_reserverefillamount` | Integer | `12` | Defines the number of bullets for `lmao_refillreserveonkill` |


## FAQ
- Why?

Why not?
