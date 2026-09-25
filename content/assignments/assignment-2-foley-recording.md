---
title: "Foley Recording"
number: "02"
weight: 2
week: 5
assigned: "2026-09-25"
due: "2026-10-05"
summary: "Record and layer the same animation's Foley in the studio."
rubric: false   # the brief carries its own rubric table
---

## Overview
Download the [REAPER starter project]({{< rel "downloads/dad310-foley-starter.zip" >}}), including the video, named tracks, and three cue beeps. Extract the whole folder before opening the project. The [video is also available separately](../HardSurface_robot_animation-346689615.mp4).

This 11.2-second animation features a robot playing with a rubber duck. Your challenge is to create believable mechanical sounds that match the robot's movements while conveying personality and rhythm.

Working in your teams from Assignment 1, use REAPER to **record** Foley sound effects for the robot animation outside class. Arrange studio time with your team. After recording, each student will **edit, layer, and mix their own complete session** using the shared recordings. Our in-class A Quiet Place spotting and recording sessions demonstrate the workflow you will use for this project.

## Group recording and individual editing

Rotate performer and recording engineer roles so everyone gains experience with both. Each student must perform several cues and engineer several cues for another teammate, handling microphone placement, input selection, recording levels, and take capture.

Keep a brief recording log identifying the performer and recording engineer for each pass. Before leaving the studio, make sure every team member has a copy of the recording session and all recordings.

After recording, each student must save their own copy of the complete REAPER session with all media and edit it to cover the entire animation. Use the shared recordings, but make your own decisions about take selection, synchronization, trimming, fades, layering, and mix balance. You may discuss approaches and offer feedback, but each student must do their own editing.

Submit your own zipped REAPER project with all required media and the group's recording log. Your individual session will be graded using the assignment rubric.

## Spotting and project setup

Follow the [REAPER spotting lab](/lectures/week-5/reaper-spotting/). Save a working copy in your team's own folder, copying all media into it. Use these project settings:

- **48 kHz / 24-bit WAV**, with new recordings saved in the relative `Media` folder.
- **Time** timebase and **30 fps**, matching the supplied video. Display the ruler in Hours:Minutes:Seconds:Frames.
- Picture starts at **00:00:10:00** and ends at **00:00:21:06**. Keep the video item's position locked and its track's master send off.
- Organize the session with category folders such as **ROBOT MOVEMENT**, **SURFACE CONTACT**, and **PROPS**. Inside each folder, create a specifically named `CUES` track for each pass.
- Put each empty cue item on its pass track. Its left edge marks the exact sync frame, and its right edge extends through the action or sound decay. Add a short item note only when the action or performance is not clear from the track name and picture. Do not add a project marker for every cue.
- Keep one count-in on **CUE BEEPS**. The starter beeps at 7, 8, and 9 seconds for a practice entrance at 10. For each recording pass, snap the beep item's right edge to the active cue item's left edge; enter on the silent fourth beat.

After the in-class A Quiet Place demonstration, prepare your team's robot cues outside class. Choose props, plan recording passes, and check that a teammate can follow the cues from the track layout. Before recording, duplicate each `CUES` track directly below it, change the duplicate's suffix to `REC`, and keep both inside the same folder.

## Recording Setup

- Record in the studio at 48 kHz / 24-bit. Select the microphone's mono hardware input and arm only the recording track you need.
- Use one of the small-diaphragm cardioids from the [recording lesson](/lectures/week-4/recording-foley/), with the AT 4041 as the first choice. Place it about 6 inches above the surface, 1 to 2 feet from the performer, angled at the contact point. This is Ament's close-mic geometry from *The Foley Grail*.
- Lay out the session the way the [spotting lesson](/lectures/week-5/spotting/) teaches. Use general category folders and specifically named tracks for each recording pass. Keep servo movements, impacts and props, surface contact, and continuous movement separate.
- Slate each take with the object, the surface, and the action, for example "metal grabber arm, rubber duck squeeze, take 3."
- Keep peaks below -6 dBFS, and re-record anything that clips.
- Use headphones for the count-in, with speakers off. At a studio with a separate headphone output, send the beeps there and disable their master send. Check for spill into the microphone. Keep the cue tracks unarmed and arm only the companion recording track.
- Use normal recording with Repeat and the musical metronome off. Start before the beeps, allow time for the slate, and keep a tail after the performance. Follow the [recording procedure](/lectures/week-4/recording-foley/#record-into-the-cues).

## Performance Notes

- The robot has weight and rhythm. Watch the animation twice and mark the beats before you record anything.
- Ament's cueing rule applies on our stage too: leave a breath before each cue and perform through the movement rather than chasing individual frames.

Use the [editing and layering guide](/lectures/week-5/editing-foley/) when assembling your takes.

## Project Requirements
1. Cover all sound-making objects and events in the supplied animation with your own recorded Foley.
2. Demonstrate high-quality recordings, precise synchronization, and a well-balanced final mix.
3. Save a version with alternate takes before cropping or removing them. Remove slates from the edited performance and mute CUE BEEPS before mixing or making a review render. Keep the original video's audio out of the mix.
4. Each student must submit a zipped (compressed) archive of their own complete, individually edited DAW session, including all audio and video files and the group's recording log, to D2L by **Monday, October 5**. Reopen your project from its folder first to check for missing media. An optional review render should cover only the picture range, 10.0 to 21.2 seconds, at 48 kHz / 24-bit WAV.


---

## Grading Rubric (45 points total)

| Criterion | Exemplary | Proficient | Developing | Emerging | Points |
| --- | --- | --- | --- | --- | --- |
| **Recording Quality (12 pts)** | Clean takes with no clipping, handling noise, or room tone intruding; levels consistent across the session | Generally clean; one or two takes with minor noise or level drift | Noticeable noise, clipping, or inconsistent levels | Recordings unusable without repair | /12 |
| **Event Coverage (10 pts)** | Every sound-making object and event in the animation is recorded and placed | All major events covered; one or two small ones missing | Several events without sound | Only the most obvious events covered | /10 |
| **Synchronization (10 pts)** | Every hit lands on frame; the track reads as production sound | Mostly on frame, drifting on one or two fast events | Noticeably early or late through much of the piece | Timing unrelated to the picture | /10 |
| **Mix Balance (8 pts)** | Elements sit in a believable relationship; nothing masks anything else, nothing jumps out | Mostly balanced, with one or two elements competing | Some elements buried or overpowering | No balancing attempted | /8 |
| **Session Delivery (5 pts)** | Zipped session with all audio and video consolidated, tracks named | Complete session with minor naming or packaging issues | Media not consolidated, or tracks unnamed | Session incomplete or will not open | /5 |

**Total: \_\_\_ / 45**
