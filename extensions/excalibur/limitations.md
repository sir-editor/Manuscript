# Limitations

Here is a list of things Excalibur can't do, because there is nothing in API that will allow to do this. Though, maybe I will be able to find workaround.

{% hint style="danger" %}
**IMPORTANT:** I didn't find the way to distinguish when Premiere Pro has text-box activated. That means if you have Excalibur shortcuts that only use letters or letters with shift modifier (**A, shift+A**) and whenever you type text (subtitles, name of a track, anything), when you will press that key, Excalibur will execute command assigned to it.

To avoid this, use **ctrl**, **alt** modifiers or multiple modifiers at once.
{% endhint %}

## Mask effect

Masks (e.g. in Opacity effect) are not supported.

## Lumetri effect

When applying video preset with Lumetri Color, color wheels, curves,  anything that has some kind of graphic interface, will be set to default

## Color parameter

If preset has colour value with keyframes (e.g. Tint), colours at keyframes won't be correct.

## Transition presets

Transition presets can't be applied

## Bezier keyframes

When applying effect preset, influence (length of keyframe handle) for all bezier keyframes will be set to `16.6%`
