# Motrol_UI
Library Of Motrol UI

# How To Use UI?

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
## Creating a Tab
```lua
local Tab = Window:NewTab("Title") -- <string>
```

## Creating a Label
```lua
local Label = Tab:AddLabel("Label") -- <string>

-- option --
Label:ChangeLabel("New Label") -- <string>
```

## Creating a Button
```lua
local Button = Tab:AddButton({
	Title = "string";
	callback = function()
		
	end,
})

-- option --
Button:ChangeCallback(function()
	
end)

Button:ChangeTitle("New Title")
```

## Creating a Toggle
```lua
local Toggle = Tab:AddToggle({
	Title = "string";
	Default = false; -- <boolen>
	callback = function(boolen)
		
	end,
})

-- option --
Toggle:ChangeToggle(true) -- change to true or false <boolen>

Toggle:ChangeLabel("New Label") -- change Label <string>

Toggle:ChangeCallback(function(boolen) -- change callback <function>
	
end)
```

## Creating a Dropdown
```lua
local Dropdown = Tab:AddDropDown({
	Title = "srting";
	ListValue = {"1","2","3"}; -- table <string>
	callback = function(name)
		
	end,
})

-- option --

Dropdown:ChangeTitle("New Title")

Dropdown:ChangeCallback(function(name)
	
end)

Dropdown:Refresh()

Dropdown:ChangeList({"5","6","7"})
```

## Creating a Slider
```lua
local Slider = Tab:AddSlider({
	Title = "srting";
	Min = 0;
	Max = 100;
	Increment = 1;
	Callback = function(number)
		
	end,
})

-- option --

Slider:ChangeTitle("New Title")

Slider:ChangeConfix({
	Title = "new srting";
	Min = 50;
	Max = 150;
	Increment = 2;
	Callback = function(number)

	end,
})
```

## Another functions
```lua
Window:Custom({WindowSize = UDim2.new(<custom - Default = UDim2.new(0.45,0,0.45,0)>)})
```
