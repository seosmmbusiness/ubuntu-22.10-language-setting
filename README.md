# Ubuntu 22.10 language setting to Shift+Alt Working

There is a bug which makes switching language in Ubuntu 22.04 and Ubuntu 22.10 a bit complicated. All settings I checked works awful.

Here is the optimal setting where you can use both Shift+Alt and Alt+Shift for language switching.

## Make not under root! 
The direct switching with Shift+Alt_L

`gsettings set org.gnome.desktop.wm.keybindings switch-input-source "['<Shift>Alt_L', 'XF86Keyboard']"`

The backward switching with Alt+Shift_L

`gsettings set org.gnome.desktop.wm.keybindings switch-input-source-backward "['<Alt>Shift_L', '<Shift>XF86Keyboard']"`
