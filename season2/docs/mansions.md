# Mansion regeneration

Select mansions will regenerate periodically to allow players to experience it in multiplayer.
Only two mansions are capable of regenerating on the season 2 map.

## Entire structure
Requirements for regenerating a mansion:
* Player must have not regenerated a mansion in the last 2-3 weeks
  * This timer is per-*player*, not per-mansion
* Mansion must not be occupied by other players (i.e. no players inside the building)
* Mansion must not be in cooldown mode (i.e. >60 seconds since last regeneration or mob spawn)

When a mansion regenerates, it randomly picks 1 of 5 layouts and randomly populates the rooms.
Loot in the chests are also randomized.
Additionally, the normally empty chests in some mansion rooms have custom loot, which can contain music discs and xp bottles.

After generating, the mansion will enter cooldown mode for 60 seconds and 
extend the player's timer by a random time between 2-3 weeks.
(specifically a random integer between 336-504 hours)

## Respawn mobs only
Requirements for respawning mobs:
* Mansion must not have respawned mobs in the past 8 hours, with exception of spawning them as part of a complete structure.
  * This timer is per-*mansion*, not per-player
* Mansion must not be occupied
* Mansion must not be in cooldown mode

The mansion will be cleared of hostile mobs, then illagers will respawn in the rooms they originated from.
Blocks may be removed if they obstruct the respawning of an illager, and a floor will be placed if one does not exist.