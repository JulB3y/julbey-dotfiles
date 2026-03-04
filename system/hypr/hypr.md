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
│   │   ├── animations.conf
│   │   ├── autostart.conf
│   │   ├── deco.conf
│   │   ├── env.conf
│   │   ├── general.conf
│   │   ├── input.conf
│   │   ├── keybinds.conf
│   │   ├── monitor.conf
│   │   ├── stdprogram.conf
│   │   └── windowrules.conf
│   ├── hyprland.conf
│   ├── ...
```

