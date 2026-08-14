---
title: "Worldizing and Futz"
summary: "Two ways to put a sound inside the film's world: re-record it through a real space, or process it to sound like a device."
tags: [worldizing, futz, dialogue, perspective, post-production]
---

A clean recording may need to sound as if it comes from a car radio, phone, PA in
another room, or the far end of a canyon. Worldizing re-records the sound in a
real acoustic space. Futzing processes it to imitate playback through a device.

## Worldizing

Worldizing plays a prerecorded sound through a loudspeaker in a real
environment, then captures the result with a microphone. The new recording
includes the acoustics of the space, the playback speaker, and the distance
between the speaker and microphone. It may also capture wind and off-axis
coloration. Moving the speaker or microphone while recording creates changes in
perspective and pitch that would take more work to build with plugins.

Walter Murch coined the term. These films use the technique in different ways:

- *American Graffiti* (1973): Murch and George Lucas played a two-hour Wolfman
  Jack radio program through a loudspeaker in a backyard. They recorded it from
  a distance while moving the speaker and microphone, then blended those tracks
  with the original program.
- *Apocalypse Now* (1979): studio ADR played through real military radio
  hardware inside an isolation box became the film's transmission voices.
- *Magnolia* (1999): recordings of frozen chickens hitting walls were played
  through speakers into a canyon and recorded again at a distance for the rain
  of frogs.
- *Daylight* (1996): dialogue played through an underwater speaker in a
  swimming pool, re-recorded by a waterproofed lav 42 feet away, produced the
  film's underwater voices.

You can worldize a sound with a portable speaker and a Zoom recorder in a space
such as a stairwell.

## Futz

Futzing uses filtering and distortion to make a signal sound as if it comes from
a phone, radio, TV, or intercom. Conventional narrowband telephone systems use a
nominal range of 300 Hz to 3.4 kHz. For film sound, a tighter bandpass can make
the effect easier to recognize.

{{< stats >}}
{{< stat value="500 Hz to 3 kHz" label="A starting EQ range" note="High-pass and low-pass filters in ReaEQ create the basic effect. Add light distortion to suggest a small speaker." >}}
{{< stat value="2 to 3 frames" label="Crossfade at the picture cut" note="Switch between the live and futzed tracks at the cut, using a short fade to smooth the transition." >}}
{{< /stats >}}

## The phone split and perspective cutting

Film and television often use the same convention for phone calls. The character
on screen sounds live and full range, while the person at the other end sounds
filtered. When the picture cuts to the other location, the processing switches.
In a split screen showing both characters, both voices may play without the
filter.

Dialogue editors build this as a phone split, four tracks for a two-person
call:

- Character A live, used when A is on screen
- Character A phone, used when B is on screen
- Character B live
- Character B phone

Run continuous room tone for each location beneath the call so the background
does not disappear when a speaker pauses. The live and phone versions are
phase-coherent splits of the same recording, so use the equal gain crossfade
described in the [dialogue editing
lesson](/lectures/dialogue-editing/).

The processing can also change with the story. In *The Deep End*, a blackmailer's
calls begin heavily filtered. The filtering decreases as the threat gets closer,
until his voice plays unfiltered inside the mother's house.

## Who applies the futz

Professional dialogue editors deliver phone splits organized and unprocessed.
The mixer applies the filtering during the mix and keeps the live recording
available. On your projects, build the split first and apply the futz as track FX
instead of rendering it into the files. This leaves the settings adjustable for
the final mix.

{{< drill label="Lab: one line, three worlds" >}}
Use the clean dialogue line you recorded on 9/23 and a portable speaker.

1. Futz it: bandpass the line to roughly 500 Hz to 3 kHz in ReaEQ on the track,
   add light distortion, and compare it with the clean take.
2. Worldize it: play the clean line through the speaker in a stairwell,
   bathroom, or hallway. Re-record it with a Zoom recorder from at least ten
   feet away. Move the recorder during one take.
3. Compare the worldized take against a reverb plugin preset on the same line.
   Note the differences between the two versions.
4. Build a minimal phone split: your clean line on one track, the futzed
   version on another, with a continuous bed of room tone underneath. Cut
   between them at an imaginary picture cut with a 2 to 3 frame fade.
{{< /drill >}}

## Reference

- [Walter Murch on worldizing *American
  Graffiti*](https://www.lucasfilm.com/news/walter-murch-american-graffiti/)
- [ITU-T P.341: conventional and wideband telephone
  ranges](https://www.itu.int/epublications/publication/itu-t-p-341-2011-03-transmission-characteristics-for-wideband-digital-loudspeaking-and-hands-free-telephony-terminals)
- John Purcell, *Dialogue Editing for Motion Pictures*, on phone splits and
  perspective cuts
- Kathryn Kalinak (ed.), *Sound: Dialogue, Music, and Effects*, on worldizing
  and playback history
