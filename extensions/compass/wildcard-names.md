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

<table><thead><tr><th>Wildcard</th><th>Description</th><th data-hidden></th><th data-hidden></th></tr></thead><tbody><tr><td><strong>#PROD</strong></td><td>Production name</td><td></td><td></td></tr><tr><td><strong>#PRJ</strong></td><td>Project name</td><td></td><td></td></tr><tr><td><strong>#SEQ</strong></td><td>Sequence name</td><td></td><td></td></tr><tr><td><strong>#BIN</strong></td><td>Sequence parent bin name</td><td></td><td></td></tr><tr><td><strong>#YYYY</strong></td><td>Year, 4 digits (2022)</td><td></td><td></td></tr><tr><td><strong>#YY</strong></td><td>Year, 2 digits (22)</td><td></td><td></td></tr><tr><td><strong>#MM</strong></td><td>Month</td><td></td><td></td></tr><tr><td><strong>#DD</strong></td><td>Day</td><td></td><td></td></tr><tr><td><strong>#hh</strong></td><td>Hour</td><td></td><td></td></tr><tr><td><strong>#mm</strong></td><td>Minute</td><td></td><td></td></tr></tbody></table>

{% hint style="info" %}
Need more options? Write to support@knightsoftheeditingtable.com
{% endhint %}
