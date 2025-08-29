---
layout: default
title: How Do I edit the ENB?
nav_order: 14
has_children: false
description: How Do I edit the ENB?
---

You can edit the various Settings of the ENB configuration inside of the ENB menu while in-game. 

The list of ENB shortcuts can be seen below:
 1. `Shift + Enter` to open the ENB menu/GUI.
 2. `Shift + F12` to disable/enable the ENB.
 3. `Shift + F6` to toggle ENB's Depth of Field shader.
 4. `F4` to toggle ENB's FPS Counter.

---

## Adjusting the FPS Cap

See the [How Do I Uncap the FPS?](/01HowDoI/FPS) page for the full instructions to change the desired FPS cap.

## Night Eye is Too Dark

See the [Known Issue](/01Support/Known%20Issues/#night-eye-effects-are-broken) regarding Night eye in Apostasy's ENB.

## Tweaking Interior Brightness

In order to tweak (brighten or darken) interiors via the ENB menu, follow the steps below:
 1. Hit `Shift + Enter` to bring up the ENB GUI.
 2. In the right tab called *Shader Parameters* at the top, expand the `ENBEFFECTPOSTPASS.FX` tab.
 3. Scroll several subcategories below this header until you see a `|==Shadows Interior==|` header.
 4. Adjust the `Gamma Interior` value for brighter or darker interiors. Lower values will brighten the interiors while higher values will darken them.
 5. Click `Save Configuration` in the top left corner of the ENB GUI to save your edits.

{: .Notice}
Any tweaks to the ENB configuration will be reset upon any list update and you will have to repeat this process.