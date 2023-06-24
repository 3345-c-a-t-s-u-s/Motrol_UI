# Motrol_UI
Library Of Motrol UI
# How To UI?

```lua
local MotrolUI = loadstring(game:HttpGet(("https://raw.githubusercontent.com/3345-c-a-t-s-u-s/Motrol_UI/main/source.lua")))()
```

## Creating a Window
```lua
local Window = MotrolUI:CreateWindow({
	Title = "String", -- Title <string>
	ToggleKey = Enum.KeyCode.X, -- Toggle Key <Keycode>
	ThemeColor3 = Color3.fromRGB(255, 0, 4), -- Theme Color <Color3 -  Default = Color3.fromRGB(45, 45, 45)>
	UseSound = false, -- sound effect <boolen - Default = false>
})
```
