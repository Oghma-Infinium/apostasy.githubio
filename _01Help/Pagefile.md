---
layout: default
title: Setting a Page File
nav_order: 3
description: Setting a Page File
---

{: .warning}
Larger Skyrim modlists require a significant amount of memory, running out of memory **will** result in crashes and other potential issues. 
Due to Apostasy's size and number of files, a page file is **NOT** optional. I do not care how much RAM or VRAM you have, you must do this.

## What is a page file?

A page file (also known as a "paging file") is an optional, hidden system file on a hard disk. Page files are utilized when your computer runs out of physical RAM to temporarily store data that isn't actively being used. Page files help prevent crashes and keep your system running smoothly.

## Why do we need a page file?

Skyrim is a very old game (originally released in 2011) that is built on the <a href="https://en.wikipedia.org/wiki/Creation_Engine" target="_blank" rel="noopener noreferrer">Creation Engine</a>, a engine based off of the <a href="https://en.wikipedia.org/wiki/Gamebryo" target="_blank" rel="noopener noreferrer">Gamebryo engine</a> that was originally used for Morrowind (released in 2002, before I was born).

Through lots of experience and trial-and-error, we have discovered that increasing the window's pagefile can fix certain types of Skyrim crashes, the two most common examples being `Unhandled native exception occurred at 0x7FF6ADC8DDDA` and `Unhandled native exception occurred at 0x0`.

But why is this? Skyrim appears to use system memory in very unexpected ways, for example it will frequently dip into the pagefile memory despite there being available RAM. Based on internal testing, Skyrim heavily favors high speed, low latency RAM.

## How do I set up a page file?

In order to set up a page file follow the steps below.

 1. Press `Win+R`.
 2. Type `sysdm.cpl ,3` and hit `ENTER`.
 3. Navigate to **Performance** and click the box `Settings...`.
 4. Click the **Advanced** tab.
 5. Under **Virtual Memory** click the box `Change...`.
 6. Uncheck `Automatically Manage` (if it is checked).
 7. Select your disk drive, ideally your fastest solid state drive.

{: .note}
Your page file does not need to be on the same drive as your Apostasy installation.

 8. Click `Custom Size:`.
 9. In the box next to **Initial Size (MB)**, type `40960`.
 10. In the box next to **Maximum Size (MB)**, type `40960`.

{: .alternative}
If you have 64GB of RAM or more, you can try setting these sizes to `20480` in order to save some space.

 11. Click `Set`.
 12. Click `OK`.
 13. Click `Apply`.
 14. Click `OK`.
 15. **Restart your PC**

![](/Assets/pagefile.png)