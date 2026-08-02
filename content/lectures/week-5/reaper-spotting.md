---
title: "Spotting Foley in Reaper"
---

To streamline your Foley workflow in Reaper, follow these steps:

 **Install Essential Extensions:**
   - Begin by installing the [ReaPack: Package manager for REAPER](https://reapack.com/) and [SWS / S&M Extension](https://www.sws-extension.org/) for added functionality.

 **Quickly Insert Empty Item:**
   - Create a hotkey for inserting an empty item for faster spotting; for example, set it to `Ctrl + E`.

 **Add Item Notes:**
   - Double-click on items to add notes of what you'll record into the Item.

 **Set Loop for Empty Item:**
   - Set up a loop.
   - Create a hotkey for setting the time selection to items; for example, set it to `Cmd + L`.

 **Configure Recording Mode:**
   - Use the "Record mode: auto-punch selected items" option to record over the empty item.
   - You can change this recording mode by right-clicking on the record button.

 **Rename Takes from Item Notes:**
   - After recording, run the script called "X-Raym_Convert selected item notes to take name.lua" to rename your active take based on the item notes.
   - Create a hotkey for running this script; for example, set it to `Ctrl + T`.

 **Crop to Active Take:**
   - Finally, when you've decided on the take you want to keep, use Reaper's cropping feature to trim to the active take.

