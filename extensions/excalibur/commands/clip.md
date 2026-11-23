# Clip

## Position, Scale, Rotation, Anchor Point, Anti-flicker Filter, Opacity, Volume

![](../../../.gitbook/assets/clip_01_psr.png)

### Set value

Replaces existing value with a new one. If property has stopwatch enabled, linear keyframe will be created.

### Add value

Adds, subtracts, multiplies, divides or takes percentage from existing value. If property has stopwatch enabled, linear keyframe will be created.

| Operation | Symbol      |
| --------- | ----------- |
| Add       | + (or none) |
| Subtract  | -           |
| Multiply  | \*          |
| Divide    | /           |
| Percent   | %           |

{% hint style="info" %}
Create two User Commands for scale, using **add value** setting:\
`scale_up: +5`  \
`scale_down: -5`\
Assign keyboard for each command. Now it is possible to control clip scale with a keyboard.

Same is useful for position, rotation and other properties.
{% endhint %}

### Add/Delete keyframe

Works the same way as in After Effects.\
If there is no keyframe at playhead position, it will be created.\
If a stopwatch is inactive, it will be activated, and a keyframe will be created.

If keyframe exists at playhead, it will be deleted.\
If no keyframes left, a stopwatch will be deactivated.

## Blend Mode

Changes blend mode of selected clips.

![](../../../.gitbook/assets/clip_02_blend_mode.jpg)

## Speed

* **Change Speed** — duration is not affected
* **Change Speed and Duration** — duration is linked to speed change
* **Change Speed and Duration**, **Ripple Edit** — trailing clips will shift, left or right depending on duration change

![](<../../../.gitbook/assets/clip_03_speed (1).gif>)

## Duration

Changes duration of selected clip, without affecting its speed.

### Ripple Edit OFF

![](../../../.gitbook/assets/clip_04_duration_off.gif)

### Ripple Edit ON

To keep the clips following the changing clips next to them.

![](../../../.gitbook/assets/clip_05_duration_on.gif)

## Reverse

Reverses clip

![](../../../.gitbook/assets/clip_06_reverse.gif)

## Rename

Renames clip.\
If multiple clips are selected, all clips will get same name.

![](../../../.gitbook/assets/clip_07_rename.gif)

## Fill Frame

Scales clip, so it fills frame.

![](../../../.gitbook/assets/clip_08_fill_frame.gif)

## Label

Change label of selected clips. List shows label colors and names, that were set in Premiere Pro preferences.

![](../../../.gitbook/assets/clip_20_label.gif)

## Move to Track

Move selected clips to a track.\
You can specify track by its name, index or calculate index (e.g. `+3` or `-2` ).

If destination track is occupied, clip will be moved to the next free track.

<figure><img src="../../../.gitbook/assets/Excalibur_move_to_track.gif" alt=""><figcaption></figcaption></figure>

## Copy to Track

Copy selected clips to a track.\
You can specify track by its name, index or calculate index (e.g. `+3` or `-2` ).

If destination track is occupied, clip will be copied to the next free track.

<figure><img src="../../../.gitbook/assets/Excalibur_copy_to_track.gif" alt=""><figcaption></figcaption></figure>



## Paste Clip

Pastes clips from clipboard to specified track:

* overlay (paste on the next free track)
* on the same track
* on the highest enabled track
* on the lowest enabled track

<figure><img src="../../../.gitbook/assets/Excalibur_paste_clip.gif" alt=""><figcaption></figcaption></figure>

## Remember/Restore selection

Remember selection of clips and restore it afterwards. Selection is saved per sequence.

<figure><img src="../../../.gitbook/assets/Excalibur_remember_restore_selection.gif" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Remember selection is useful for user commands, where you need to get back to original selection, e.g.:\
\- remember selection\
\- copy clips to another track\
\- modify copied clips (effects, labels, etc)\
\- restore selection\
\- modifiy original clips
{% endhint %}

## Nest Clips

Creates nested sequence from selected clips and moves it to "Nested Clips" bin.

By default nested sequence named:\
`ParentSequenceName_nest_counter`

### Premiere Pro nest

Uses native nest command.

![](../../../.gitbook/assets/clip_21_nest_clips_native.gif)

### Excalibur nest

API method to nest clips. Allows to nest audio clips.

![](../../../.gitbook/assets/clip_12_nest_clips.gif)

## Nest Individual Clips

Creates nested sequences from **each** selected clip and moves it to "Nested Clips" bin. Linked clips will be nested together.

By default nested sequences named:\
`ParentSequenceName_ClipName_nest_counter`

### Premiere Pro nest

Uses native nest command.

![](../../../.gitbook/assets/clip_22_nest_ind_clips_native.gif)

### Excalibur nest

API method to nest clips. Allows to nest audio clips.

![](../../../.gitbook/assets/clip_13_nest_individual_clips.gif)

## Trim In/Out Point to Playhead

Trims In/Out Point of selected clips to Playhead.

![](../../../.gitbook/assets/clip_14_trim_in.gif)

If there is already another clip at playhead position, trim will be performed to End/Start of this clip.

![](../../../.gitbook/assets/clip_15_trim_out_fill.gif)

{% hint style="warning" %}
**UI bug**: after performing command some selected clips might look like they are not selected.
{% endhint %}

## Move Clip Start/End to Playhead

Moves clips Start/End to Playhead.

![](../../../.gitbook/assets/clip_16_move_end.gif)

If there is already another clip at playhead position, move will be performed to End/Start of this clip.

![](../../../.gitbook/assets/clip_17_move_start_fill.gif)

## Remove Transitions

Removes transitions from selected clips or whole sequence

### From Selected Clips

![](../../../.gitbook/assets/clip_18_remove_trans.gif)

### From Sequence (all transitions)

![](../../../.gitbook/assets/clip_19_remove_trans_seq.gif)

## **Show Clip Keyframes**

Simulates right click on a clip and clicks on a selected menu.

How to use:\
Place coursor on top of a video clip (**don’t move it after that**), call up Excalibur search bar and select menu item needed.\
It is advised to create User command and assign shortcut to it.

![](../../../.gitbook/assets/clip_23_show_clip_keyframes.gif)
