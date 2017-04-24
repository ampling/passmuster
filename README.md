`passmuster` is a [dmenu][]-based interface to [pass][], the standard Unix
password manager.  This design allows you to quickly copy multiple pass 
entries without having to open up a terminal window.  Use Ctrl-Return to 
confirm selection.  Passmuster will queue up entries and continue. Press 
Return when finished. 

Passmuster aims to be the most consistent pass tool by default. Pass enties
are typed using [xdotool][] instead of copied to the clipboard.  Passmuster 
will wait for a clipboard event to paste or autotype your next entry.  
Notifications are set using libnotify.


# Usage

    passmenu [-h help] [-k kill] [-v version] [-c clip] [-q quiet] [dmenu arguments...]

[dmenu]: http://tools.suckless.org/dmenu/
[xdotool]: http://www.semicomplete.com/projects/xdotool/
[pass]: http://www.zx2c4.com/projects/password-store/
