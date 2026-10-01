---
title: "SFX Editing and Processing"
number: "04"
weight: 4
week: 9
assigned: "2026-10-23"
due: "2026-11-11"
summary: "Select and edit your field-recorded takes, then name and export 17 production-ready library sounds."
# this assignment carries its own rubric table in the body
rubric: false
---

Use the [LISTEN editing mantra](/lectures/week-7/listen-mantra/) as a checklist throughout this assignment: listen, identify problems, signal process as needed, trim, examine fades, then normalize and name. Recheck the result after every change. The goal is a useful library sound that preserves the character of its source.

### Part 1 - Editing

Use the five sources from [Assignment 3](/assignments/assignment-3-field-recording/). Edit copies and keep the original recordings intact.

- **Beds:** Edit the large- and small-space recordings into two continuous, one-minute stereo beds.
- **Details:** Select and edit five distinct recorded takes from each of the three detail sources, giving you 15 mono effects.
- Remove slates and unwanted sounds, preserve natural attacks and decays, and use fades or crossfades for clean edits.

**Total: 17 finished sounds.**

### Part 2 - Processing

1. **Listen and compare**: Identify a specific problem before applying EQ, compression, or noise reduction. Compare the processed sound with the original at similar listening loudness. Keep processing only when it improves the sound without damaging its character. A clean recording can remain unprocessed.

2. **Ambience beds**: Use EQ or noise reduction only where needed. Preserve the space's texture and continuity. Avoid compression that makes the background audibly pump.

3. **Detail variations**: Use EQ, light compression, or cleanup only where needed. Preserve the differences between recorded takes and listen for softened attacks, lost decay, and noise-reduction artifacts.

4. **Document decisions**: Add a brief note for each of the five sources describing one problem and what you changed, or why you left it unprocessed. A sentence or two is enough.

### Part 3 - Final Production

1. **Final levels**: After editing and processing, normalize each detail export to a peak of **-0.5 dBFS**. For each ambience bed, choose a peak target between **-18 and -6 dBFS**, following LISTEN. These are peak levels, not average loudness targets. Check the rendered files, since processing after item normalization can change the final peaks.

2. **UCS naming**: Follow the [library organization lesson](/lectures/ucs-library-organization/). Use [UCS Finder](https://www.ucs-finder.com/) to choose a CatID for each finished sound. In REAPER, open Item properties with F2 and name each item's active take using `CatID_FXName_CreatorID_SourceID`, without the file extension. Use your initials as CreatorID and `DAD310` as SourceID. Give each variation a distinct number within FXName, such as `DOORWood_Knock Hollow Interior 01_TC_DAD310`.

3. **Exporting**: Export all 17 finished sounds into a FINAL-SFX folder inside your REAPER project folder: two stereo environment beds and 15 mono detail variations. Use **WAV, 96 kHz / 24-bit**, matching Assignment 3. If your recorder required a lower sample rate for Assignment 3, export at that recorded rate in 24-bit and note it in your submission. For a mixed mono/stereo batch, set Channels to **Stereo** and enable **Tracks with only mono media to mono files**. Keep detail sources on tracks containing only mono media and beds on their stereo tracks. Check the output channel counts in the render file list or a dry run. If a detail source is stored as stereo or uses stereo effects, check its channel handling explicitly; use a separate mono render when needed. Each export must contain the complete sound: glue a finished bed into one item before naming it, or use a named region around the full bed. Choose **Selected media items** in File > Render and use `$item` for the filename. If the sound depends on track, bus, or master processing, use **Selected media items via master** and check the routing. For layered sounds, render named regions using `$region`. Preview the filenames for duplicates and listen to every export for clean starts, complete decays, and the intended processing.

4. **Submission**: Submit the zipped REAPER project folder with five clearly labeled source tracks and uniquely named finished items or regions. Include the five brief processing notes in the project or a separate document. Use colors if they help you navigate the session. Include the 17 UCS-named WAVs in FINAL-SFX and all source audio needed to open the project.

---

## Grading Rubric (40 points total)

| Criterion | Exemplary | Proficient | Developing | Emerging | Points |
| --- | --- | --- | --- | --- | --- |
| **Editing Quality (12 pts)** | Clean cuts and fades with no clicks, unwanted sounds removed, each environment running exactly one minute | Clean overall; a click or a slightly off duration | Audible clicks or stray sounds, or durations noticeably off | Edits rough throughout | /12 |
| **Variations (10 pts)** | Five distinct, usable recorded takes from each of the three detail sources: 15 effects differing in duration, intensity, or perspective | All 15 present; a few vary only slightly | Fewer than 15, or variations too alike to be separately usable | Little variation attempted | /10 |
| **Processing and Polish (10 pts)** | Final export peaks meet the specified targets; processing choices preserve source character without artifacts; brief notes explain changes or why processing was unnecessary | Usable overall; one sound or processing explanation needs another pass | Export peaks outside targets, audible processing artifacts, or weak explanations | Major unresolved sound problems or artifacts throughout; decisions unexplained | /10 |
| **Deliverables and Annotation (8 pts)** | FINAL-SFX folder with all 17 UCS-named WAVs in the required format; five labeled source tracks and named edits; complete source media and processing notes | All exports present; minor naming or annotation omissions | Exports missing, repeated naming errors, or missing source labels and notes | Neither exports nor annotation | /8 |

**Total: \_\_\_ / 40**
