---
title: "ADR: Replacing a Line to Picture"
summary: "How dialogue gets re-recorded in a studio and fitted back into the film so no one can tell."
tags: [ADR, dialogue, recording, post-production]
---

ADR (automated dialogue replacement, also called looping) re-records a line in a
studio and fits it back to picture. It can replace dialogue affected by radio mic
breakup, rain on the zeppelin, or other location problems. Productions also use
ADR for performance or script changes, lines added over off-camera moments,
group walla, and TV-safe alternates.

The notes below follow Purcell's *Dialogue Editing for Motion Pictures*. In class,
we will replace lines from the same *Night of the Living Dead* scene you practiced
in the [dialogue recording lab](/lectures/dialogue-editing/).

## Spotting and cueing

ADR is spotted after picture lock. Each line gets a searchable cue code built
from the character and reel, such as REB 309 for Rebecca, reel 3, cue 9.

Break long lines into sections the actor can perform comfortably. Purcell
recommends placing breaks:

- at the end of a sentence
- at a breath, which gives the actor a natural reset
- at an inflection, where the pitch or emphasis shifts

## The session

The actor watches the scene and hears three beeps. A streamer wipes across the
screen, and on the imaginary fourth beep the guide track mutes and the actor
delivers the line. Expect many takes. The recordist keeps a log of every take,
marking the holds worth keeping and the buy, which is the selected take.

Actors may become frustrated while trying to match their original performance.
Keep the session patient and concentrate on the line's pitch, rhythm, and
emphasis rather than its words. If an actor gets stuck, ask them to close their
eyes and listen to the guide track or trace the rhythm with nonsense syllables.
If a cue still does not work, move on and return to it later.

Purcell notes that a take can look synchronized and still sound wrong if the
actor stresses a different syllable than in the production take. "How NOW brown
cow" will not match footage of "how now, BROWN cow." Check the stress pattern as
well as the lip movement.

## Matching the room

The studio take needs to match the location recording. Make that match during the
recording session rather than relying on processing later.

- Check the sound report for the production microphone. Use the same model, or
  the closest available option, at the same distance and angle as the original
  boom or lav.
- Match the space. ADR stages have live and dead areas; pick the one closer to
  the scene's acoustics.
- Run Purcell's in-session test early. Record one line, synchronize it, add
  production room tone around it, and play the transition in context. If the
  sound changes noticeably, adjust the microphone or room before recording the
  remaining lines.

## Fitting the line

Trim the selected take, leaving a little audio before and after the line for fades and timing adjustments. Align it using the same techniques used
for alternate takes in the [dialogue editing
lesson](/lectures/dialogue-editing/): work in blocks of three or four words,
anchor on hard consonants, and place internal edits within sibilants. Do not cut
inside a vowel because the splice may click or phase.

If manual editing is not enough, stretch only the words that need it, and keep
an untouched, synchronized copy on a work track. Use alignment software such as
VocAlign only after editing the cadence by hand. Processing a poorly synchronized
line can damage its sibilants.

Two practices carry over from the dialogue lesson:

- Keep the original line. Edit it fully and leave it synchronized on a muted
  safety track so the mixer can compare or restore it.
- A studio take is drier than a location recording. Place room tone under the ADR
  to maintain the scene's background. Leave the final EQ and reverb matching for
  the mix session, where you can make those decisions on the mix monitors.

## Cueing tools in REAPER

