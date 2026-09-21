+++
title = "Spotting, Cueing, and Editing Foley"
outputs = ["Reveal"]
[reveal_hugo]
# show_notes = "separate-page"
+++

## Spotting, Cueing, and Editing Foley

This lesson follows Vanessa Theme Ament, *The Foley Grail*, 3rd ed., ch. 4 and 5.

{{% note %}}
The process starts before anyone steps on a stage. In a spotting session, the supervising Foley editor sits with the supervising sound editor, the director, and the picture editor to break down each scene, set the film's sonic style, and divide the work between library effects and performed Foley. The editor then maps every cue into a session, and that map is what makes the stage day efficient.

Ament's benchmark is worth quoting to students: an experienced editor takes about four hours to cue ten minutes of film. Cueing is real editorial work, not clerical prep.
{{%/ note %}}

---

<img src="script.png" width=500>

{{% note %}}
What the spotting session decides:

- Who attends: the supervising sound editor, the director, and the picture editor, sometimes joined by the ADR supervisor or the Foley supervisor.
- What gets settled: which sounds will be performed as Foley, which come from libraries, and what style the film's sound should have.
- Why it survives budget pressure: a planned session saves real money at the final mix, because problems get solved on paper instead of on the stage clock.
{{%/ note %}}

---

![](cue-session.png)

{{% note %}}
Ament's track layout, which is still the standard shape of a Foley session:

- Principal footsteps go first, one character per track for the whole reel: Mimi on track 1, Joe on track 2, and so on.
- Background footsteps follow, tagged so the artist can find the person instantly on screen: "tall man, blue shirt, right to left" or "two girls running center."
- Props group by what Ament calls food groups: paper together, metal together, hand pats together, leather together. The mixer can then set the microphone once per texture instead of once per cue.
- A single cloth pass sits on its own track at the end. The re-recording mixer tucks cloth under the dialogue, and cloth spread across several tracks turns into an unusable whoosh.

Cue sheets used to be handwritten in vertical columns; the same layout now lives horizontally in a DAW timeline, and cue sheets can still be printed from the session.
{{%/ note %}}

---

## Cue with a breath

- Play the lead-in so the artist can anticipate the action.
- Mark the exact sync point separately from recording boundaries.
- Keep continuous movement together across picture cuts.

{{% note %}}
- Ament's lead-in and continuous-performance principles come from ch. 5: the artist performs a scene, not a list of timestamps.
- This is also why Foley cueing is looser than ADR cueing, which must hit lip-sync exactly.
- In our REAPER lab, an empty cue-map item includes preparation and decay, while a named marker identifies the exact contact or action to synchronize. A three-beep count-in lands its silent fourth beat at that marker. Normal recording begins before the count-in and continues after the action. Do not shift the intended sync point earlier just to create a lead-in.
{{%/ note %}}

---

## Two stories worth knowing

- *The Turning Point*: Jerry Trent recreated Baryshnikov's dance sounds, even while sitting down.
- *The Godfather Part II*: Murch and Berger walked real marble stairs, keeping time with a flashing metronome.

{{% note %}}
- Jerry Trent was hired to Foley Mikhail Baryshnikov's dancing in *The Turning Point* (1977). The film's choreographer doubted a Foley artist could match the steps. Trent's answer: "I don't have to do the same steps, they just have to sound like the steps. I can do most of this sitting down."
- For *The Godfather Part II*, Walter Murch and mixer Mark Berger skipped the Foley stage entirely. They calibrated a metronome to the film's frames per footstep, set it to flash instead of click, and walked real marble stairs in San Francisco in sync with the silent light.
- The Trent story teaches the foundational Foley truth: the job is the sonic illusion, not literal reenactment.
- The Murch story teaches the opposite lesson: sometimes the illusion requires the real place, real marble, and real architectural reflections. Both stories are in Ament, ch. 1 and 8.
{{%/ note %}}

---

## Cuing process

<style>
/* Reserve space for the wide monospace numerals inside the slide edge. */
.reveal #cuing-process ~ ol {
  margin-left: 0;
  padding-left: 2em;
  box-sizing: border-box;
}
</style>

1. Watch the scene several times before cueing.
2. Main characters first: one track per character and surface.
3. Background characters next: label their direction.
4. Props last: group similar materials together.

{{% note %}}
- Add tracks when a character's walk crosses different surfaces.
- Identify background characters with descriptive direction tags rather than names.
- Group props by Ament's "food groups" so the mixer can record similar textures in sweeps without resetting the microphone for every cue.
- Precision with conciseness: if multiple men carry children in a scene, "man carrying child" fails and the cue must say which man.
- The end goal is a road map that lets the artist, the mixer, and the editor work the stage day without stopping to ask questions.
- Source: Ament, ch. 5.
{{%/ note %}}

---

## Set up the session

- 48 kHz / 24-bit WAV; Time timebase.
- Match the video frame rate; show a timecode ruler.
- Lock picture at 10 seconds; silence its audio.
- Save the project and media in one folder.

{{% note %}}
Demonstrate in the shared A Quiet Place project on the studio computer. The instructor prepares the video and project settings before class. Match the frame rate to the imported clip and set the end marker to its actual end.

Review VIDEO, CUE BEEPS, CUE MAP, and the footstep, prop, and cloth recording tracks. Keep cue notes separate from recorded audio. Students help build the cue map; they do not need their own REAPER projects for this activity. The robot starter and its 30 fps settings are for Assignment 2.
{{%/ note %}}

---

## Three beeps, then perform

- Hear three evenly spaced beeps.
- Enter on the silent fourth beat.
- Our practice: beeps at 7, 8, 9 seconds; enter at 10.
- Use headphones; mute beeps before mixing.

{{% note %}}
Use one-second spacing as our classroom convention. Start playback at 6 seconds. The three-second audio item contains all three beeps; its right edge and snap offset mark the silent fourth beat. For a cue at T, position the item at T minus 3 seconds without changing its length or rate. Keep one count-in active at a time. First rehearse an entrance, then apply it to a spotted action. The starter's practice item is not a finished cue map.

Stage methods can use different intervals or visual streamers. The count-in prepares the entrance; the performer follows picture after it. A 2-pop is a separate synchronization reference, not this three-beep count-in.

The starter routes beeps through the master for headphone practice. At a studio with a separate headphone output, route beeps there and turn off their master send. Keep speakers off during microphone recording, check headphone spill, and record the microphone input rather than loopback.

Sources: [Solange Schwalbe on Foley cueing](https://www.production-expert.com/production-expert-1/mastering-foley-insights-from-solange-schwalbe); [one-second ADR count-in example](https://www.crashsymphony.com.au/adr-studio-sydney/).
{{%/ note %}}

---

## Spot A Quiet Place together

- Identify actions and choose props for the scene.
- Label each cue and mark its exact sync point.
- Plan separate recording passes by material.
- Rehearse one entrance with the three beeps.

{{% note %}}
Use the [REAPER spotting guide](/lectures/week-5/reaper-spotting/) alongside the [shared studio activity](/lectures/week-4/recording-foley/#a-quiet-place-in-class-spotting). The instructor operates REAPER while students identify and describe cues. Each cue note needs an ID, object/action, material, destination track, sync time, and performance direction.

Keep sustained movement together and allow decay after impacts. Cue notes stay on CUE MAP while audio is recorded on the named layer tracks.

End September 23 with a saved shared cue map and one successful rehearsal. September 25 demonstrates recording in this project; October 2 is the class Foley recording session. September 30 demonstrates editing with A Quiet Place takes from the recording demo. Students complete their robot spotting, recording, and editing outside class for Assignment 2.
{{%/ note %}}
