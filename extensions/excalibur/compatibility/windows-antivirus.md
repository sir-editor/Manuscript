# Windows Antivirus

If you have antivirus installed, it might block Excalibur from listening shortcuts and simulating a shortcut press. To be sure that Excalibur works properly, whitelist following files:

**spell\_win.exe** – detects a shortcut press. It is essential for calling up search bar and executing any command that has a shortcut assigned. Full path:`C:\Users\*USERNAME*\AppData\Roaming\Adobe\CEP\Extensions\knights_of_the_editing_table.spellbook\client\lib\spell_win.exe`

**spellcast\_win.exe** – simulates a shortcut press. This one needed for "Keyboard Shortcut", "Apply Transition", "Timecode" commands. Full path:`C:\Users\*USERNAME*\AppData\Roaming\Adobe\CEP\Extensions\knights_of_the_editing_table.excalibur\client\lib\exec\spellcast_win.exe`



