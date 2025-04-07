# Ghostty Terminal Configuration

This repository contains my personal configuration for the [Ghostty](https://github.com/mitchellh/ghostty) terminal emulator.

## Configuration Options

### Font Settings
```
font-family = Berkeley Mono Variable  # Using Berkeley Mono Variable font
font-size = 15                       # Font size in points
```

### Theme Configuration
```
theme = tokyonight                   # Using the Tokyo Night color scheme
```

### Window Settings
```
window-padding-balance = true        # Automatically balance window padding
macos-titlebar-style = hidden       # Hide the macOS titlebar
window-save-state = always          # Always save window state
window-colorspace = "display-p3"    # Use display-p3 color space for better color reproduction
```

### Mouse Settings
```
mouse-hide-while-typing = true      # Hide mouse cursor while typing
copy-on-select = clipboard          # Automatically copy selected text to clipboard
```

### Keybindings

#### Split Navigation
```
keybind = shift+ctrl+h=goto_split:left    # Navigate to left split
keybind = shift+ctrl+j=goto_split:bottom  # Navigate to bottom split
keybind = shift+ctrl+k=goto_split:top     # Navigate to top split
keybind = shift+ctrl+l=goto_split:right   # Navigate to right split
```

#### Tab Management
```
keybind = super+shift+t=new_tab           # Create new tab
keybind = super+shift+h=previous_tab      # Go to previous tab
keybind = super+shift+l=next_tab          # Go to next tab
keybind = super+shift+comma=move_tab:-1   # Move tab left
keybind = super+shift+period=move_tab:1   # Move tab right
```

#### Clipboard Operations
```
keybind = super+c=copy_to_clipboard       # Copy to clipboard
keybind = super+v=paste_from_clipboard    # Paste from clipboard
```

#### Split Management
```
keybind = super+shift+a=new_split:down    # Create new split below
keybind = super+shift+y=new_split:right   # Create new split to the right
```

#### Window Controls
```
keybind = super+shift+n=toggle_quick_terminal  # Toggle quick terminal
keybind = super+shift+f=toggle_fullscreen     # Toggle fullscreen
keybind = super+shift+i=inspector:toggle      # Toggle inspector
keybind = super+shift+m=toggle_split_zoom     # Toggle split zoom
keybind = super+shift+r=reload_config         # Reload configuration
keybind = super+shift+s=write_screen_file:open # Save screen to file
keybind = super+shift+w=close_surface         # Close current window
```

### Other Settings
```
quit-after-last-window-closed = true    # Quit Ghostty when last window is closed
```

## Installation

1. Clone this repository to your Ghostty config directory:
```bash
git clone https://github.com/yourusername/ghostty-config ~/.config/ghostty
```

2. Restart Ghostty to apply the changes.

## Customization

To customize the configuration, edit the `config` file in this directory. Ghostty will automatically reload the configuration when changes are detected.

## License

MIT License
