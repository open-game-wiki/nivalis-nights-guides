---
title: "Fix Stutter, Crashes & Loading Problems"
description: "Troubleshoot Nivalis Nights stutter and crashes with a repeatable graphics check, update notes and a guide to saving logs for 505 Games support."
category: "Technical"
publishDate: "2026-10-16"
updatedDate: "2026-10-16"
lang: "en"
---

## Start with a repeatable symptom
Before changing settings, write down where the issue happens: at launch, after travelling, in a crowded street, at a venue or when loading a save. Record the game build, graphics preset, resolution and whether mods are installed. A consistent short route is more useful than comparing two unrelated areas of the city.

## Change one setting at a time

| Symptom | A useful next check | What to compare |
| --- | --- | --- |
| Low frame rate everywhere | Compare a lower graphics preset at the same resolution | The same location and camera direction |
| Stutter in crowded areas | Revisit the same route after updating the game | Frequency and duration of the pauses |
| Crash after travelling | Record the starting and destination areas | Whether the crash repeats with the same save |
| Stuck loading | Keep the current save backed up and note the last action | Whether a different existing save can load |
| Issue after installing a mod | Check the mod's version requirements | A backed-up, unmodified test setup |

Do not change resolution, preset and multiple system options together if your goal is to identify the cause. Keep a short before-and-after note and stop a change that makes the symptom worse. For hardware targets and SSD requirements, use the [official PC requirements](/guides/system-requirements/).

## Preserve useful evidence before restarting
505 Games requests a DxDiag report on Windows and the game's `Player.log` and `Player-prev.log`. A new launch replaces older logs, so preserve them immediately after the failure. Save files share the [Windows save folder](/guides/save-location/); they are only needed by support when requested.

Include the exact action, location and reproduction steps with the report. A screenshot of an error message is more useful than a description such as “it crashed again”. Share logs privately through the support channel, especially if they contain machine or account information.

## Check recent fixes
[Update 4](/guides/patch-notes/) addressed travel memory use and added graphics options; Update 5 added further performance and loading improvements. Apply the current game update before comparing with an older troubleshooting claim. These changes do not establish one universal FPS preset for every PC or handheld.

## Source
[505 Games troubleshooting and log instructions](https://support.505games.com/support/solutions/articles/150000235215-please-read-this-if-you-have-an-issue-playing-nivalis-nights), checked October 16, 2026. For update-specific changes, follow the official links in [patch notes](/guides/patch-notes/).
