
| Field | Value |
|---|---|
| Severity | Low-Medium |
| Game Version | Quasimorph 0.8192S (Beta-branch) |
| Platform | Steam, Windows|
| Reported | 29 Oct 2024 |
| Reproducibility | Always |
| Status | Fixed |

## Summary
During an escort mission, the escort followed me through a damaged door, but would not go back through the same door when I returned and waited right beside him. The door behaves as passable in one direction only.

## Steps to Reproduce
1. Start an escort mission.
2. Move to a second room while the VIP is on the other room.
3. Damage the door connecting the two rooms until it has a red outline by shooting or hitting it with melee weapon.
4. Wait until the VIP move through the damaged door. The escort passes through.
5. Move back through the door and wait right beside the escort, which should trigger them to move back one tile.
6. Observe that the escort does not follow back through the door.

## Expected Result
The escort moves through the damaged door in both directions, or in neither direction.

## Actual Result
The escort passes through the damaged door going forward but cannot go back through it, even when the player waits right beside them.

## Evidence
Screenshot 1: The VIP is on the tile with the damaged door, normally the door can only be stepped on after the door is destroyed.

![Escort and damaged door](QA%20Evidence/VIP_Through_Damaged_Door1.png)

Screenshot 2: The VIP now moved to the current room. The tile with the damaged door can be seen with the red outline.

![Escort and damaged door](QA%20Evidence/VIP_Through_Damaged_Door2.png)

## Impact
This remove the strategy to lock the VIP to a room, saving them from dangerous encounter.

## Notes
- Posted in the Enemies/AI category.
- The developer acknowledged the report. No fix has been confirmed (the fix has been mentioned when the beta branch is closed).
