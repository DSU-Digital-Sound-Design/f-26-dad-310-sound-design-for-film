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

## September 25: recording demo

Reopen the shared *A Quiet Place* project spotted on September 23. Choose one prepared cue and demonstrate microphone placement, input gain, headphone routing, and recording with a lead-in and tail. Follow the [REAPER recording procedure](/lectures/week-5/reaper-spotting/#record-into-the-cues), then compare two takes with picture.

Students will use this workflow to spot, record, and edit the robot outside class for [Assignment 2](/assignments/assignment-2-foley-recording/). We'll return to the shared project for class Foley recording on October 2.

## A Quiet Place: in-class spotting

We'll spot and record this scene together in **one REAPER project on the studio computer**. The instructor operates the session while students identify cues, choose and perform props, and compare takes. Students do not need to download a project or set up REAPER on their own computers for this activity.

### Before September 23: instructor setup

[Download A Quiet Place: first 10 minutes]({{< rel "downloads/a-quiet-place-first-10-minutes.mkv" >}}) · MKV, 26 MB. Use this clip in our shared REAPER project.

Use the [Foley starter template]({{< rel "downloads/foley-spotting-template.zip" >}}) to create a single working project. Installing it in REAPER's template menu is optional.

1. Extract the folder and open `Foley-Spotting-Template.RPP` on the studio computer. Save it as `A-Quiet-Place-Spotting` in its own folder, with **Copy all media into project directory** enabled.
2. Import the downloaded movie clip onto VIDEO at **10 seconds**, then lock the video item. Its track's master send is already off.
3. Match **Project settings > Video > Frame rate** to the clip's source properties. The template's 30 fps is a placeholder. Keep 48 kHz / 24-bit WAV and the Time timebase.
4. Add a picture-end marker and set the picture-length render selection. Prepare footstep, prop, and cloth tracks, and check the microphone input, headphone cue routing, and levels. Leave the cue map for the class to build together.

### September 23: spot and rehearse

1. Watch the scene and identify the actions that need sound. Describe the character's weight and movement, then suggest props and materials.
2. Build the cue map on the studio screen as students call out actions. The instructor labels each cue with its material, recording track, performance direction, and exact sync marker. Keep continuous movement together across picture cuts.
3. Choose a cue and move the three-second beep item to start three seconds before its sync point. A student rehearses the entrance on the silent fourth beat while watching picture.
Save the cue map and rehearsed entrance for the September 25 demo and October 2 recording session.

### October 2: perform and record

1. Reopen the saved project and review the spotted cues.
2. Record the lead-in, performance, and tail using the [recording procedure](/lectures/week-5/reaper-spotting/#record-into-the-cues). Rotate students through performing, preparing props, and listening for timing and unwanted noise while the instructor runs REAPER.
3. Compare takes as a class. Decide whether to change the prop, performance, mic placement, or timing, then record another pass. Mute the beeps when listening to the assembled scene.

This is a shared, ungraded studio exercise with no separate student project submission.

<iframe width="560" height="315" src="https://www.youtube.com/embed/f6MwssY8_oE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---

Source: Vanessa Theme Ament, *The Foley Grail*, 3rd ed. (Routledge, 2021), ch. 6 on the stage and miking, ch. 7 on the mixer's perspective, and ch. 8 on footsteps.
