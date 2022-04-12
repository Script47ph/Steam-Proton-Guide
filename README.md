# Steam-Proton-Guide
My note for run windows game on linux with steam play proton

### Requirement

- Winetricks
- Protontricks

### Play AC Origins on linux with Steam Play Proton

1. Enable Steam Play for all other titles and restart Steam.
2. Force the use of a specific Steam Play compatibility tool. In this case AC Origins.
3. Wait until the Steam Play Proton version your choose has been installed. Don't play! Just close the Steam App.
4. Create Ubisoft Connect folder source file, ``` mkdir -p ~/.cache/winetricks/uplay/ ```
5. Download Ubisoft Connect from https://ubisoft.com/ and save to folder just created above. Rename the file "UbisoftConnectInstaller.exe" to "UplayInstaller.exe".
6. Open Protontricks and choose the game, Install Application -> Uplay. Wait until installation process has finished and close Ubisoft Connect.
7. Open Steam App again, and try run the game.


### Play other Ubisoft game with Steam Play Proton

1. Enable Steam Play for all other titles and restart Steam.
2. Add a Non-Steam Game and choose "UbisoftConnectInstaller.exe".
3. Properties -> Compatibility -> Force the use of a specific Steam Play compatibility tool. Choose Steam Play Proton version what you want.
4. Run, Ubisoft Connect Installer will open up, just install like in Windows.
5. Add shortcut, repeat step 2 and add ubisoft.lnk from the Proton installation folder in "~/.local/share/Steam/steamapps/compatdata/123456/pfx/drive_c/users/steamuser/Desktop/Ubisoft Connect.lnk". Replace "123456" with your right folder installation, you can check 1 by 1 or sort from modified date.
6. Properties -> Shortcut -> click Browse and choose "UbisoftConnect.exe" from step 5 in directory "Program Files (x86)\Ubisoft\Ubisoft Game Launcher\". Still in the same Properties -> Compatibility -> Force the use of a specific Steam Play compatibility tool. Choose Steam Play Proton version what you want.
7. Try run Ubisoft Connect.lnk.
