# 0xAlok's Dotfiles

My personal configuration files managed with [GNU Stow](https://www.gnu.org/software/stow/).

## Setup

- **OS**: Arch Linux (Omarchy)
- **WM**: Hyprland
- **Terminal**: Ghostty
- **Editor**: Neovim 
- **Shell Prompt**: Starship
- **Status Bar**: Waybar
- **Launcher**: Walker
- **System Monitor**: Btop
- **System Info**: Fastfetch

## 📦 Modules

- `ghostty` - Terminal emulator configuration
- `nvim` - Neovim setup with LazyVim
- `hypr` - Hyprland window manager with keybindings and shaders
- `waybar` - Status bar styling and modules
- `starship` - Shell prompt customization
- `fastfetch` - System information display
- `btop` - System resource monitor theme
- `walker` - Application launcher config

## Installation

1. **Clone this repository:**
   ```bash
   git clone https://github.com/0xAlok/dotfiles.git ~/dotfiles
   cd ~/dotfiles
   ```

2. **Install GNU Stow:**
   ```bash
   sudo pacman -S stow  # Arch/Omarchy
   ```

3. **Use Stow to symlink configs:**
   ```bash
   # Install individual modules
   stow ghostty
   stow nvim
   stow hypr
   stow waybar
   stow starship
   stow fastfetch
   stow btop
   stow walker
   
   # Or install everything at once
   stow */
   ```

4. **Reload your configuration:**
   ```bash
   hyprctl reload  # For Hyprland
   ```

## Updating Configs

After making changes to any config:

```bash
cd ~/dotfiles
git add .
git commit -m "Description of changes"
git push
```
