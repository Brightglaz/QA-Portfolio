| Field | Value |
|---|---|
| Severity | High |
| Game Version | Quasimorph 0.7.1 (save created after the 0.7.1 patch) |
| Platform | [Steam, OS] |
| Reported | 25 Jul 2024 |
| Reproducibility | Seen on a retry after the first operative died on a later level. The developer reports it works for most players. |
| Status | Fixed |

## Summary
On my second attempt at the Obbibjord-3 story mission, the elevator at the top middle of the first floor was already in its broken state and could not be interacted with. This elevator is the only way to reach the other levels, and entering it starts the quest line. The story dialogue and the scripted supply drops did not trigger. The softlock cleared only after forfeiting the mission and then closing and reopening the game.

## Steps to Reproduce
This was seen once. It occurred under these circumstances:
1. Start the Obbibjord-3 story mission on a save created after the 0.7.1 patch.
2. Use the elevator at the top middle of the first floor to go to another level. The elevator changes to its broken state, as scripted.
3. The operative dies on the other level, and the run is lost.
4. Equip a second operative and start the mission again.
5. Go to the elevator on the first floor and try to interact with it.

## Expected Result
The elevator is usable on arrival, so the player can travel to other levels and start the quest line. It changes to its broken state only after the player has moved to a different level, as a scripted event.

## Actual Result
The elevator is already in its broken state on arrival and cannot be interacted with in any way. There is no other way to go down.

## Evidence
![Broken elevator on the first floor](QA%20Evidence/Oddibjord_broken_elevator.png)

## Impact
- **Progression is blocked:** the elevator is the only route to the other levels, and the quest line starts after entering it. This is a softlock.
- **Scripted content is skipped:** the story dialogue introducing the Realware operatives does not trigger, and neither do the two supply drops of equipment from the employer (not mandatory, but useful for the mission).
- **Restarting is not enough on its own:** closing and reopening the game without forfeiting leaves the save softlocked, and starting the mission again immediately after forfeiting brings the same broken elevator back.
- **Failure cost:** the only way out was to forfeit the mission by deliberately ending the second operative's run. This lost that operative and all the equipment they carried.

## Workaround
Forfeit the mission (losing the operative and all carried equipment), then close and reopen the game before starting the mission again. The elevator was normal after that. Starting the mission again without reopening the game reproduced the softlock. No other workaround was found.

## Notes
- **Possible cause:** in the first attempt, I used the elevator and the operative died on the other level, so the elevator had already entered its broken state. On the retry it was already broken on arrival. Since it only reset after a full game restart, the broken state may be held in memory while the game is running and not cleared when a mission ends. This is my assumption and has not been confirmed.
- The developer asked whether the save came from version 0.7 or 0.7.1. I confirmed it was created fresh on 0.7.1, after the patch released.
- The developer replied that they were still investigating why it works for most players.
