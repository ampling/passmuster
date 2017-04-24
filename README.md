`passmuster` is a [dmenu][]-based interface to [pass][], the standard Unix
password manager.  This design allows you to quickly copy multiple pass 
entries without having to open up a terminal window.  Use Ctrl-Return to 
confirm selection.  Passmuster will enlist entries and continue. Press 
Return when finished. 

Passmuster aims to be a consistent pass tool, by default. Pass enties are 
typed using [xdotool][] instead of copied to the clipboard.  Notifications
are sent using libnotify in addition to STDOUT. 

Passmuster rejects sloppy X-selection events and guards against race conditions. 
Use Esc to clear the muster roll. 




# Usage

    passmenu [help] [kill] [version] [clip] [quiet] [dmenu...]

# Example
    <dmenu>                       <action>
    github                        type
    github.com/ampling/https      Ctrl^Return
    github.com/ampling/login      Ctrl^Return
    github.com/ampling/pass       Return
    
    <browser>
    ******                        Shift^Insert
    ******                        Shift^Insert
    ******                        Shift^Insert

[dmenu]: http://tools.suckless.org/dmenu/
[xdotool]: http://www.semicomplete.com/projects/xdotool/
[pass]: http://www.zx2c4.com/projects/password-store/
