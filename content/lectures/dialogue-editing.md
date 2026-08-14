---
title: "Dialogue Editing"
summary: "Room tone, splits, and repair: the invisible work that makes recorded speech play as if it were never edited."
tags: [dialogue, editing, post-production, room tone]
---

Dialogue editing removes the artifacts of filmmaking and smooths the transitions
between shots. It also gives the mixer organized tracks that are quick to work
with. The audience should hear people talking in a room, not the edits between
their lines.

Everything below follows John Purcell's *Dialogue Editing for Motion Pictures*,
adapted here for REAPER.

## Room tone

Room tone is what remains in a take when no one is speaking or moving. Each
location sounds different, and none is completely silent.

A jarring change between shots often comes from the room tone rather than the
actors' voices. A wide shot might have been recorded with the boom four feet away
and a refrigerator running. During the close-up, the refrigerator may have cycled
off. Cutting those takes together changes the background beneath the dialogue.

Purcell recommends playing only one source of room tone at a time and overlapping
sources only during transitions. If a take's handles do not contain enough clean
tone for a crossfade, copy tone from another part of the same take to bridge the
gap.

### Building fill in REAPER

Do not loop a short snippet. Repeating the same two-second section eight times
makes small sounds within it easy to recognize.

1. Copy a stretch of the take onto a work track below your dialogue.
2. Cut out every word, breath, and click, closing the gaps as you go. `Item >
   Dynamic split items` can make the first pass by splitting on silence. Clean up
   anything it misses.
3. Crossfade every join to prevent clicks.
4. Glue the result into one item, then trim the ends so you keep handles for
   crossfading into the scene.

If the tone rises in pitch or level across the clip, copy it, reverse the copy,
and crossfade the two. The reversed copy meets the original at a similar level,
which helps hide the join.

## Splits: one track per angle

Splitting means assigning each camera angle, microphone, and character to a
separate track. A three-angle scene recorded with a boom and two lavs might need
six tracks before any repair work begins.

Separate tracks give the mixer control over each source. A wide shot may need
different EQ from a close-up, just as a lav under a jacket may need different
processing from a boom. Putting them on the same track prevents the mixer from
treating them independently.

Two practices go along with splitting:

- Sound edits do not need to land on picture cuts. Moving an audio edit a few
  frames away from the visual edit can make the transition less noticeable.
- Remove unnecessary inserts. If the picture cuts to a silent reaction shot, a
  half-second of different room tone adds two transitions without helping the
  scene. Let the speaking character's tone continue underneath instead.

When you move to the next scene, start on different tracks than the scene before
it. Purcell calls this checkerboarding. It keeps the processing for one scene
separate from the next, at the cost of additional tracks.

## Fades at the cut

Do not place a fade in the middle of a spoken line. Find a gap instead.

Choose the crossfade shape based on the sources you are joining.

{{< stats >}}
{{< stat value="Equal power" label="Two different sources" note="Crossfading the boom into the lav, or one take into another. The curve dips about 3 dB at the midpoint so the level stays steady. This is REAPER's default." >}}
{{< stat value="Equal gain" label="One file against itself" note="Splitting a continuous take across two tracks, like a perspective cut or a phone split. The identical audio sums, so you need a deeper 6 dB dip to avoid a bump in level." >}}
{{< /stats >}}

Right-click any crossfade in REAPER to change its shape. `Alt + X` toggles
automatic crossfades, so overlapping two items fades them together for you.

When two actors talk over each other, play both tracks if the microphones are
clean. If the room tones conflict, run the dominant tone, usually the boom,
underneath. Dip it by no more than 3 dB while the other microphone carries the
line.

## Repair

You already know most of this from the [editing lesson](/lectures/week-7/editing/).
Dialogue needs extra care because rerecording a performance is harder than
rerecording a sound effect.

- For clicks, pops, and mouth noise, zoom in and find the transient. Replace it
  with adjacent room tone and add short crossfades on both sides.
- Hum and buzz appear as stacked spikes in a spectrum analyzer because they are
  steady and harmonic. Make narrow, deep cuts at the fundamental and its
  harmonics. Leave broad tonal changes to the mixer and concentrate on the noise.
- For broadband noise, use ReaFIR in subtract mode. Build a noise profile from a
  section that contains only noise, then uncheck the box.
- Make several gentle passes with restoration plugins instead of one aggressive
  pass. Heavy denoising can make dialogue sound metallic or unstable.

These methods cannot repair clothing rustle that is ground into a lavalier or
peaks distorted by over-modulation. Use a different take for those problems.

## When to stop repairing

{{< stats >}}
{{< stat value="Alternate take" label="First choice" note="A clean version of the same line from another take or angle. Cheap, and it preserves the performance from the day." >}}
{{< stat value="ADR" label="Last resort" note="Re-recorded in a studio, when noise is unfixable or the performance is unusable. Expensive, and it never quite matches the room." >}}
{{< /stats >}}

When cutting in an alternate take, work in groups of three or four words instead
of replacing whole sentences. Hard consonants such as P, B, T, and D create clear
waveform landmarks for synchronization. Sibilants such as S and Sh can hide a
splice within their noise.

Keep the original of anything you replace. Edit it, leave it in sync on a labeled
and muted safety track, and make it easy to retrieve if the director changes the
decision during the mix.

{{< drill label="In-class lab: fix a scene" >}}
Work with the dialogue line you recorded on 9/23, the clean take and the one
recorded in a space, plus a room tone file from the [Setting
deck](/lectures/week-6/sdff-chapter-3/).

1. Put the two takes on separate tracks, as if they were two camera angles.
2. Build 30 seconds of continuous room tone fill from the quiet parts of one
   take without looping a short snippet.
3. Cut between the two takes mid-scene. Listen to the bump, then fix it: run the
   fill underneath, crossfade at the transition, and move your edit off the
   picture cut.
4. Find a click or a mouth noise in one take and patch it with adjacent tone.
5. Play the result for someone who wasn't watching you work. If they can hear
   where the edit is, keep going.
{{< /drill >}}

## Reference

- John Purcell, *Dialogue Editing for Motion Pictures: A Guide to the Invisible
  Art*
- [Dialog editing with room
  tone](https://reaper.blog/2015/03/video-dialog-editing-with-room-tone/), a
  REAPER-specific walkthrough
