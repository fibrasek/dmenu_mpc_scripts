# dmenu_mpc_scripts
A little set of scripts to change your playlist and music via `dmenu`

# Installing

To use it properly, you must have it installed and configured `dmenu`, `mpd/mopidy` and `mpc` in your system.

To use it simply clone this repository:
```
git clone https://github.com/Fibrasek/dmenu_mpc_scripts.git
cd dmenu_mpc_scripts
```

Then copy/move or link it to the folder of your choice:
```
# In this case, I am using a symbolic link...
ln -s ./dmenu_change_music <target_dir>
ln -s ./dmenu_change_playlist <target_dir>
```

To ensure it will run just fine, make it executable:
```
chmod +x dmenu_change_music
chmod +x dmenu_change_playlist
```

# Using
To use it simply run:
```
dmenu_change_music
# or
dmenu_change_playlist
```

### i3
To use it within i3, make sure you add those following lines to your `config`, usually located at `~/.config/i3/config`
```
# Change Mod4+Tab/Mod4+Shift+Tab to your liking...
# Spawn dmenu to choose playlist
bindsym Mod4+Shift+Tab exec --no-startup-id ~/.config/scripts/dmenu_change_playlist

# Spawn dmenu to choose music
bindsym Mod4+Tab exec --no-startup-id ~/.config/scripts/dmenu_change_music

```

# Contributing
Feel free to open PRs, issues or anything you find that will make it more usuful to people :)
