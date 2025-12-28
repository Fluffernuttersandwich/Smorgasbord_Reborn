# 🧯 Smörgåsbord — Troubleshooting, Performance & Known Issues

This document contains **all troubleshooting, diagnostics, performance tuning, and known issues** for the **Smörgåsbord by FNS** Wabbajack ModList.

If you skipped the README: go back and read it.  
If you didn’t read it: this document will hurt your feelings.

---

## 📚 Table of Contents

- [Before You Ask for Help](#before-you-ask-for-help)
- [Log Files (Required)](#log-files-required)
- [Basic Sanity Checks](#basic-sanity-checks)
- [Common Installation Problems](#common-installation-problems)
- [Graphics, Freezes & Crashes](#graphics-freezes--crashes)
- [World Loading & Crafting Bugs](#world-loading--crafting-bugs)
- [Multiplayer Issues](#multiplayer-issues)
- [Antivirus & Background Apps](#antivirus--background-apps)
- [MO2 Interface Problems](#mo2-interface-problems)
- [Known Issues](#known-issues)
- [Performance & Lossless Scaling](#performance--lossless-scaling)

---

## Before You Ask for Help

> **No logs = no assistance.**

I am not paid tech support.  
I am not psychic.  
Screenshots of the F1 console are **not logs**.

If you contact me without logs, I will tell you to send logs.

---

## Log Files (Required)

When using **MO2 + Wabbajack**, logs are stored here:
C:\Users\YourUserName\AppData\LocalLow\The Fun Pimps\7 Days To Die

Attach the **entire log file**, not screenshots.

---

## Basic Sanity Checks

### 1. Game Version

You **must** be on **7 Days to Die v2.5 (Stable)**.

Experimental builds are **not supported**.

---

### 2. Easy Anti-Cheat (EAC)

EAC **must be disabled**, not muted.

Disable it in the Steam launcher — permanently.

---

### 3. Harmony Folder

You **must not delete**: 
C:\Program Files (x86)\Steam\steamapps\common\7 Days To Die\Mods\0_TFP_Harmony


If you deleted it:
- Verify game files in Steam
- It will be restored

---

### 4. Mods in the Wrong Folder

There must be **NO mods** in:
C:\Users\YourUserName\AppData\Roaming\7DaysToDie\Mods


The **only** mod allowed in the base game folder is **Harmony**.

---

## Common Installation Problems

### Wabbajack Issues

- Update Wabbajack to the **latest version**
- Old versions **do not support 7DtD**
- Clear Wabbajack cache occasionally

To reset Wabbajack:
1. Close Wabbajack
2. Press `Win + R`
3. Enter `%localappdata%`
4. Delete the `_Wabbajack_` folder
5. Relaunch and log in again

---

### Nexus Mods Login

You **must** be logged into Nexus Mods **inside Wabbajack**.

Being logged in via browser alone is not enough.

---

## Graphics, Freezes & Crashes

If you see errors like:

d3d11: failed to create buffer


### Fixes:

1. Update GPU drivers
2. Lower graphics from Ultra → High
3. Disable Dynamic Mesh
4. Do **not** blindly copy someone else’s graphics settings

If the game crashes mid-session, the save **may** be unrecoverable.

---

## World Loading & Crafting Bugs

### Symptoms:
- Stuck on “Building Environment…”
- Crafting queue never completes
- Endless red errors in console

### Causes:
- Mods added that aren’t part of the list
- Mods removed mid-save
- Load order broken
- Mods present in Roaming Mods folder

### Fix:
- Remove all mods from:
C:\Users\YourUserName\AppData\Roaming\7DaysToDie\Mods

- Reinstall the ModList if load order was changed

---

## Multiplayer Issues

### Crossplay
Crossplay **must be disabled** for multiplayer with this list.

### Dedicated Servers
- Server and all clients must have **identical mods**
- EAC must be off
- Do not mix client-side and server-side mods casually

---

## Antivirus & Background Apps

Common offenders:
- Antivirus
- Firewalls
- RGB software
- Performance overlays
- SteelSeries
- iCUE

Create exceptions for:
- `ModOrganizer.exe`
- `7daystodie.exe`

---

## MO2 Interface Problems

### “My load order is messed up!”

Click the **Priority** column header to re-sort.

You didn’t break anything.

---

## Known Issues

- WalkerSim produces many yellow warnings — **normal**
- Descent + Bait Bags produces a benign error — **harmless**
- Experimental mods are **not vetted**
- khzZombies is glitchy but functional

I have hundreds of hours played with these warnings present.

---

## Performance & Lossless Scaling

Lossless Scaling (LS) is a **paid Steam app**.

It can:
- Add Frame Generation
- Reduce stutter
- Improve smoothness on high-refresh monitors

### Requirements:
- 120Hz+ monitor recommended
- Windowed mode
- RTX GPUs benefit most (not required)

### Important:
- Disable **VSync in-game**
- You may keep VSync enabled in:
  - Monitor
  - NVIDIA Control Panel
  - Lossless Scaling app

### Guide:
https://www.youtube.com/watch?v=qc3zZEYpfLY

Lossless Scaling is **system-specific**.  
Your mileage may vary.

---

## Final Reminder

If you:
- Read the README
- Read this document
- Sent logs
- Followed instructions

…and it still doesn’t work?

Then yes — contact me.

If you skipped steps and winged it?

That’s on you.

🍽️ **Enjoy the buffet — but read the menu first.**
