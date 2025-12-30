# 🧯 Smörgåsbord — Troubleshooting, Performance & Known Issues

This document contains **all troubleshooting, diagnostics, performance tuning, and known issues** for the **Smörgåsbord by FNS** Wabbajack ModList.

If you skipped the README: go back and read it.  
If you didn’t read it: this document will hurt your feelings, and yes, you deserve that.


## ⚡ Quick Troubleshooting Flowchart (Read This First)

**Game will not launch / crashes immediately?**
→ Check EAC is **disabled**

→ Verify game files in Steam to ensure Harmony is there.

→ Update GPU drivers  

**Stuck on “Building Environment…” or crafting queue frozen?**
→ Press F1

→ Endless red errors?

→ You removed or added mods mid-save

→ Start a new world  

**Game frozen, or the Console is a waterfall of Red Errors?**
→ Mods exist in `AppData\Roaming\7DaysToDie\Mods`

→ Remove ALL mods from that folder  

**Multiplayer not working?**
→ Crossplay should be **disabled**

→ Server + clients must match mods exactly  

**Random crashes after playing for a while?**
→ Too high graphics

→ Too large RWG map

→ Insufficient RAM

→ Reduce settings and map size  

If none of the above applies:

→ **Send logs**


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

---

## Before You Ask for Help

> **No logs = no assistance.**

If you contact me without logs, I will tell you to send logs.

Logs can be posted in the Guppy's Unofficial 7DtD Modding Discord Server in the fns-smorgasbord channel.

I or one of the other community members will assist you as time permits.  


**Be kind:**

→ We are not paid tech support.  

→ We are not psychic.  

→ Screenshots of the F1 console are **not logs**.

→ You will not be assisted without logs!

---

## Log Files (Required)

When using **MO2 + Wabbajack**, logs are stored here:

C:\Users\YourUserName\AppData\Roaming\7DaysToDie\logs

Attach the **entire log file**, not screenshots.

Within the game, you can press the F1 Key, and in the top right there is a button for "Folder Location of Logs". 
Get your most recet log with the problem.


<img width="618" height="247" alt="image" src="https://github.com/user-attachments/assets/c3ffe936-4b6c-4d8f-82cc-84d23dfbb18d" />




**"Why do you guys stress Logs so much?"**

Because they generally help us narrow down the problem in seconds rather than playing 20 Questions with you. 

We all like our limited time on this world to be respected. You want to get back to your game, and so do we.


**Here's a funny real life example:**

User1: "Help, I don't know why my game is so dark?! I am only using ModAuthor1's mod called "Light".

ModAuthor1: _Proceeds to play 20 Questions with User 1 for all the reasons that could be causing their game to be dark._

ModAuthor2: Hi User1, are you absoloutely certain, like 100% sure you are only using ModAuthor1's mod, and no other mods, right?

User1: Yep, I am only using ModAuthor1's mod "Light". I'm totally 100% sure.

ModAuthor1: _Continues to play 20 Questions with User1 to determine the root cause. It's literally pages long of back and forth at this point._

ModAuthor2: User1, please just post your log for a sanity check.

_User1 posts logs. What do you know, the Log includes additional mods? Nope, never seen that before (*sarcasm). And one of them is named "DARK"._

ModAuthor2: So, you're 100% sure you had no others mods right? What about the one in your log called "DARK"? lol

User1: 🤦‍♂️ 


We stress logs because we see similar stories like this, almost daily!


Respect your time, and respect ours.  **JUST POST THE LOGS!**


---

## Basic Sanity Checks

### 1. Game Version

You **must** be on the current stable version of **7 Days to Die**.

Experimental builds are **not supported**.

---

### 2. Easy Anti-Cheat (EAC)

EAC **must be disabled**, not muted.

Disable it in the Steam 7DtD Game Launcher — permanently.


<img width="1278" height="542" alt="image" src="https://github.com/user-attachments/assets/552b4508-b815-42ec-b97e-0db2646475ab" />


<img width="1107" height="648" alt="image" src="https://github.com/user-attachments/assets/785ccd11-0c9c-4724-9414-835868584f14" />



---

### 3. Harmony Folder

You **must not delete**: 

C:\Program Files (x86)\Steam\steamapps\common\7 Days To Die\Mods\0_TFP_Harmony

The **only** mod allowed in the base game folder is **Harmony**.

If you deleted it:
- Verify game files in Steam
- It will be restored


Notice: Some Smorgasbord mods will add folders to your Mods folder, these are fine, they store your local settings for those mods.


---

### 4. Mods in the Wrong Folder

There must be **NO mods** in:

C:\Users\YourUserName\AppData\Roaming\7DaysToDie\Mods



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
2. Lower graphics from Ultra → High, or lower as your system allows
3. Disable Dynamic Mesh
4. Do **not** blindly copy someone else’s graphics settings

If the game crashes mid-session, the save **may** be unrecoverable.


## Disapearring folliage

Trees, plants, and textures flickering in and out?

A. Go to Video (Graphics) settings and Disable Occlusion. If you are playing with Better Biomes and Urban Decay, the author also suggests this.

B. Some overlarge POIs like those from The Walking Dead POI Pack and Fallout Vaults will not render correctly. This is a game engine limitation. POIs larger than 150x150 blocks will have issues with roads, textures, and RWG spawning.


<img width="3188" height="1110" alt="image" src="https://github.com/user-attachments/assets/77fd3da4-b1ef-40d6-9535-709f88209766" />



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
- 
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

Create Antivirus exceptions for:
- `ModOrganizer.exe`
- `7daystodie.exe`

## Windows Issue
This is an obscure one, but could be messing with 0_Harmony... Windows Security > Exploit Protection > Randomize Memory Allocations(Bottom-up ASLR).
If a user has Randomize Memory Allocations(Bottom-up ASLR) turned off, 
0_Harmony will not be able to properly patch any method and will cause null pointers on the first method that is called that is patched. 
To turn on ASLR, go to settings, look up Exploit Protection, set Randomize Memory Allocations(Bottom-up ASLR) to On by Default or Use default (On).

<img width="834" height="1153" alt="image" src="https://github.com/user-attachments/assets/92961937-1550-499e-b44f-e42d31713fe3" />


---

## MO2 Interface Problems

### “My load order is messed up!”

Click the **Priority** column header to re-sort.

You didn’t break anything.


<img width="1754" height="417" alt="image" src="https://github.com/user-attachments/assets/b4262a38-e6f5-41a5-9acf-b8d04d18b829" />



---

## Known Issues

**Benign Warnings and Errors**

Warnings come in yellow font within the (F1) Console.

Errors are listed in Red within the (F1) Console.

- WalkerSim produces many yellow warnings — **normal**
- Descent + Bait Bags produces a benign error — **harmless**
- Closer Weapon's Pack
-  OCB Maurice's Parachute mod. It will open the console with an Error, but it still works.  
The mod is disabled by default until he updates it. 
This happens every time TFP updates the game, but OCB usually only recompiles his mods when something is actually broken.
- There's likely more I'm missing


I have hundreds of hours played with these warnings present.


- Experimental mods are **not vetted**

---

## Final Reminder

If you:
- Read the README
- Read this Troubleshooting guide
- Followed instructions

…and it still doesn’t work?

Then yes — contact us over at Guppy's in the fns-smorgasbord channel.

Post logs with a description of the issue.

Reminder: No Logs = No Assistance!

If you skipped steps and winged it?

That’s on you.

🍽️ **Enjoy the buffet — but read the menu first.**
