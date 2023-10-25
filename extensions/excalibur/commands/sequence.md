# Sequence

## Open Sequence

Shows list of all sequences in the project and opens selected one.

![](../../../.gitbook/assets/seq\_01\_open\_seq.gif)

## Duplicate and Increment

Duplicates active sequence to "Archived Sequences" bin and opens new (identical) sequence with incremented name.

| Before            | After             |
| ----------------- | ----------------- |
| SequenceName\_006 | SequenceName\_007 |

![](../../../.gitbook/assets/seq\_02\_duplicate\_increment.gif)

## Add Marker to Sequence

Adds marker to active sequence with specified name and label colour at playhead position.

![](../../../.gitbook/assets/seq\_03\_add\_marker.jpg)

## Add Marker to Selection

Adds marker to active sequence with specified name and label colour, which has duration of current selection.

![](../../../.gitbook/assets/seq\_04\_add\_marker\_selection.gif)

## Add Marker to Clip

Adds marker to a clip with specified name and label colour, which has duration of the selected clip.

![](../../../.gitbook/assets/seq\_10\_add\_marker\_clip.gif)

## Target Video/Audio Tracks

Targets specified tracks.

| **Option**                            | Behaviour                                                                          |
| ------------------------------------- | ---------------------------------------------------------------------------------- |
| **Target tracks**                     | Number input, targets **specified tracks\***, additive behaviour                   |
| **Toggle tracks**                     | Number input, toggles only **specified tracks\***                                  |
| **Target tracks with selected clips** | Targets tracks with selected clips, additive behaviour                             |
| **Toggle tracks with selected clips** | Toggles only tracks with selected clips                                            |
| **Target All tracks**                 | Targets all tracks                                                                 |
| **Toggle All tracks**                 | Toggles all tracks. If at least one track is targeted, will toggle all tracks off. |
| **un-Target All tracks**              | Toggles all tracks off.                                                            |

**\*** To affect multiple tracks, type track numbers separated by comma

![](../../../.gitbook/assets/seq\_11\_targetTracks.gif)

## Mute Video/Audio Tracks

Mutes specified tracks. For list of options look at [Target Video/Audio Tracks](sequence.md#target-video-audio-tracks).

![](../../../.gitbook/assets/seq\_12\_muteTracks.gif)

## Lock Video/Audio Tracks

Locks specified tracks. For list of options look at [Target Video/Audio Tracks](sequence.md#target-video-audio-tracks).

![](../../../.gitbook/assets/seq\_13\_lockTracks.gif)

## Sync Lock Video/Audio Tracks

Sync Locks specified tracks. For list of options look at [Target Video/Audio Tracks](sequence.md#target-video-audio-tracks).

![](../../../.gitbook/assets/seq\_14\_syncLockTracks.gif)

## Solo Mute Tracks

Toggles off track output/mutes all tracks except ones that have clips selected.

Submenu has options to use this command for:

* All tracks
* Video tracks
* Audio tracks

![](../../../.gitbook/assets/seq\_05\_solo\_tracks.gif)

After "Solo Mute Tracks" command was used, it will appear as "un-Solo Mute Tracks", executing it will reset toggles/mutes to original value.

![](../../../.gitbook/assets/seq\_06\_unsolo\_tracks.gif)

## Solo Lock Tracks

Locks all tracks except ones that have clips selected.

Submenu has options to use this command for:

* All tracks
* Video tracks
* Audio tracks

![](../../../.gitbook/assets/seq\_07\_solo\_lock\_tracks.gif)

After "Solo Lock Tracks" command was used, it will appear as "un-Solo Lock Tracks", executing it will reset locks to original value.

![](../../../.gitbook/assets/seq\_08\_unsolo\_lock\_tracks.gif)

## New Item

Will create syntetic media file, with same settings as active sequence and overwrites it on the lowest enabled track

Available Items:

* Adjustment layer
* Color Matte
* Black Video
* Transparent Video
* Bars and Tone

![](../../../.gitbook/assets/seq\_09\_new\_item.gif)
