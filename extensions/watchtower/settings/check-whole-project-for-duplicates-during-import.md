---
description: Added in Watchtower 1.3.2
---

# Check whole project for duplicates during import

## ON

Watchtower will scan whole project for duplicates. In general, if project has less than 1000 assets, scan takes a second.

With this setting ON, it is possible to move assets in and out of a project watch-bins, duplicates won't be imported.

## OFF

If project has large amount of assets \(e.g. 2000 and more\), scan takes more time. To speed it up, turn off "Check whole project for duplicates during import".

With this setting OFF, if asset is moved out of a project watch-bin, it will be imported again during next import.

{% hint style="warning" %}
Initial scan will take longer, because Watchtower needs to create index map of watch-bins.

If any bin will be moved or deleted, Wathctower will need to re-index project again.
{% endhint %}