Professional cueing tools include [Viper](https://www.vennaudio.com/our-new-plugin-viper/), which provides a visual cue line, and [Rythmoband](https://www.extremraym.com/en/downloads/reascripts-pack-rythmoband/), which provides scrolling dialogue text in REAPER.

For this class, use [DAD 310 ADR Cue](https://github.com/tatecarson/reaper-adr-cue), the tool I built to prepare, rehearse, and record your line to picture in REAPER. Download, installation, and usage instructions are on GitHub.

## Practice scene

*Night of the Living Dead* (1968), the cemetery exchange from our dialogue lab.

<video controls preload="metadata" poster='{{< rel "downloads/notld-cemetery-adr.jpg" >}}' width="640" height="480" style="width: 100%; max-width: 640px; height: auto;" aria-label="Night of the Living Dead cemetery dialogue excerpt">
  <source src='{{< rel "downloads/notld-cemetery-adr.mp4" >}}' type="video/mp4">
  Your browser does not support embedded video.
</video>

### Separated audio

Download the dialogue-free video and dialogue WAV below. In REAPER, align their starts and use the dialogue track as the rehearsal guide.

<video controls preload="metadata" poster='{{< rel "downloads/notld-cemetery-adr.jpg" >}}' width="640" height="480" style="width: 100%; max-width: 640px; height: auto;" aria-label="Cemetery scene with dialogue removed">
  <source src='{{< rel "downloads/notld-adr/notld-cemetery-dialogue-free.mp4" >}}' type="video/mp4">
  Your browser does not support embedded video. Use the download link below.
</video>

<a href='{{< rel "downloads/notld-adr/notld-cemetery-dialogue-free.mp4" >}}' download>Download the dialogue-free scene (MP4)</a>

- [Dialogue WAV](/downloads/notld-adr/dialogue.wav): use as the guide in ADR Cue.

<details>
<summary>Optional audio files</summary>

- [Background WAV](/downloads/notld-adr/background.wav)
- [Original soundtrack WAV](/downloads/notld-adr/original-guide.wav)
- [Music WAV](/downloads/notld-adr/music.wav)
- [Effects WAV](/downloads/notld-adr/effects.wav)

</details>

The video already includes the background; no extra background track is needed. All files share the same start time. The separation may leave faint voice remnants or alter some effects.

## Script and cue breaks

Use the [practice passage from the dialogue lab](/lectures/dialogue-editing/#1-record-the-practice-passage), reproduced below. Follow the film for the exact wording and delivery.

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

### Divide the script

Record one short speaker turn at a time. For Johnny's opening speech, split at these pauses:

- After “It was from right over there.”
- After “Boy, you'll be damned to hell.”
- At the end of the speech.

Short sections are easier to rehearse and match to picture.

Within a section, use `|` to divide the scrolling text into phrases you can align separately to the original dialogue. This gives the performer timing cues throughout the line:

`Do you remember one time when we were small, | we were out here? | It was from right over there.`

Adjust each phrase's timing to the film. Record the whole section in one take; `|` does not cut the audio.

{{< drill label="Lab: replace the cemetery dialogue together" >}}
**Goal:** match a new performance to the original actor's timing, phrasing, and lip movements.

Work together on the studio computer.

### 1. Install and listen · 10 minutes

1. Follow the [ADR Cue installation instructions](https://github.com/tatecarson/reaper-adr-cue) and confirm that the tool opens on your computer.
2. Watch the embedded scene above together. Listen for entrances, pauses, emphasis, and breaths.
3. Choose a cue using the [script guidance above](#divide-the-script).

### 2. Prepare the shared session · 5 minutes

1. Import the dialogue-free video and dialogue WAV onto separate REAPER tracks. Align both starts at ten seconds, open the video window, and save the project with its media.
2. Set the dialogue track as the guide in ADR Cue. Leave the video's background audio audible during rehearsal and recording.
3. Select the cue's time range and click **New line**. Enter and align the phrases using the guidance above. Check the result with **Rehearse**.

### 3. Rotate through the session · 25 minutes

Take turns as **performer**, **ADR Cue operator**, and **director/take logger**.
The rest of the class listens and offers specific feedback. Rotate roles after each short round.

1. The performer rehearses with the original line and picture.
2. The operator checks the microphone input and level, then uses **Record** for two or three takes. Confirm that the guide silences during the line. Monitor through headphones.
3. The director gives one concrete adjustment, such as an earlier entrance, a shorter pause, or a different stressed word. Log the performer and preferred take.
4. Replay with picture, then rotate roles. Try the same cue again or choose another.

### 4. Fit and compare · 10 minutes

1. Choose a take together. Split the dialogue-guide item around the replaced line and mute that section. Keep the video's background audio playing beneath the new take.
2. Fit the take using the [editing guidance above](#fitting-the-line).
3. Compare by alternating the guide section and the replacement, playing one at a time. Do the words fit the mouth movements? Identify one successful match and one remaining problem.
4. Save the shared session. Everyone contributes through a session role or listening feedback. No separate submission.
{{< /drill >}}

### Scene notes

Source: [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Night_of_the_Living_Dead_(1968).webm), approximately **5:43–6:22**, with extra time around the excerpt.

Match timing and phrasing; you do not need to imitate the actor's voice. Focus on performance and sync before final EQ and reverb.

Check the video's background for voice remnants or missing effects at the edit.

## Reference

- John Purcell, *Dialogue Editing for Motion Pictures: A Guide to the Invisible
  Art*, ADR chapters
- [Viper](https://www.vennaudio.com/our-new-plugin-viper/), a streamer and beep
  plugin with a free trial
