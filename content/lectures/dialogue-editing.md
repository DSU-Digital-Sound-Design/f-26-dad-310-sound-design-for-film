---
title: "Dialogue Editing"
summary: "Record two takes, comp the strongest words and phrases, and preserve natural timing and room sound."
tags: [dialogue, editing, post-production, room tone]
---

## Project instructions

**Goal:** combine the strongest words and phrases from two takes into one believable conversation. This revisits comping from your Audio Production I satirical PSA.

Work in pairs using a **portable Zoom recorder, headphones, and REAPER**. Follow the steps below in class. This is audio-only practice with no separate graded submission; Friday's [ADR lab](/lectures/adr/) adds synchronization to picture.

Your finished work should include:

- A complete comp using at least three selected passages from both takes.
- At least one word or phrase replacement within a spoken line, with smooth joins at both ends.
- Natural delivery and timing, with continuous room sound.
- One saved REAPER project containing the comp, untouched original recordings, and a two-sentence editing note.

## 1. Record the practice passage

**0–15 minutes**

Perform this exchange from *Night of the Living Dead* (1968). Johnny teases his sister Barbra; she becomes increasingly uneasy. Take one role each and aim for about 45–60 seconds.

> **Johnny:** Do you remember one time when we were small, we were out here? It was from right over there. I jumped out at you from behind the tree. And grandpa got all excited, and he shook his fist at me, and he said, “Boy, you'll be damned to hell.” Remember that? Right over there. Well, you used to really be scared here.
>
> **Barbra:** Johnny.
>
> **Johnny:** Well, you're still afraid.
>
> **Barbra:** Stop it now. I mean it.
>
> **Johnny:** They're coming to get you, Barbra.
>
> **Barbra:** Stop it. You're ignorant.
>
> **Johnny:** They're coming for you, Barbra.
>
> **Barbra:** Stop it. You're acting like a child.

1. Find a quiet spot around the building or outside, **out of hearing distance of other student groups**. Avoid nearby conversations, intermittent loud noises, and wind hitting the microphone. If you can hear another group performing, move farther away. Place the Zoom on a stand or stable surface and check recording level and microphone placement with headphones.
2. Record **two complete takes**. Keep the speakers, microphone, and gain in the same positions and settings. Try small differences in emphasis or pauses in Take B. Avoid overlapping speech.
3. Leave a few seconds of quiet before and after each take. Then record **30 seconds of room tone** with nobody speaking, moving, or handling the recorder.
4. Listen back before leaving. Redo a take if speech is clipped, interrupted, or unclear.
5. Copy the files to a folder on your computer. Name the copies `Take_A`, `Take_B`, and `Room_Tone`, retaining their file extensions. Keep the recorder files until you have checked the copies.

## 2. Organize the session

**15–23 minutes**

1. Create a new REAPER project. Import each recording onto its own track and name the tracks `ORIGINAL_A`, `ORIGINAL_B`, and `ORIGINAL_TONE`.
2. Use **Save project as** to name the project `Dialogue_Comp`. Enable **Create subdirectory for project** and **Copy all media into project directory**. Keep the full original audio items untouched and **mute all three ORIGINAL tracks**.
3. Create **three new working tracks** named `DIALOGUE_A`, `DIALOGUE_B`, and `FILL`. Copy Take A's audio item to `DIALOGUE_A`, Take B's to `DIALOGUE_B`, and the room-tone item to `FILL`. Mute `FILL` for now.
4. Turn ripple editing off. Audition `DIALOGUE_A` and `DIALOGUE_B` one at a time, muting the other. Mark at least three preferred words or phrases across the two takes, with a brief reason for each choice.
5. Choose one dialogue track as your base performance. Leave it audible and mute the other dialogue track. Save the project. Keep the ORIGINAL tracks muted and untouched for comparison.

## 3. Prepare room-tone fill

**23–27 minutes**

1. On the `FILL` track, select a short clean section without speech, breaths, clicks, or handling noise. Keep only this section on the working track; the full recording remains on `ORIGINAL_TONE`.
2. Leave `FILL` muted and continue to Step 4. You will place tone only where the comp needs it.

Keep the background already present in speech and pauses. Use the separate tone to fill holes created by editing, rather than adding another layer beneath the whole scene. See the room-tone explanation below for more detail.

## 4. Build the dialogue comp

**27–45 minutes**

Keep the script's words and order.

