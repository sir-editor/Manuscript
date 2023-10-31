# Special

## **Undo**

Undos Excalibur commands. It respects order of native Premiere Pro and Excalibur commands, so if there is no Excalibur command to undo, it will undo Premiere Pro command. When working on timeline, you can completely switch to Excalibur Undo.

![](../../../.gitbook/assets/special\_01\_undo.gif)

{% hint style="info" %}
Some of commands fill up history stack pretty fast with multiple actions.\
To give yourself more control over it, increase History level (max allowed value 100). Open the History panel `Window > History`and choose Settings from the Flyout (hamburger) menu.
{% endhint %}

{% hint style="warning" %}
Be careful in case you have this order of actions executed:

1. Native command
2. Native command
3. Excalibur command

If you use native undo command, you will get to **#1** in history stack and record of Excalibur command **#3** will be lost.
{% endhint %}

## Excalibur Settings

Opens Excalibur Settings

![](../../../.gitbook/assets/special\_02\_excalibursettings.png)
