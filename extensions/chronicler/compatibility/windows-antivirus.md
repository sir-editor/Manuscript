# Windows Antivirus

If you have antivirus installed, it might block Chronicler from checking which application is active. To be sure that Chronicler works properly, whitelist following file:

**knights\_of\_the\_editing\_table.chronicler.exe** – detects an active application. It is essential to for automatic tracking, so Chronicler doesn't track time when Adobe app is not active. Full path:

```
C:\Program Files\Common Files\Adobe\CEP\extensions\knights_of_the_editing_table.chronicler\assets\exec\win\knights_of_the_editing_table.chronicler.exe
```
