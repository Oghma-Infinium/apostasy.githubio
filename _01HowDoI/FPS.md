---
layout: default
title: How Do I Uncap the FPS?
nav_order: 4
has_children: false
description: How Do I Uncap the FPS?
---

Apostasy is capped to 61 FPS by default. While [SSE Display Tweaks](https://www.nexusmods.com/skyrimspecialedition/mods/34705) fixes the vanilla engine bug that tied Havok physics to the frame rate, some mods may use their own custom code that still assumes a ~60 FPS limit. Running the game above these anticipated frame rates can cause issues with their Havok-based interactions. Additionally, the modlist includes some mods that run calculations based on a target FPS, which has been set to Apostasy's default of 61 FPS.  

To properly uncap the FPS, please follow the steps below:  
 1. In Mod Organizer 2, open the `Shadow Boost` mod under the `Performance Optimizations` separator.
 2. Navigate to the `ShadowBoost.ini` file and open it in your preferred text editor (e.g., [Notepad++](https://notepad-plus-plus.org/)).
 3. Under the `[Settings]` header, edit the `fTargetFPS = 61.000000` (line 2) to reflect your desired Target FPS.
 4. Save and Close the `ShadowBoost.ini` file.
 5. In Mod Organizer 2, open the `SSE FPS Stabilizer` mod under the `Performance Optimizations` separator.
 6. Navigate to the `SSEFpsStabilizer.ini` file and open it in your preferred text editor (e.g., [Notepad++](https://notepad-plus-plus.org/)).
 7. Under the `[Settings]` header, edit the `TargetFps = 61` (line 13) to reflect your desired Target FPS.
 8. Save and Close the `SSEFpsStabilizer.ini` file.
 9. Once in game, open the ENB GUI (`Shift+Enter`) and set your new FPS cap.
 10. Click `Save Configuration` in the top left of the ENB GUI and close the menu (`Shift+Enter`).

{: .warning} 
Failure to follow all of the above instructions will limit your potential performance as you exceed the list's target FPS. Also remember that these `.ini` files will be reset upon any list update and you will have to repeat this process.