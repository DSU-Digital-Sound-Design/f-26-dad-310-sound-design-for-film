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

Working in your teams from Assignment 1, use REAPER to **record** and **layer** Foley sound effects for the robot animation outside class. Arrange studio time with your team. Our in-class A Quiet Place spotting and recording sessions demonstrate the workflow you will use for this project.

## Spotting and project setup

Follow the [REAPER spotting lab](/lectures/week-5/reaper-spotting/#prepare-the-cues). Save a working copy in your team's own folder, copying all media into it. Use these project settings:

- **48 kHz / 24-bit WAV**, with new recordings saved in the relative `Media` folder.
- **Time** timebase and **30 fps**, matching the supplied video. Display the ruler in Hours:Minutes:Seconds:Frames.
- Picture starts at **00:00:10:00** and ends at **00:00:21:06**. Keep the video item's position locked and its track's master send off.
- Keep cue notes on **CUE MAP**, separate from the recording tracks. Each cue needs an ID, object/action, material, destination track, exact sync time, and performance direction.
- Keep one count-in on **CUE BEEPS**. The starter beeps at 7, 8, and 9 seconds for a practice entrance at 10. Move the three-second item to start three seconds before the actual cue you are recording; enter on the silent fourth beat.

After the in-class A Quiet Place demonstration, prepare your team's robot cue map outside class. Choose props, plan recording passes, and check that a teammate can follow your cues. Replace the starter's practice cue with your team's spotting plan before recording.

## Recording Setup

- Record in the studio at 48 kHz / 24-bit. Select the microphone's mono hardware input and arm only the recording track you need.
- Use one of the small-diaphragm cardioids from the [recording lesson](/lectures/week-4/recording-foley/), with the AT 4041 as the first choice. Place it about 6 inches above the surface, 1 to 2 feet from the performer, angled at the contact point. This is Ament's close-mic geometry from *The Foley Grail*.
- Lay out the session the way the [spotting lesson](/lectures/week-5/spotting/) teaches: one track per layer, with the robot's servo movements, the impacts and props, and the surface contact each on their own track, and any continuous movement on a separate pass.
- Slate each take with the object, the surface, and the action, for example "metal grabber arm, rubber duck squeeze, take 3."
- Keep peaks below -6 dBFS, and re-record anything that clips.
- Use headphones for the count-in, with speakers off. At a studio with a separate headphone output, send the beeps there and disable their master send. Check for spill into the microphone; keep the cue tracks unarmed.
- Use normal recording with Repeat and the musical metronome off. Start before the beeps, allow time for the slate, and keep a tail after the performance. Follow the lab's distinction between playback start, recording boundaries, and the sync point.

## Performance Notes

- The robot has weight and rhythm. Watch the animation twice and mark the beats before you record anything.
- Ament's cueing rule applies on our stage too: leave a breath before each cue and perform through the movement rather than chasing individual frames.

## Project Requirements
1. Cover all sound-making objects and events in the supplied animation with your own recorded Foley.
2. Demonstrate high-quality recordings, precise synchronization, and a well-balanced final mix.
3. Save a version with alternate takes before cropping or removing them. Remove slates from the edited performance and mute CUE BEEPS before mixing or making a review render. Keep the original video's audio out of the mix.
4. Submit a zipped (compressed) archive of your entire DAW session, including all audio and video files, to D2L by **Monday, October 5**. Reopen the project from its folder first to check for missing media. An optional review render should cover only the picture range, 10.0 to 21.2 seconds, at 48 kHz / 24-bit WAV.


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
