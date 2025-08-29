---
layout: home
title: Common Installation Issues
nav_order: 6
description: Common Installation Issues
---

![image](/Assets/images/apostasy-header.png)

---

# Common Installation Issues

## Table of contents
{: .no_toc }
<details markdown="block">
  <summary>
     Expand to view
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

---
## Why is the list showing "in maintenance" on Wabbajack?

### What does it mean?

When a mod is updated, hidden, or removed, any modlist that is using that mod will automatically be put into maintenance mode to prevent users from downloading an incomplete installation.

If Skyrim updates the modlist will also undergo forced maintenance as it will need to be recompiled against the newest version of Skyrim.

### How long does maintenance last?

As long as necessary. No one can give you an ETA, maintenance will take as long as it needs to take. Please do not give our support staff a migraine asking about an update.

List updates will be posted in the `#server-updates` channel of the <a href="https://discord.gg/4WwqfK5yHg" target="_blank" rel="noopener noreferrer">Waking Dreams discord</a> server and in the `#skyrim-se` announcements channel of the <a href="https://discord.gg/wabbajack" target="_blank" rel="noopener noreferrer">Wabbajack discord</a> server.

### Can I download the list while it is under maintenance?

No.

### Can I partially download the list while it is under maintenance?

If you want to do it manually via the list manifest on the Wabbajack website, sure. Automatically, no.

### My install was in progress, can't someone just give me the missing file(s)?

No, Apostasy respects all mod author permissions. If a mod or file has been taken down, and has not allowed redistribution from another source, we will not provide you a link. 

Asking for one anyway is a violation of rules. (Even if you ask staff in a private chat) Sharing a link "you found" or reuploading a file is strictly prohibited unless you can prove you have permission to do so.

### Can't I just manually install / Is there a "Manual Installation" guide?

Not any more - As Wabbajack is a more reliable install method which requires little user interactions and produces a consistent install every time - the manual installation guide was removed.

### Can I edit the Wabbajack file so it installs anyway?

No. Wabbajack files are compiled and cannot be manually edited. 

---
## Wabbajack browser not loading anything on the login to Nexus Page.

Please install WebView2 by using the installer from this link: <a href="https://developer.microsoft.com/en-us/microsoft-edge/webview2/" target="_blank" rel="noopener noreferrer">Evergreen Standalone Installer <svg viewBox="0 0 24 24" aria-labelledby="svg-external-link-title" width="1em" height="1em"><use xlink:href="#svg-external-link"></use></svg></a>

If you already have it - uninstall and reinstall

---
## Wabbajack finds no results.

Typically caused by network management software "Killer control panel" which comes pre-installed with some laptops and PC's. (It may also be called Killer Intelligence Center or it's a K icon in your system tray)

To resolve, disable the **Prioritization Center** and **Auto Bandwidth**. Then restart Wabbajack.

