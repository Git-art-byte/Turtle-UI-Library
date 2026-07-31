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
    100,                               
    16,                                
    function(value)                    
        print("Volume set to:", value)
    end
)
```
