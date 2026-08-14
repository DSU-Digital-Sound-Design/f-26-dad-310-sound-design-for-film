---
title: "Worldizing and Futz"
summary: "Two ways to put a sound inside the film's world: re-record it through a real space, or process it to sound like a device."
tags: [worldizing, futz, dialogue, perspective, post-production]
---

A sound effect or a dialogue line arrives clean and close. The scene may need it
to come from somewhere: a car radio, a phone, a PA in another room, the far end
of a canyon. This lesson covers the two standard ways to get it there.
Worldizing re-records the sound through a real acoustic space. Futzing processes
it to sound like it is playing through a device.

## Worldizing

Worldizing plays a prerecorded sound through a loudspeaker in a real
environment and re-records the result with a microphone. The room, the air, and
the distance do the processing. Reverb plugins model reflections, but a real
space adds what plugins approximate: wind, off-axis coloration, and the way a
sound softens as it travels. Moving the speaker or the microphone during the
re-record adds perspective shifts and Doppler that would be tedious to fake.

Walter Murch coined the term, and the classic examples are worth knowing:

- *American Graffiti* (1973): Murch and George Lucas played a fake two-hour
  Wolfman Jack radio show through car radios in a backyard, re-recording from
  varying distances while moving speakers and microphones. The cruising scenes'
  radio sound is that backyard.
- *Apocalypse Now* (1979): studio ADR played through real military radio
  hardware in an isolation box became the film's transmission voices.
- *Magnolia* (1999): recordings of frozen chickens hitting walls were played
  into a canyon and re-recorded at a distance for the rain of frogs.
- *Daylight* (1996): dialogue played through an underwater speaker in a
  swimming pool, re-recorded by a waterproofed lav 42 feet away, produced the
  film's murky underwater voices. The water stripped the lows on its own.

The equipment barrier is low. A portable speaker, a Zoom recorder, and a
stairwell are a worldizing rig.

## Futz

Futzing filters and degrades a signal until it reads as a device: phone, radio,
TV, intercom. The traditional phone voice is a bandpass, because telephone
systems historically carried only a narrow midrange band.

{{< stats >}}
{{< stat value="500 Hz – 3 kHz" label="The classic phone band" note="High-pass and low-pass in ReaEQ gets you most of the way. Modern digital calls are cleaner, so designers add light distortion to suggest a small speaker working hard." >}}
{{< stat value="2–3 frames" label="Crossfade at the picture cut" note="Perspective changes are cut tight. The voice switches between live and futzed exactly at the cut, softened by a very short fade." >}}
{{< /stats >}}

## The phone split and perspective cutting

Phone calls follow a convention the audience has internalized: when a character
is on screen, their voice is live and full range; the person on the far end is
filtered. When the picture cuts to the other location, the roles reverse
instantly. In a split screen showing both characters, the convention drops the
filter and plays both voices direct.

Dialogue editors build this as a phone split, four tracks for a two-person
call:

- Character A live, used when A is on screen
- Character A phone, used when B is on screen
- Character B live
- Character B phone

Two details make the split believable. First, run a continuous line of each
location's room tone in parallel; a phone line does not go silent when the
speaker pauses, and neither should the scene. Second, the cuts between live and
phone are phase-coherent splits of one continuous recording, which is the equal
gain crossfade case from the [dialogue editing
lesson](/lectures/dialogue-editing/).

The convention is also a dramatic instrument. In *The Deep End*, a
blackmailer's calls start heavily filtered, and the filtering falls away as his
threat gets closer, until his voice sits unfiltered inside the mother's house.

## Who applies the futz

Professional dialogue editors deliver phone splits flat: organized, cut, and
unprocessed. The mixer applies the actual filtering on the mix stage, where the
monitoring can be trusted, and keeps the live recording underneath as room to
maneuver. You are both people on your projects, so borrow the discipline: build
the split first, then put the futz on the track as FX rather than rendering it
into the files. You can retune it during the final mix.

{{< drill label="Lab: one line, three worlds" >}}
Use the clean dialogue line you recorded on 9/23 and a portable speaker.

1. Futz it: bandpass the line to roughly 500 Hz to 3 kHz in ReaEQ on the track,
   and add a light distortion plugin. A/B against the clean take.
2. Worldize it: play the clean line through the speaker in a stairwell,
   bathroom, or hallway and re-record it with a Zoom recorder from at least ten
   feet away. Move the recorder during one take.
3. Compare the worldized take against a reverb plugin preset on the same line.
   Note what the real space did that the plugin did not.
4. Build a minimal phone split: your clean line on one track, the futzed
   version on another, with a continuous bed of room tone underneath. Cut
   between them at an imaginary picture cut with a 2 to 3 frame fade.
{{< /drill >}}

## Reference

- John Purcell, *Dialogue Editing for Motion Pictures*, on phone splits and
  perspective cuts
- Kathryn Kalinak (ed.), *Sound: Dialogue, Music, and Effects*, on worldizing
  and playback history
