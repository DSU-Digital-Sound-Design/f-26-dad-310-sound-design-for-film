---
title: "Editing and Cleaning Up Audio in REAPER"
---

First work through LISTEN with the supplied files, including a finished export.
Then open one of your own Assignment 3 recordings and work through the
[LISTEN checklist](/lectures/week-7/listen-mantra/) to finish and export it.

By the end of class, you should have one edited field-recorded take, a checked
WAV export, and a short note explaining what you changed or left alone. This
is practice for [Assignment 4](/assignments/assignment-4-sfx-editing/), not an
additional submission.

## Have these ready

- REAPER, headphones, and your Assignment 3 recordings.
- A short detail recording to edit during the lab.
- These demonstration files:
  [clicky.wav](../clicky.wav), [pops.wav](../pops.wav), and
  [low-freq-hum.wav](../low-freq-hum.wav).

## Practice with the supplied files

### L: Listen and mark the examples

1. Use **File > Save project as** to create a project named `Editing Practice`. Enable
   **Create subdirectory for project** and **Copy all media into project directory**.
2. Import `clicky.wav`, `pops.wav`, and `low-freq-hum.wav` onto separate tracks.
   Name each track after its file. Keep full-length copies on muted backup
   tracks, and label those tracks `ORIGINAL`.
3. Solo each working track in turn and listen through it before editing.
   Identify the wanted sound and the click, pop, or low-frequency noise.
   Place the edit cursor at a problem and press `M` to add a marker.
   Double-click the marker to name it, such as `click` or `pop`.
4. Keep only the example you are working on audible. Leave your Assignment 3
   recordings closed until the next section, **Edit your own recording**.

Turn **Ripple editing** off and turn **Snap** off for these free-time SFX edits.
You can use the toolbar buttons; hover over them to check their state. Removing
an item should not unexpectedly move the rest of the session.

### I: Repair clicks and pops

Solo the working `clicky` track. Select the item, place the cursor near
the click, and zoom horizontally until you can see the brief disturbance.
Increase the track height if the waveform is difficult to inspect.

1. Listen across the suspected click to confirm its location. Place the cursor
   just before it and press `S` to split the selected item. Split again just
   after it.
2. On the working copy, delete the tiny section containing the click. Listen
   to the gap. This shows why removing the waveform alone may leave an audible
   hole or a new boundary click.
3. If the surrounding sound can tolerate a shorter duration, move the right
   item left so it slightly overlaps the left item. Enable **Auto-crossfade**
   on the toolbar and adjust the overlap until the join is unobtrusive.
4. Alternatively, if duration or continuity must stay intact, undo any shortening
   and keep the original gap in place. Copy a
   clean piece of nearby background from the same recording onto a repair
   track, place it across the gap, and fade it in and out. Check that it does
   not repeat an obvious event or create a level bump at either end. Unsolo
   other tracks and solo both the working track and repair track to hear the
   complete edit together.
5. Compare with the original. Undo the repair if it removes a wanted attack or
   draws more attention than the click.

Unsolo and mute `clicky` and any repair track, then solo the working `pops`
track and locate the pop. If the pop overlaps wanted sound, do not cut away
the entire event. Try a local level reduction by splitting around the problem
and lowering that item's volume in **Item properties** with `F2`, then check
the new boundaries. For your own recordings, an alternate take may be better
than repair. For speech-specific repair, see
[dialogue editing](/lectures/dialogue-editing/).

### S: Compare processing on the hum example

Keep each example on its own track so one track's processing does not affect
the other practice files. Add one processor at a time through the track's
**FX** button. Use the effect's checkbox in the FX chain to bypass it, and
compare at similar listening loudness.

#### ReaEQ: reduce unwanted low frequencies

Unsolo and mute `pops`, then solo the working `low-freq-hum` track.

1. Add **ReaEQ**. Select a band and change its type to **High pass**.
2. Begin with the cutoff low, then raise it while listening. Stop when the
   unwanted low-frequency energy is reduced; back off if the wanted sound
   becomes thin.
3. Bypass the band and compare. Describe what disappeared besides the noise.
4. If the problem is a steady pitched hum, inspect the analyzer for a narrow
   peak. Try a narrow cut at that frequency instead of raising the high-pass
   cutoff through useful sound. Do not cut every visible peak.

There is no single cutoff setting for all your field recordings. Save the
setting only if this recording sounds more useful with it.

#### ReaFIR: compare noise reduction on a fresh copy

Duplicate the original `low-freq-hum` item onto a new track with no FX. Unsolo
and mute the ReaEQ version, then solo this new track. Look for a passage containing only
the unwanted background. If the file has no suitable noise-only passage, skip
this comparison; do not switch to your Assignment 3 recording yet.

1. Add **ReaFIR** and set its mode to **Subtract**.
2. Drag a time selection over the noise-only passage. Enable repeat playback
   and play that selection.
3. Check **Automatically build noise profile** while the noise plays, then
   **uncheck it before playing any wanted sound**. Stop repeat playback and
   clear the time selection.
4. Play the wanted event and its tail. Bypass ReaFIR and compare at similar
   loudness. Listen for missing texture or a metallic, watery decay.
5. Use REAPER's FX wet/dry control to blend some untreated signal back in if
   the fully processed result is too aggressive. Some noise will return too.
   Bypass the effect if the tradeoff is worse than the original.

Do not leave profiling enabled during the event: it would learn frequencies
you wanted to keep. You do not need ReaFIR on every source for Assignment 4.

### T: Check whether trimming is needed

