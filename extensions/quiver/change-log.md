# Change log

## 1.1.3 — 2026-02-09

### New

* Orientation setting - set buttons to vertical, horizontal, or keep auto orientation
* Items added from libraries are now stored in "Quiver Library/Library Name" bin

### Fixed

* Quiver library projects now have separate project files for each Premiere version
* Improved loading of Quiver library project

***

## 1.1.2 — 2025-12-03

### Fixed

* Locked tracks were treated as empty tracks
* Spell Book limit removed
* Random addition was not random enough
* License verification failed in some cases

***

## 1.1.1 — 2025-07-23

### Fixed

* Library projects were automatically closed during activation without saving unsaved changes
* Quiver panel lost focus after activation of library project

***

## 1.1.0 — 2025-05-03

### New

* "Un-nest sequence (copy/paste)" option added for Quiver sequence items. The source sequence will be opened, and clips will be copied and pasted to the timeline, preserving all effects and transformations applied to clips inside the source sequence. Limitation: not possible to use with live playback.
* For Quiver sequence items with "Add as individual clips" enabled and "Un-nest sequence (copy/paste)" disabled, effects will be transferred from clips inside a source sequence to clips added to the timeline (e.g., blend mode, opacity keyframes). This allows you to use a mix of clip effects and source effects. Limitations: only linear keyframes, no masks, and limited Lumetri support (the same as for the Excalibur extension).
* Import/Export Quiver library projects.
* Mogrt items added to a timeline will get the label color of the "transparent video" placeholder.
* Open Quiver library projects or sequences from context menu

### Fixed

* If clip was dragged to quickly over Quiver panel and left it, drop region (blue zone) would stay on forever.

***

## 1.0.2 — 2025-03-14

### New

* "Group clips" option for items with "Add as individual clips" enabled
* If "Replace selected clips" is disabled, item added with Quiver will stay selected (useful in combination with Excalibur)

### Fixed

* Start marker didn't work for some clips

***

## 1.0.1 — 2025-03-03

### New

* Spell Book commands to activate a quiver project
* Option to set the amount of items shown in Spell Book
* Option to toggle replace selected clips behavior

### Fixed

* If clip speed was changed, it would not be placed correctly on a timeline
* Spell Book: on Windows Stream Deck couldn't trigger URL links
* Spell Book: on Windows shortcuts were not registered

***

## 1.0.0 — 2025-02-23

Official release
