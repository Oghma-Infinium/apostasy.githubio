---
layout: default
title: How Do I Change my Resolution?
nav_order: 5
has_children: false
description: How Do I Change my Resolution?
---

{: .warning} 
Skyrim scales very poorly at resolutions above 1080p (1920x1080) and depending on your hardware, it might be difficult to achieve consistent FPS on higher resolutions.

By default, Wabbajack will set the resolution in the list's `Skyrimprefs.ini` to match the native resolution of your monitor. The preferable way to change your resolution is to modify the `SSEDisplayTweaks.ini`. 

To properly adjust your Resolution, please follow the steps below: 
 1. In Mod Organizer 2, open the `SSE Display Tweaks` mod under the `???` separator.
 2. Navigate to the `SSEDisplayTweaks.ini` file and open it in your preferred text editor (e.g., [Notepad++](https://notepad-plus-plus.org/)).
 3. Under the `[Render]` header, edit the `#Resolution=1920x1080` (line 66) and change it to your desired resolution.

![](/Assets/ini_SSEDisplayTweaks01.png)

 4. **(Optional)** Adjust the `#ResolutionScale=0.75` (line 67) to your desired resolution scaling.
 5. Ensure that you remove the `#` before `Resolution=` and `ResolutionScale=` to uncomment those lines so that they take effect.

![](/Assets/ini_SSEDisplayTweaks02.png)

{: .highlight}
Remember that these `.ini` files will be reset upon any list update and you will have to repeat this process.