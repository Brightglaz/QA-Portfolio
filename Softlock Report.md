# [BUG] Input Lock After Combat: Cannot Move, Look Around, or Use Keybinds
**Severity:** Critical 
**Priority:** High
**Game Version:** Quasimorph 0.8.5 - Beta Branch
**Reported at:** 16 Jan 2025

## Summary
After a fight with a patrol team, I tried to move to a tile and the game stopped responding to movement, looking around (RMB) and the keybinds I tried (Tab, I, H). Only Esc still worked. A developer suspects a previously unseen softlock involving AI patrols and said they would investigate.

## Conditions 
- **Mission:** Escort mission, the escort directly behind my character.
- **Situation:** I had just fought a patrol team and was moving to the tile below the damaged container (bottom-left of the operative).

## Steps to Reproduce
Steps cannot be reliably reproduced during gameplay.

## Observed Behavior
After I selected a tile, the game stopped accepting movement, camera look, and in-game keybinds including TAB (opening inventory), H (Health UI), and C (Character UI). ESC was the only key that still worked. The video shows about 20 seconds of me trying to click other tiles with no response.

## Expected Behavior
After combat, I should still be able to move, look around and open the inventory

### Additional Observation and Hypothesis
**Observation:** My wound percentage dropped to 0% suddenly. However, I can't tell whether that's the trigger or triggered by the input-lock.
**Possible explanation:** One of the two wounds may have healed and cleared the infection. I wondered whether infection dropping while a similar wound was still active could be related, but I could not establish a link, so this is a hypothesis only.

## Follow-up with the Developers
1. A developer asked my version and whether I used mods. Additionally stated that the issue might have been fixed internally.
2. I replied that I was on the Steam beta branch, assumed to be the latest version, with no mods.
3. I submitted an in-game report as requested, using the text they gave me to identify it. It contained the same description as my first paragraph.
4. The developer then said it looked like a new softlock involving AI patrols and that they would investigate.
