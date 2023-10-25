# Convert .kys file

Convert Premiere Pro keyboard shortcuts between macOS and Windows.

![](../../.gitbook/assets/convertKYS.gif)

After upload .kys file you can remap your shortcuts.

{% tabs %}
{% tab title="macOS -> Windows" %}
**⌘** _(cmd)_ becomes **Ctrl**, **⌃**_(ctrl)_ becomes **Ctrl**

In case of conflict shortcut will be outlined with orange color.

{% hint style="warning" %}
If you choose to download without solving command conflicts, these commands will no longer have a shortcut
{% endhint %}
{% endtab %}

{% tab title="Windows -> macOS" %}
**Ctrl** becomes **⌘** _(cmd)_
{% endtab %}
{% endtabs %}

The location of the customized keyboard shortcuts file depends on whether you've signed in to Creative Cloud Sync Settings in Premiere Pro or not.

{% tabs %}
{% tab title="macOS" %}
Signed into Creative Cloud Sync Settings

```
Users/[username]/Documents/Adobe/Premiere Pro/[version]/Profile-CreativeCloud-/Mac/
```

Signed out of Creative Cloud Sync Settings

```
Users/[username]/Documents/Adobe/Premiere Pro/[version]/Profile-username/Mac/
```
{% endtab %}

{% tab title="Windows" %}
Signed into Creative Cloud Sync Settings

```
Users\[username]\Documents\Adobe\Premiere Pro\[version]\Profile-CreativeCloud-\Win\
```

Signed out of Creative Cloud Sync Settings

```
Users\[username]\Documents\Adobe\Premiere Pro\[version]\Profile-username\Win\
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
More information about keyboard shortcuts in Premiere Pro on [official website](https://helpx.adobe.com/premiere-pro/using/keyboard-shortcuts.html)
{% endhint %}
