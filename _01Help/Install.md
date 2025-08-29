---
layout: home
title: Installation Guide
nav_order: 2
description: Installation Guide
---

![image](/Assets/images/apostasy-header.png)

---

# Installation Guide

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
## Before We Begin

Apostasy and Wabbajack are licensed under the <a href="https://creativecommons.org/licenses/by-nc-sa/4.0" target="_blank" rel="noopener noreferrer">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International</a> license. This installation guide is provided "as-is" and will be updated if deemed necessary. For any assistance and support with the modlist, please see the ["Modlist Assistance and Support"](http://localhost:4000/#modlist-assistance--support) section on the home page of this Wiki. 

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

Before proceeding with the Installation Guide, please ensure that you have the following:

* **Windows 10** (sevice pack 22H2 or later) or **Windows 11** (service pack 24H2 or later).
* At least **400 GB** of free space on your PC. The size of the installation on disk is approximately **215 GB**, with an additional **175 GB** needed for mod downloads. Some additional temp space is required for the installation process itself.
* **The latest version** of ***Skyrim Special Edition***, in **English**, on <a href="https://store.steampowered.com/app/489830/The_Elder_Scrolls_V_Skyrim_Special_Edition/" target="_blank" rel="noopener noreferrer"> Steam</a>. This is **required**, other methods of game ownership <strong><a href="/01Support/FAQs/#why-steam-i-have-skyrim-from-another-source-and-it-wont-let-me-install" target="_blank" rel="noopener noreferrer">are not compatible</a></strong>.
* A <a href="https://users.nexusmods.com/register" target="_blank" rel="noopener noreferrer">Nexus Mods</a> account.

We also ***strongly*** recommend a <a href="https://users.nexusmods.com/account/billing" target="_blank" rel="noopener noreferrer">Nexus Premium Membership <svg viewBox="0 0 24 24" aria-labelledby="svg-external-link-title" width="1em" height="1em"><use xlink:href="#svg-external-link"></use></svg></a>, which speeds up the install by auto-downloading mods. (Without Premium, you are looking at a twelve hour, highly manual task.)

If you are **updating from a previous installation**, [click here for update instructions](/01HowDoI/UpdatingModlist/).

---
## Pre-Installation

Before we begin the actual installation process, some steps must be taken to ensure that all necessary prerequisites and dependencies are installed on your system.

---
### Installing Microsoft Visual C++ & .NET

 1. Install <a href="https://aka.ms/vs/17/release/vc_redist.x64.exe" target="_blank" rel="nooperner noreferrer">Visual C++ x64</a>.
 2. Install <a href="https://dotnet.microsoft.com/en-us/download/dotnet/9.0" target="_blank" rel="nooperner noreferrer">.NET Runtime 9.X.X Desktop x64</a>.
 3. Install <a href="https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-6.0.30-windows-x64-installer" target="_blank" rel="nooperner noreferrer">.NET 6.0 Runtime Desktop x64</a>.

{: .important}
If you have already installed Visual C++, please make sure to install it again and use the `Repair` option to get the latest version of the redistributable. **DO NOT SKIP THIS STEP** or Mod Organizer 2 and the game may fail to launch.

---
### Page file and Crash Prevention

Larger Skyrim modlists require a significant amount of memory to run, running out of memory **will** result in crashes and many other potential issues. Due to Apostasy's size and the number of files, this step is **NOT** optional, regardless of your PC specs.

If you are limited on space, the page file can be set after the installation process is over. A detailed guide on [how to set your page file can be found here](/01Help/Pagefile/).

#### Shader Cache (NVIDIA Users Only)

{: .important}
For NVIDIA GPU users, it is recommended to boost the size of your shader cache. These settings have been shown to improve stability, and while they may not be entirely necessary, they are still recommended.

In order to adjust your Shader Cache settings follow the steps below.

 1. Right click on your desktop and select `NVIDIA Control Panel`
 2. Navigate and click `Manage 3D Settings` in the left pane.
 3. Scroll down the **Global Settings** tab until you see **Shader Cache Size**.
 4. Double click `Driver Default` to the right of **Shader Cache Size** and select `10 GB`.
 5. Click `Apply` in the bottom right hand corner.
 6. Exit out of the NVIDIA Control Panel.

![](https://raw.githubusercontent.com/iAmMe27/Tahrovin/main/img/ShaderCache.png)

---
### Steam Setup

{: .warning}
If your Steam Library is located in the Program Files folder, please <a href="https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide" target="_blank" rel="noopener noreferrer">read this guide by LostDragonist</a>. Storing your library in locations such as Desktop, Documents, Downloads, OneDrive, or any other Windows-managed folders *will* cause issues with installing or running Apostasy.

 1. In Steam, <a href="https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable" target="_blank" rel="noopener noreferrer">disable automatic updates</a> for *Skyrim Special Edition*.
 2. Right-click on *Skyrim Special Edition*, go to **Properties** > **General** and uncheck `Enable Steam Overlay while in-game`.
 3. Ensure that your *Skyrim Special Edition* is [installed in English](#changing-the-game-language).
 4. Ensure that you properly [install the Creation Club](#installing-creation-club-files) content to prevent hashing errors while downloading the list.

#### Changing the Game Language

{: .important}
Due to limitations with Wabbajack, [Apostasy only supports the English Steam version of *Skyrim Special Edition*](/01Support/FAQs/#does-apostasy-support-any-other-languages). 

 1. Right click on Skyrim Special Edition in Steam.
 2. Click `Properties`.
 3. Click `Language`.
 4. Set the Language to `English`.

#### Installing Creation Club Files

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
> * **DO NOT** `Alt+Tab` during this process or it will fail to properly download these files. 
> * **DO NOT** verify your game files after doing the steps above as it will revert the "correct" file hashes for the CC files you just downloaded.

---
### Running the Game

Before continuing onto the rest of the installation process, *Skyrim Special Edition* needs to be ran at least once. This step should have been accomplished if you have been following along, however if it somehow has not been done, the game must be ran at least one time through Steam in order to generate files that Apostasy needs to function.

 1. Select *The Elder Scrolls V: Skyrim Special Edition* within your Steam library, then click `Play`.
 2. The *Skyrim Special Edition* launcher will offer to auto-detect your settings. When this happens, click `OK` and then click `OK` again, these settings do not matter.
 3. Click `Exit` to exist the *Skyrim Special Edition* launcher.

---
## Wabbajack Installation