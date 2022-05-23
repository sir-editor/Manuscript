# Wildcard names

Wildcard name is a placeholder for a project/sequence name or time.

e.g. for sequence "DrakeShip" in Vikings.prproj, on 15:30 20th May, 2022\
this Compass export media path:\
`/Users/Dropbox/EXPORT/`**`#YYYY#MM#DD`**`/`**`#PROJ`**`/`**`#SEQ`**`_`**`#hh#mm`**

will generate a path:\
`/Users/Dropbox/EXPORT/`**`20220520`**`/`**`Vikings`**`/`**`DrakeShip`**`_`**`1530`**



When input is activated, wildcards will appear at the bottom of Compass panel.\
Click on any of them to insert a wildcard at cursor position.

![](../../.gitbook/assets/Compass\_wildcards.gif)

#### Available Wildcards:

| Wildcard  | Description              |   |   |
| --------- | ------------------------ | - | - |
| **#PROD** | Production name          |   |   |
| **#PRJ**  | Project name             |   |   |
| **#SEQ**  | Sequence name            |   |   |
| **#BIN**  | Sequence parent bin name |   |   |
| **#YYYY** | Year, 4 digits (2022)    |   |   |
| **#YY**   | Year, 2 digits (22)      |   |   |
| **#MM**   | Month                    |   |   |
| **#DD**   | Day                      |   |   |
| **#hh**   | Hour                     |   |   |
| **#mm**   | Minute                   |   |   |

{% hint style="info" %}
Need more options? Write to support@knightsoftheeditingtable.com
{% endhint %}
