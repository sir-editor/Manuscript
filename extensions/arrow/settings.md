---
layout:
  width: default
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

# Settings

## Copy

<figure><img src="../../.gitbook/assets/Arrow_Copy_settings (2).png" alt=""><figcaption></figcaption></figure>

### Show Notifications

Toggle to show notification about copied frame.

### Save frame

If enabled, copied frame will be saved at absolute or relative to a project path location.

To enable **relative path**, toggle "R" button.

***

## Paste

<figure><img src="../../.gitbook/assets/Arrow_Paste_settings (2).png" alt=""><figcaption></figcaption></figure>

### Pasted frame save location

Pasted image will be saved at absolute or relative to a project path location.\
If destination path doesn't exist, it will be created.

To enable **relative path**, toggle "R" button.

### Pasted frame project bin path

Pasted image will be imported to a specified bin in the Project panel.

If value is not set, image will be imported in `Arrow` bin.

<figure><img src="../../.gitbook/assets/Arrow_paste_bin_path.gif" alt=""><figcaption><p>Bin path set to "/PASTED/#SEQ/#hh_#mm"</p></figcaption></figure>

***

## Wildcards

Wildcard name is a placeholder for a project/sequence name or time.\
It is available both for Copy and Paste save paths.

> e.g. for sequence "DrakeShip" in Vikings.prproj, on 15:30 20th May, 2022
>
> ```
> /Users/Knight/COPY/#YYYY#MM#DD/#PROJ/#SEQ_#hh#mm
> ```
>
> will generate a path:
>
> ```
> /Users/Knight/COPY/20220520/Vikings/DrakeShip_1530/DrakeShip_00_00_09_22
> ```

When input is activated, wildcards will appear below input.\
Click on any of them to insert a wildcard at cursor position.

#### Available Wildcards:

<table><thead><tr><th width="199.12880874796468">Wildcard</th><th width="332.73460910089955">Description</th><th data-hidden></th><th data-hidden></th></tr></thead><tbody><tr><td><strong>#PROD</strong></td><td>Production name</td><td></td><td></td></tr><tr><td><strong>#PRJ</strong></td><td>Project name</td><td></td><td></td></tr><tr><td><strong>#SEQ</strong></td><td>Sequence name</td><td></td><td></td></tr><tr><td><strong>#BIN</strong></td><td>Sequence parent bin name</td><td></td><td></td></tr><tr><td><strong>#YYYY</strong></td><td>Year, 4 digits (2022)</td><td></td><td></td></tr><tr><td><strong>#YY</strong></td><td>Year, 2 digits (22)</td><td></td><td></td></tr><tr><td><strong>#MM</strong></td><td>Month</td><td></td><td></td></tr><tr><td><strong>#DD</strong></td><td>Day</td><td></td><td></td></tr><tr><td><strong>#hh</strong></td><td>Hour</td><td></td><td></td></tr><tr><td><strong>#mm</strong></td><td>Minute</td><td></td><td></td></tr></tbody></table>

{% hint style="info" %}
Need more options? Write to support@knightsoftheeditingtable.com
{% endhint %}
