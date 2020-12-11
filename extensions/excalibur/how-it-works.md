# How it works

Excalibur is a complex extension. It consists of three modules:

1. [Shortcut Listener](how-it-works.md#shortcut-listener)
2. [Premiere Pro API](how-it-works.md#premiere-pro-api)
3. [Shortcut Presser](how-it-works.md#shortcut-presser)

## Shortcut Listener

There is no possibility in Premiere Pro API to register shortcut press and execute attached action. This is a big limitation for developers.

Essentially any program that has shortcuts has a shortcut listener, e.g.:  
Keyboard Maestro, AutoHotKey, Alfred.

That is why I developed a second extension, that goes along with Excalibur: [**Spellbook**](../spellbook/)  
It listens for shortcut press inside Premiere Pro only, this allows to assign shortcuts to Excalibur search bar and any other command.

## Premiere Pro API

The core of Excalibur, it is what makes Excalibur different from automation software, which relies on visual cues and replication of user interaction with Premiere Pro.

Excalibur knows which track is active, clip postion value, sequence name, playhead position, export presets, marker label, etc.

## Shortcut Presser

When I developed Excalibur, I realized that adding transitions is not very convenient via Premiere Pro API, so I decided to make shortcut presser.  
With its help Excalibur easily adds transitions and moves selected clips with timecode.

Because not all commands are available in API \(for example change label of a clip on timeline\), I thought that it would be great to allow users to press any shortcut, as part of User Commands. This allows creating better and more complex workflows.

