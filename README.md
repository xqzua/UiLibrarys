# Boot lib
```lua
local DiscordLib = loadstring(game:HttpGet"https://raw.githubusercontent.com/dawid-scripts/UI-Libs/main/discord%20lib.txt")()
```
Title
```lua
local win = DiscordLib:Window("discord library")
```
Server/Tab
```lua
local serv = win:Server("Server", "")
```
Channels
```lua
local chs = serv:Channel("Channel")
```
Button
```lua
chs:Button("print", function()
print("hello world")
end)
```
Seperator
```lua
chs:Seperator()
```
Toggle
```lua
chs:Toggle("Toggle",false, function(bool)
print(bool)
end)
```
Sliders
```lua
local chs = sldrs:Slider("Slide me!", 0, 1000, 400, function(t)
print(t)
end)
```
Drop Down
```lua
local chs = drops:Dropdown("Pick me!",{"Option 1","Option 2","Option 3","Option 4","Option 5"}, function(bool)
print(bool)
end)
```
TextBox
```lua
chs:Textbox("Gun power", "Type here!", true, function(t)
print(t)
end)
```
Label
```lua
chs:Label("This is just a label.")
```
Keybind
```lua
bnds:Bind("Kill bind", Enum.KeyCode.RightShift, function()
print("Killed everyone!")
end)
```
