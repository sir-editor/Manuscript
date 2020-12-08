# Clip

## Position, Scale, Rotation, Anchor Point, Anti-flicker Filter, Opacity, Volume

![](../../../.gitbook/assets/clip_01_psr.jpg)

### Set value

Replaces existing value with a new one. If property has stopwatch enabled, linear keyframe will be created.

### Add value

Adds or substracts from existing value. If property has stopwatch enabled, linear keyframe will be created.

{% hint style="info" %}
Create  two User Commands for scale, using **add value** setting:  
`scale_up:   +5  
scale_down: -5`  
Assign keyboard for each command. Now it is possible to control clip scale with a keyboard.

Same is useful for position, rotation and other properties.
{% endhint %}

## Blend Mode

Changes blend mode of selected clips.

![](../../../.gitbook/assets/clip_02_blend_mode.jpg)

## Speed

Changes speed of selected clip, without affecting its duration.

![](../../../.gitbook/assets/clip_03_speed.gif)

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

Renames clip.  
If multiple clips are selected, all clips will get same name.

![](../../../.gitbook/assets/clip_07_rename.gif)

## Fill Frame

Scales clip, so it fills frame.

![](../../../.gitbook/assets/clip_08_fill_frame.gif)

## Paste Clip

Pastes clips from clipboard to specified track.

### On the same track

![](../../../.gitbook/assets/clip_09_paste_clip_same.gif)

### On the highest enabled track

![](../../../.gitbook/assets/clip_10_paste_clip_high.gif)

### On the lowest enabled track

![](../../../.gitbook/assets/clip_11_paste_clip_low.gif)

{% hint style="warning" %}
In Premiere Pro CC 2019, "Paste Clip" command works only with clips that were copied in clipboard. Cut clips will be ignored.
{% endhint %}

## Nest Clips

Creates nested sequence from selected clips and moves it to "Nested Clips" bin.

By default nested sequence named:  
`ParentSequenceName_nest_counter`

![](../../../.gitbook/assets/clip_12_nest_clips.gif)

{% hint style="info" %}
It is possible to nest audio clips!
{% endhint %}

## Nest Individual Clips

Creates nested sequences from **each** selected clip and moves it to "Nested Clips" bin.

By default nested sequences named:  
`ParentSequenceName_ClipName_nest_counter`

![](../../../.gitbook/assets/clip_13_nest_individual_clips.gif)

## Trim In/Out Point to Playhead

Trims In/Out Point of selected clips to Playhead.

![](../../../.gitbook/assets/clip_14_trim_in.gif)

If there is already another clip at playhead position, trim will be performed to End/Start of this clip.

![](../../../.gitbook/assets/clip_15_trim_out_fill.gif)

{% hint style="warning" %}
This command can not be undone.  
**UI bug**: after performing command some selected clips might look like they are not selected.
{% endhint %}

## Move Clip Start/End to Playhead

Moves clips Start/End to Playhead.

![](../../../.gitbook/assets/clip_16_move_end.gif)

If there is already another clip at playhead position, move will be performed to End/Start of this clip.

![](../../../.gitbook/assets/clip_17_move_start_fill.gif)

{% hint style="warning" %}
This command can not be undone.  
**UI bug**: after performing command some selected clips might look like they are not selected.
{% endhint %}

## Remove Transitions

Removes transitions from selected clips or whole sequence

### From Selected Clips

![](../../../.gitbook/assets/clip_18_remove_trans.gif)

### From Sequence \(all transitions\)

![](../../../.gitbook/assets/clip_19_remove_trans_seq.gif)

