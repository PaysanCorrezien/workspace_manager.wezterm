# 🖥️ WezTerm Workspace Manager Plugin

An extension to [smart_workspace_switcher.wezterm](https://github.com/MLFlexer/smart_workspace_switcher.wezterm) that adds pane management capabilities for WezTerm.
It also allow renaming

## ⭐ Features

- 🔄 Switch between panes across workspaces
- ✏️ Rename workspaces on the fly
- 📑 Create or switch to workspaces
- 🔍 Fuzzy search support for all selectors
- 🏷️ Detailed labeling with Nerd Font icons

## 🚀 Installation

```lua
local wez = require('wezterm')
local workspace_manager = wez.plugin.require("https://github.com/PaysanCorrezien/workspace_manager.wezterm")
```

## 💡 Usage

Add to your WezTerm configuration:

```lua
local config = {
  keys = {
    -- Quick pane switcher
    {
      key = "f",
      mods = "LEADER",
      action = workspace_manager.SwitchPanes(),
    },
    -- Rename workspace
    {
      key = "r",
      mods = "LEADER",
      action = workspace_manager.RenameWorkspace(),
    },
  }
}
```

### Navigation

- Use number keys (1-9) for quick selection
- Press `/` to activate fuzzy search
- `ESC` to cancel

## 🤝 Contributing

Contributions are welcome! Please note:

- This project is maintained as time permits
- Focus on meaningful improvements that don't add unnecessary complexity

## 📝 Credits

MLFlexer for the original [smart_workspace_switcher.wezterm](https://github.com/MLFlexer/smart_workspace_switcher.wezterm)

## 📄 License

This project follows the MIT License conventions. Feel free to use, modify, and distribute as per MIT License terms.
