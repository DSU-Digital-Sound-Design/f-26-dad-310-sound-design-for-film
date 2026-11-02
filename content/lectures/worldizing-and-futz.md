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

The DJ scene in *La Haine* (1995) performs the technique inside the fiction. A
DJ points his speakers out an apartment window and the camera drifts over the
housing estate as the music reverberates off the buildings, changing with every
distance. It is the stairwell exercise at the scale of a neighborhood. Watch how
the sound changes as the camera moves, and describe it in the same terms you
will use for your own worldized line.

<iframe width="560" height="315" src="https://www.youtube.com/embed/PE6UdMGfjHQ" title="La Haine (1995) DJ scene" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Alvin Lucier: I am sitting in a room

Lucier records his voice, plays the recording into a room, and records that
playback. He repeats the process with each new recording. The room's resonant
frequencies become more prominent, and the words become less intelligible.

Compare the opening speech with a later iteration. What does the room add or
change as the process repeats?

<iframe width="560" height="315" src="https://www.youtube.com/embed/fAxHlLK3Oyk" title="Alvin Lucier: I am sitting in a room" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

This uses the playback-and-recording process of worldizing repeatedly. In our
lab, compare a first re-recording with later generations to hear how the device
and room change the sound each time.

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

Keep each location's audible background continuous across the call. Preserve
useful background already in the dialogue and add matching room tone where
needed, without unnecessarily doubling it. Start with an equal gain crossfade
for aligned copies of the same line, then listen for dips, swells, or tonal
changes as processing changes their relationship. See the [dialogue editing
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

## Lab: one voice, different devices and spaces

**Goal:** make one recorded voice suggest a different playback device or space,
then explain the audible clues behind that impression.

Work together on a shared booth recording, then compare devices and locations
in small groups. This is in-class practice with no separate graded submission.
Save the recordings and your REAPER session for later sound-design work.

### 1. Record the source · 5 minutes

Record a short spoken passage in the audio booth. Include a few pauses so we
can hear the room and the decay after the words. Listen back for clear speech
without clipping, then keep this original file unchanged.

Transfer the same original file to a phone and a computer or another available
playback device.

### 2. Compare playback devices · 10 minutes

Predict which device will sound thinner, brighter, or less clear. Play the
original through the phone speaker and re-record it with the booth microphone.
Then repeat with a computer speaker or another student device in the booth.

Keep the booth microphone, recording settings, speaker-to-microphone distance,
and playback level as consistent as practical. Check levels before each take
and avoid clipping. Label each file with the playback device and room.

### 3. Re-record the re-recording · 10 minutes

Stay in the booth and use the same speaker and booth microphone setup from the
device comparison. Play that setup's first re-recording through the speaker
and record the playback. Use the new recording as the source for the next
pass, repeating two or three times as time allows.

Label the files `Generation_1`, `Generation_2`, and so on, including the device
and room in the names. For this experiment, each generation uses the previous
recording. For the device and room comparisons, each take uses the original.

Predict what will accumulate, then listen for changes in speech clarity,
brightness, noise, and reverberation. Compare the original, first pass, and last
pass in REAPER at similar listening loudness.

### 4. Change the room · 10 minutes

Next, use a Zoom recorder to take the experiment into other spaces. First
re-record the **original booth file** through one playback device in the booth
with the Zoom. Take that same device and Zoom to a classroom, hallway, or
stairwell and repeat. Keep the speaker-to-microphone distance and recording
settings roughly the same for these Zoom takes so we can compare the rooms.

Listen before recording and avoid capturing other groups. If equipment or time
is limited, make one shared recording in each space for the class to compare.

### 5. Compare and choose · 15 minutes

Play selected comparisons for the class. Each group should identify:

- One audible difference and the device, room, or repeated pass that may explain it.
- A film situation where one version would work, such as a voice from another
  room or a small radio, and the audible clue that makes it convincing.

Finish with a short instructor demonstration: use ReaEQ on the original to make
a phone-like bandpass, starting around 500 Hz to 3 kHz. Compare this with the
physical phone-speaker recording. What does filtering reproduce, and what else
do you hear in the re-recording?

Keep the phone-split example above as a later editing extension. When adding
room tone, aim for continuous audible background; preserve useful background
already in the recording and fill gaps where needed, following the
[dialogue editing lesson](/lectures/dialogue-editing/).

## Free tools for a software comparison

These tools simulate aspects of playback devices and spaces. Use them on a copy
of the original booth recording, then compare with the physical re-recordings
at similar listening loudness. Installation is optional; an instructor demo is
enough for this lab.

- **[Soundly Place it](https://getsoundly.com/tools/):** a free speaker and space
  simulation plugin with 40 acoustic environments based on recorded impulse
  responses. This is the closest match to our experiment. Choose a speaker and
  space, then describe what sounds similar to or different from the real recording.
- **[Voxengo Boogex](https://www.voxengo.com/product/boogex/):** a free guitar amp,
  speaker-cabinet simulator, and impulse-response loader. Turn off the amp stage
  to use it as a convolution processor. It is an additional option for exploring
  speaker coloration; the result depends on the impulse response you load.

An impulse response captures how a system responds to a brief excitation.
Convolution applies that response to another sound. Our repeated recording
experiment also lets us hear noise and other changes accumulating across passes.


## Reference

- [Walter Murch on worldizing *American
  Graffiti*](https://www.lucasfilm.com/news/walter-murch-american-graffiti/)
- [ITU-T P.341: conventional and wideband telephone
  ranges](https://www.itu.int/epublications/publication/itu-t-p-341-2011-03-transmission-characteristics-for-wideband-digital-loudspeaking-and-hands-free-telephony-terminals)
- John Purcell, *Dialogue Editing for Motion Pictures*, on phone splits and
  perspective cuts
- Kathryn Kalinak (ed.), *Sound: Dialogue, Music, and Effects*, on worldizing
  and playback history
