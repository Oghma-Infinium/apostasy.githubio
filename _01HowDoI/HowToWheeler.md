---
layout: default
title: How Do I Use the Wheel?
nav_order: 13
has_children: false
description: How Do I Use the Wheel?
---

Apostasy uses [Wheeler](https://www.nexusmods.com/skyrimspecialedition/mods/97345) as a psuedo-replacement for the vanilla favorites menu. While the original favorites menu can still be accessed with `G` by default, and is needed for Vampire and Werewolf forms, it is mostly deprecated by the addition of the quick wheel system. This page will explain how to utilize and configure Wheeler.  

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

# The wheel

## Structure
Wheeler's hierarchy goes like this:

Wheels -> Wheel -> Slot -> Item

Simply put, you can have more than one wheel, in which you can have some slots, and each slot can contain more than one item. This hierarchy allows you to store basically your whole inventory/magic menu into the wheels.

![Wheel Hierarchy](https://github.com/D7ry/wheeler/blob/main/images/hierarchy_wheel.gif?raw=true)  

*Browsing through multiple wheels(mouse scroll up/down by default)*

![Slot Hierarchy](https://raw.githubusercontent.com/D7ry/wheeler/refs/heads/main/images/hierarchy_slot.gif)  

*Switching between different items in a single slot(mouse 4 and 5 by default)*

## Display
Each slot displays the texture of the name of its current item (slots can have multiple items in it), and the center of the wheel displays an enlarged texture as well as a detailed description of the item, when applicable.

![Item Display](https://raw.githubusercontent.com/D7ry/wheeler/refs/heads/main/images/item_display.gif)  

*Spinning the wheel*

## Item usage
Using (equipping/consuming) an item through the wheel is no different from using it in the inventory; simply left/right-click on the item will equip it to the corresponding hand.

![Item Usage](https://github.com/D7ry/wheeler/blob/main/images/item_usage.gif?raw=true)  

*Equipping items with ease*

## Wheel Editing

### Edit Mode

Changes to the wheel can be made when you open the wheel in either the inventory or magic menu. When you open the wheel in these two menus, the background will grey out, suggesting that you're now in "edit mode".

![Enter Edit Mode](https://github.com/D7ry/wheeler/blob/main/images/enter_edit_mode.gif?raw=true)  

*Enter edit mode by opening the wheel in the inventory/magic menu*

### Creating New Wheel/Slot

By default, create an empty wheel using the "N" key and an empty slot using the "M" key. You can create as many wheels and as many slots in a single wheel as you'd like.

![Slot Insertion](https://github.com/D7ry/wheeler/blob/main/images/slot_insertion.gif?raw=true)  

*Have as many slots as you'd like*

### Item Insertion

To insert an item or magic into the slot, hover on the item you desire in the inventory, open the wheel, and left-click (right shoulder) on the entry you wish to insert the item into.

![Item Insertion](https://github.com/D7ry/wheeler/blob/main/images/item_insertion.gif?raw=true)  

*As convenient as the favorite menu*

### Slot/Wheel Ordering
To change a slot's order in a wheel, press the up/down arrow to swap its position with neighboring slots.
To change a wheel's ordering among all wheels, press the left/right arrow to swap its position with neighboring wheels.

![Slot Ordering](https://github.com/D7ry/wheeler/blob/main/images/slot_ordering.gif?raw=true)  

*Visualize your edits in real-time*

### Deletion

To delete an item from a slot, simply right-click (left shoulder) on the item you wish to delete.  
Right-clicking (left shoulder) on an empty slot deletes the slot.
Right-clicking (left shoulder) on an empty wheel deletes the wheel (you can't delete the last wheel).

![Slot Deletion](https://github.com/D7ry/wheeler/blob/main/images/slot_deletion.gif?raw=true)  