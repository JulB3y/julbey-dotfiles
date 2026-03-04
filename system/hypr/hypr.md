# Hypr Config
## Hyprland Config
my hyprland config in split into multiple files for easier access to settings and for easier replacements if something changes.

### structure
the main file is still the same. Its `hyprland.conf` and should be located in `~/.config/hypr/`. It contains all the paths for the children `.conf` files. 
Sub configs are:

```bash
├── hypr
│   ├── ...
│   ├── hyprland
│   │   ├── animations.conf   # animations config 
│   │   ├── autostart.conf    # services and applications to start with hyprland
│   │   ├── deco.conf         # decoration config
│   │   ├── env.conf          # environment variables
│   │   ├── general.conf      # general, misc, dwindle
│   │   ├── input.conf        # input config
│   │   ├── keybinds.conf     # keybinds and modifier config
│   │   ├── monitor.conf      # monitor setup
│   │   ├── stdprogram.conf   # standard applications (e.g. browser->firefox, etc)
│   │   └── windowrules.conf  # windowrules
│   ├── hyprland.conf         # config sourcing all the other .conf files
│   ├── ...
```

### fixes, tips and tricks
#### Ghostty - keyboard compose layer
Ghostty used to not be able to write symbols from the compose layer (e.g. ü with Compose + u + "). 
Its a problem with the newer GTK versions. 
To fix add environment variable with: `env = GTK_IM_MODULE,simple` to your hyprland config or export the environment variable through your preferred way.
