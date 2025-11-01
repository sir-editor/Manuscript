---
description: Learn how to add Spell Book support to your extension
---

# API Reference

Spell Book works both in **CEP** and **UXP** platforms.

It consists of application and extension, which acts as a bridge between Spell Book app and your extension.\
I've created two npm modules, both for [CEP](https://www.npmjs.com/package/@knights-of-the-editing-table/spell-book) and [UXP](https://app.gitbook.com/u/S44malNHPqNYGj2frrNU4XHIoMc2). These modules provide interface for commands registration and handling command event.

## Installation

{% tabs %}
{% tab title="CEP" %}
Make sure that Spell Book is installed (both app and Spell Book extension).

### Installation

```sh
npm install @knights-of-the-editing-table/spell-book
```

### Usage

```javascript
// code.js
import Spellbook from '@knights-of-the-editing-table/spell-book';

const commands = [
    {
        commandID: 'command.id',
        name: 'Command 1', // use localised name if needed
        group: 'Group 1', // optional
        action: () => { // run action when command is triggered
            console.log('command.id triggered!')
        }
    }
];

const spellbook = new Spellbook('Extension name', 'extension.id', commands);
```
{% endtab %}

{% tab title="UXP" %}
Make sure that Spell Book is installed (both app and Spell Book extension).

### Installation

```sh
npm install @knights-of-the-editing-table/spell-book-uxp
```

### Usage

Add command entrypoint and enablePluginCommunication to manifest.json, for [Inter Plugin Communication](https://developer.adobe.com/indesign/uxp/plugins/tutorials/inter-plugin-comm/):

```json
// manifest.json
{
    "entrypoints": [
        {
            "type": "command",
            "id": "spellbook.plugin",
            "label": {
                "default": "- spellbook plugin" // you can use your label
            }
        }
    ],
    "requiredPermissions": {
        "ipc": {
            "enablePluginCommunication": true
        }
    }
}
```

Add Spell Book plugin:

```javascript
// code.js
import Spellbook from '@knights-of-the-editing-table/spell-book-uxp';

const commands = [
    {
        commandID: 'command.id',
        name: 'Command 1', // use localised name if needed
        group: 'Group 1', // optional
        action: () => { // run action when command is triggered
            console.log('command.id triggered!')
        }
    }
];

const spellbook = new Spellbook('Extension name', 'extension.id', commands);

// add spellbook.plugin to entry points
const { entrypoints } = require("uxp");
entrypoints.setup({
    commands: {
        'spellbook.plugin': {
            run: (data, args) => spellbook.plugin(data, args),
        },
    },
});
```
{% endtab %}
{% endtabs %}

#### **Spellbook constructor**

```javascript
const spellbook = new Spellbook(
    pluginName: string,
    pluginID: string,
    commands?: Command[])
```

#### **Methods**

```javascript
spellbook.register(commands) // Add or update commands
spellbook.start() // Start listening for command events
spellbook.stop() // Stop listening for command events
```

#### **Events**

The plugin extends EventEmitter and emits events when commands are triggered:

```javascript
spellbook.on('command.id', (commandID) => {
    console.log('command.id triggered!')
});
```

