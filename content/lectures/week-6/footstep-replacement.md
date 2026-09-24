---
title: "Footstep replacement lab"
summary: "Film a short walk, spot the contacts, and record replacement footsteps together on the studio computer."
---

This is our optional October 2 lab if we have finished the shared *A Quiet Place* Foley session. The full process takes 50 minutes. If we begin partway through class, start with filming and spotting, then save our progress.

Students will film one short walking clip, then we will replace its footsteps together in one REAPER project on the studio computer. Use what we practiced in [spotting](/lectures/week-5/reaper-spotting/) and [recording Foley](/lectures/week-4/recording-foley/): identify the action, rehearse with picture, and record a performance that matches the force and rhythm of the steps.

By the end of class, we should have a short scene with replacement footsteps, two recorded takes to compare, and a saved project. We will make only the edits needed to check synchronization. [The editing lesson](/lectures/week-5/editing-foley/) covers editing and layering in more detail.

## A 50-minute session

| Class time | Task |
| --- | --- |
| 0–8 minutes | Film one short walk and return to the studio |
| 8–13 minutes | Transfer the clip and prepare the shared project |
| 13–21 minutes | Watch, spot, and describe the footsteps |
| 21–27 minutes | Choose the sound and rehearse |
| 27–39 minutes | Record and compare two passes |
| 39–46 minutes | Choose a take and adjust synchronization |
| 46–50 minutes | Watch the result and save |

## 1. Film one short walk · 8 minutes

Choose one person to walk and another to film on a phone. Make **one class clip**, about 8–12 seconds long, with six to eight visible steps on one surface near the studio.

- Hold the phone horizontally and keep the camera still.
- Keep the walker's feet visible, including where the shoes contact the floor.
- Leave a couple of seconds before the first step and after the last.
- Walk naturally. Avoid dialogue, stairs, doors, and other actions that would need extra sound passes.
- Keep the phone's original sound as a reference. We will mute it when playing the replacement.

Watch the clip before returning. Can you see the contacts clearly? If not, make one more attempt. Keep the route short and avoid filming bystanders or blocking the hallway.

## 2. Prepare the shared project · 5 minutes

Transfer the selected clip to the studio computer. Save it in a new folder for this lab and create a separate REAPER project there, keeping it separate from the *A Quiet Place* session.

Use the familiar 48 kHz / 24-bit recording setup and Time timebase. Import the clip onto a `VIDEO` track, place its start at 10 seconds, and keep its position fixed. Check that the picture plays before moving on. If using a timecode ruler, match it to this clip rather than assuming the robot video's frame rate.

Inside a `FOOTSTEPS` folder, add two tracks named for the actual footwear and surface:

- `WALKER - SNEAKERS - TILE - CUES`
- `WALKER - SNEAKERS - TILE - REC`

Use the three-beep item from the spotting template on a separate `CUE BEEPS` track. Keep cue items and recordings off the folder track itself.

Listen to the original once, then turn off the VIDEO track's master send so its sound does not play with the replacements. Keep the video visible.

## 3. Spot the walk · 8 minutes

Watch the clip silently, then describe the walk before choosing a sound:

- Do the steps look firm or gentle, hurried or relaxed?
- Is the pace steady, or does it change?
- Which contacts are easiest to identify in the picture?

On the `CUES` track, create an empty item for the walking sequence. Place its left edge on the first visible foot contact and extend it through the final step. Add a short note if the walk includes a pause or a change in how firmly the foot lands.

Step through the remaining contacts together and count the rhythm aloud. Keep the sequence as one performed pass rather than creating a separate recording for every step. The cue marks the entrance; the picture guides the rest of the walk.

## 4. Choose the sound and rehearse · 6 minutes

Try the footwear and an available surface in the recording area. Choose a sound that matches how the shoe contacts the visible surface. If the exact surface is unavailable, choose the closest useful sound and identify what differs.

Use the microphone placement from the recording lesson as a starting point. Select the microphone's mono input and arm only the `REC` track. Perform the loudest step while setting gain, keeping peaks below -6 dBFS. Record a brief test and listen for clipping or unwanted noise.

Move the three-beep item's right edge to the cue's left edge. Start playback before the first beep and rehearse the entrance on the silent fourth beat. After that, follow the feet rather than continuing at the beeps' spacing.

## 5. Record two passes · 12 minutes

Record the whole sequence in normal recording mode, starting before the count-in and leaving a little time after the final step. Keep the empty cue above the recording.

After the first pass, mute the beeps and watch it with picture. Describe one specific change for the next pass:

- A contact is early or late.
- The footstep impacts sound too forceful or too soft for the movement.
- The shoe or surface does not match the image.
- The rhythm is steady, but the person in the clip changes pace.

Make that change and record a second pass. Another student can perform the second pass while classmates watch for timing and character. Keep both takes and compare the same section of picture. If time remains, record a third pass to address the clearest remaining problem.

## 6. Fit the performance to picture · 7 minutes

Choose the take with the most convincing rhythm and character, then save a new project version before editing.

1. If the whole performance is early or late by about the same amount, move the audio item so the first audible contact matches the picture. Leave the video and cue in place.
2. Watch the middle and end. If the performance drifts, a fresh pass may work better than moving every footstep.
3. For one isolated timing problem, split in the gap around that step and move the small audio item. Turn snapping off if it prevents the needed adjustment. Preserve the sound's beginning and decay, and add short fades if an edit clicks.
4. Adjust the footstep level while watching the scene. Check that it fits the walker's distance from the camera and the force of each step.

Do not stretch the video or add processing to rescue a poor performance. Today, a convincing pass and a few clean adjustments are enough.

## 7. Watch and save · 4 minutes

Play the whole clip with the original audio and cue beeps muted. Do the steps feel attached to the feet? Name one improvement between the first pass and the final version, and one thing you would record differently next time.

Save the project with both takes. Keep the video and recorded media in its project folder, using **Save project as** with **Copy all media into project directory** if needed. Confirm the files are there before closing.

Use the same listen–perform–compare process when recording your team's [robot Foley assignment](/assignments/assignment-2-foley-recording/).
