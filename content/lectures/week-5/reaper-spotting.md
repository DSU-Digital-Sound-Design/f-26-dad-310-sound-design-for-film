---
title: "Spotting Foley in REAPER"
---

Prepare a session that another person can record from. On September 23, finish the cue map and rehearse one entrance. On September 25, record into the prepared session. On September 30, edit and layer the recordings for [Assignment 2](/assignments/assignment-2-foley-recording/).

[Download the REAPER starter project]({{< rel "downloads/dad310-foley-starter.zip" >}}). Extract the whole folder before opening `DAD310-Foley-Starter.RPP`. Keep its `Media` folder beside the project. The download includes the robot video, a three-beep audio file, named tracks, and a practice cue. No extensions or third-party plug-ins are required.

The *A Quiet Place* activity is a [shared session on the studio computer](/lectures/week-4/recording-foley/#a-quiet-place-in-class-spotting). The instructor prepares one project; students help spot cues, perform sounds, and evaluate takes. No individual computer setup is needed for that activity.

## Prepare the cues

### 1. Watch and decide

Watch the robot animation several times before adding cues. Describe its weight, speed, and personality. Choose two contrasting directions, such as delicate and heavy, then decide which one your team will pursue.

Identify each sound-making action. For each one, name a prop or material you could perform. Discuss which sounds a professional production might obtain from a library, but record your own Foley for this assignment. The starter's cue is an entrance exercise, not a completed spotting plan.

### 2. Check the project setup

Use **File > Save project as** to make your team's working copy in its own folder. Enable **Create subdirectory for project** and **Copy all media into project directory** when saving to a new location. Do not move the source media out of the starter.

| Setting | Use for this project |
| --- | --- |
| Project sample rate | 48000 Hz, enabled in File > Project settings |
| New recordings | WAV, 24-bit PCM, in the Media tab |
| Recording path | `Media`, relative to the project folder |
| Project timebase for items/envelopes/markers | Time |
| Video frame rate | 30 fps, matching the supplied file |
| Timeline ruler | Hours:Minutes:Seconds:Frames, available by right-clicking the ruler |
| Picture position | `00:00:10:00`; the supplied video lasts 11.2 seconds and ends at `00:00:21:06` |
| Video item | Position locked; VIDEO track's master send disabled so original audio is not heard |
| Record input | Mono input for the connected microphone; verify it on each recording track |

Open the video window from the View menu. Scrub or play the video to check it displays correctly. If REAPER reports missing media, check that you extracted the entire folder. If the video does not decode, ask for help before you begin spotting.

The starter leaves every track unarmed. Audio devices and physical inputs differ between computers, so verify yours at the recording station. Turn off the musical metronome and Repeat for this exercise.

### 3. Organize the passes

The starter contains these tracks:

| Track | Purpose |
| --- | --- |
| VIDEO | Locked picture reference, with its audio excluded from the master |
| CUE BEEPS | Count-in for the performer; mute before mixing or rendering |
| CUE MAP | Empty items with instructions; never record on this track |
| SERVO MOVEMENT | Performed mechanical movement |
| SURFACE CONTACT | Contact with the supporting surface |
| IMPACTS AND PROPS | Grabs, hits, squeezes, and other prop actions |
| CONTINUOUS MOVEMENT | A separate sustained movement pass, if the scene needs one |

Keep similar materials together. Add or rename recording tracks when different textures need separate passes. For a human scene, cue principal footsteps first, background footsteps next, and props after that; put cloth movement on its own pass. The robot does not require background characters or human clothing sounds. Apply the footstep layout in the September 28 lab.

### 4. Build the cue map

1. On CUE MAP, make a time selection around a complete action, with a short lead-in and enough tail for the sound to decay. Choose **Insert > Empty item**.
2. Open the empty item's notes by double-clicking it. Give it a cue ID and an instruction with the **object, action, material, destination track, exact sync time, and performance direction**. For example: `C03 | ROBOT squeezes duck | rubber | IMPACTS AND PROPS | sync [your timecode] | hesitant, then firm`.
3. Put a named marker at the exact sync point. The empty item's left edge is preparation time; the marker is where the action must land. They are different positions.
4. Keep a continuous movement in one cue, even if the picture cuts during it. Split when the action, material, or recording pass changes, rather than at every frame or camera cut.
5. Group cues by material when planning the recording order. For overlapping cues, use additional CUE MAP tracks and identify the destination recording track in each note.

Read your cues to a partner. They should be able to identify the action, choose a prop, and locate the sync point without asking you what the label means. For background characters, use a visible description and direction, such as "blue shirt, right to left."

### 5. Rehearse with three beeps

The artist hears three equally spaced beeps and performs on the **silent fourth beat**. For this class, use one-second spacing. This is our classroom convention; stage workflows can use different intervals or visual streamers.

| Project time | What happens in the starter |
| --- | --- |
| `00:00:06:00` | Start playback here |
| `00:00:07:00` | Beep 1 |
| `00:00:08:00` | Beep 2 |
| `00:00:09:00` | Beep 3 |
| `00:00:10:00` | Silent fourth beat: practice entrance and picture start |

The three beeps are inside **one three-second audio item**. Its right edge marks the silent fourth beat. Keep its length and playback rate unchanged. For a new cue at time **T**, set the beep item's position to **T minus 3 seconds** in Item properties. For example, a cue at `00:00:14:00` needs the item at `00:00:11:00`. Its snap offset is also at the right edge, so you can align that edge to a cue marker when snapping is enabled.

Use one active count-in at a time. Move this item for the cue you are recording instead of filling a short scene with overlapping count-ins. Start playback at least one second before its first beep. For the first rehearsal, tap a prop on the silent fourth beat, then rehearse an actual spotted action against picture.

Listen on headphones. The starter sends CUE BEEPS through the master for simple headphone practice. At a studio with a separate headphone output, route the beeps to that output and disable their master send. Keep speakers off during microphone recording and check for headphone spill. Do not record the computer's output or loopback input.

A count-in prepares the entrance; it does not set the rhythm of every subsequent step. Follow the picture after the entrance. These three beeps are also different from a **2-pop**, which is a single synchronization reference.

### Before you leave on September 23

Save your team's project with named recording tracks, labeled cues covering the animation, and exact sync markers. Have a partner perform one entrance using your count-in. Check that the video and beeps still load after reopening the project. This preparation is ungraded and will be used in Friday's recording session.

## Record into the cues

Use the [recording lesson](/lectures/week-4/recording-foley/) for mic choice and placement. Rotate performer, mixer, and editor roles.

1. Choose the cue and destination track. Move the count-in so its silent fourth beat lands at the sync marker. Rehearse with picture.
2. Select the microphone's **mono hardware input** and arm only the destination recording track. Use direct monitoring or REAPER input monitoring as appropriate; avoid hearing both with a delay. Keep CUE MAP and CUE BEEPS unarmed.
3. Perform the loudest part while setting the interface gain. Aim around -18 to -12 dBFS for typical levels, with peaks below -6 dBFS. Record a test and check it for clipping, room noise, and beep spill.
4. Right-click the transport Record button and choose **Record mode: normal**. Start recording before the count-in, slate the object, surface, action, and take number, then perform on the silent fourth beat. Leave a tail after the action before stopping. Start earlier if you need more time for the slate.
5. Record another take and compare. Use the cue map as a reference; record the sound on its named layer track, leaving the cue notes intact. Keep alternate recordings until you have made your choices.

Normal recording keeps the lead-in and tail in the recorded item. Once you understand this workflow, try time-selection auto-punch with boundaries that include those handles. The recording boundary, the cue's sync point, and the playback start are separate decisions. Do not punch exactly at an impact and lose its approach.

## Edit and layer the recordings

1. Save a new project version before choosing or removing takes.
2. Mute CUE BEEPS. Keep the VIDEO track's master send off. Compare your takes with picture and choose the strongest performances.
3. Align the audible contact or impact with its sync marker. Adjust timing by listening and watching, not just by matching the item's left edge. Preserve the rhythm of continuous movement.
4. Trim slates and unwanted noise while leaving natural attacks and decays. Add short fades or crossfades where edits click. If using REAPER takes, crop to the active take only after comparing them and saving a version with the alternatives.
5. Balance the separate layers so actions remain clear and the robot has a consistent weight and personality. Check for missing actions and accidental double hits.
6. Listen through the full picture range, `00:00:10:00` to `00:00:21:06`. Exclude beeps, slates, and guide audio from the mix. If you make a review render, use this range and 48 kHz / 24-bit WAV.
7. Save and reopen the project from its own folder to confirm all media are present. Submit the complete zipped project folder, including audio and video, as required by Assignment 2.

## Optional shortcuts and extensions

The core exercise uses REAPER's built-in tools. Learn the menu actions first, then assign shortcuts in the Actions list if useful. Existing shortcuts can differ between machines.

[ReaPack](https://reapack.com/) and [SWS](https://www.sws-extension.org/) are optional workflow tools. Install them before class if you want to explore scripts; they are not part of the lab's setup time. The X-Raym script for converting selected item notes to take names is an optional later exercise for notes attached to recorded items. It is not needed for our separate cue-map workflow.

## References

- [REAPER User Guide](https://www.reaper.fm/userguide.php), project settings, recording modes, media items, and video.
- Vanessa Theme Ament, *The Foley Grail*, 3rd ed., chapters 4 and 5.
- [Solange Schwalbe on Foley cueing](https://www.production-expert.com/production-expert-1/mastering-foley-insights-from-solange-schwalbe), including three-beep entrances.
- [A studio example of one-second ADR beep spacing](https://www.crashsymphony.com.au/adr-studio-sydney/).
