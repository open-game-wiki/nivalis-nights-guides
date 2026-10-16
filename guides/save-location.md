---
title: "Save Location, Manual Saves & Backup"
description: "Find the official Nivalis Nights Windows save folder, back up .sav files safely, and check manual saving and Steam Cloud before restoring progress."
category: "Technical"
publishDate: "2026-10-16"
updatedDate: "2026-10-16"
lang: "en"
---

## Windows save location
505 Games identifies this folder for game logs and `.sav` files:

```text
%USERPROFILE%\AppData\LocalLow\ION LANDS\Nivalis Nights
```

Press **Win + R**, paste the path and press Enter. Look for `.sav` files; `Player.log` and `Player-prev.log` in the same folder are diagnostic logs, not save files.

## Make a backup before changing files
1. Make a manual save from the pause menu, then close the game normally.
2. Copy the whole save folder to a separate dated folder. Copy rather than move, so the active files remain in place.
3. Keep the backup outside the game's active directory. If you are about to test a mod or restore an older file, preserve a second copy of the current state first.
4. When restoring, keep the game closed and confirm the file you are replacing. Restart and check the expected day, venue and quest before continuing.

Steam Cloud is a synchronization service, not a substitute for keeping your own dated backups. If Steam reports a conflict, inspect the timestamps and preserve both local candidates before choosing which version to keep. Avoid repeatedly overwriting a save while investigating missing progress.

## Manual saves and autosaves
The developer FAQ says the game autosaves at the end of a day and supports manual saving from the pause menu. Save manually before quitting if you want to preserve progress since the previous end-of-day autosave. Cloud synchronization needs an internet connection.

## When saving fails
Record the error, the slot or file involved, and the last successful save. Keep an untouched copy before trying a restore. If the issue repeats, [505 Games support](https://support.505games.com/) can request diagnostic logs and a save. The support article asks for saves only when requested; do not upload your entire folder publicly.

## Sources
- [505 Games save and log location](https://support.505games.com/support/solutions/articles/150000235215-please-read-this-if-you-have-an-issue-playing-nivalis-nights), checked October 16, 2026.
- [Developer FAQ — saving](https://steamcommunity.com/app/1488490/discussions/0/598530855994991183/).
