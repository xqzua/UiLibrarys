# Discord Lib

Boot the Discord library
```lua
local DiscordLib = loadstring(game:HttpGet"https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt")()
```
Window
```lua
local win = DiscordLib:Window("discord library")
```
Server/Tab
```lua
local serv = win:Server("Preview", "")
```
Channel
```lua
local Tab = serv:Channel("Buttons")
```
Button
```lua
Tab:Button("print", function()
print("this is a print.")
end)
```
Seperator
```lua
Tab:Seperator()
```
Toggle
```lua
Tab:Toggle("toggle",false, function(bool)
print(bool)
end)
```
Sliders
```lua
local Tab = Tab:Slider("Slide me!", 0, 1000, 400, function(t)
print(t)
end)
```
Drop down
```lua
local drop = Tab:Dropdown("Pick me!",{"Option 1","Option 2","Option 3","Option 4","Option 5"}, function(bool)
print(bool)
end)
```
TextBox
```lua
Tab:Textbox("Gun power", "Type here!", true, function(t)
print(t)
end)
```
Label
```lua
Tab:Label("This is just a label.")
```
Bind
```lua
Tab:Bind("kill", Enum.KeyCode.RightShift, function()
print("Killed everyone!")
end)
```
