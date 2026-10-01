---
title: "Naming Sounds: UCS and Library Organization"
summary: "The Universal Category System, embedded metadata, and the habits that make a recording findable a year later."
tags: [UCS, metadata, library, organization, field recording]
---

Five field recordings are easy to track, but a larger library needs consistent
filenames and metadata. A shared naming system makes recordings easier to find
and allows you to add this semester's work to a library you can keep using.

## The Universal Category System

The [Universal Category System](https://universalcategorysystem.com/) (UCS) is
a public-domain system for categorizing and naming sound effects. Version 8.2.1
has 82 main categories and 753 subcategories, each with a short category ID.
Sound library applications such as SoundQ, Soundminer, and BaseHead can use UCS
categories and filenames.

For this class, use four blocks separated by underscores:
`CatID_FXName_CreatorID_SourceID`.

{{< stats >}}
{{< stat value="CatID" label="Category ID" note="Choose an ID from the official UCS list, such as DOORWood or WEATRain." >}}
{{< stat value="FXName" label="Short description" note="Describe the specific sound in a few words, such as Creak Slow Interior. Spaces are allowed in this block." >}}
{{< stat value="CreatorID" label="Who recorded it" note="Use your initials or a short handle." >}}
{{< stat value="SourceID" label="Where it came from" note="The project, library, or session: DAD310 or ZOOMH4n." >}}
{{< /stats >}}

For example, a door recording from the field assignment might be:

`DOORWood_Creak Slow Interior_TC_DAD310.wav`

Use underscores only to separate the four blocks. Search [UCS
Finder](https://www.ucs-finder.com/) using a sound description, such as
"footsteps," "metal," or "water." Read the category explanation, choose the
closest match, and copy its CatID. The [official UCS
resources](https://universalcategorysystem.com/) also include a spreadsheet of
categories and synonyms.

## Name items, then export in REAPER

Apply this workflow in [Assignment 4: SFX Editing and Processing](/assignments/assignment-4-sfx-editing/). Assignment 3 requires original recordings, named source tracks, and a recording log.

For individual field recordings, use one finished media item per exported sound.
If a bed contains several edited items, glue the finished bed into one item before
naming it, or use a named region around the complete bed. Name the item or region
before rendering.

1. Save an editing project with copies of your recordings. Keep the original
   recordings, including their slates, unchanged.
2. Listen to each slate and write a short description. Trim the slate and excess
   silence from the export item. Keep the full sound, including its natural
   decay, and add short fades where needed to prevent clicks.
3. Use UCS Finder to choose a CatID. Select an item, open **Item properties**
   with **F2**, and set the active take's **Take name** to the complete UCS name,
   without `.wav`. For example: `DOORWood_Creak Slow Interior 01_TC_DAD310`.
   Give each variation a unique number in the description block. Changing a
   take name does not rename the original audio file.
4. Select the finished items and choose **File > Render**. Set **Source** to
   **Selected media items** and **File name** to `$item`. This wildcard uses
   each item's active take name. Use the **Wildcards** button to insert it.
   REAPER adds the file extension from the chosen output format.
5. Render to a separate library folder using the assignment's WAV settings.
   For a mixed batch, set **Channels: Stereo** and enable **Tracks with only
   mono media to mono files**. Keep mono details and stereo beds on separate
   source tracks, and check the output channel counts. Stereo source files or
   stereo effects need an explicit channel check; render separately if needed. Use **Selected media items via master**
   if the export needs your track, bus, or master processing; check that routing
   and effect tails are included as intended.
6. Use the render window's file list or **Dry run** to check names and the number
   of exports before rendering. Resolve duplicate names instead of overwriting
   another recording.
7. Listen to the exported WAVs, check their beginnings and endings, and find
   them by searching their CatIDs and descriptions.

For a sound built from several layered items, make a named region around the
complete sound and render the region with `$region`. An item export is best for
one recording; a region export keeps a layered sound together.

Save a render preset once the settings are correct so you can reuse the workflow.
The filename and embedded metadata are separate: naming a take does not by
itself add a description or keywords to the exported WAV's metadata.

## Metadata

The filename remains visible when a recording moves between operating systems,
DAWs, and storage locations. Library software can also search metadata embedded
in the file, including descriptions and keywords. Use the slate at the start of
each take when writing that description instead of relying on memory.

Name and tag recordings on the day you make them, while the details are still
fresh.

## Project hygiene

Apply the same organization to your REAPER sessions:

- Save projects with "create subdirectory" and "copy media into project" on, so
  each project folder contains its media.
- Name tracks before recording. The recorded files will inherit those names
  instead of untitled numbers.
- Keep your finished exports in one master library folder and give them UCS names.
  Clear filenames reduce the need for deep folder trees.
- Edit copies in project folders and leave the library originals untouched.

{{< drill label="Lab: organize your recordings" >}}
Use your finished Assignment 4 edits made from the five Assignment 3 sources.

1. Use UCS Finder to choose a CatID for each finished sound.
2. Name each finished item's active take in the full pattern, with your initials
   as CreatorID and DAD310 as SourceID. Export the selected items using `$item`.
3. Use the slate and recording log to check that each filename describes the sound accurately.
4. Put the finished exports in one library folder. Find each sound with search rather
   than by browsing through folders.
{{< /drill >}}

## Reference

- [UCS Finder](https://www.ucs-finder.com/), searchable categories, explanations,
  and synonyms with copyable CatIDs
- [REAPER User Guide](https://www.reaper.fm/reference.php), item properties,
  rendering, and filename wildcards
- [Universal Category System](https://universalcategorysystem.com/), the
  official site with the category list and full documentation
- [UCS categories in BaseHead](https://baseheadinc.com/kb/ucs-categories/)
- [UCS support in
  Soundminer](https://store.soundminer.com/blogs/news/ucs-universal-category-system)
- [SoundQ](https://www.prosoundeffects.com/soundq), including its UCS support
- [Understanding the
  UCS](https://www.spencerbruce.com/blog1/2025/10/3/understanding-the-universal-category-system-ucs),
  a readable walkthrough
