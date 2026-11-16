---
title: "Explosion SFX"
---

We'll build an explosion in REAPER and compare versions as we add each layer. Listen for what makes the blast sound heavy, what gives it an electrical character, and how close it seems to the camera.

This is an instructor demo followed by workshop practice. There is no separate submission or grade, and you do not need to add an explosion to Assignment 6.

## Watch the clip

<video controls muted playsinline preload="metadata" style="width:100%;max-width:960px;">
  <source src="/videos/charge-explosion-demo.mp4" type="video/mp4">
  Your browser does not support embedded video. Use the download link below.
</video>

[Download the silent demo clip](/videos/charge-explosion-demo.mp4) · [Watch the full film](https://www.youtube.com/watch?v=UXqq0ZvbOnk&t=73s)

This 20-second excerpt from Blender Studio's *CHARGE* runs from **1:13 to 1:33** in the full film. A battery bursts, an electrical blast fills the factory, fragments fly, and the confrontation continues through several camera cuts. Along with the initial burst, we can design the fragments flying past, hitting surfaces, and settling around the characters.

Use impacts and rumble for the main blast, with crackling sounds for the electrical discharge. The smaller battery rupture and later weapon sounds should be distinguishable from that blast.

*Footage credit: CHARGE, Blender Studio, 2022. [Source and download](https://commons.wikimedia.org/wiki/File:Charge_-_Blender_Open_Movie-full_movie.webm), [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). This classroom adaptation extracts 1:13–1:33, removes the original audio, and converts the video to MP4.*

### Spot the sequence

Watch silently before opening the sound library. These ranges are approximate positions in the **downloaded excerpt**, starting at 0:00. Find the exact frames in REAPER.

| Part of the excerpt | Events to spot | Sound-design decisions |
| --- | --- | --- |
| 0:00–0:05 | The battery moves through the air and ruptures; the camera cuts to the robot. | Give the moving battery and its rupture separate sounds. How can the rupture sound smaller than the blast that follows? |
| 0:05–0:12 | Flashes and sparks lead into the electrical blast; fragments fly past the character and machinery. | Give the blast a clear attack and body. Pick two visible fragments and time a pass-by or impact to each one. |
| 0:12–0:20 | The robot moves and fires; the character reacts as the confrontation continues. | Let the blast fade enough to hear the machinery and later attacks. Keep its reverb tail audible across the cuts. |

For today's demo, concentrate on the main blast and two debris events. Leave the rest of the soundtrack unfinished.

## What to listen for

By the end of the session, you should be able to:

- Identify the attack, body, texture, and decay of a layered effect, and explain what each contributes.
- Compare pitch shifting with playback-rate changes and describe their effect on pitch and duration.
- Adjust the balance and reverb to make an effect sound closer or farther away.

## Before class

Download the clip and check that it plays in REAPER. Put it a few seconds into the timeline, leaving room before the burst and after the picture ends. Mute any source audio. Choose a few sounds from SoundQ or your own recordings before class so we have time to edit them during the demo.

Create folders named **Punch**, **Rumble**, **Electrical texture**, **Debris**, and **Tail**, plus a muted **Video** track. Prepare a few metal hits, scrapes, and small rattles for the fragments. Keep any existing factory ambience separate from the foreground effects. Start at a comfortable playback level and leave room on the master for additional layers.

## Demo and workshop, 50 minutes

### 1. Spot the event, 5 minutes

Watch silently and mark the battery rupture, main blast, two debris events, and one later mechanical action. Ask the class which event should be loudest and what we should hear after it. Follow one fragment from flight to impact. If it lands offscreen, try adding a landing sound and decide whether to keep it.

### 2. Build the attack and body, 12 minutes

Start with one short impact on the Punch track. Try a heavy metal hit or a snare. Trim and fade it, then align its onset with the chosen attack marker.

Add a low, longer sound on Rumble. Listen to the punch alone, the rumble alone, and both together. Ask: **What did the second layer add?** If the answer is only loudness, lower it or try another source. The punch should still be easy to hear with the rumble playing.

Save this two-layer version for comparison.

> **REAPER: place and trim a hit**
>
> Select the item and press **S** at the edit cursor to split it. Delete unwanted sections. Toggle **Options → Snap/grid → Enable snapping** off for fine alignment. Drag the item's upper corners inward to add short fades; keep the attack intact.

### 3. Compare pitch and duration, 8 minutes

Duplicate one source for an A/B comparison. Lower its pitch with duration preserved. On the other copy, reduce playback rate with pitch preservation disabled, so pitch and duration change together. Audition each separately against the picture at similar perceived loudness.

Ask students which version fits the main blast and what they hear that supports their choice.

> **REAPER: pitch versus playback rate**
>
> Select one audio item and press **F2** for Item Properties. Compare these settings on separate copies:
>
> - **Pitch adjust: −6 semitones; Playback rate: 1.0** lowers pitch without changing duration.
> - **Playback rate: 0.5; Preserve pitch when changing rate: unchecked** drops pitch an octave and doubles duration.
>
> Recheck sync after changing rate.

### 4. Follow the debris, 8 minutes

Add an electrical crackle or processed texture around the main blast. Use its volume envelope to follow the discharge, then lower the level if it masks the punch.

Now build two debris events. Start with a short movement or pass-by, followed by a metal impact where the fragment hits. Add a quieter bounce or rattle if the action calls for one. Vary the timing and pitch so the pieces do not sound like copies. Keep the main attack louder than the debris, with the smaller hits audible as the blast fades.

Compare **blast only** with **blast plus debris** at similar loudness. Ask: **Which sounds tell us that objects have been thrown into the room?** Mute the debris folder again and listen for what disappears.

> **REAPER: move one fragment**
>
> Select its item, open **F2 → Take envelopes**, and enable **Pan**. Shift-click the envelope to add points, then drag them up or down to set left or right pan positions. Keep movement modest. Take envelopes affect this item, so other fragments on the track stay put.

### 5. Add room reverb, 7 minutes

Compare the dry effect with the same sounds sent to a room reverb. Use a shared reverb send for the blast and debris, adjusting each send to suit its distance. Try reducing high-frequency detail on a farther impact. Pan selected fragments to follow their visible paths without moving the whole blast with them.

Play across a camera cut. Does the tail continue, or does it disappear as though the room has changed? Let the decay carry across the cut while making room for the robot's next movement and weapon sound. Ask students which event now draws their attention and why.

> **REAPER: share one factory reverb**
>
> Create a track outside the effects folders named **Factory reverb**. Add **ReaVerbate** through **FX**; set **Dry** to **−inf** and **Wet** to **0 dB**. On each source folder, open **Route → Add new send → Factory reverb**. Start with low send levels and raise them until you hear enough reverb. Mute the return to compare dry and reverberant versions.

### 6. Try one change, 8 minutes

Use the supplied sounds to change the weight of the blast, the debris, or the distance. You can also try these techniques on another foreground effect in your own footage.

Before making the edit, tell your partner what you expect to hear. Compare the two versions at similar loudness, then discuss what improved and what still needs work.

### 7. Exit check, 2 minutes

Name one layer you would keep and explain its job. Then describe one technique from this demo you could use in your final project, and where you would use it.

## Listening checklist

- Does the attack land on the intended visual event?
- Can you hear what each layer contributes when you mute and restore it?
- Do the debris contacts follow the picture, and does the decay carry the factory space across cuts?
- Do edits play cleanly, with no unintended clicks or master clipping?
- Does your revision still work when compared at similar loudness?

## Further study

The [original sound-design tutorial](https://www.youtube.com/watch?v=TdktuXuYkjg) is an optional process reference. Ric Viers's *The Sound Effects Bible* is further reading on sound-effects recording and design. Try a technique on the clip, then listen before and after to decide whether to keep it.

REAPER controls are described in the [REAPER User Guide](https://dlx.reaper.fm/userguide/html/), under media item properties, take envelopes, and track routing.
