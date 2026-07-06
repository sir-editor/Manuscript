# Import and export

## Export

Select a folder or item, right-click, and choose **Export…**.

<figure><img src="../../.gitbook/assets/Quiver_15_export_context_menu.png" alt=""><figcaption></figcaption></figure>

Quiver copies the selected content to a destination folder. For sequence items, media is included in a **sequence media** bin so the export is portable.

A progress overlay shows export status.

## Import

To import exported items, drag and drop the exported folder onto the Quiver main panel.

<figure><img src="../../.gitbook/assets/Quiver_15_import_export.gif" alt=""><figcaption></figcaption></figure>

## Legacy library import

When you first launch Quiver 1.5, it scans for legacy Quiver library projects from earlier versions and offers to import them.

{% hint style="warning" %}
Legacy libraries cannot be used directly in Quiver 1.5. Import converts them into the new folder structure. See [Quiver folders](quiver-folders.md#legacy-library-import).
{% endhint %}

## Copy vs reference

When sharing quivers, prefer **copy** import mode so all media is included in the Quiver data folder. Items added in **reference** mode point to original file paths and may be offline on another machine.

Configure the default import mode in [Settings](settings.md#import-mode).