![image](https://user-images.githubusercontent.com/26418143/210167325-998f3644-447e-43f5-8aad-49209c20edd2.png)

---
## Wabbajack fails to start with a "Unknown Error".

Delete Wabbajack.exe, Redownload from <a href="http:\\Wabbajack.org" target="_blank" rel="noopener noreferrer">Wabbajack <svg viewBox="0 0 24 24" aria-labelledby="svg-external-link-title" width="1em" height="1em"><use xlink:href="#svg-external-link"></use></svg></a>.

---
## Wabbajack fails to start "You Cannot run as a Admin".

Wabbajack cannot be run as an Admin. 

If you are not manually running the game as an Admin, check your windows UAC settings and make sure that UAC is not "off" as this will run everything as an admin.

![](/Assets/UAC.png)

Reboot your PC after making this change.

### If you have installed a custom version of windows and cannot turn on UAC (or you have and it doesnt work)

Apostasy does not support custom versions of windows. The instructions below are taken from the <a href="https://wiki.wildlandermod.com/01Support/Faq/#if-you-have-installed-a-custom-version-of-windows-and-cannot-turn-on-uac-or-you-have-and-it-doesnt-work" target="_blank" rel="noopener noreferrer">Wildlander Wiki</a> and may or may not work for you.

1. Create a basic user account (Accounts -> Other users then add other user, click on Users, more actions and create new user).
1. login to that account - start Skyrim to add the registry entries for that user.
1. Log back into your primary account.
1. Then Holding shift, right click the .exe which will give a "Run as different user" command, select your created basic user and if that user is not administrator it should work.

---
## Do I have to install both game and downloads to same drive

No, you can have them on separate drives - just make sure you point your Download location to where you want the zip files to live.

You can even share download folders between multiple modlists.

---
## How much drive space do I need?

Check out the [System Requirements & Installation](/02ModlistBasics/RequirementsInstall/) page for accurate information regarding the required drive space for Apostasy.

---
## Do I need to download everything? I am playing on a potato and would like to install the list without the visual mods.

Wabbajack will not support partial installations of modlists and requires any installation to have all of the mods it was compiled with. Creating a version of the list for potato users only is not easy to do and would require a completely separate Wabbajack modlist to be created and maintained.

There are no plans at this time to create a performance-cut of Apostasy.

---
## Can I just download the Graphics only?

No, again this would be a completely separate list which would need its own separate Wabbajack modlist.

There are no plans at this time to create a visual-only version of Apostasy.

---
## Wabbajack fails to find SkyrimSE.exe. / Wabbajack can not find my game folder.

There are several potential causes of this:

 1. You haven't ran Skyrim before after installing it.
 2. You do not own a Steam copy of Skyrim. See the [related FAQ](/01Support/FAQs/#why-steam-i-have-skyrim-from-another-source-and-it-wont-let-me-install) about non-Steam versions of the game.
 3. You have moved your Skyrim folder from where it was originally installed without utilizing the Steam "move install" option.
 4. There is a problem with your Steam install which is preventing Wabbajack's gamefinder library to identify the game. 
 5. You have a cracked version of Skyrim. See the [related FAQ](/01Support/FAQs/#cracked--steamemu) about cracked or emulated versions of the game.

---
## Wabbajack is asking me to login but isn't displaying the captcha.

Go to the settings menu, log out and then log back in - this page should display the captcha correctly.

---
## Wabbajack freezes with the error "Outside of Standard Install folder" or does not start downloading mods.

This issue is typically caused by a corrupted cache file. In order to fix this, reset your Wabbajack installation.

 1. Close Wabbajack if it is open.
 2. Press `Win+R` on your keyboard and type in `%localappdata%`
 3. You should see a Windows Explorer window pop up, find and delete the folder called `Wabbajack` inside.
 4. Restart Wabbajack, log back in again, and restart your installation.

---
## Every Nexus mod fails to download.

This is caused by your Nexus API tokoen expiring. It can be resolved by logging out and logging back into your Nexus through the Wabbaajck settings.

 1. Open Wabbajack and click the **Settings** button in the bottom-left corner of the Wabbajack app.
 2. Under the **Logins** box, click `Log out` next to the Nexus Mods login.
 3. Click the Nexus Mods `Log in` button.
 4. Restart Wabbajack and restart your installation.

![](/Assets/wj_nexusrelog.png)

---
## Wabbajack fails to download mods or hangs for a long time during installation.

Check Task Manager, if Wabbajack is not using any network resources, it is likely that the download has failed or timed out. If this is the case, check the suggestions below.

 1. If your Wabbajack log shows `“Wabbajack.Networking.Http.HttpException: Http Error Unauthorized - Unauthorized”`, this means your Nexus API token has expired and you need to relog into Nexus on the Wabbajack app.
 2. Close and restart Wabbajack - Start the Apostasy install process again, entering the same criteria as last time. Wabbajack will CRC check your existing files and should resume where it failed & complete the install without any further intervention.
 3. If that does not resolve the issue, try using a VPN service. Apostasy and the Waking Dreams staff is not affiliated with and does not endorse any specific VPN service. We do not provide user support for VPN services.

---
## Antivirus reports a virus with Wabbajack or the modlist!

Antivirus programs are notorious for false flagging <a href="https://stepmodifications.org/wiki/Guide:Mod_Organizer/Advanced" target="_blank" rel="noopener noreferrer">MO2's Virtual File System</a>, which can and will cause crashes and other problems. Antivirus programs like BitDefender, Norton, and Webroot are especially aggressive, and you will need to fully remove them from your PC in order to actually launch the game through MO2. 

Windows 10/11 may automatically quarantine a key file which is needed for Mod Organizer. This can be fixed by adding an exclusion for Mod Organizer in Windows Defender.

 1. Press the `Win` key.
 2. Type "Windows Security" in the search bar and hit `ENTER`.
 3. Click on **Virus & threat protection** in the left pane.
 4. Click **Manage settings** option under **Virus & threat protection settings**.
 5. Scroll down to **Exclusions** and click **Add or remove exclusions**.
 6. Windows Defender will now prompt you with a Run As Administrator pop-up, just hit `YES`.
 7. Click the **Add an exclusion** button at the top and choose **Folder**.
 8. Navigate to your Apostasy install folder and click `Select Folder`.
 9. **(OPTIONAL)** Repeat these steps for your Wabbajack (program) folder.

---
## "Missing Manual Downloads" error in Wabbajack

Wabbajack frequently has trouble downloading mods hosted on sites other than Nexus. If you fail on any of the following files then you should manually download and add them to your downloads folder.

{: .important}
**DO NOT** unzip these files. 

### Google Drive Files:

* <a href="https://drive.google.com/uc?id=15_0njBUjHKidNnJPmLXEygzGVWsA3Zbq&export=download" target="_blank" rel="noopener noreferrer">High Poly Head v1.4 (SE).zip</a>  
* <a href="https://drive.google.com/file/d/1CXdZi2vOpxKde6H_5NZaJOeHmMsJIreT/" target="_blank" rel="noopener noreferrer">HDT-SMP Elite Wolf Armor Patch.rar</a>  
* <a href="https://drive.google.com/file/d/1Xz3EXwzvY1pmzS9RiLl21m89eaYJ00-g" target="_blank" rel="noopener noreferrer">HDT-SMP Elite Wolf Armor Patch for CBBE 3BA.rar</a>  
* <a href="https://drive.google.com/file/d/1qsW6gFcmZdS5yZLnS0owQQyf0b-J6thB" target="_blank" rel="noopener noreferrer">HDT-SMP Elite Wolf Armor Patch for HIMBO.rar</a>  
* <a href="https://drive.google.com/file/d/1rX4INfO3ieWp25gPh0NiLPl1ktLoegZ9" target="_blank" rel="noopener noreferrer">Olivier Kenjutsu Battleaxe and Warhammer v1.0 AMR SE.zip</a>  

### Patreon Files: 

The following patreon mods are freely available and utilized by the modlist.  

* <a href="https://www.patreon.com/file?h=68233071&i=11449877" target="_blank" rel="noopener noreferrer">Eskyrim MCO Installer 1.2.7z</a>  
* <a href="https://www.patreon.com/file?h=79874952&i=13365775" target="_blank" rel="noopener noreferrer">_Fuse00_ArmorHighlander_CBBE.rar</a>  
* <a href="https://www.patreon.com/file?h=79874952&i=13365782" target="_blank" rel="noopener noreferrer">_Fuse00_ArmorHighlander_VanillaMale.rar</a>  
* <a href="https://www.patreon.com/file?h=67711235&i=10980531" target="_blank" rel="noopener noreferrer">_Fuse00_ArmorMelonyCBBE.rar</a>  
* <a href="https://www.patreon.com/file?h=115658146&m=376483627" target="_blank" rel="noopener noreferrer">_Fuse00_ArmorSpriggan_CBBE.rar</a>  
* <a href="https://www.patreon.com/file?h=115658146&m=376483634" target="_blank" rel="noopener noreferrer">_Fuse00_ArmorSpriggan_Vanilla Male.rar</a>  
* <a href="https://www.patreon.com/file?h=68902488&i=12781379" target="_blank" rel="noopener noreferrer">_Fuse00_ArmorSonaCBBE_V1.1.rar</a>  
* <a href="https://www.patreon.com/file?h=68902488&i=13158956" target="_blank" rel="noopener noreferrer">_Fuse00_ArmorSonaVanillaMale_V1.2.rar</a>  

---
## Unable to download Skyrim_Default.ini or SkyrimPrefs.ini

Apostasy only supports an English installation of Skyrim through Steam. To change the language of your installed Skyrim Special Edition, follow the steps below:

 1. Right click on Skyrim Special Edition in Steam.
 2. Click `Properties`.
 3. Click `Language`.
 4. Set the Language to `English`.

---
## Unable to download Data_ccbgssse037-curios

Due to some change Bethesda made with the 1.6.1130 update (January 17, 2024), Steam has begun including the free Creation Club (CC) files with the base installation of Skyrim. However, these files do not have the same file hash as the files that are downloaded from the in-game **Creations** menu for Anniversary Edition (AE) users. In order to comply with Wabbajack policy, and minimize issues for users who own the AE update, Apostasy is compiled using the versions of the CC content that are obtained from the in-game **Creations** menu.

Please follow the steps below if you are failing to download the Rare Curios files:

 1. Navigate to your Skyrim Special Edition's Steam `Data` folder.
 2. Delete *both* Rare Curios files: `ccbgssse037-curios.bsa` & `ccbgssse037-curios.esl`.
 3. Launch Skyrim Special Edition from Steam and select **Creations** at the main menu.
 4. Select **Search** at the bottom and search for `Rare Curios`.
 5. Select the card titled `Rare Curios` and press **Download**.
 6. Once the download is finished, exit the game and rerun the Wabbajack installer.

![](/Assets/skyrim_curios.png)

{: .warning}
* **DO NOT** `Alt+Tab` during this process or it will fail to properly download these files.
* **DO NOT** verify your game files after doing the steps above as it will revert the "correct" file hashes for the CC files you just downloaded.

---
## Wabbajack could not find part of the path "TEMP_BSA_FILES"

This error is typically cuased by some problem with extracting zip files. The quickest solution is as follows:

 1. Close Wabbajack.
 2. Go to your install folder and locate the `TEMP_BSA_FILES` folder (if it exists).
 3. Delete that folder (if it exists).
 4. Restart Wabbajack.
 5. Rerun the Wabbajack installer.

If the `TEMP_BSA_FILES` folder does not exist, then delete the download file for the mod being referenced before restarting Wabbajack.

{: .note}
Using the **Retry** button will not work as Wabbajack does not understadng that there was an issue with file extraction and will not retry the extraction process.

---
## Sanity check error extracting file.

Wabbajack will occassionally have issues extracting files if they use special characters. If you encounter this issue within your Wabbajack log, please try the steps below:

 1. Press `Win+R`.
 2. Type `intl.cpl` and hit `ENTER`.
 3. Navigate to **Administrative** and click `Change system locale...`.
 4. Change the **Current system locale:** to `English (United Kingdom)`.
 5. **Uncheck** `Beta: Use Unicode UTF-8 for worldwide language support`.
 6. Click `OK`
 7. **Restart your PC** and rerun the Wabbajack installer.

---
## Wabbajack is crashing during the installation!

If you find yourself struggling to run Wabbajack without it crashing, freezing up, or blue-screening your PC, please try lowering Wabbajack's resource usage with these steps:

 1. Open Wabbajack and click the **Settings** button in the bottom-left corner of the Wabbajack app.
 2. Under the **Performance** box, lower *each number for each category* to half of what it is currently set to.
 3. Restart Wabbajack.
 4. Rerun the Wabbajack installer.

![](/Assets/wj_resources.png)