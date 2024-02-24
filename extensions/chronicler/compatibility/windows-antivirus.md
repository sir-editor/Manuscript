# Windows Antivirus

If you have antivirus installed, it might block Chronicler from checking which application is active. To be sure that Chronicler works properly, whitelist following file:

**chronicler\_win.exe** – detects an active application. It is essential to for automatic tracking, so Chronicler doesn't track time when Adobe app is not active. Full path:

```
C:\Users\*USERNAME*\AppData\Roaming\Adobe\CEP\Extensions\knights_of_the_editing_table.chronicler\assets\exec\chronicler_win.exe
```
