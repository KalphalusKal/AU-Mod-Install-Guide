# Kals Mod Install Guide
Guides installing the mods I use which are currently:
Town of Us Mira
<!--Submerged-->
<!--ChaosTokens-->
LevelImposter

This guide assumes your on Windows or Linux



### Installing Among Us
First, we need to get the right version of Among Us. As of 11/9/25, the latest is the correct version, so just install the latest version of Among Us on Steam/Itch/Epic/Microsoft Store. Note that you cant downgrade the Microsoft Store version if it updates to a unsupported version. 
If the latest version is no longer supported, ill try to remember to update this
<!-- Theoretically you CAN downgrade the microsoft store versions, but theres no tool for it yet. This project has done it for Minecraft Bedrock but it only works on Minecraft: "https://github.com/MCMrARM/mc-w10-version-launcher"-->

### Opening game folders
When Among Us is installed, open the folders. 

From the Steam Library tab, you can right click the game, hover over "Manage", and hit "Browse Local Files"

In the Itch (App), you can right click the game and hit "Show in file manager"

From the Epic Library tab, you can hover over the game, click the 3 dot icon, hit "Manage", and hit "Show in Explorer" <!--I cant confirm this one, I found it online but I dont have Epic-->

In the Xbox (app) Library tab, go to the game, click the 3 dot icon, hit "Manage", go to the "Files" tab, hit "BROWSE...", and open the "Content" folder

Leave the file browser window open in the background

### Creating seperate mod folders
**If** you are modding a Microsoft Store copy, **skip this step**
*You can skip this, BUT if you do your game platform will auto update your modded game, breaking it*

Open the folder containing the Among Us Install Folder. If you dont know how to do this, heres how (Windows): To the left of the search thing in file explorer, theres a bar that shows the folder your in. Each folder is seperated by ">". Click the folder name thats left to the furthest right folder name.

Copy the Among Us folder and name it anything. For this guide, ill call it "Modded Among Us"

Open your Modded Among Us folder and close the other file browser window that you put in the background a bit ago. Dont close the Modded Among Us folder until the end of the guide

### Installing the mods
Normally, we would need to install BepInEx, but each mod includes it in its drag/drop to install files.
In this case, we will use the version of BepInEx that comes with Town of Us Mira as it uses the newest version.

To install Town of Us Mira, download the ZIP file labeled with the platform your modding from [here (https://github.com/AU-Avengers/TOU-Mira/releases/tag/v1.3.1-4)](https://github.com/AU-Avengers/TOU-Mira/releases/tag/v1.3.1-4)
When its downloaded, open the ZIP. You will see a folder named something like "TouMira-v1.3.1-4-(architecture)-(platforms)". Open that folder, and move/copy all its contents into the Among Us folder thats in the file browser. 

<!--Once thats done, download the file "submerged.dll" from [here (https://github.com/SubmergedAmongUs/Submerged/releases/tag/v2025.10.22)](https://github.com/SubmergedAmongUs/Submerged/releases/tag/v2025.10.22). Your browser might warb about it being potentially dangerous, thats because it is a type of executable, you can review its code if you dont trust it. Go to the file browser window, open the "BepInEx" folder, then open the "plugins" folder, and put "submerged.dll" in the folder.-->

<!--Once thats done, download the file "ChaosTokens.dll" from [here ([https://github.com/SubmergedAmongUs/Submerged/releases/tag/v2025.10.22](https://github.com/xChipseq/ChaosTokens/releases/tag/1.1.3))]([https://github.com/SubmergedAmongUs/Submerged/releases/tag/v2025.10.22](https://github.com/xChipseq/ChaosTokens/releases/tag/1.1.3)). Your browser might warb about it being potentially dangerous, thats because it is a type of executable, you can review its code if you dont trust it. Go to the file browser window, open the "BepInEx" folder, then open the "plugins" folder, and put "ChaosTokens.dll" in the folder.-->

Finally, download this GitHub actions build of LevelImposter from [here (https://github.com/DigiWorm0/LevelImposter/actions/runs/18235251840)](https://github.com/DigiWorm0/LevelImposter/actions/runs/18235251840), open the zip, and put LevelImposter.dll into the "plugins" folder. If the artifact expired or you cant access the action page, you can download a mirror that I put up [here (https://github.com/KalphalusKal/AU-Mod-Install-Guide/blob/main/.files/mods/LevelImposter.10a38d6.zip)](https://github.com/KalphalusKal/AU-Mod-Install-Guide/blob/main/.files/mods/LevelImposter.10a38d6.zip)

# Final Steps (Windows)
### Creating a Start Menu Shortcut (Windows)
If your on Epic, do the following on "EpicGamesStarter.exe" instead of "Among Us.exe", otherwise do "Among Us.exe"
Left click the game executable once, then hold right click on it and drag to a part of file explorer that doesnt have any files. Name the shortcut whatever you want it to show as.

Now that the shortcut exists, press Windows+R and type (or copy/paste) the following file path: `%APPDATA%\Microsoft\Windows\Start Menu\Programs`

Now hit enter on your keyboard and it will open a file browser window with the folder "Programs" open. Move the shortcut from the first window to the second window that has the Programs folder.

Now you have Modded your Among Us! Test it by opening it. It should have the Town of Us Mira logo if you did everything correctly

# Final Steps (Linux)
This assumes that your running the game through Steam Proton (Specifically "Proton Hotfix") and that your launching through Steam (Even if its the Epic/Itch version)

In the Steam Library tab, hit "Add a Game", followed by "Add a Non-Steam Game...", then hit "Browse..." and browse to your Modded Among Us launch file. This is "Among Us.exe" if you own Among Us on Steam/Itch, and is "EpicGamesStarter.exe" if you own Among Us on Epic

Now right click the newly added game entry, hit "Properties", and rename it to whatever. Then go to the "Compatibility" tab, hit the toggle for "Force the use of a specific Steam Play compatiblity tool", and select "Proton Hotfix" from the dropdown. If Proton Hotfix isnt installed, it will install.

Now launch the modded game. It wont have any mods yet as theres a few more steps after this that requires your modded copy to have loaded at least once.

Install [ProtonTricks](https://flathub.org/en/apps/com.github.Matoking.protontricks) from [Flathub (https://flathub.org/en/apps/com.github.Matoking.protontricks)](https://flathub.org/en/apps/com.github.Matoking.protontricks)

Open ProtonTricks, click your modded among us from the list, and hit "OK". The window will dissapear for a bit while its loading.

When its loaded, hit "OK" on the default selection, click "Run winecfg", and hit "OK". The window will dissapear again to load winecfg.

Go to the "Libraries" tab and type "winhttp" in the text box thats labeled "New override for library". Now hit "Add", followed by "OK".

Finally, hit close on ProtonTricks twice.

Now you have Modded your Among Us! Test it by opening it. It should have the Town of Us Mira logo if you did everything correctly
