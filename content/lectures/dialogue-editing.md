---
title: "Dialogue Editing"
summary: "Room tone, splits, and repair: the invisible work that makes recorded speech play as if it were never edited."
tags: [dialogue, editing, post-production, room tone]
---

Foley and effects are the sounds you notice. Dialogue editing is the work you're
meant to miss entirely. The job is to strip out the artifacts of filmmaking,
smooth the seams between shots, and hand the mixer tracks that are organized
enough to mix quickly. When it's done well, an audience hears people talking in
a room. When it's done badly, they hear editing.

Everything below follows John Purcell's *Dialogue Editing for Motion Pictures*,
translated into REAPER.

## Room tone is the air the scene breathes

Room tone is what's left of a take once you remove the words, the footsteps, and
the clothing rustle. Every location has its own, and it is never silence.

Here's the part that surprises people: the jarring bump you hear at a shot change
usually isn't the actors' voices. It's the room tone changing underneath them.
The wide shot was recorded with the boom four feet away and a refrigerator
running; the close-up was recorded after the fridge cycled off. Cut them together
and the floor of the sound drops out from under the scene.

Purcell's first rule follows from that: **play only one source of room tone at a
time**, and overlap sources only at transitions. When a take's handles don't
contain enough clean tone to crossfade with, you build a bridge out of tone
copied from elsewhere in the same take.

### Building fill in REAPER

Never loop a short snippet. A two second scrap repeated eight times reads as a
machine, because the ear locks onto whatever tiny event sits inside it.

1. Copy a stretch of the take onto a work track below your dialogue.
2. Cut out every word, breath, and click, closing the gaps as you go. `Item >
   Dynamic split items` automates the first pass by splitting on silence, and
   then you clean up what it missed.
3. Crossfade each join. Butt-joined tone clicks.
4. Glue the result into one item, then trim the ends so you keep handles for
   crossfading into the scene.

If the tone rises in pitch or level across the clip, copy it, reverse the copy,
and crossfade the two. The seam disappears because the reversed copy meets the
original at a matched level.

## Splits: one track per angle

Splitting means giving every camera angle, microphone, and character its own
track. A three-angle scene with a boom and two lavs might occupy six tracks
before you've fixed anything.

The reason is control. Each angle is its own instrument: the wide shot needs
different EQ from the close-up, and the lav under a jacket needs different
treatment from the boom. If they share a track, the mixer can't treat them
separately, and every fix you apply to one damages the other.

Two habits that come with splitting:

- **Your edits don't have to land on the picture cuts.** Sound edits are usually
  staggered a few frames off the visual edit, which is part of why the seam
  disappears.
- **Kill unnecessary inserts.** When the picture cuts to a silent reaction shot,
  that half second of a different room tone buys you nothing and costs you two
  transitions. Delete it and let the speaking character's tone run underneath.

When you move to the next scene, start on different tracks than the scene before
it. Purcell calls this checkerboarding. It keeps one scene's processing from
colliding with the next scene's, and it costs nothing but track count.

## Fades at the cut

One rule outranks the rest: **never place a fade in the middle of a spoken
line.** Find the gap.

The shape of the crossfade matters more than it looks, because two different
situations need two different curves.

{{< stats >}}
{{< stat value="Equal power" label="Two different sources" note="Crossfading the boom into the lav, or one take into another. The curve dips about 3 dB at the midpoint so the level stays steady. This is REAPER's default." >}}
{{< stat value="Equal gain" label="One file against itself" note="Splitting a continuous take across two tracks, like a perspective cut or a phone split. The identical audio sums, so you need a deeper 6 dB dip to avoid a bump in level." >}}
{{< /stats >}}

Right-click any crossfade in REAPER to change its shape. `Alt + X` toggles
automatic crossfades, so overlapping two items fades them together for you.

When two actors talk over each other, play both tracks if the microphones are
clean. If the room tones fight, run the dominant tone (usually the boom)
underneath and dip it slightly, no more than 3 dB, while the other microphone
carries the line.

## Repair

You already know most of this from the [editing lesson](/lectures/week-7/editing/).
Dialogue just raises the stakes, because you can't re-record a performance the
way you can re-record a door slam.

- **Clicks, pops, mouth noise.** Zoom in, find the transient, and patch it with a
  slice of adjacent room tone. Short crossfades on both sides. This works because
  the patch is the same air as the material around it.
- **Hum and buzz.** These are steady and harmonic, so look at a spectrum
  analyzer and you'll see them as stacked spikes. Cut narrowly and deeply at the
  fundamental and again at its harmonics. Leave broad tone shaping to the mixer;
  your job is the exceptional noise, not the overall sound.
- **Broadband noise.** ReaFIR in subtract mode, the same workflow as before:
  build a noise profile from a section that's only noise, then uncheck the box.
- **Restoration plugins.** Several gentle passes beat one aggressive pass. Push a
  denoiser hard and the dialogue starts to swim and sound metallic, which is more
  distracting than the noise you removed.

Clothing rustle ground into a lavalier and clipped, over-modulated peaks are the
two problems that don't respond to any of this. Those need a different take.

## When to stop repairing

{{< stats >}}
{{< stat value="Alternate take" label="First choice" note="A clean version of the same line from another take or angle. Cheap, and it preserves the performance from the day." >}}
{{< stat value="ADR" label="Last resort" note="Re-recorded in a studio, when noise is unfixable or the performance is unusable. Expensive, and it never quite matches the room." >}}
{{< /stats >}}

Cutting in an alternate take is a sync problem. Work in blocks of three or four
words rather than whole sentences. Hard consonants like P, B, T, and D give you
sharp visual landmarks in the waveform to line up against, and sibilants like S
and Sh make clean edit points because a splice hides inside the noise.

Whatever you replace, **keep the original**. Edit it properly, leave it in sync
on a muted safety track, and label it. Directors change their minds in the mix,
and the person who can produce the original in five seconds is the person who
gets hired again.

{{< drill label="In-class lab: fix a scene" >}}
Work with the dialogue line you recorded on 9/23, the clean take and the one
recorded in a space, plus a room tone file from the [Setting
deck](/lectures/week-6/sdff-chapter-3/).

1. Put the two takes on separate tracks, as if they were two camera angles.
2. Build 30 seconds of continuous room tone fill from the quiet parts of one
   take. No looping a short snippet.
3. Cut between the two takes mid-scene. Listen to the bump, then fix it: run the
   fill underneath, crossfade at the transition, and move your edit off the
   picture cut.
4. Find a click or a mouth noise in one take and patch it with adjacent tone.
5. Play the result for someone who wasn't watching you work. If they can hear
   where the edit is, keep going.
{{< /drill >}}

## Reference

- John Purcell, *Dialogue Editing for Motion Pictures: A Guide to the Invisible Art*, the standard text on this craft
- [Dialog editing with room tone](https://reaper.blog/2015/03/video-dialog-editing-with-room-tone/), a REAPER-specific walkthrough
