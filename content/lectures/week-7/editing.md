---
title: "Editing in Reaper"
---

## I - Identify Clicks, Pops, and Errors

We'll start with a [piece of audio](../clicky.wav) that has a click in it. There is specialized software for getting rid of clicks and pops, but we can do an ok job just in Reaper.

First find the beginning of the click and add a split. Notice that Reaper automatically adds a fade out and fade in to the splits. Now you can adjust the fades so that the sound is as natural as possible while still removing the click.

We can use the same concept as before to remove pops or plosive sounds. Here's some [popping audio](../pops.wav).

Also try different fade shapes.

You can use equalization to further clean up your audio files. A high pass filter is perfect for getting rid of low frequency rumble. Here's some [rumbley sounds](../low-freq-hum.wav).

If the high pass filter is not enough, the the ReaFir plugin. First put the plugin into subtract mode. Then, find a place in your audio that has only material you want to remove. Select "Automatically build noise profile" and then play this section a few times. Now uncheck that box and the offending frequencies should be removed.
