---
title: "Recording Foley"
---

## Mic choice

Start with one of these microphones for Foley. Record a short test with your prop and choose the one that captures the sound most clearly.

- **[Austrian Audio CC8 pair](https://austrian.audio/product/cc8/)**. A good starting choice for footsteps, scrapes, and detailed prop work. Use one microphone for our mono Foley workflow.
- **[RØDE NTG5](https://rode.com/en-us/products/ntg5)**. A strong option for quiet Foley because of its low self-noise. Aim this directional shotgun at the action and keep the performance within its pickup area.
- **[Audio-Technica AT4041](https://www.audio-technica.com.hk/index.php?cid=31&lang=eng&op=productdetails&pid=151&sid=54)**. A good choice for footsteps, impacts, and other clear attacks. Try the CC8 or NTG5 first for very quiet rustles.

## Placement

Ament describes the standard Hollywood close-mic setup: the microphone sits about 6 inches above the surface, 1 to 2 feet in front of the performer, angled down at the contact point. That geometry catches the shoe or the prop while rejecting body movement and clothing rustle.

Two cautions:

- Recording too close adds proximity effect, an artificial bass boost. If the prop sounds boomy, back off before you reach for EQ.
- A distance of 2 to 3 feet gives a natural sound with a little room in it, which is what Ament calls the New York style. Try a cue both ways and compare.

## Footsteps

The beginner tells are over-articulated heel-toe walking, which sounds like "ta-da, ta-da," and flat-footed walking, which sounds like "plop, plop, plop." Watch the character's weight and pace before you perform, and walk the character rather than the shoe.

## Prepare to record

Open the shared *A Quiet Place* project prepared in the [spotting lesson](/lectures/week-5/reaper-spotting/). Its empty cue items are already arranged on specific Foley pass tracks inside category folders. Add or use a companion `REC` track directly below the selected `CUES` track. Keep both inside the same folder.

## Optional Foley Cue tool

[DAD 310 Foley Cue](https://github.com/tatecarson/reaper-foley-cue) reads the action descriptions and timing from your labeled empty items. It can browse cues by track, create or assign a companion `REC` track, rehearse and record with a three-beep count-in, and display the action text over the video.

**This tool has not been fully tested yet.** It is an experimental prerelease. Automated tests and limited macOS playback checks have passed, but microphone recording, physical mouse operation, picture sync, hardware latency, and Windows still need hands-on testing. Try it on a copy of your project. The manual workflow below remains available.

[Download Foley Cue v0.1.0](https://github.com/tatecarson/reaper-foley-cue/releases/download/v0.1.0/dad310-foley-cue-v0.1.0.zip) and follow the [installation and usage instructions](https://github.com/tatecarson/reaper-foley-cue#install).

Keep the empty cue items on their `CUES` tracks and add an action description to each item's notes. In the tool, select a cue, create or assign its `REC` track, then choose the microphone input and arm only that recording track. Leave four seconds before the cue for the count-in. Mute the template's separate CUE BEEPS track when using the tool's beeps. Turn on **Video overlay** to show the action and countdown on the picture. The tool stops one second after the action and clears the overlay.

## Record into the cues

1. Choose an empty cue item on its Foley pass track. Move the count-in until the beep item's right edge snaps to the cue item's left edge. Rehearse with picture.
2. Select the microphone's **mono hardware input** and arm only the companion `REC` track. Check that the microphone does not pick up the cue beeps. Keep the `CUES` and CUE BEEPS tracks unarmed.
3. Perform the loudest part while setting the interface gain. Aim around -18 to -12 dBFS for typical levels, with peaks below -6 dBFS. Record a test and check it for clipping, room noise, and beep spill.
4. Turn off the musical metronome. Right-click the transport Record button and choose **Record mode: normal**. Start recording before the count-in, then perform on the silent fourth beat. Leave a little room after the action before stopping. You may leave Repeat on to record several takes in a row.
5. Compare your takes and adjust the prop, performance, or microphone placement before recording again. Leave the empty cue items intact above the recordings. Keep your alternate takes until you have made your choices, and mute the beeps when you listen to the scene.

Record a little before and after each cue so you have room to edit.

Save the project with alternate takes for the [editing and layering lesson](/lectures/week-5/editing-foley/).

There is nothing to turn in today. Record the robot scene with your team outside class, then edit and mix your own complete session for [Assignment 2](/assignments/assignment-2-foley-recording/).

---

Source: Vanessa Theme Ament, *The Foley Grail*, 3rd ed., chapters 6, 7, and 8.
