# Orchis theme

Orchis is a [Material Design](https://material.io) theme for GNOME/GTK based desktop environments.
Based on nana-4 -- [materia-theme](https://github.com/nana-4/materia-theme)

## Requirements

- GTK `>=3.20`
- `gnome-themes-extra` (or `gnome-themes-standard`)
- Murrine engine — The package name depends on the distro.
  - `gtk-engine-murrine` on Arch Linux
  - `gtk-murrine-engine` on Fedora
  - `gtk2-engine-murrine` on openSUSE
  - `gtk2-engines-murrine` on Debian, Ubuntu, etc.
- `sassc` — build dependency

## Donate

If you like my project, you can buy me a coffee:

<span class="paypal"><a href="https://www.paypal.me/vinceliuice" title="Donate to this project using Paypal"><img src="https://www.paypalobjects.com/webstatic/mktg/Logo/pp-logo-100px.png" alt="PayPal donate button" /></a></span>

## Installation

### Manual Installation

Run the following commands in the terminal:

```sh
./install.sh
```

> Tip: `./install.sh` allows the following options:

```
OPTIONS:
  -d, --dest DIR          Specify destination directory (Default: $HOME/.themes)
  -n, --name NAME         Specify theme name (Default: Orchis)

  -t, --theme VARIANT     Specify theme color variant(s) [default|purple|pink|red|orange|yellow|green|teal|grey|nord|all] (Default: blue)
  -c, --color VARIANT     Specify color variant(s) [standard|light|dark] (Default: All variants)s)
  -s, --size VARIANT      Specify size variant [standard|compact] (Default: All variants)

  -l, --libadwaita        Link installed Orchis gtk-4.0 theme to config folder for all libadwaita app use Orchis theme

  --tweaks                Specify versions for tweaks [solid|compact|black|primary|macos|submenu|(nord/dracula)] (Options can mix [nord and dracula can not mix use!])
                          1. solid:              No transparency panel variant
                          2. compact:            No floating panel variant
                          3. black:              Full black variant
                          4. primary:            Change radio icon checked color to primary theme color (Default is Green)
                          5. macos:              Change window buttons to MacOS style
                          6. submenu:            Theme sub-menus, by Default submenus contrast
                          7. [nord|dracula]:     Nord/dracula colorscheme themes

  --round                 Change theme round corner border-radius [Input the px value you want] (Suggested: 2px < value < 16px)
                          1. 3px
                          2. 4px
                          3. 5px
                          ...
                          13. 15px

  --shell                 install gnome-shell version [38|40|42]
                          1. 38:                 Gnome-shell version < 40.0
                          2. 40:                 Gnome-shell version = 40.0
                          3. 42:                 Gnome-shell version >= 42.0

  -r, --remove,
  -u, --uninstall         Uninstall/Remove installed themes

  -h, --help              Show help
```

> For more information, run: `./install.sh -h`

### Fix for libadwaita (Gnome-shell >= 42.0)

run: `./install.sh -l`

![1](images/libadwaita.png?raw=true)

![1](images/tweaks-view.png?raw=true)

### Flatpak Installation

Automatically install your host GTK+ 3.0 theme as a Flatpak. Use this:

- [stylepak](https://github.com/refi64/stylepak)

Also if you want to use this theme on a GTK+ 4.0 flatpak app, you can give the permission to access this file

local:
```
flatpak override --user --filesystem=xdg-config/gtk-4.0
```

global:
```
flatpak override --filesystem=xdg-config/gtk-4.0
```

### Firefox theme
[Install Firefox theme](src/firefox)

![Firefox-theme](src/firefox/preview01.png?raw=true)
![Firefox-theme](src/firefox/preview02.png?raw=true)

## Preview
![1](images/preview.jpg?raw=true)
