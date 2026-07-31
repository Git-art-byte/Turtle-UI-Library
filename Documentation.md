# Documentation

## Library
```lua
local TurtleLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/Git-art-byte/Turtle-UI-Library/refs/heads/main/Turtle.luau"))()
```

## Window
```lua
local Window = TurtleLib:Window("My Awesome Hub")
```

## Keybind
```lua
TurtleLib:Keybind("RightShift")
```

## Buttons
```lua
Window:Button("Button Name",
 function()
    print("Hello")
end)
```

## Labels
```lua
Window:Label("This is a label")
```

## Toggles
```lua
Window:Toggle("Toggle Name", false, function(state)
    print("Toggle is now:", state)
end)
```

## TextBox
```lua
Window:Box("Background Text",
 function(text, focused)
    if focused then
        print("Final input:", text)
    else
        print("Live typing:", text)
    end
end)
```

## Sliders
```lua
local volumeSlider = Window:Slider(
    "Volume",                          
    0, -- Minimum Value                          
    100, -- Maximum Value                             
    16, -- Default Value                              
    function(value)                    
        print("Volume set to:", value)
    end
)
```

## Dropdown
```lua
local classDropdown = Window:Dropdown(
    "Select Class", -- Dropdown Name
    { "Warrior", "Mage", "Rogue" },     -- list of options
    function(choice)                   
        print("You picked:", choice)
    end,
    true                               
)
```

## Color Picker
```lua
local colorPicker = Window:ColorPicker(
    "Theme Color",
    Color3.fromRGB(255, 100, 50),
    function(color, isRainbow)
        if isRainbow then
            print("Rainbow mode enabled!")
        else
            print("Color changed to:", color)
        end
    end
)
```

## GUI Visibility
```lua
TurtleLib:Hide()
```
## Destroy GUI
```lua
TurtleLib:Destroy()
```
