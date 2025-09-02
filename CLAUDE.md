# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a configuration repository for the Ghostty terminal emulator. It contains terminal customization settings including fonts, themes, keybindings, and window behavior.

## Key Files

- `config` - Main Ghostty configuration file using key-value format with `=` delimiter
- `README.md` - Documentation of all configuration options and keybindings

## Configuration Format

The config file uses plain text format:
```
# Comments start with #
setting-name = value
```

Settings are organized into categories:
- Fonts
- Theme
- Mouse
- Window
- Keybindings
- Other

## Common Tasks

### Modifying Settings
When updating configuration:
1. Edit the `config` file directly
2. Settings take effect when Ghostty is restarted
3. Use exact setting names as documented in Ghostty's documentation

### Keybinding Conventions
- The config clears default keybindings first with `keybind = clear`
- Split navigation uses `shift+ctrl` prefix
- Most other operations use `super+shift` prefix
- Format: `keybind = modifier+key=action`

## Important Notes

- This is a macOS configuration (uses `super` key modifier)
- The repository tracks personal preferences - be careful about changing defaults
- No build or test commands - changes are applied by restarting Ghostty
- Check README.md for detailed explanations of each keybinding action
