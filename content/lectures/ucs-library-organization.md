---
title: "Naming Sounds: UCS and Library Organization"
summary: "The Universal Category System, embedded metadata, and the habits that make a recording findable a year later."
tags: [UCS, metadata, library, organization, field recording]
---

A recording you cannot find does not exist. Five field recordings are easy to
track. Five hundred are not, and working sound editors search libraries of
hundreds of thousands. The industry's answer is a shared naming standard, and
adopting it now means every sound you record this semester goes straight into a
library you can still use in ten years.

## The Universal Category System

The [Universal Category System](https://universalcategorysystem.com/) (UCS) is
a free, public standard for naming sound effects. It defines 82 main categories
and 753 subcategories, each with a short category ID, and a filename pattern
built from four blocks separated by underscores. Search tools like Soundly,
SoundQ, Soundminer, and BaseHead all understand it, which is the point: a UCS
filename sorts and filters correctly in software you have not chosen yet.

The pattern is `CatID_FXName_CreatorID_SourceID`:

{{< stats >}}
{{< stat value="CatID" label="Category ID" note="From the official UCS list, such as DOORWood or WEATRain. Look it up; do not invent one." >}}
{{< stat value="FXName" label="Short description" note="A few words about the specific sound: Creak Slow Interior. Spaces are allowed inside this block." >}}
{{< stat value="CreatorID" label="Who recorded it" note="Your initials or a short handle. This follows your work everywhere it travels." >}}
{{< stat value="SourceID" label="Where it came from" note="The project, library, or session: DAD310 or ZOOMH4n." >}}
{{< /stats >}}

A door recording from your field assignment becomes:

`DOORWood_Creak Slow Interior_TC_DAD310.wav`

Underscores separate the blocks, so never use an underscore inside one. Find
the right CatID by searching the [official category
list](https://universalcategorysystem.com/); the download includes a
spreadsheet of every category with plain-language synonyms.

## Metadata

The filename is the metadata that survives everywhere: every OS, every DAW,
every file transfer. Search tools go further and index metadata embedded inside
the file, including a longer description and keywords. The slate you record at
the top of each take is the raw material for that description; when you name
and tag a file, transcribe the slate instead of trying to remember the take.

The habit that matters: name and tag recordings the same day you make them.
Every day between the recording and the naming deletes detail you will not get
back.

## Project hygiene

The session-side versions of the same idea, most of which you are already
doing:

- Save projects with "create subdirectory" and "copy media into project" on, so
  a project folder is complete and portable.
- Name tracks for what they carry, before recording, so the recorded files
  inherit sensible names instead of untitled numbers.
- Keep one master library folder for your own recordings, in UCS names. Deep
  folder trees matter less than good names; search beats browsing.
- Keep originals. Edit copies in project folders, and leave the library masters
  untouched.

{{< drill label="Lab: make your library real" >}}
Use your five Assignment 3 recordings.

1. Look up the correct CatID for each of the five on the official UCS list.
2. Rename each file in the full pattern, with your initials as CreatorID and
   DAD310 as SourceID.
3. Write a one-line description for each from its slate.
4. Drop all five into a single library folder and find each one by search
   alone, without opening a folder tree.
{{< /drill >}}

## Reference

- [Universal Category System](https://universalcategorysystem.com/), the
  official site with the category list and full documentation
- [Understanding the
  UCS](https://www.spencerbruce.com/blog1/2025/10/3/understanding-the-universal-category-system-ucs),
  a readable walkthrough
