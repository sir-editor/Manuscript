# Limitations & Bugs

Here is a list of things Excalibur can't do. I break them in two categories:

* **API limitation** – this means, there is nothing in API that will allow to do this. Though, maybe I will be able to find workaround.
* **Premiere Pro bug** – it's a bug, so hopefully, it will be fixed at some point by Adobe team.

## Limitations

{% hint style="danger" %}
**IMPORTANT:** I didnt' find the way to distinguish when Premiere Pro has textbox activated. That means if you have Excalibur shortcuts that only use letters or letters with shift modifier \(**A, shift+A**\) and whenever you type text \(subtitles, name of a track, anything\), when you will press that key, Excalibur will execute command assigned to it.

To avoid this, use **ctrl**, **alt** modifiers or multiple modifiers at once.
{% endhint %}

### **Undo command**

Some of the commands won't be shown in Premiere Pro history stack, so it will be impossible to undo them.

Some of commands fill up history stack pretty fast with multiple actions.  
To give yourself more control over it, increase History level \(max allowed value 100\). Open the History panel `Window > History`and choose Settings from the Flyout \(hamburger\) menu.

{% hint style="info" %}
I'm working on implementing Excalibur history stack, it will be available in future updates and should solve "undo" limitation.
{% endhint %}

### Paste Clip

Paste Clip command won't work with clips that were cut \(not copied\) in Premiere Pro 2019

### Lumetri effect

When applying video preset with Lumetri Color, color wheels, curves,  anything that has some kind of graphic interface, will be set to default

### Color parameter

If preset has colour value with keyframes \(e.g. Tint\), colours at keyframes won't be correct.

### Transition presets

Transition presets can't be applied

## Bugs

* When applying preset, all non-linear keyframes will be set to linear
