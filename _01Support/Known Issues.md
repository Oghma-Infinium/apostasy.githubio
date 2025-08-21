---
layout: default
title: Known Issues & Workarounds
nav_order: 4
description: Known Issues & Workarounds
---

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
## Issues which cannot be resolved.

This section includes issues which cannot presently be resolved due to the issue being related to the technical functionality of a mod, the time it would take to correct would not be of benefit, or a engine issue related to Skyrim itself.

### Getting "Failed to start Dialogue Quest" error in the Start Room.

This issue is caused by the Alternate Start scripts breaking during the character creation process. This issue only seems to occur if you:

 A. Start a New Game by backing out of an existing save into main menu without restarting the game entirely. You can read more on why this is an issue [here]().  
 B. Modified the list and have conflicts with the scripts that [Alternate Perspective](https://www.nexusmods.com/skyrimspecialedition/mods/50307) edits.  

There is nothing we can do to correct this and any New Game created that receives this issue will be corrupted, **bug reports on this topic will be deleted.**

### When leveling up skills, new perk nodes do not get highlighted until exiting and re-entering the perk menu!

This is a Skyrim bug that has to deal with menus not being updated while open and occurs due to [Static Skill Leveling](https://www.nexusmods.com/skyrimspecialedition/mods/89940) causing skills to advance while the menu is open.  

Perks can still be selected while the menu is open if the pre-requisites are met, this is purely a visual bug. 

### Lights are flickering on and off.

This is caused by Skyrim's engine limitation of 4 light sources in a 30ft radius of the player. When you move the camera in a area with more than 4 light sources they alternate/cycle and turn on and off. This includes your torches and/or lantern.

There is nothing we can do to correct this, **bug reports on this topic will be deleted.**

### NPC's added by mods don't have voice lines or are immersion breaking.

Unfortunately, this would require a great deal of effort to replace the voice lines and dialog so they fit.

### Bookshelves can be used to duplicate items placed upon them.

E.g Placing a book on a shelf, removing the book from the shelf by "picking it up" then using the shelf inventory to get a copy.

Unfortunately, this is a engine issue where removing the book from the shelf by pickup doesn't edit the container.

### SkyUI Groups broken.

When a item changes condition, either via tempering or via degredation, any groups that that item was assigned to no longer functions.

SkyUI uses SKSE to find the specific item (via CRC) to equip. changes to a weapon, either name or temper causes the CRC to change and prevents groups from functioning. There is nothing we can do to prevent the CRC from changing.

### Thieves guild quests not starting when handing in the previous quest.

This is a vanilla issue, there is a section further down this page which contains work arounds for the common problems.

### Night Eye effects are broken.

This is an issue with the way [ENB](https://enbdev.com/) shaders interact with [ImageSpace Modifiers](https://ck.uesp.net/wiki/ImageSpace_Modifiers). 

Fixing Night Eye effects would require us to rewrite a large amount of the shader code for parts of the ENB used by the modlist, and we have decided that the marginal benefit is not worth the time investment.

---