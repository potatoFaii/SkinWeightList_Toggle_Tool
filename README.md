![MEL](https://img.shields.io/badge/MEL-Autodesk_Maya-blue?style=for-the-badge)

# Toggle Paint Weight Item for Autodesk Maya

## Overview

**Toggle Paint Weight Item** is a lightweight MEL utility designed to simplify skin-weight painting in Autodesk Maya.

The script toggles the influence list in the **Paint Skin Weights Tool** between showing **unlocked joints only** and showing **all joints**. This helps riggers focus on the influences they are currently painting without manually navigating a long joint list.

## Features

- Hide locked influences from the Paint Skin Weights influence list.
- Reveal all influences again with the same script.
- Quickly switch between a focused and complete influence list.
- Keep existing skin weights and joint lock settings unchanged.
- Simple MEL script suitable for assigning to a Maya shelf button or hotkey.

## Usage

1. Open **Paint Skin Weights Tool** in Maya with a skinned mesh.
2. Run `Toggle_paintweight_item.mel` using Maya's MEL Script Editor, or add the script to a shelf button.
3. Run it again to switch the influence-list visibility mode.

> **Note:** The script operates on Maya's Paint Skin Weights influence tree (`theSkinClusterInflList`). It only changes which list items are visible, not the underlying skinning data. Depending on the initial toggle state, the first execution may show all influences; subsequent executions alternate between the two modes.

## Credits

**Created by Lui Kit Fai**  
Category: Rigging / Skin Weight Utilities

Developed to reduce repetitive influence-list management during skin-weight painting.
