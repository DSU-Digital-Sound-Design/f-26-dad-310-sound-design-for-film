---
title: "ADR: Replacing a Line to Picture"
summary: "How dialogue gets re-recorded in a studio and fitted back into the film so no one can tell."
tags: [ADR, dialogue, recording, post-production]
---

ADR (automated dialogue replacement, also called looping) re-records a line in a
studio and fits it back to picture. It is the escape hatch when repair fails:
radio mic breakup, rain on the zeppelin, an unusable location, or a performance
or script change. Productions also use it to add lines over off-camera moments
and to record group walla and TV-safe alternates.

The workflow below follows Purcell's *Dialogue Editing for Motion Pictures*,
with current REAPER tools noted at the end.

## Spotting and cueing

ADR is spotted after picture lock. Each line gets a searchable cue code built
from the character and reel, such as REB 309 for Rebecca, reel 3, cue 9.

Long lines get broken into fragments an actor can actually perform. Purcell's
rules for where to break:

- at the end of a sentence
- at a breath, which gives the actor a natural reset
- at an inflection, where the pitch or emphasis shifts

## The session

The actor watches the scene and hears three beeps. A streamer wipes across the
screen, and on the imaginary fourth beep the guide track mutes and the actor
delivers the line. Expect many takes. The recordist keeps a log of every take,
marking holds worth keeping and the buy, the take that will be used.

Directing ADR is a psychological job. Actors find it frustrating to chase their
own performance, so stay patient and keep the attention on the cadence of the
line: its pitch, rhythm, and emphasis, not the words. If an actor is stuck, have
them close their eyes and listen to the guide track, or trace the rhythm with
nonsense syllables. If a cue will not land, move on and circle back rather than
beating it to death.

A cadence warning from Purcell: a take can look perfectly in sync and still be
wrong because the actor accented a different syllable than they did on set. "How
NOW brown cow" will never sit against footage of "how now, BROWN cow." Listen
for the accent, not just the lips.

## Matching the room

The studio take has to pass for the location take, and that match is built at
the recording stage, not fixed later.

- Check the sound report for the production microphone and use the same model,
  or the closest available, at the same distance and angle as the original boom
  or lav.
- Match the space. ADR stages have live and dead areas; pick the one closer to
  the scene's acoustics.
- Run Purcell's in-session test early: record one line, sync it immediately,
  fill around it with production room tone, and play the transition in context.
  If it jars, move the mic or change the room before recording everything else.

## Fitting the line

Back in the edit, top and tail the buy take, then align it using the same sync
craft as alternate takes in the [dialogue editing
lesson](/lectures/dialogue-editing/): work in blocks of three or four words,
anchor on hard consonants, and make internal edits inside sibilants. Never cut
inside a vowel; the splice clicks or phases.

If manual editing is not enough, stretch only the words that need it, and keep
an untouched, in-sync copy on a work track first. Alignment software such as
VocAlign is a finishing polish, not a first move: hand-edit the cadence close,
then let the software close the last gap. Forcing a badly-synced line through
alignment software mangles the sibilants.

Two more rules carry over from the dialogue lesson:

- The replaced original never gets deleted. Edit it fully and park it in sync on
  a muted safety track so the mixer can A/B or revert.
- The studio take is drier than the scene. Lay room tone fill under the ADR so
  the ambient backdrop continues through it, and leave the final EQ and reverb
  match to the mix, where the monitoring can be trusted.

## The modern session

The three-beep convention survives, but the streamer is now drawn by software.
Professional stages use dedicated cueing tools; two affordable ones are
[Viper](https://www.vennaudio.com/our-new-plugin-viper/) (about £42, with a free
trial), which wipes a cue line across the video, and
[Rythmoband](https://www.extremraym.com/en/downloads/reascripts-pack-rythmoband/)
(€30 for students), which adds dubbing-style scrolling text to REAPER. Neither
is required here: click items as beeps and REAPER's video window do the job in
our lab.

{{< drill label="Lab: replace a line to picture" >}}
Work in pairs. You need a phone, the studio, and one line of dialogue.

1. Film your partner on a phone delivering one line somewhere noisy: a hallway,
   the stairwell, outside. This is your production take, defects included.
   Record 30 seconds of that location's room tone before you leave.
2. Import the video into REAPER and open the video window. Top and tail the
   line, and cue it: three short click items as beeps, one beat apart, ending
   where the line starts.
3. In the studio, your partner re-records the line to picture. Roll playback
   with the beeps, mute the guide on the fourth beat, and log every take. Mark
   the buy. Direct for cadence, not just words.
4. Fit the buy take: anchor on a hard consonant, edit inside sibilants if the
   rhythm drifts, and lay the location's room tone underneath.
5. Play both versions for another pair: the original noisy take, then the ADR
   line sitting in its tone fill. They should agree the second one passes.
{{< /drill >}}

## Reference

- John Purcell, *Dialogue Editing for Motion Pictures: A Guide to the Invisible
  Art*, ADR chapters
- [Viper](https://www.vennaudio.com/our-new-plugin-viper/), a streamer and beep
  plugin with a free trial
