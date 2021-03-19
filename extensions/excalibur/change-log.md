# Change Log

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

