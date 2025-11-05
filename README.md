# Aggressive Mobs

Aggressive Mobs is a Minecraft Forge mod for **1.20.1** that dramatically increases the challenge of survival by giving hostile mobs smarter AI and additional abilities. Zombies will tear through walls to reach you, skeletons shoot faster and harder after they miss, creepers prime when burned and even become nuclear, and spiders can trap you in webs. Many behaviours are configurable via a TOML file so you can tune the difficulty to your liking.

## Key Features

### Siege Days and Player Targeting

- On configurable "siege days," all monsters listed on the siege whitelist automatically target the nearest player or villager. The mod adds a global speed boost to mobs and forces them to continuously retarget the nearest player.
- Monsters will even continue targeting players while underground or across large distances.
- You can adjust how frequently sieges occur and which entities participate via `aggressive-mobs-config.toml` (e.g., daily, weekly, etc.).

### Enhanced Zombies

- Random weapons and armor. When zombies spawn they may be equipped with a random pickaxe, sword or axe and a random set of armor pieces, making them much tougher.
- Digging and block-breaking. Zombies are capable of digging through blocks to reach the player. If their navigation path is obstructed, they will swing and break two-high tunnels or obstacles around them. You can configure how far away they begin digging and which blocks are immune via a blacklist.
- Building bridges and pillars. Zombies can place cobblestone to bridge over gaps and build upwards toward high-ground players. They place blocks under themselves, climb up, snap to the block center and continue chasing.
- TNT placement and fire-setting. A zombie near a player may drop TNT on the ground with a configurable chance and distance. Zombies and piglins can also light adjacent flammable blocks on fire when close to a target.
- Duplication (swarming). Certain monsters (e.g., zombies, skeletons, blazes, endermen, ravagers and others) can duplicate themselves on spawn. When duplication is enabled, the mod clones the mob at random nearby positions. Dungeons and spawners can generate even more clones.
- Jockey mobs and rideable mounts. Enemies may spawn riding animals such as pigs, chickens or spiders. Both the list of rideable mobs and the jockeying mobs are configurable.
- Bloodlust and angry variants. Some mobs (hoglins, husks, zombies, zombified piglins, etc.) can spawn with a "bloodlust" effect, increasing their maximum health by 50% and giving them a speed boost and health-boost potion effect.

### Skeleton Improvements

- Fast attack goal. Default bow-attack goals are removed and replaced with a fast attack goal that forces skeletons to shoot roughly every five ticks. This makes their arrow barrages much harder to dodge.
- Super Skeletons. Skeletons have a configurable chance of spawning as "Super Skeletons." These super variants receive the bloodlust treatment, gaining extra health and speed.
- Arrow adaptation. Each time a skeleton’s arrow misses a living target, a miss counter increments. After three misses, the skeleton’s next arrow is automatically boosted—moving at double speed, dealing double damage and leaving a crit trail. The counter resets when the arrow hits.
- Random armor. Like zombies, skeletons may spawn wearing random armor pieces.

### Creeper Changes

- Fire triggers explosions. Creepers now ignite when taking fire damage (including being hit by a flaming arrow), emitting their hiss and starting the fuse.
- Charged and Nuclear creepers. When a creeper spawns it has a configurable chance to be charged and a separate chance to be nuclear. Nuclear creepers are powered, have a larger explosion radius and fuse time, move faster, and suffer reduced health.
- Wall-breaching. Creepers that cannot get line-of-sight to a player start tracking their distance. If they remain stuck for a number of ticks, they ignite and blow up, effectively breaching walls.
- Amplified explosions on "ICBM" creepers. Naming a creeper "ICBM" turns it into a massive bomb with a huge explosion radius and long fuse.

### Spider Behaviour

- Web-shooting. Spiders (including cave spiders) can shoot cobwebs at players when close enough, trapping them in place. There is a configurable chance and distance for web-shooting.

### Other Enhancements

- Ocean movement. Entities that step into or onto water get a temporary movement and swim-speed boost, allowing them to "bounce" across oceans more quickly. When on land again, the boost is removed.
- Sleep prevention. If sleeping is disabled in the config, attempting to sleep sets the player’s spawn point and returns the "not safe" message rather than letting them skip the night.
- Target villagers. Monsters may optionally target villagers in addition to players.

## Configuration

All of these features are controlled through the `aggressive-mobs-config.toml` file generated in your `config` folder. Each option has a clear comment explaining what it does and sensible default values. You can:

- Toggle entire systems: siege mode, duplication, jockey mobs, charged creepers, angry entities, zombie building/digging, spider webs, etc.
- Adjust the chances and distances for each behaviour.
- Define block-breaking blacklists.
- Set mob whitelist/blacklist lists.
- Decide which mobs can be ridden or act as jockeys.
- Control siege frequency, entity duplication counts, explosion radii, TNT and fire probabilities, and many other parameters.

## Installation

1. Install Minecraft Forge for Minecraft **1.20.1**.
2. Download the latest release of Aggressive Mobs from the releases page (the JAR built in `build/libs`).
3. Place the downloaded JAR file into your Minecraft `mods` folder.
4. Launch Minecraft using the Forge profile. A configuration file will be generated on first run at `config/aggressive-mobs-config.toml`.

## Tips

- The mod can be extremely challenging at its default settings; consider tweaking the configuration to suit your desired difficulty.
- Use defensive building strategies—mobs can break blocks and build around obstacles. Reinforced blocks listed in the blacklist (e.g., obsidian, bricks, metal blocks) are harder for zombies to break.
- Watch out for named "ICBM" creepers; their explosions are devastating.
- Bloodlusted mobs move and hit much harder.

## Credits

Aggressive Mobs is developed by birdsprime. It is released under the All Rights Reserved license. Feel free to submit issues or suggestions on the GitHub repository.
