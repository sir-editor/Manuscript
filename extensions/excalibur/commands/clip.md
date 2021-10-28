# Clip

## Position, Scale, Rotation, Anchor Point, Anti-flicker Filter, Opacity, Volume

![](../../../.gitbook/assets/clip\_01\_psr.jpg)

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
`scale_up: +5  `\
`scale_down: -5`\
Assign keyboard for each command. Now it is possible to control clip scale with a keyboard.

Same is useful for position, rotation and other properties.
{% endhint %}

## Blend Mode

Changes blend mode of selected clips.

![](../../../.gitbook/assets/clip\_02\_blend\_mode.jpg)

## Speed

Changes speed of selected clip, without affecting its duration.

![](../../../.gitbook/assets/clip\_03\_speed.gif)

## Duration

Changes duration of selected clip, without affecting its speed.

### Ripple Edit OFF

![](../../../.gitbook/assets/clip\_04\_duration\_off.gif)

### Ripple Edit ON

To keep the clips following the changing clips next to them.

![](../../../.gitbook/assets/clip\_05\_duration\_on.gif)

## Reverse

Reverses clip

![](../../../.gitbook/assets/clip\_06\_reverse.gif)

## Rename

Renames clip.\
If multiple clips are selected, all clips will get same name.

![](../../../.gitbook/assets/clip\_07\_rename.gif)

## Fill Frame

Scales clip, so it fills frame.

![](../../../.gitbook/assets/clip\_08\_fill\_frame.gif)

## Label

Change label of selected clips. List shows label colors and names, that were set in Premiere Pro preferences.

![](../../../.gitbook/assets/clip\_20\_label.gif)

## Paste Clip

Pastes clips from clipboard to specified track.

### On the same track

![](../../../.gitbook/assets/clip\_09\_paste\_clip\_same.gif)

### On the highest enabled track

![](../../../.gitbook/assets/clip\_10\_paste\_clip\_high.gif)

### On the lowest enabled track

![](../../../.gitbook/assets/clip\_11\_paste\_clip\_low.gif)

{% hint style="warning" %}
In Premiere Pro CC 2019, "Paste Clip" command works only with clips that were copied in clipboard. Cut clips will be ignored.
{% endhint %}

## Nest Clips

Creates nested sequence from selected clips and moves it to "Nested Clips" bin.

By default nested sequence named:\
`ParentSequenceName_nest_counter`

### Premiere Pro nest

Uses native nest command.

![](../../../.gitbook/assets/clip\_21\_nest\_clips\_native.gif)

### Excalibur nest

API method to nest clips. Allows to nest audio clips.

![](../../../.gitbook/assets/clip\_12\_nest\_clips.gif)

## Nest Individual Clips

Creates nested sequences from **each** selected clip and moves it to "Nested Clips" bin. Linked clips will be nested together.

By default nested sequences named:\
`ParentSequenceName_ClipName_nest_counter`

### Premiere Pro nest

Uses native nest command.

![](../../../.gitbook/assets/clip\_22\_nest\_ind\_clips\_native.gif)

### Excalibur nest

API method to nest clips. Allows to nest audio clips.

![](../../../.gitbook/assets/clip\_13\_nest\_individual\_clips.gif)

## Trim In/Out Point to Playhead

Trims In/Out Point of selected clips to Playhead.

![](../../../.gitbook/assets/clip\_14\_trim\_in.gif)

If there is already another clip at playhead position, trim will be performed to End/Start of this clip.

![](../../../.gitbook/assets/clip\_15\_trim\_out\_fill.gif)

{% hint style="warning" %}
This command can not be undone.\
**UI bug**: after performing command some selected clips might look like they are not selected.
{% endhint %}

## Move Clip Start/End to Playhead

Moves clips Start/End to Playhead.

![](../../../.gitbook/assets/clip\_16\_move\_end.gif)

If there is already another clip at playhead position, move will be performed to End/Start of this clip.

![](../../../.gitbook/assets/clip\_17\_move\_start\_fill.gif)

{% hint style="warning" %}
This command can not be undone.\
**UI bug**: after performing command some selected clips might look like they are not selected.
{% endhint %}

## Remove Transitions

Removes transitions from selected clips or whole sequence

### From Selected Clips

![](../../../.gitbook/assets/clip\_18\_remove\_trans.gif)

### From Sequence (all transitions)

![](../../../.gitbook/assets/clip\_19\_remove\_trans\_seq.gif)

## **Show Clip Keyframes**

Simulates right click on a clip and clicks on a selected menu.

How to use:\
Place coursor on top of a video clip (**don’t move it after that**), call up Excalibur search bar and select menu item needed.\
It is advised to create User command and assign shortcut to it.

![](../../../.gitbook/assets/clip\_23\_show\_clip\_keyframes.gif)