1. Compare a preferred phrase from the alternate take with the base performance. Decide what it improves: delivery, clarity, or timing.
2. Split around that phrase on the alternate working track, leaving small handles of surrounding audio. Copy the selected item.
3. On the **base working track**, split around the words to replace and delete only that working section. Select the base track, place the edit cursor at the start of the gap, and paste the copied phrase. Keep the ORIGINAL tracks untouched and the alternate dialogue track muted.
4. Fit the replacement by ear. Adjust its position and the neighboring pauses without clipping consonants, doubling words, or disrupting natural breaths.
5. Enable **Auto-crossfade** on the toolbar. Make short overlaps at both ends of the replacement and adjust each fade while listening. If a word sounds pasted in, try a larger phrase.
6. Match small level differences with item gain. If an edit leaves a background gap, copy your prepared tone to that position on `FILL` and trim it to length. Overlap its edges with quiet audio on either side of the gap, then drag the item fade handles to crossfade the backgrounds. Remove any unused tone items from `FILL` and unmute it. Listen for a continuous background without a dip or swell.
7. Repeat for your other selections. Include at least one replacement **within** a spoken line. Label selected items or add notes identifying their source take and your reason for choosing them. Save the project.

## 5. Listen and finish

**45–50 minutes**

1. Play the comp for another pair without showing edit locations. Ask whether the words are clear, the delivery and pauses feel natural, and the background stays continuous.
2. Compare with the original base take: mute `DIALOGUE_A`, `DIALOGUE_B`, and `FILL`, then unmute only the corresponding ORIGINAL track. Afterward, mute that ORIGINAL track and restore the comp playback.
3. Revise any specific problem the comparison reveals. Replay the whole scene, then save and check that the project reopens with all media.
4. Point out your three selections, including the replacement within a line. Write **two sentences** explaining one performance choice and one continuity adjustment. Keep a clean full take for the November 4 [worldizing lab](/lectures/worldizing-and-futz/).

If your recording or file transfer fails, ask another pair to share its takes and matching room tone. Credit the recording pair in your notes.

---

## Explanation and reference

The sections below support the project. They are not additional required tasks.

### Choosing words and phrases

Comping builds one performance from selected parts of several takes. Try combining the opening of Johnny's speech from one take with a stronger later phrase from the other, or replacing the ending of Barbra's response.

A word must fit the surrounding pitch, stress, and pronunciation. If an isolated word sounds unnatural, expand the selection to a phrase or breath group. Preserve complete consonants and natural breaths. Choose by listening, not just by waveform appearance.

### Why room-tone fill goes in gaps

The Zoom records the room along with the voices. Preserve that background wherever it already works, including pauses. Crossfade matching fill into any holes created by editing so the **total background stays continuous**. Audible pumping, swells, or dropouts mean the matching, levels, or fades need adjustment.

Purcell recommends avoiding unnecessary simultaneous room-tone layers. Adding a second layer beneath a dialogue item can raise the background rather than fix its mismatch. Start with tone from the same take or recording setup. FX-project room tones are alternatives only if they match by ear.

Select tone manually for this exercise. Dynamic Split's silence-removal settings can discard the quiet material you need. Do not repeatedly loop a tiny fragment if its pattern becomes audible.

### Fade shapes

Equal power can suit unrelated background material; equal gain can suit aligned, identical audio. At the midpoint of a symmetrical crossfade, each source is about −3 dB for equal power or −6 dB for equal gain. These are individual source gains, not guaranteed dips in the combined sound.

Use REAPER's crossfade editor to adjust curves. Source correlation and timing affect the result, so listen for a click, dip, swell, doubled word, or weakened consonant.

### Optional noise repair

Apply the [LISTEN checklist](/lectures/week-7/listen-mantra/) and [REAPER cleanup techniques](/lectures/week-7/editing/) only where needed. For a click **between words**, replace the affected interval with matching tone and crossfade both sides without shortening the passage.

Replacing noise that overlaps speech with tone would also remove the voice. Try another performance instead. Keep noise reduction restrained and compare with the original at similar loudness. Stop if the voice becomes thin, metallic, or unstable.

### Later work with picture

Dialogue editing to picture also requires synchronization and perspective matching. Separate tracks by source, character, or perspective when the mixer needs independent control. Audio transitions can fall away from picture cuts while dialogue remains synchronized. Friday's ADR lab practices recording a replacement performance to picture.

### Script and sources

- [*Night of the Living Dead* dialogue transcript](https://www.springfieldspringfield.co.uk/movie_script.php?movie=night-of-the-living-dead). Speaker labels and punctuation added for this exercise.
- [Library of Congress: the original 1968 film's U.S. public-domain status](https://blogs.loc.gov/copyright/2020/10/copyright-horror-stories/).
- John Purcell, *Dialogue Editing for Motion Pictures: A Guide to the Invisible Art*, on room tone, transitions, track organization, and alternate takes.
- [REAPER User Guide](https://www.reaper.fm/userguide.php), on fades, crossfades, and Dynamic Split.
- [Dialog editing with room tone](https://reaper.blog/2015/03/video-dialog-editing-with-room-tone/), a REAPER-specific walkthrough.
