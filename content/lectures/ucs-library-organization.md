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

Use underscores only to separate the four blocks. Find the appropriate CatID in
the [official category list](https://universalcategorysystem.com/). The UCS
download includes a spreadsheet of categories and plain-language synonyms.

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
- Keep your recordings in one master library folder and give them UCS names.
  Clear filenames reduce the need for deep folder trees.
- Edit copies in project folders and leave the library originals untouched.

{{< drill label="Lab: organize your recordings" >}}
Use your five Assignment 3 recordings.

1. Look up the correct CatID for each of the five on the official UCS list.
2. Rename each file in the full pattern, with your initials as CreatorID and
   DAD310 as SourceID.
3. Write a one-line description for each from its slate.
4. Put all five in one library folder. Find each recording with search rather
   than by browsing through folders.
{{< /drill >}}

## Reference

- [Universal Category System](https://universalcategorysystem.com/), the
  official site with the category list and full documentation
- [UCS categories in BaseHead](https://baseheadinc.com/kb/ucs-categories/)
- [UCS support in
  Soundminer](https://store.soundminer.com/blogs/news/ucs-universal-category-system)
- [SoundQ](https://www.prosoundeffects.com/soundq), including its UCS support
- [Understanding the
  UCS](https://www.spencerbruce.com/blog1/2025/10/3/understanding-the-universal-category-system-ucs),
  a readable walkthrough
