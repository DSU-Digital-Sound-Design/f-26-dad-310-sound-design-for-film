---
title: "Spotting Foley in REAPER"
summary: "Spot A Quiet Place, organize Foley passes, place cue items, and rehearse three-beep entrances."
---

We will spot *A Quiet Place* together in one shared REAPER project. Your job is to identify the actions that need Foley, organize them into recording passes, place clear cue items, and rehearse an entrance with three beeps.

## Class files

- [Download *A Quiet Place*: first 10 minutes]({{< rel "downloads/a-quiet-place-first-10-minutes.mkv" >}}) · MKV, 26 MB
- [Download the Foley project template]({{< rel "downloads/foley-spotting-template.zip" >}})

<iframe width="560" height="315" src="https://www.youtube.com/embed/f6MwssY8_oE" title="A Quiet Place class clip" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The shared project uses 48 kHz / 24-bit WAV, the Time timebase, and a timecode ruler. The video starts at 10 seconds, stays locked, and does not send its original audio to the mix.

## 1. Watch and decide

Watch the scene several times before adding cues. Describe each character's weight, pace, and movement. Decide which actions need performed Foley and which sounds a production might obtain from a library.

For every performed sound, name a likely prop or material. Keep continuous movement together across picture cuts.

## 2. Build folders and pass tracks

Use folders for broad Foley categories. Put specifically named cue and recording tracks inside them.

| Folder | Name the tracks inside it like this |
| --- | --- |
| FOOTSTEPS | `CHARACTER - FOOTWEAR - SURFACE - CUES` |
| BACKGROUND FOOTSTEPS | `DESCRIPTION - DIRECTION - FOOTWEAR - SURFACE - CUES` |
| PROPS | `MATERIAL - OBJECT OR ACTION - CUES` |
| CLOTH | `CHARACTER - GARMENT - CUES` |

The folder track organizes and controls the group. Do not place cue items or recordings on the folder itself. Put them on the named tracks inside it.

Examples:

- `EVELYN - BARE FEET - CONCRETE - CUES`
- `BLUE SHIRT - RIGHT TO LEFT - BOOTS - TILE - CUES`
- `PAPER - MAP HANDLING - CUES`
- `REGAN - JACKET - CUES`

Create another track when the character, footwear, surface, material, or performer changes. Grouping similar sounds lets the Foley artist complete a pass without changing props or microphone placement after every cue.

## 3. Put each cue on its pass track

The session pictured in *The Foley Grail* assigns cue regions to specific tracks before the Foley session. We will use the same layout in REAPER.

1. Select the specific cue track for the sound.
2. Find the exact frame where the action begins.
3. Drag a time selection from that frame through the movement or sound decay.
4. Choose **Insert > Empty item**. Its left edge should remain on the action's first frame.
5. If the action is not obvious, double-click the item and add a short note. Include only what the track name does not already provide. Example: `sets bag down, heavy and careful`.

The item's left edge is the sync point. Its length shows how long the action or sound continues. Begin playback and recording earlier to give the performer enough preparation time. Reserve project markers for global references such as picture start, picture end, and playback start.

When cues overlap, put them on their respective pass tracks. Add a track when two performers or materials need separate passes.

Someone who did not write the cue should be able to understand the action and performance direction without guessing.

## 4. Rehearse with three beeps

The Foley artist hears three equally spaced beeps and performs on the **silent fourth beat**. We use one-second spacing for this exercise.

| Project time | What happens in the template |
| --- | --- |
| `00:00:06:00` | Start playback |
| `00:00:07:00` | Beep 1 |
| `00:00:08:00` | Beep 2 |
| `00:00:09:00` | Beep 3 |
| `00:00:10:00` | Silent fourth beat and picture start |

The three beeps are one three-second audio item. The silent fourth beat occurs at its right edge. For each pass, move the beep item until its right edge meets the active cue item's left edge. Keep the item's length and playback rate unchanged.

Use one count-in at a time. Start playback at least one second before the first beep. The count-in prepares the entrance; it does not set the rhythm of every action that follows. Follow the picture after entering.

Listen on headphones. Mute CUE BEEPS before mixing or rendering. A three-beep count-in is different from a **2-pop**, which is a single synchronization reference.

## Ready to record

Before recording, duplicate each cue track directly below itself. Change the duplicate's suffix from `CUES` to `REC`.

For example:

- `EVELYN - BARE FEET - CONCRETE - CUES`
- `EVELYN - BARE FEET - CONCRETE - REC`

Leave the empty items on the CUES track. Record audio on the REC track. Keep both tracks inside the same folder so the cue sheet remains visible above its takes.

Save and reopen the project to check that the video and beeps load. Then continue with [Recording Foley](/lectures/week-4/recording-foley/).

## Apply this to Project 2

Use the same folder and track structure for the robot animation. Download the [robot starter project]({{< rel "downloads/dad310-foley-starter.zip" >}}) and follow [Assignment 2's project settings and requirements](/assignments/assignment-2-foley-recording/#spotting-and-project-setup). Complete the robot spotting, recording, and editing with your team outside class.

## References

- [REAPER User Guide](https://www.reaper.fm/userguide.php)
- Vanessa Theme Ament, *The Foley Grail*, 3rd ed., chapters 4 and 5
- [Solange Schwalbe on Foley cueing](https://www.production-expert.com/production-expert-1/mastering-foley-insights-from-solange-schwalbe)
- [One-second ADR beep spacing](https://www.crashsymphony.com.au/adr-studio-sydney/)
