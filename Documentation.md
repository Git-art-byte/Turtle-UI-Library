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
Window:Button("Print Hello",
 function()
    print("Hello")
end)
```

## Labels
```lua
Window:Label("This is a label")

Window:Label("This is a rainbow label", true)
```
