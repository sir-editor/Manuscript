# Uninstall

## Application

Remove **Spell Book** application from:

### macOS

```
/Applications/Spell Book.app
```

### Windows

```
C:\Program Files\Knights of the Editing Table\Spell Book.exe
```

***

## CEP Extension

Remove **`knights_of_the_editing_table.spell_book`** folder from:

### macOS

```markup
/Library/Application Support/Adobe/CEP/extensions/
```

### Windows

```markup
C:\Program Files\Common Files\Adobe\CEP\extensions\
```

***

## UXP Extension

Run following command in Terminal/Command Prompt.

{% hint style="warning" %}
You will need to run command multiple times for each Adobe host app,\
to remove every instance of Spell Book plugin.
{% endhint %}

### macOS

```markup
"/Library/Application Support/Adobe/Adobe Desktop Common/RemoteComponents/UPI/UnifiedPluginInstallerAgent/UnifiedPluginInstallerAgent.app/Contents/macOS/UnifiedPluginInstallerAgent" --remove "Spell Book"
```

### Windows

```markup
"C:\Program Files\Common Files\Adobe\Adobe Desktop Common\RemoteComponents\UPI\UnifiedPluginInstallerAgent\UnifiedPluginInstallerAgent.exe" /remove "Spell Book"
```
