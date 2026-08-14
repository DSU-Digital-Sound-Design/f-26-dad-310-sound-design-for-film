---
title: "The Final Mix and Deliverables"
summary: "How a film mix comes together: dialogue first, then everything else, measured against a loudness spec and delivered as stems."
tags: [mixing, loudness, stems, post-production]
---

The re-recording mix is the last stage of postproduction. This is where dialogue,
ADR, Foley, effects, ambiences, and music are balanced into a single soundtrack.
For the final project, you will handle both editing and mixing, so the session
needs to stay organized through both stages.

The mixing workflow below follows Purcell's *Dialogue Editing for Motion
Pictures*. The loudness targets come from current delivery standards.

## Mix dialogue first

Mix dialogue first, then balance the other elements against it. The dialogue
premix establishes the level, tone, and noise floor that the music and effects
must work around. If the film has spoken lines, set their levels before adding
the other elements. Adjust an effect rather than moving the dialogue to make room
for it.

For the final mix, work in this order: dialogue, Foley, effects, ambiences, and
music. The [final project brief](/assignments/final-project/) uses the same order.

Do not use heavy compression or limiting simply to make dialogue loud. Purcell
warns that this can make dialogue sound thin and metallic on more revealing
speakers. Match levels from shot to shot with fader automation and preserve most
of the original dynamics.

## Session organization

Professional mix sessions keep the same track layout from reel to reel. They also
include muted work tracks, sync pops, and cue sheets for navigating the film. The
[dialogue editing lesson](/lectures/dialogue-editing/) covers the related editing
practices: splits, checkerboarding, and safety tracks.

For the final project:

- Name each track for its contents and group the tracks into dialogue, Foley,
  effects, ambience, and music categories.
- Use one folder or bus for each category so you can render stems later.
- Mute and hide your work tracks instead of deleting them.
- Keep any sound that is not speech off the dialogue tracks. Door slams and
  props captured with dialogue belong on separate tracks.

## Stems and the M&E

A film mix includes more than a single stereo file. It is also rendered as stems:
separate, synchronized files for dialogue, music, and effects that combine to
reproduce the full mix. These files allow someone to create a TV cut, trailer, or
censored airline version without rebuilding the mix.

The M&E track contains music and effects without dialogue. Foreign distributors
use it when dubbing a film into another language. If a door slam remains on the
dialogue track, removing the original dialogue will also remove the slam. Keep
non-speech production sound on separate tracks so it remains in the M&E.

To render stems in REAPER, select the tracks in one category and choose `File >
Render`. Set the source to the selected tracks or the category's parent folder.

## The loudness spec

Delivery specifications define a measured loudness rather than relying on the
listener's monitoring level. They use integrated loudness in LUFS, also written
as LKFS, along with a true peak ceiling.

{{< stats >}}
{{< stat value="-27 LKFS" label="Netflix, dialogue-gated" note="Measured only where dialogue is present, with a tolerance of 2 LU either way and a -2 dBTP true peak ceiling." >}}
{{< stat value="-24 LKFS" label="US broadcast (ATSC A/85)" note="Full-program measurement, -2 dBTP. European broadcast (EBU R128) is -23 LUFS with a -1 dBTP ceiling." >}}
{{< /stats >}}

Netflix measures a film program-gated at -24 LKFS when dialogue makes up less
than 15% of the program. Many projects in this class fit that description. Use
the same target for the final render: -24 LUFS integrated with true peak below
-2 dB.

In REAPER, right-click the master meter and enable the loudness readout to monitor
LUFS-I as you work. To measure the finished file, select "Calculate loudness" in
the render dialog or run a dry render. If the result is -20 LUFS, lower the
master until it reads -24. If it is -30 LUFS, raise the master. Do not use a
limiter simply to reach the target.

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