Return to the working `clicky` track and any repair track it uses. Unsolo and
mute the other examples; solo the working track and its repair track together.
Keep the repairs you decided to retain. Use this same example through T, E, and N.

1. Listen to the beginning and end. Is there a slate, excess silence, or unwanted
   material outside the sound you want to keep? `clicky.wav` is already trimmed;
   keep its existing boundaries if they still work after your repair.
2. Only if needed, split with `S` or drag the item's edges to remove unwanted
   material. Preserve the quiet beginning, full attack, and complete decay,
   with enough room for any needed fades. Leave the original track intact.
3. If extending an edge makes the item repeat its contents, open **Item
   properties** with `F2` and disable **Loop source**. Listen to the complete
   result and confirm that any boundary change helped.

Checking the boundaries satisfies this step. You do not need to shorten a
recording that is already edited well.

### E: Check every fade and join

1. Listen to the existing boundaries first. Keep fades that already work. To
   add or adjust one, drag inward from an item's upper-left or upper-right
   corner. Zoom in if the handle is hard to grab.
2. If a boundary clicks, try a short fade and extend it only as far as needed.
   Right-click the fade to compare curve shapes.
3. Check internal joins, including any repair patch. Where adjoining items
   can overlap, enable **Auto-crossfade** and adjust the overlap and curves by
   ear. Keep fixed-duration edits in place.
4. Listen once close up, then again with several seconds of surrounding audio.
   Check for a softened attack, a missing tail, a dip, or a sudden texture change.

Keep the impact and decay intact. Do not add a long fade simply because it
makes the waveform look tidy.

### N: Normalize, name, and check the example

Export the repaired `clicky` example. Save this practice export separately from
your Assignment 4 deliverables.

1. Drag a time selection around the complete repaired example, including all
   its edited pieces and any repair patch. Include the full decay. Solo the
   working `clicky` track and its repair track, if used; keep originals and
   other examples muted. Play the selection to check what will be exported.
2. Open **File > Render**. Set **Source: Master mix** and **Bounds: Time selection**.
   This combines the edited pieces and any repair track into one file and
   includes their processing.
3. Set **File name** to `ClickRepair_Practice` and the destination to a
   `Practice-Exports` folder inside this practice project. Choose WAV, 24-bit,
   and match the source file's sample rate and channel count.
4. Open the render window's **Normalize/Limit/Fade** settings and use **peak
   normalization** with a target of **-0.5 dBFS** for this practice export. Do not
   substitute a LUFS target or add a limiter to meet the peak target.
5. Check the output filename and render statistics, then import the exported
   WAV onto a fresh track with no FX. Solo that track, listen from beginning
   to end, and verify its peak, channel count, start, and decay. Do not play
   it through the cleanup chain again.

## Edit your own recording

Save and close the practice project. Open a separate editing project for
**one short detail from your Assignment 3 recordings**, then repeat LISTEN:

1. **Listen:** Save the new project with **Copy all media into project directory**
   enabled. Keep the full recording on a muted `ORIGINAL` track and a working
   copy on an `EDIT` track. Listen through it and mark what to preserve or repair.
2. **Identify:** Locate any clicks, pops, or other unwanted sounds. Use the
   repair methods above only where they fit the problem.
3. **Signal process:** Try EQ or noise reduction only if needed. Compare with
   the original at similar listening loudness; a clean take can stay unprocessed.
4. **Trim:** Check the start and end. Remove a slate or unwanted material only
   if present, preserving the full attack and decay. Keep existing boundaries
   when they already work.
5. **Examine:** Check fades and joins by ear, including several seconds around
   each edit.
6. **Normalize and name:** Use the
   [UCS naming and export workflow](/lectures/ucs-library-organization/) and
   Assignment 4's WAV format and sample rate. Export this detail as mono to
   `FINAL-SFX`, with a final peak of **-0.5 dBFS**. Reimport it onto a clean
   track and listen to the entire file. If your finished sound spans several
   items or tracks, use the complete time-selection export above with the UCS
   filename, or a named-region export from the UCS guide, so it remains one WAV.

Play the result for a partner. Switch between the original and edit at similar
listening loudness, and ask them to listen without
watching the screen.

Before you leave, have:

- A saved session containing the original and the working edit.
- One checked export with a complete attack and decay and clean boundaries.
- A sentence identifying the source, the problem, and the result, or explaining
  why no processing was needed. This can become one of Assignment 4's five notes.

For an optional comparison, audition a similar sound in Soundly or SoundQ.
Compare its boundaries and usable tail with yours. This is a reference check, not another
export requirement.

## When you edit an ambience bed

Use the same workflow on your Assignment 3 ambience recordings when preparing
Assignment 4's two beds.

For an Assignment 4 ambience bed, make a time selection exactly **1:00** long
using the selection start/end or length fields. Choose a usable stretch and
trim the working items to those boundaries. Keep the stereo bed on its own
track. Internal edits must preserve the one-minute duration; keep ripple
editing off. Finish assembling the bed before preparing its export.

Listen to both stereo channels across every join. A clean-looking cut in one
waveform does not prove the other channel is clean. Export each bed as stereo
with a peak target between **-18 and -6 dBFS**, then check its duration and
continuity in the rendered WAV.

## REAPER references

- [REAPER User Guide](https://www.reaper.fm/userguide.php): item editing,
  fades, render settings, and the ReaEffects guide.
- [ReaPlugs reference](https://www.reaper.fm/reaplugs/): ReaEQ filters and
  ReaFIR's Subtract mode. These effects are included in REAPER.
