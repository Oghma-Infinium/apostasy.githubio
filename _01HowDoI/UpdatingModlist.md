---
layout: default
title: How Do I Update the Modlist?
nav_order: 15
has_children: false
description: How Do I Update the Modlist?
---

## Before proceeding

 1. Make sure that any instance of Mod Organizer 2 is closed.
 2. Make sure that any instance of Skyrim is closed.
 3. Make sure that any instance of Wabbajack is closed.

---

{: .warning } 
> **We recommend that everyone performs a clean install every time they upgrade.**  
>
> The reason for this is Wabbajack reads through and CRC-checks everything in the mods folder. Unfortunately, this process is time-consuming and doesn’t always detect corrupted files.

## Clean Installation (optional)

Although clean installations are *optional*, they are highly recommended, especially for major updates.

To perform a clean installation, delete the `\Mods` folder within your modlist directory. By doing this, you will reduce the chance of corruption (or carrying over corrupted files) when updating the list. 

![image](/Assets/folderpath_mods.PNG)

## Updating the Modlist

Updating the modlist is similar to installing the list (see [Installation](/01Help/Install)). Simply point Wabbajack to the same `Installation Location` (red) and `Download Location` (green) as your existing installation (e.g., `F:\Apostasy`).

![image](/Assets/wj_installpage.PNG)

Please keep in mind that any mods you may have added to your personal install of the list will be deleted when updating. To prevent Wabbajack from deleting your added mods when updating, add `[NoDelete]` as a prefix to them.

![image](/Assets/wj_nodelete.PNG)

## Modlist Versioning

Versioning for this modlist will generally adhere to the following format: `MAJOR.MINOR.PATCH`  

 - `MAJOR`: Generally indicates that at least one core area of the list has received a massive overhaul. These updates will **NEVER** be Save-Safe.
 - `MINOR`: Generally indicates that the modlist has received a multitude of bug fixes, minor mod changes, and/or has had LODs regenerated. These updates will not be Save-Safe unless otherwise specified.
 - `PATCH`: Generally indicates that the modlist has received only minor bug fixes or mod updates. These updates will always be Save-Safe.

The [Changelog](/06ModlistVersions/CHANGELOG) will contain more detailed information for any given modlist update and will indicate whether an update is Save-Safe with one of the tags below:

Save-Safe 
{: .label .label-green}

Save-Safe, with exception or conditions
{: .label .label-yellow}

Not Save-Safe. New Game Needed 
{: .label .label-red }