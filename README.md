# QA-Portfolio

This repository collects hand-picked bug reports I wrote while playing the **Early Access and beta builds** of indie games that were asking for community's help to find bugs and feedback. Each report shows how I find an issue, reproduce it, narrow down the conditions, and describe it so a developer can act on it.

## About these reports
- **Independent and Unpaid.** I reported these through the developers' public Discord bug-report and feedback channels as a player. I am not an employee, and there was no formal QA program.
- **Black-box testing.** Everything comes from observing the game. I did not access the source code or developer tools.
- **Early builds.** The reports are done during early-access or beta branches announced during that early-access. Some issues I've reported have been fixed since.
  
## Reports

| ID | Title | Severity | Reported | Status |
|---|---|---|---|---|
| [BUG-001](BUG-001%20Softlock%20Report.md) | Input lock after combat on escort mission | High | 16 Jan 2025 | Fixed |
| [BUG-002](BUG-002%20Enclosed%20Room%20with%20Hostiles%20Generated%20in%20%22Unbroken%20Chain%22%20Quest%20Level%20Contains%20Spawned%20Units,%20Risking%20Softlock.md) | Enclosed room with hostiles in "Unbroken Chain" quest | High | 23 Oct 2024 | Fixed |
| [BUG-003](BUG-003%20Combat%20AR%20Leaving%20Blood%20Pools.md) | Combat ARs leave blood instead of oil | Low-Medium | 23 Oct 2024 | Fixed |
| [BUG-004](BUG-004%20Elevator%20Already%20in%20the%20Broken%20State%20on%20Arrival%20at%20First%20Floor%20of%20Oddibjord-3%20Story%20Quest.md) | Elevator already broken on arrival, Oddibjord-3 mission | High | 25 Jul 2024 | Fixed |
| [BUG-005](BUG-005%20Escort%20NPC%20Can%20Pass%20Through%20a%20Damaged%20Door%20in%20One%20Direction%20but%20Cannot%20Return%20Through%20It.md) | Escort can pass a damaged door one way but not return | Low-Medium | 29 Oct 2024 | Fixed |

  ## How I approach a bug and feedback
1. Check for duplicates before reporting.
2. Reproduce it and write numbered steps, with the build, platform and conditions.
3. Change one variable at a time to narrow down the cause, and compare against other builds or similar cases.
4. Separate what I observed from what I think. Hypotheses are labeled as hypotheses, and my expected behavior is labeled as my expectation, not a confirmed requirement.
5. Record the developer's response accurately, without describing a report as confirmed or fixed unless the developers said so.
6. Follow up when asked for more information, such as the version, mods or an in-game report.

## Notes
All mentioned games and it's assets belong to their respective owners. This repository is not affiliated with the developers. Screenshots and videos are included only to document the reports.
