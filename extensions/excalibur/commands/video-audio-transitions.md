# Video/Audio Transitions

There are 5 ways to apply transitions.

By default **Apply Transition** command will be used with default transition duration (could be set in `Premiere Pro>Preferences>Timeline`).

![](../../../.gitbook/assets/trans\_01\_default.gif)

{% hint style="info" %}
When switching keyboard layout in Keyboard shortcuts, save project, for Excalibur to see that it was changed.
{% endhint %}

## Apply Transition

Applies transition to cuts under playhead.\
If cuts are selected, transition will be applied to them,\
If clips are selected, transition will be applied to in/out points of selected clips.

![](../../../.gitbook/assets/trans\_02\_apply\_trans.gif)

{% hint style="info" %}
Transition duration uses units (frames/seconds) that are set for each transition type in`Premiere Pro>Preferences>Timeline`
{% endhint %}

## Apply Transition To/From Playhead

Applies transition to cuts on the left/right of playhead and stretches transition to playhead position.

![](../../../.gitbook/assets/trans\_03\_apply\_to\_play.gif)

In comparison to [legacy](video-audio-transitions.md#apply-transition-to-from-playhead-legacy) version, "Apply Transition To/From Playhead" adds proper transition between clips.

{% hint style="warning" %}
"Apply Transition To/From Playhead" command presses **Select Clip at Playhead **shortcut. Make sure it is assigned in Keyboard Shortcuts menu.
{% endhint %}

## Apply Transition To/From Playhead (legacy)

Applies transition to cuts on the left/right of playhead and stretches transition to playhead position. (Standard Premiere Pro command)

![](../../../.gitbook/assets/trans\_04\_apply\_from\_play\_legacy.gif)

"Apply Transition To/From Playhead (legacy)" doesn't add transition between clips, but adds fade to/from black/silence.

{% hint style="warning" %}
"Apply Transition To/From Playhead" command presses **Apply Default Video/Audio Transition to/from Playhead** shortcuts. Make sure they are assigned in Keyboard Shortcuts menu.
{% endhint %}
