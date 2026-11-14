# [BUG] Input Lock After Combat: Movement and Actions Stop Responding

**Severity:** High
**Priority:** High
**Game Version:** Quasimorph 0.8.5 - Beta Branch
**Platform:** Steam
**Reported:** 16 Jan 2025
**Reproducibility:** Intermittent / Not reliably reproducible

## Summary
After a fight with a patrol team, I tried to move to a tile and the game stopped responding to movement, looking around (RMB) and the keybinds I tried (Tab, I, H, etc.). Only Esc still worked and a restart is required, which means the player need to redo the level. A developer suspects a previously unseen softlock involving AI patrols and said they would investigate.

## Conditions 
- **Mission:** Escort mission, the escort directly behind my character.
- **Situation:** I had just fought a patrol team and was moving to the tile below the damaged container (bottom-left of the operative).

## Steps to Reproduce
Steps cannot be reliably reproduced during gameplay. The following sequence describes the circumstances in which it occured:

1. Starts an Escor mission with the VIP following the player character.
2. Engage and fight a newly spawned enemy patrol team.
3. After combat, attempt to move to the tile with a destroyed container.
4. Attempt to move, look around, or use the in-game keybind.

## Observed Behavior
After I selected a tile, the game stopped accepting movement, camera look, and in-game keybinds including TAB (opening inventory), H (Health UI), and C (Character UI). ESC was the only key that still worked. The video shows about 20 seconds of me trying to click other tiles with no response.

## Expected Behavior
After combat, movement, camera controls, and other gameplay actions should remain functional. Opening UI interface should not be the only responsive form of input.

### Additional Observation and Hypothesis
**Observation:** My wound percentage dropped to 0% suddenly. However, I can't tell whether that's the trigger or triggered by the input-lock.
**Possible explanation:** One of the two wounds may have healed and cleared the infection. I wondered whether infection dropping while a similar wound was still active could be related, but I could not establish a link, so this is a hypothesis only.

## Follow-up with the Developers
1. A developer asked my version and whether I used mods. Additionally stated that the issue might have been fixed internally.
2. I replied that I was on the Steam beta branch, assumed to be the latest version, with no mods.
3. I submitted an in-game report as requested, using the text they gave me to identify it. It contained the same description as my first paragraph.
4. The developer then said it looked like a new softlock involving AI patrols and that they would investigate.
