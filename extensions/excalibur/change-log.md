# Change Log

## 1.1.3 — 2021-07-14

### **New**

* **Sequence module:**
  * Add Marker to Clip
  * Target Video/Audio Tracks
  * Mute Video/Audio Tracks
  * Lock Video/Audio Tracks
  * Sync Lock Video/Audio Tracks
* **Preferences module:**
  * Display Color Management
  * Snap playhead in Timeline
  * Selection Follows Playhead
  * Linked Selection
  * Transparency Grid
  * Show Rulers
  * Show Guides
  * Snap in Program Monitor
* **Selection module:**
  * Select Clip Above/Below
  * Extend Selection
  * Select All Clips after/before Playhead
  * Invert Selection
  * Select All Disabled Clips
* Multiply, divide, percent operations are added for Position/Scale/Rotation and etc
* Excalibur Settings could be open from a search bar

### **Fixed**

* "Copy Frame to Clipboard" didn't work on some macOS machines
* "Export Media/Selected Clips" in a search bar used project location as an export path. Now it defaults to Premeire Pro last used export path \(which could be controlled with [Compass](../compass/)\)
* Unnecessary undo step was performed for Duration/Speed command if duration/speed couldn't be changed or was the same for an affected clip
* Effect presets that used "Vector Motion" \(part of Essential Graphics\) added additional "Vector Motion" effect instead of changing values of an existing one
* Optimized "Nest Clips" command
* Optimized "Paste Clip on Same track" command
* Optimized preloading of a search bar
* Enter pressed multiple times in a search bar caused Excalibur to execute command multiple times

### Renamed

* "Add Marker" renamed to "Add Marker to Sequence"
* "Solo Tracks" renamed to "Solo Mute Tracks"

## 1.1.2 — 2021-05-13

### **New**

* **Copy Frame to Clipboard**
* **Wait** command \(for User Commands\)
* **Duplicate and Increment**, **Increment and Save** now have user command options. One can define how naming will look like.
* Date wildcards for **Nest Clips**
* **Apply Transition** doesn't need shortcut to be set in "Premiere Pro -&gt; Keyboard shortcuts"

### **Fixed**

* If audio preset included change of volume, it won't be applied
* Timecode command didn't work with selected clips on Windows
* Trim out point to playhead worked incorrectly with clips that have changed speed
* Film Impact transitions did't work: Light Leaks Impacts; Kaleido Impacts; Stripes Impacts; Chroma Leaks Impacts
* Optimized work with bigger timelines

## 1.1.1 — 2021-04-09

### **New**

* Export Selected Clips: audio is included

### **Fixed**

* Undo command didn't work for some of actions
* Adjustment layer, Nest clips command didn't work on Windows
* Transitions and shortcut press commands
* Intrinsic effects value change on clips with changed speed
* Multiple Exports in user command resulted in same exports
* Doubling effect for Effect presets that also affect intrinsic effects
* Excalibur didn't respond or worked with a delay
* Timecode command

## 1.1.0 — 2021-03-19

### **New**

* **Undo** command for Excalibur commands
* **Label** command \(change label of clips\)
* Adjustment layer added to New Item command
* Nest Clips and Nest Individual Clips now have two type of nest command:
  * Premiere Pro nest
  * Excalibur nest
* Audio preset can be applied to audio track with values changed \(keyframes are not supported\)
* Show Clip Keyframes command
* Control Surfaces on macOS support added. Stream Deck, Loupedeck, Orbital 2, etc are supported.
* Windows OS search bar options:
  * Instant search bar 
  * Panel mode for search bar 
* Submenus now have search bar
* User can set height of Excalibur search bar
* Transitions now support all languages

### **Fixed**

* Nest Individual Clips didn’t respect linked clips.
* Speed command when applied would set lower speed \(target: 400%, result: 238%\). Now speed command will be applied multiple times, until it will set proper speed value.
* Effect presets that used intrinsic effects in languages other than English would add to clip another copy of intrinsic effect \(e.g. second copy of Motion\)
* Japanese IME support improvement:
  * on macOS it wasn't possible to use Japanese characters in Project panel
  * Excalibur would quit when user selected suggestion from IME dropbox

## 1.0.1 — 2021-01-05

### Transitions

* Added support for Boris FX Continuum, Sapphire, Red Giant Universe and Film Impact v3 transitions
* Added support for Japanese and Italian transition names

### Fixed

* Excalibur could take several minutes to launch after "Unsheathe Excalibur" shortcut was pressed \(related to _Effect Presets and Custom Items.prfpset_ big file size\)
* Effect presets wouldn't show up in Excalibur
* If an effect preset has more than one of the same effects, only one of them would be applied
* **Duplicate and Increment** placed new sequence in a random bin
* **Fill Frame** used on clips that have "Scale to Frame Size" enabled, would deliver inaccurate results
* A keyboard shortcut assigned to **Nest Individual Clips** would show an empty search bar
* When changing an existing transition without specifying its length, the length would be set to the default transition length
* **F1-F24** keys couldn't be assigned as shortcuts on Windows
* After pressing down arrow on an empty search bar to show all commands, selected command wouldn't execute
* UI fixes

## 1.0.0 — 2020-12-01

Official release

