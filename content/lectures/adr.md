---
title: "ADR: Replacing a Line to Picture"
summary: "How dialogue gets re-recorded in a studio and fitted back into the film so no one can tell."
tags: [ADR, dialogue, recording, post-production]
---

ADR (automated dialogue replacement, also called looping) re-records a line in a
studio and fits it back to picture. It can replace dialogue affected by radio mic
breakup, rain on the zeppelin, or other location problems. Productions also use
ADR for performance or script changes, lines added over off-camera moments,
group walla, and TV-safe alternates.

The workflow below follows Purcell's *Dialogue Editing for Motion Pictures*. The
last section lists cueing tools for REAPER.

## Spotting and cueing

ADR is spotted after picture lock. Each line gets a searchable cue code built
from the character and reel, such as REB 309 for Rebecca, reel 3, cue 9.

Break long lines into sections the actor can perform comfortably. Purcell
recommends placing breaks:

- at the end of a sentence
- at a breath, which gives the actor a natural reset
- at an inflection, where the pitch or emphasis shifts

## The session

The actor watches the scene and hears three beeps. A streamer wipes across the
screen, and on the imaginary fourth beep the guide track mutes and the actor
delivers the line. Expect many takes. The recordist keeps a log of every take,
marking the holds worth keeping and the buy, which is the selected take.

Actors may become frustrated while trying to match their original performance.
Keep the session patient and concentrate on the line's pitch, rhythm, and
emphasis rather than its words. If an actor gets stuck, ask them to close their
eyes and listen to the guide track or trace the rhythm with nonsense syllables.
If a cue still does not work, move on and return to it later.

Purcell notes that a take can look synchronized and still sound wrong if the
actor stresses a different syllable than in the production take. "How NOW brown
cow" will not match footage of "how now, BROWN cow." Check the stress pattern as
well as the lip movement.

## Matching the room

The studio take needs to match the location recording. Make that match during the
recording session rather than relying on processing later.

- Check the sound report for the production microphone. Use the same model, or
  the closest available option, at the same distance and angle as the original
  boom or lav.
- Match the space. ADR stages have live and dead areas; pick the one closer to
  the scene's acoustics.
- Run Purcell's in-session test early. Record one line, synchronize it, add
  production room tone around it, and play the transition in context. If the
  sound changes noticeably, adjust the microphone or room before recording the
  remaining lines.

## Fitting the line

In the edit, top and tail the buy take. Align it using the same techniques used
for alternate takes in the [dialogue editing
lesson](/lectures/dialogue-editing/): work in blocks of three or four words,
anchor on hard consonants, and place internal edits within sibilants. Do not cut
inside a vowel because the splice may click or phase.

If manual editing is not enough, stretch only the words that need it, and keep
an untouched, synchronized copy on a work track. Use alignment software such as
VocAlign only after editing the cadence by hand. Processing a poorly synchronized
line can damage its sibilants.

Two practices carry over from the dialogue lesson:

- Keep the original line. Edit it fully and leave it synchronized on a muted
  safety track so the mixer can compare or restore it.
- A studio take is drier than a location recording. Place room tone under the ADR
  to maintain the scene's background. Leave the final EQ and reverb matching for
  the mix session, where you can make those decisions on the mix monitors.

## Cueing tools in REAPER

The streamer began as a literal line drawn on the film print, wiping across the
screen as the reel played toward the cue. Today software draws the same moving
line over the video. Two affordable options are
[Viper](https://www.vennaudio.com/our-new-plugin-viper/) (about £42, with a free
trial), which wipes a cue line across the video, and
[Rythmoband](https://www.extremraym.com/en/downloads/reascripts-pack-rythmoband/)
(€30 for students), which adds dubbing-style scrolling text to REAPER. Neither is
required for this lab. You can use click items for the beeps and REAPER's video
window for the picture.

{{< drill label="Lab: replace a line to picture" >}}
Work in pairs. You need a phone, the studio, and one line of dialogue.

1. Film your partner on a phone delivering one line somewhere noisy: a hallway,
   the stairwell, or outside. Use this as the production take, including its
   defects. Record 30 seconds of room tone before leaving the location.
2. Import the video into REAPER and open the video window. Top and tail the
   line, and cue it: three short click items as beeps, one beat apart, ending
   where the line starts.
3. In the studio, your partner re-records the line to picture. Roll playback
   with the beeps, mute the guide on the fourth beat, and log every take. Mark
   the buy. Direct for cadence, not just words.
4. Fit the buy take: anchor on a hard consonant, edit inside sibilants if the
   rhythm drifts, and lay the location's room tone underneath.
5. Play both versions for another pair: the original noisy take, then the ADR
   line with room tone underneath. Ask whether the ADR sounds like part of the
   original scene.
{{< /drill >}}

## Reference

- John Purcell, *Dialogue Editing for Motion Pictures: A Guide to the Invisible
  Art*, ADR chapters
- [Viper](https://www.vennaudio.com/our-new-plugin-viper/), a streamer and beep
  plugin with a free trial
