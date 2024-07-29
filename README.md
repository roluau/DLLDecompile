# DLLDecompile Script

## Description

The `DLLDecompile` script is a Lua script designed for Roblox. It allows you to **save and decompile** game instances from various parts of a Roblox game. This tool is ideal for developers and researchers who need to **inspect, back up**, or **analyze** game data with customizable options for how the data is processed.

## Features

- **Customizable Options**: Configure how instances are saved and processed. ⚙️
- **Decompile**: Option to decompile the saved data. 🔄
- **Extra Instances**: Include additional instances in the decompilation. 📂
- **Anonymous**: Save data without revealing personal information. 🤫
- **Treat Unions As Parts**: Decide whether unions are treated as individual parts. 🧩

## Usage

1. **Load the Script**
   ```lua
local dlldecompile = loadstring(game:HttpGet("https://raw.githubusercontent.com/roluau/DLLDecompile/main/dlldecompile.luau", true), "dlldecompile")()
local config = {
    mode = "custom",  -- Set the mode of operation
    ExtraInstances = {  -- List of instances to include
        game.workspace,
        game.ReplicatedStorage,
        game.Lighting,
        game.ReplicatedFirst,
        game.StarterPack,
        game.Players,
        game.StarterPlayer,
        game.StarterGui,
        game.Teams
    },
    Decompile = true,  -- Enable decompiling
    decomptype = "custom",  -- Type of decompilation
    noscripts = false,  -- Exclude scripts
    Anonymous = true,  -- Save anonymously
    TreatUnionsAsParts = true,  -- Handle unions as parts
    RemovePlayerCharacters = false,  -- Keep player characters
    IsolateLocalPlayerCharacter = true  -- Isolate local player character
}
dlldecompile(config)
   ```

## Disclaimer

📢 **Important**: This script was originally created by @dll_inject(textbox).  
⚠️ **Do Not** claim ownership or authorship of this script.  
🔍 The original creator invested significant effort into developing and sharing this tool.  
🛡️ **Respect** intellectual property and acknowledge the original creator.  
🚫 **Unauthorized** copying or claiming this script as your own is prohibited.  
🔗 Always refer to the [original source](https://raw.githubusercontent.com/roluau/DLLDecompile/main/dlldecompile.luau) for updates.  
👏 Thank you for your respect and cooperation.  
✨ **Happy scripting**! Enjoy using the script responsibly! 🌟
