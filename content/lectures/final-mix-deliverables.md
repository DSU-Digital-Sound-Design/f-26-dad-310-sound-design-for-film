---
title: "The Final Mix and Deliverables"
summary: "How a film mix comes together: dialogue first, then everything else, measured against a loudness spec and delivered as stems."
tags: [mixing, loudness, stems, post-production]
---

The re-recording mix is the last stage of postproduction, where dialogue, ADR,
Foley, effects, ambiences, and music are balanced into one soundtrack. On your
final project you are the editor and the mixer at once, which makes it worth
knowing how the professional version works. The habits scale down.

Most of this follows Purcell's *Dialogue Editing for Motion Pictures*; the
loudness specs come from current delivery standards.

## Dialogue leads

Dialogue is mixed first, and everything else is balanced against it. The level,
tone, and noise floor established in the dialogue premix decide how loud and how
wide the music and effects are allowed to play. If your film has spoken lines,
set them first and do not move them to make room for a sound effect. Move the
effect.

For your final mix, work in this order: dialogue, then Foley, then effects, then
ambiences, with music placed against the finished balance. This is the same
order the [final project brief](/assignments/final-project/) asks for.

One warning from Purcell that applies directly to you: do not crush dialogue
with heavy compression or limiting to make it loud. Tracks squeezed that way
sound thin and metallic on better speakers than yours. Match levels from shot to
shot, ride the faders, and leave the dynamics mostly alone.

## Organize like a mixer is coming

Professional mixers receive sessions with a fixed track layout that never
changes from reel to reel, muted work tracks, sync pops, and cue sheets that let
them navigate the film without watching it. You already know the editing side of
this from the [dialogue editing lesson](/lectures/dialogue-editing/): splits,
checkerboarding, and safety tracks.

The student version of that hygiene:

- Name every track by what it carries, and group tracks by category: dialogue,
  Foley, effects, ambience, music.
- Keep one folder or bus per category. This is what makes stems possible later.
- Mute and hide your work tracks instead of deleting them.
- Keep any sound that is not speech off the dialogue tracks. Door slams and
  props that came in with the dialogue recording get their own track, for the
  reason below.

## Stems and the M&E

A finished film is not delivered as one stereo file. The mix is recorded into
**stems**: separate, synchronized renders of dialogue, music, and effects that
sum to the full mix. Stems exist so the film can be reversioned without
remixing: a TV cut, a trailer, a censored airline version.

The clearest example is the **M&E track**, music and effects with no dialogue.
Foreign distributors need it to dub the film into other languages. If a door
slam is baked into your dialogue track, it disappears along with the English,
and the dubbed version has a silent door. That is why non-speech production
sound gets split onto its own tracks.

In REAPER, stems are cheap if your session is organized: select the tracks in
one category and use `File > Render`, with the source set to selected tracks or
the category's parent folder.

## The loudness spec

Distributors do not accept "it sounded right on my headphones." Delivery specs
state a measured loudness, and the measurement is integrated loudness in LUFS
(also written LKFS; same thing), with a true peak ceiling.

{{< stats >}}
{{< stat value="-27 LKFS" label="Netflix, dialogue-gated" note="Measured only where dialogue is present, with a tolerance of 2 LU either way and a -2 dBTP true peak ceiling." >}}
{{< stat value="-24 LKFS" label="US broadcast (ATSC A/85)" note="Full-program measurement, -2 dBTP. European broadcast (EBU R128) is -23 LUFS with a -1 dBTP ceiling." >}}
{{< /stats >}}

Netflix has a rule that matters for this class: if a film is less than 15%
dialogue, which describes many of your projects, it is measured program-gated at
**-24 LKFS** instead. That is the target for your final render: **-24 LUFS
integrated, true peak under -2 dB**.

Measuring in REAPER costs nothing. Right-click the master meter and enable the
loudness readout to watch LUFS-I while you work, and check the "Calculate
loudness" option in the render dialog (or run a dry render) to get an exact
integrated number for the finished file. If you land at -20, lower the master
until the measurement reads -24. If you land at -30, raise it. Do not reach for
a limiter to close the gap.

{{< drill label="Lab: measure, hit spec, render stems" >}}
Bring your final project session in whatever state it is in.

1. Group your tracks into category folders if they are not already: dialogue,
   Foley, effects, ambience, music.
2. Run a dry render and write down the integrated LUFS and true peak of your
   current mix.
3. Adjust the master until the mix measures -24 LUFS integrated with true peak
   under -2 dB. Listen to what changed. Nothing should, except overall level.
4. Render stems: one file per category folder, plus the full mix. Play the
   stems together and confirm they sum to the mix.
5. If you have dialogue, mute it and listen to what remains. That is your M&E.
   Any speech-adjacent sound that vanished with it is on the wrong track.
{{< /drill >}}

## Reference

- John Purcell, *Dialogue Editing for Motion Pictures: A Guide to the Invisible
  Art*, chapters on premixes and delivering to the mix
- [Loudness delivery specs
  explained](https://www.production-expert.com/production-expert-1/what-is-loudness-lufs-lkfs-and-delivery-specs-explained-2026),
  a current survey of the standards above
