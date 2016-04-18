Sentinel NPCs: Combat NPCs for Spigot!
--------------------------------------

![AnimatedSentinel](http://i.imgur.com/VDwTzrs.gif)

**Version 0.3**: Compatible with Spigot 1.9

**Download (Developmental builds)**: http://ci.citizensnpcs.co/job/Sentinel/  
**Download (Spigot releases)**: (COMING SOON)  

### Info

Created by mcmonkey4eva on behalf of the Citizens and Denizen teams.

### Usage

- First, get acquainted with Citizens in general for best luck using Sentinel.
- Second, download the plugin and put it into your server's `plugins` folder.
- Third, start the server to generate a config, then close the server and edit the config to your liking and finally restart the server.
- Now, to create your first Sentinel:
	- Select or create an NPC (`/npc sel` or `/npc create Bob`)
	- Run command: /trait Sentinel
	- Run command: /npc equip
	- Give the NPC items as needed, by right click the NPC with the wanted item.
	- Run command: /sentinel addtarget MONSTERS
	- Spawn a zombie via creative inventory eggs and watch it die!
	- Run command: /sentinel help
		- This will list all your options to edit the NPC's Sentinel settings.
			- Play with them freely, just be careful if you have other players around!
- Examples:
	- To make your NPC attack sword wielders, use `/sentinel addtarget helditem:.*sword`

### Commands

- /sentinel help - Shows help info.
- /sentinel addtarget TYPE - Adds a target.
- /sentinel removetarget TYPE - Removes a target.
- /sentinel addignore TYPE - Ignores a target.
- /sentinel removeignore TYPE - Allows targetting a target.
- /sentinel range RANGE - Sets the NPC's maximum attack range.
- /sentinel damage DAMAGE - Sets the NPC's attack damage.
- /sentinel armor ARMOR - Sets the NPC's armor level.
- /sentinel health HEALTH - Sets the NPC's health level.
- /sentinel attackrate RATE - Changes the rate at which the NPC attacks, in ticks.
- /sentinel healrate RATE - Changes the rate at which the NPC heals, in ticks.
- /sentinel respawntime TIME - Changes the time it takes for the NPC to respawn, in ticks.
- /sentinel chaserange RANGE - Changes the maximum distance an NPC will run before returning to base.
- /sentinel guard (PLAYERNAME) - Makes the NPC guard a specific player. Don't specify a player to stop guarding.
- /sentinel invincible - Toggles whether the NPC is invincible.
- /sentinel fightback - Toggles whether the NPC will fight back.
- /sentinel needammo - Toggles whether the NPC will need ammo.
- /sentinel safeshot - Toggles whether the NPC will avoid damaging non-targets.
- /sentinel chaseclose - Toggles whether the NPC will chase while in 'close quarters' fights.
- /sentinel chaseranged - Toggles whether the NPC will chase while in ranged fights.
- /sentinel info - Shows info on the current NPC.
- /sentinel stats - Shows statistics about the current NPC.
- /sentinel targets - Shows the targets of the current NPC.

### Permissions
- sentinel.basic for the /sentinel command
- sentinel.admin to edit other player's Sentinel NPCs.
- Everything else is "sentinel.X" where "X" is the command name, EG "sentinel.info".

### Targets

These are all valid targets and ignores:

- Primary set: NPCS, OWNER, PASSIVE_MOB, MOBS, MONSTERS, PLAYERS, PIGS, OCELOTS, COWS, RABBITS, SHEEP, CHICKENS, HORSES, MUSHROOM_COW, IRON_GOLEMS, SQUIDS, VILLAGER, WOLF, SNOWMEN, WITCH, GUARDIANS, SHULKERS, CREERERS, SKELETONS, ZOMBIES, MAGMA_CUBES, ZOMBIE_PIGMEN, SILVERFISH, BATS, BLAZES, GHASTS, GIANTS, SLIME, SPIDER, CAVE_SPIDERS, ENDERMEN, ENDERMITES, WITHER, ENDERDRAGON
- Also allowed: player:NAME(REGEX), npc:NAME(REGEX), entityname:NAME(REGEX), helditem:MATERIALNAME(REGEX)

### Some random supported things

- Weapons:
	- Fists
	- Bow
		- equip NPC with arrows of any given type in their inventory to set fired arrow type!
	- Blaze rod (shoots fire balls!)
	- Potions (splash, lingering)
	- Nether star (strikes lightning!)
	- Spectral arrow (makes the target glow, without damaging it.)
		- (To make a target glow ++ damage it, equip a bow + arm it with spectral arrows!)
- Respawning can be set to "-1" to cause the NPC to delete itself on death, or "0" to prevent respawn.

### TODO

**Beta**:

- Ammo:
	- Basically, optionally require ammo be fed into the NPC for bows/fireballs, or spare swords if the current sword breaks. (waiting on Citizens2 issue 721)
- Mounting:
	- Ride a horse or whatever other NPC (waiting on Citizens2 issue 719)
- Commands:
	- `/sentinel forgive PLAYERNAME/all` forgives attackers
- Other:
	- old Sentry saves importer?

**Future**:

- Events
	- Java and Denizen level events
- Denizen tags

### Need help using Sentinel? Try one of these places:

**IRC** (Modern): http://webchat.esper.net/?channels=citizens  
(irc.esper.net in the channel #citizens)  
**Spigot Info Page** (Modern): (COMING SOON)  

### Dependencies

**Spigot (Plugin-ready server mod)**: https://www.spigotmc.org/  
**Citizens2 (NPC engine)**: https://github.com/CitizensDev/Citizens2/  

#### Also check out:

**Denizen (Powerful script engine)**: https://github.com/DenizenScript/Denizen-For-Bukkit  
