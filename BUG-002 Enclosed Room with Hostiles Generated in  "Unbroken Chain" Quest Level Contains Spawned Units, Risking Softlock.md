| Field | Value |
|---|---|
| Severity | High |
| Game Version | Quasimorph 0.8 |
| Platform | Steam, Windows 10 |
| Reported | 23 Oct 2024 |
| Reproducibility | Intermittent (randomized level generation; the generated map is saved once it is reached) |
| Status | Fixed |

## Summary
During the Unbroken Chain quest, level generation can produce a fully enclosed room with hostile units spawned inside. The quest requires killing all hostiles, so these units block completion. The player can only find them with the floor scanner or by using sneak mode to hear footsteps, and can only reach them by destroying walls with projectiles or grenades (melee cannot break walls). Because the generated level is saved, reloading does not fix it.

## Steps to Reproduce
Depends on the level generation, it cannot be triggered on demand. It occured under these circumstances:
1. Start the Unbroken CHain quest.
2. Reach the floor called "Engine Room".
3. If it happens, the room would be visible with the floor scanner (if the player have the upgrade), if not, by chance using the "sneak" mode to hear footsteps.

## Expected Result
All spawned hostile units are in areas the player can reach, or no units spawn in sealed rooms.

## Actual Result
A fully enclosed room is generated with hostile units inside, with no accesible entrance.

## Evidence
![Enclosed room with spawned units](QA%20Evidence/Faulty%20generation_1.png)

## Impact
- The quest requires killing every hostile, so enclosed units make it unfinishable until they are found and reached.
- **Detection depends on the player's upgrade or playstyle:** the floor scanner or sneak mode (footstep audio) reveals the level or the units respectively. A player with neither has no indication anything is wrong.
- **Reaching them depends on ranged resources:** walls can only be broken with projectiles or grenades, not melee. A player without ammo or grenades cannot reach the room (unlikely, but possible).
- **Reloading does not help:** the generated map is saved with the level.
- **Failure cost is high:** a player who cannot complete the quest must abandon the run. On Normal and Unfair difficulty, this means the operative is lost, along with all carried equipment and loot, and the operative's experience level (returning to level 1). Players playing with Easy difficulty is spared from this setback.

## Notes
Reported together with BUG-003 in the same Discord post. The developer offers his thanks and mentioned the problem is fixed in the next patch.
