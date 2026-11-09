---
title: "Ambience Demo: Build a Place"
summary: "Build a background in REAPER, place an offscreen detail, and hear how one change affects the scene."
---

## What to listen for

Watch as I build a short environment in REAPER. Listen for how the bed,
offscreen details, and perspective establish the place and change its mood.
You will discuss the choices; you do not need to open REAPER or build along.
Use the demonstration as a starting point for
[Assignment 6: Ambiences](/assignments/assignment-6-ambiences/).

## Find the sounds together

I'll search Freesound through SoundQ and audition a few candidates before
bringing them into REAPER. Try searches such as `wind trees`, `distant traffic`,
and `single crow`. Listen for the source's distance, background noise, and mood,
not just whether its name matches the scene.

For each candidate, decide: **keep, reject, or try in context?** What makes it
fit? Is it too close, busy, or distinctive? Could editing or a level change help?
A useful recording may need only a short passage. Note its creator, source link,
and license when we choose it. I'll keep a few backup sounds ready so searching
doesn't take over the demo.

## Instructor demonstration

Our starting intention: **A quiet cemetery in daylight, heard from beside the
characters, with wind in the trees and a road somewhere beyond the grounds.**

<video controls muted playsinline preload="metadata" width="640" height="480" style="width:100%;max-width:640px;height:auto" aria-label="Silent 30-second cemetery excerpt from Night of the Living Dead">
  <source src='{{< rel "downloads/cemetery-ambience-30s.mp4" >}}' type="video/mp4">
  <p><a href='{{< rel "downloads/cemetery-ambience-30s.mp4" >}}'>Download the silent cemetery clip</a></p>
</video>

[Download the silent clip (MP4)]({{< rel "downloads/cemetery-ambience-30s.mp4" >}})

This is a 30-second excerpt from *Night of the Living Dead* (1968), drawn from
our ADR class clip with its audio removed. Watch once before choosing sounds.
Which environmental cues are visible? What could we hear beyond the frame?

Import the MP4 into REAPER on a track named `VIDEO`, open the video window,
and align its start with the beginning of your 30-second work area. This file
has no audio track. Leave the characters' speech and movements silent today;
we are designing the environment around them.

### Layered ambience layout

| Track | Contents |
| --- | --- |
| `VIDEO` | Silent cemetery clip |
| `WIND BED` | Steady, low-level wind that holds the space together |
| `LEAVES` | A separate foliage layer that adds texture and gentle variation |
| `DISTANT ROAD` | Traffic beyond the cemetery |
| `BG SPECIFICS` | Occasional bird calls or rustles |

This gives us five tracks including video. Wind and leaves form the layered
bed, traffic establishes the wider location, and specifics add occasional
events. Choose recordings with different roles rather than stacking similar
full ambiences.

### 1. Establish the bed

In REAPER, mark a 30-second time selection. Start with a stable wind recording
on `WIND BED`, then add a separate foliage recording on `LEAVES`. Choose a
foliage layer that contributes texture without duplicating strong leaf sounds
already in the wind recording. Trim unwanted events and add short boundary
fades. If joining sections, overlap and crossfade them; listen for a dip, bump,
or conspicuous repeated sound.

Audition each layer alone, then together. Ask what the leaves add. Mute them
and bring them back at a lower level. Keep the combination only if it sounds
like one environment; remove a layer if it merely makes the bed louder or busier.

Room tone is the location's quiet background, often used to fill gaps in
production dialogue. Designed ambience establishes the broader environment.
They can share material, but adding an ambience does not automatically repair
an abrupt change in a dialogue recording.

Mute both bed layers briefly, then restore them. What disappears when they stop?

### 2. Extend the world outside the frame

Add traffic on a separate track named `DISTANT ROAD`. Lower it until it feels
beyond the cemetery. Compare the untreated recording with a modest reduction of high
frequencies using ReaEQ. Keep the treatment only if it supports that perspective.

Add a short bird call or isolated leaf rustle on its own track named
`BG SPECIFICS`. These intermittent details are **background specifics**. The
bed sustains the environment; specifics enter and leave, suggesting activity
within or beyond the frame.

Ask where one call would help the scene, then try it there. Leave space before
another event. Compare it too loud, quieter, and muted: when does it enrich the
setting, and when does it steal attention? Avoid an obvious repeating pattern
or doubling a detail already present in the bed. Keep sources separate so each
can be adjusted later.

Ask: **Are we hearing one place, or several unrelated recordings?** Adjust or
remove a layer that does not belong. Offscreen sounds establish the surrounding
world; they need not become foreground events.

### 3. Change the mood

Save the first version. Keep the setting and listening position, but change
one choice: remove the traffic, introduce a distant crow, or
alter the wind's level. Compare both versions at comfortable, similar loudness.

Play both versions against the same picture. What changed in the scene's mood? Which version serves the
intention? Keep a choice because of what it does for the scene.

## Discuss and apply later

Before I change a layer, predict what it will do. After the comparison, explain
what you heard: which sound placed us outside, what felt near or far, and what
made the same picture feel different?

Name one choice you could use for your own setting. Begin your Assignment 6
session outside class, using your existing recordings or credited library
material. There is no separate demo submission.

## Reading connections

This exercise draws on the distinction between room tone and backgrounds in
John Purcell's *Dialogue Editing for Motion Pictures*, alongside the notebook's
ambience material from Ric Viers' *The Sound Effects Bible*, David Lewis
Yewdall's *Practical Art of Motion Picture Sound*, and Tomlinson Holman's
*Sound for Film and Television*. The cemetery exercise is a class demonstration,
not an exercise reproduced from those books.

For a practical description of beds and background specifics, see
[Matt Yocum's background-design demonstration](https://blog.prosoundeffects.com/how-to-sound-design-immersive-backgrounds-video).

For the earlier examples, revisit [Setting: ambience, immersion and sense of
place](/lectures/week-6/sdff-chapter-3/).
