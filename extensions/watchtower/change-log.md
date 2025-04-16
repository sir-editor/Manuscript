---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Change log

## 1.5.7 — 2025-04-16

### Fixed

* Spell Book didn't load or crashed

***

## 1.5.6 — 2025-03-13

### Fixed

* Watchtower couldn't be activated in Premiere 2024 and below
* Translation typos

***

## 1.5.5 — 2025-03-12

### New

* Spell Book support

### Fixed

* On Windows if project and folders/files were on different drives, folders/files were ignored.
* Another fix for allowed extensions setting

***

## 1.5.4 — 2025-01-20

### Fixed

* Some of file extensions not allowed in settings, were still imported (e.g. ".mts")

***

## 1.5.3 — 2024-11-18

### New

* Support for .wav files in RED camera folder structure
* White theme added

### Fixed

* Premiere Pro team projects were not shown correctly in watch folder manager
* Sequence auto detection didn't work correctly in some cases
* Other minor fixes

***

## 1.5.2 — 2024-09-30

### Fixed

* Auto sync didn't work with ExFAT drives on macOS
* After Effects: in some cases Watch folders panel couldn't load

***

## 1.5.1 — 2024-07-30

### Fixed

* Watchtower didn’t wait for files to be written on disk
* Special characters in project name wouldn’t allow Watchtower to work
* When linking bins, sub-bins were not linked
* After Effects: in some cases Watch folders panel couldn’t load
* Other minor fixes

***

## 1.5.0 — 2024-05-23

### New

* Watchtower rewritten from zero
* Performance improvement
* Stable auto-sync, waits for files to be written on disk
* Label option for imported items
* Import Date metadata for Premiere Pro

***

## 1.3.2 — 2020-10-31

### General

* fixed relative paths bug for Premiere Pro 14.3.1 on Windows

### Settings

* "Check whole project for duplicates during import" checkbox added
* folder name regex filter now is case-insensitive
* UI update

#### Select Folders

* UI update

***

## 1.3.1 — 2020-07-28

### Settings

* folder name regex filter

### Select Folders

* fixed blank menu issue for Premiere Pro 14.3.1 on Windows

***

## 1.3.0 — 2020-07-03

### General

* team projects support
* possible to sync folder to an existing bin (Premiere supports from 2018)&#x20;
* relink missing folders menu
* mapped drives now always use UNC path
* stability improvements

### Settings

* folder name filter

### Select Folders

* opening time speed up
* keyboard interaction

***

## 1.2.0 — 2020-04-06

### General

* watchtower panel could be closed and auto sync will work in background
* auto sync works with multiple projects open
* Japanese localisation added, thanks to Jo Bellamy and Masahiro Sagawa
* fixed issue for After Effects when files in Korean language were imported multiple times

### Settings

* **auto sync option added**
* time interval sync is removed
* customisable filter for file extensions to import
* possibility to deactivate license on current machine

### Select Folders

* standard and advanced sections added
* automatic detection of image sequences in folders
* automatic detection of camera folder structures: ARRIRAW, RED, AVCHD, Canon XF, Panasonic P2 (spanned clips are not supported at the moment), XDCAM-EX, XDCAM-HD, Sony HDV, Sony a7S
* flatten folders setting
* relative paths setting

***

## 1.1.4 — 2019-12-09

### General

* Premiere Pro 14.0.1 support
* bug fixes

***

## 1.1.3 — 2019-11-01

### General

* license check issue fixed
* .braw files support added
* stability improvements

***

## 1.1.2 — 2019-09-23

### General

* .swf files support added
* stability improvements

***

## 1.1.1 — 2019-09-15

### General

* Premiere Pro & After Effects CC2017 and above support

### Settings

* "show import options" setting for Premiere Pro, Illustrator & Photoshop files

***

## 1.0.1 — 2019-07-23

### General

* single user can install extension on two machines

### Select Folders

* special characters in folder name are now supported

***

## 1.0.0 — 2019-07-08

Official release

