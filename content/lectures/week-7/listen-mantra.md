---
title: "The Editing Mantra: LISTEN"
---

Adapted from Ric Viers' *The Sound Effects Bible*. Use LISTEN to turn a raw
recording into a useful library sound while preserving what makes the source
interesting.

By the end of this lesson, you should be able to choose a usable take, explain
an editing decision, and check that the finished sound has clean boundaries
and an appropriate level.

## Start with your favorite recordings

We'll listen to short excerpts from some of your favorite field recordings.
Before you play yours, tell us what the source is and what you like about it.
Then listen together:

- What gives this recording its character: the attack, decay, texture, or sense of space?
- What would you keep, and what would you change to make it useful in a scene?

Describe what you hear before proposing a tool. A distant engine may belong
in an ambience bed; it is not automatically noise to remove.

## The checklist

- **L** - Listen critically
- **I** - Identify clicks, pops, and errors
- **S** - Signal process only as needed
- **T** - Trim/crop the file
- **E** - Examine fades and edit boundaries
- **N** - Normalize and name the file

Follow this as a checklist, then return to earlier steps when an edit changes
what you hear. You can trim around a useful take before processing it. Work on
copies and keep your original recordings intact.

## 1. Listen critically

Play the take from beginning to end. Identify the sound you want to preserve
and its likely use: a continuous ambience bed or an individual detail. Listen
for unwanted handling noise, wind, clipping, and interruptions.

Choose the strongest take before attempting repairs. If a problem overwhelms
the source and repair damages it, choose another take or record again. Keep
the original so you can compare or use another part of it later.

## 2. Identify clicks, pops, and errors

Mark the time of each problem and describe it. A single click calls for a
different approach from steady hiss or low-frequency rumble.

For a brief unwanted sound, try an edit with short fades or a crossfade. Avoid
cutting into the wanted attack or shortening an ambience in a way that breaks
its continuity. For a gap in a bed, try a clean section from the same recording
and listen across the joins.

Noise reduction can help with a steady background problem, but it is not a
general fix for every click or pop. Listen for new metallic or watery artifacts.

See [Editing and cleaning up audio in REAPER](/lectures/week-7/editing/) for
practice files and demonstrations.

## 3. Signal process only as needed

Name the problem before adding a processor.

- **EQ:** reduce unwanted rumble or adjust a frequency range that masks the source. Check that you have not removed its weight or character.
- **Compression:** control a dynamic range that makes the sound difficult to use. Listen for flattened attacks or a background that audibly pumps.
- **Noise reduction:** reduce a persistent unwanted background cautiously. Keep the source's texture and natural decay.

Compare the processed and original versions at similar listening loudness.
Keep a change only when you can explain how it helps. A clean recording can
remain unprocessed.

## 4. Trim/crop the file

Remove the slate and unwanted material before and after the chosen take.
Preserve the complete attack and natural decay. Leave enough space for a
clean fade without cutting off the sound.

For an ambience bed, select a continuous stretch and check any internal joins.
In [Assignment 4](/assignments/assignment-4-sfx-editing/), each finished bed
must be one minute long. A continuous bed does not have to loop seamlessly
unless the task asks for a loop.

## 5. Examine fades and edit boundaries

An abrupt jump in the waveform at a cut can produce a click. A cut near a zero
crossing can help, but it does not guarantee a clean edit, especially in stereo.
Use short fades at exposed boundaries and crossfades where clips join.

Adjust the fade length and shape by ear. A fade that is too long can soften an
attack or remove a useful tail. Listen across every edit, then play the whole
sound without watching the waveform. Can you hear a click, gap, or sudden
change in background texture?

## 6. Normalize and name the file

Peak normalization changes the gain so the highest peak reaches a chosen
level. It does not reduce dynamic range, remove noise, or make different
sounds equally loud to a listener. Raising the gain also raises any remaining
background noise.

For **Assignment 4**, use these final export targets:

- **Individual details:** normalize each to a peak of **-0.5 dBFS**.
- **Ambience beds:** choose a peak target between **-18 and -6 dBFS**.

These are course delivery targets for library files, not universal mixing
levels or average loudness targets. Check the rendered files: processing after
item normalization can change their final peaks.

Name each finished take using the [UCS workflow](/lectures/ucs-library-organization/).
Embedded descriptions and keywords can also make a library searchable; they
are separate from filenames and optional for Assignment 4.

## Try it on one take

Use a copy of a short detail recording. This is in-class practice, not another
submission.

1. Play the original and name one quality to preserve and one problem to address, if there is a problem.
2. Make a clean edit using LISTEN. Leave processing off if it is unnecessary.
3. Compare before and after at similar listening loudness. Explain what improved and check that the attack and decay remain intact.

Before you finish, answer: did your change solve the problem without creating
another one? If not, revise it or choose a better take. Use this same check
throughout Assignment 4; the REAPER editing lesson will cover the tools in
more detail.

## Reference

The [REAPER user guide and official tutorials](https://www.reaper.fm/userguide.php)
provide further help with item editing, fades, processing, and rendering.
