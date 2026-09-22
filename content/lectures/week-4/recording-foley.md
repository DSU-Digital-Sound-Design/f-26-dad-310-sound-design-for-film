---
title: "Recording Foley"
---

## Mic choice

We record Foley with a condenser microphone in a cardioid pattern. Try both a large diaphragm and a small diaphragm on your source and keep whichever serves it better.

Our small-diaphragm options:

- AT 4041
- Slate Digital ML2
- ST31 FET
- Carvin CM90e
- MXL 990

The industry workhorse on professional stages is a shotgun, most often the Sennheiser MKH 416, chosen for its midrange punch and its rejection of off-axis sound. Our cardioids play the same role at our scale: focus on the prop, reject the room.

## Placement

Ament describes the standard Hollywood close-mic setup: the microphone sits about 6 inches above the surface, 1 to 2 feet in front of the performer, angled down at the contact point. That geometry catches the shoe or the prop while rejecting body movement and clothing rustle.

Two cautions:

- Recording too close adds proximity effect, an artificial bass boost. If the prop sounds boomy, back off before you reach for EQ.
- A distance of 2 to 3 feet gives a natural sound with a little room in it, which is what Ament calls the New York style. Try a cue both ways and compare.

## Footsteps

The beginner tells are over-articulated heel-toe walking, which sounds like "ta-da, ta-da," and flat-footed walking, which sounds like "plop, plop, plop." Watch the character's weight and pace before you perform, and walk the character rather than the shoe.

## Prepare to record

Open the shared *A Quiet Place* project prepared in the [spotting lesson](/lectures/week-5/reaper-spotting/). Its empty cue items are already arranged on specific Foley pass tracks inside category folders. Add or use a companion `REC` track directly below the selected `CUES` track. Keep both inside the same folder.

## Record into the cues

Work from a cue prepared during the spotting session. Assign roles for operating REAPER, performing, preparing props, and listening for timing or unwanted noise.

1. Choose an empty cue item on its Foley pass track. Move the count-in until the beep item's right edge snaps to the cue item's left edge. Rehearse with picture.
2. Keep speakers off and listen on headphones. Route CUE BEEPS to a separate headphone output when available; otherwise use the master for headphone playback. Check for beep spill and avoid loopback inputs. Select the microphone's **mono hardware input** and arm only the companion `REC` track. Use direct monitoring or REAPER input monitoring as appropriate; avoid hearing both with a delay. Keep the `CUES` and CUE BEEPS tracks unarmed.
3. Perform the loudest part while setting the interface gain. Aim around -18 to -12 dBFS for typical levels, with peaks below -6 dBFS. Record a test and check it for clipping, room noise, and beep spill.
4. Turn off Repeat and the musical metronome. Right-click the transport Record button and choose **Record mode: normal**. Start recording before the count-in, slate the object, surface, action, and take number, then perform on the silent fourth beat. Leave a tail after the action before stopping. Start earlier if you need more time for the slate.
5. Record another take and compare. Leave the empty cue items intact above the recorded takes. Keep alternate recordings until you have made your choices.

Normal recording keeps the lead-in and tail in the recorded item. Once you understand this workflow, try time-selection auto-punch with boundaries that include those handles. The recording boundary, the cue's sync point, and the playback start are separate decisions. Do not punch exactly at an impact and lose its approach.

Save the project with alternate takes for the [editing and layering lesson](/lectures/week-5/editing-foley/).

## Class recording session

Continue recording the prepared *A Quiet Place* cues in the same studio project. Rotate through operating REAPER, performing, preparing props, and listening. Use the recording procedure above, compare takes, and adjust the prop, performance, or microphone placement before another pass. Mute the beeps when listening to the assembled scene.

This is an ungraded class exercise with no separate submission. Complete the robot spotting, recording, and editing with your team **outside class** for [Assignment 2](/assignments/assignment-2-foley-recording/).

---

Source: Vanessa Theme Ament, *The Foley Grail*, 3rd ed., chapters 6, 7, and 8.
