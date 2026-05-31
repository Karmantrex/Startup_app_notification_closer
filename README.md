## SilenceOnLogin

SilenceOnLogin is a small macOS startup cleanup script. It runs automatically after login, waits until desktop services are ready, then briefly closes visible startup apps and clears notification banners.

### Features

- Runs automatically after macOS login using a LaunchAgent.
- Waits for desktop readiness by checking Finder, Dock, SystemUIServer, and System Events.
- Closes visible startup apps using normal Command + Q behavior.
- Does not force-kill apps.
- Does not use the Notification Center Clear All UI button.
- Clears visible notification banners by restarting NotificationCenter and usernoted.
- Protects important apps and helpers such as Finder, Terminal, MagicCut, MagicQt, Mac Mouse Fix Helper, BetterTouchTool, Logi Options+, Karabiner, Rectangle, AltTab, and Raycast.
- Uses a temporary lock folder to prevent duplicate runs.

### Install

bash cd /Users/nickinoz/mySpace/SilenceOnLogin_v27 chmod +x *.command SilenceOnLogin.zsh ./install.command 

### Test manually

bash cd /Users/nickinoz/mySpace/SilenceOnLogin_v27 ./run_now.command 

### Check status and logs

bash cd /Users/nickinoz/mySpace/SilenceOnLogin_v27 ./status.command 

### Uninstall

bash cd /Users/nickinoz/mySpace/SilenceOnLogin_v27 ./uninstall.command 

### Notes

The script is intended to clean startup clutter only. It runs during a short window after login and then exits. It does not stay running all day.
