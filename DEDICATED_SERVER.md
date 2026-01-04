## How to convert this ModList to run on a **Self-Hosted** Dedicated Server:


**Warning!** Setting up a dedicated server is for _advanced_ users. 

FNS and the kind community members over at Guppy's are not your paid tech support for this. 

You can ask for help, but Dedi's are not our focus.


One of our Community Members named **Kajdaniec** has converted this ModList to run on a Dedicated Server using MO2.  

In Steam, you must have "Tools" checked in your games Library Games dropdown:

<img width="326" height="308" alt="image" src="https://github.com/user-attachments/assets/344aa76c-43f1-452f-8c73-0d435fdaef3d" />

Then you must download the latest stable version of the 7 Days to Die Dedicated Server tool. 

_The image might be old by the time you are reading this!_

<img width="737" height="419" alt="image" src="https://github.com/user-attachments/assets/caae90e0-0274-42a5-9068-69ed94409b48" />

In MO2 -> From the top of the Application, in the Tools tab -> press Executables.

This will open up the Modify Executables pop-up window.

For the machine you are converting into a Dedicated Server, you will want to change the **"Binary"** and **"Start in"** line from this:

<img width="902" height="684" alt="image" src="https://github.com/user-attachments/assets/7198d1f0-247f-4716-87d1-bd45c4f14322" />

**_To this:_**

<img width="949" height="687" alt="image" src="https://github.com/user-attachments/assets/cc6e7953-aeab-4b65-a30c-8193b35828cb" />



There are users who have used Kajdaniec's method on a separate computer, and some users who have self-hosted the Dedicated Server from the same machine they are running their own game from.  


Here are the XML changes he made:

![image](https://github.com/user-attachments/assets/54b55fe3-7728-46b1-a5cc-a1ec055c160c)

![image](https://github.com/user-attachments/assets/69a11a3a-9c11-4c9d-a2b4-48fd2fffc979)

______________________________________________________________________________________________________________________


## How to convert this ModList to run on a Service Provider **Hosted** Dedicated Server:

This section was largely trail-blazed by community member RipJammer. If you see him around, just give him a thank you if you used this process.  

1. In MO2, enable the mods you want to include into your Dedicated Server version of the Smorgasbord Mod List for your users.

2. Open MO2 -> change the top dropdown from 7 Days to Die to Explore Virtual Folder. Hit Run.
(remember to revert this when you go back to single player)

<img width="576" height="386" alt="image" src="https://github.com/user-attachments/assets/60011efb-2f39-463b-9aff-5f991d4fd7fe" />


3. Grab all of the mods from the Mods - Explorer++ virtual folder that opened when you hit Run within MO2. 

<img width="2423" height="1226" alt="image" src="https://github.com/user-attachments/assets/aca0fa81-ec26-4d18-93a5-9a39cb756c33" />

4. Within the Mods - Explorer++ virtual folder, Ctrl+a and Ctrl+c to select and copy all of those mods. 
From the top of that window, press the "Copy to" button.

<img width="730" height="304" alt="image" src="https://github.com/user-attachments/assets/f9c689e6-2719-4b81-9177-a8bb7ef9a881" />

5. Make a New Folder.

<img width="415" height="507" alt="image" src="https://github.com/user-attachments/assets/52a60df8-1323-48cb-832f-46629b6607e7" />

The copying process can take a while. 

<img width="445" height="283" alt="image" src="https://github.com/user-attachments/assets/769482cf-44db-4c3e-9a64-9114f4645117" />

Once it's complete, you can exit the virtual folder and MO2 as you like. 

Your temp_mods folder is now full. You can zip this folder and store it online for redistribution for users.

You can host this with a Server Provider, a Google Drive (if you've paid for extra storage beyond the 15 GB free), or somewhere else like Azure.


I would not recommend hosting from Google for security reasons, but you do you. 
If you are playing with a private group of friends, it's probably fine.
For public servers, you open up yourself and other users to being hacked.
It's just not a secure platform, and I wouldn't personally download random dll files from disreputable Google Drives.


> [!WARNING]
> Do _not_ host this on NexusMods, or other mod hosting sites!
> **This is not your work!**
> Bundling other people's mods as your own will have negative consequences. You will be branded a mod thief!
> You are only allowed to distribute this to people using your Dedicated Server directly.
> If you ignore this advice. I promise you your Mod Page will get delisted, and account could be banned.


Next Steps:

Drag a copy of all of the mods you just made, and place them into the 7DtD Dedicated Server Tool Mods folder.


Configure and Launch your server as you normally would.


Remember, all users (Clients) and the server itself must have all of these mods. 
Smorgasbord has both Client and Server side mods. 
FNS does not have the time to track down which mods are client side.  
Make sure everyone (and the server) has all of the mods!

Your players must add the list of mods from your zip, unzipped, into their Mods folder. 

They must have Harmony present!

You must play with EAC disabled! Too many of the mods on this list will trigger EAC if it is enabled. 
I would be careful who you invite into your dedicated server when EAC is off!

I'm no Dedicated Server expert, but here is a small list of Mod considerations: 

**1. You might consider going into the XML of SCore, Gears Manages Score, and Guppy Fire to disable Fire.**
Fire can be hard on server performance and sometimes act buggy.  


2. Also, I would recommend not using on Better Biomes, or Urban Decay because they will bring your performance down


3. Depending on your server specs, The Descent and CompoPack/CUBP can be hard on performance.


4. Also be aware of things like your settings on either Remote Crafting/Beyond Storage 2 if you choose either.
