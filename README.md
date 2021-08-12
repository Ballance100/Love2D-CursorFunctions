# What is CursorFunctions
### Cursor Functions allow you to check if the mouse is a certain area and/or clicking
### It can also scale the mouse position. This can be useful when using love.graphics.scale or libraries such as push
### It adds JoyCon support as well 






**Load the library**
```lua
local CursorFunctions = require("CursorFunctions")
```
# Setup
```lua
function love.load()
CursorFunctions.Settings(Scale,gameWidth,gameHeight,JoyStickMouseEnabled)
end
```
Scale:**Bool**
<br >gameWidth,gameHeight are used for scaling:**Int**
<br >JoyStickMouseEnabled is used to allow a gamepad to control the mouse:**Bool**</br >

# Is Clicked
### Area
#### Check if the Cursor is in a certain *area* and pressing a mouse button(Type). Can be used for making buttons etc
##### Returns true/false
```lua
CursorFunctions.IsClicked(Type,posX,posY,Width,Height)
```
<br >Type is what mouse button you want to use 1,2,3:**Int**</br >
PosX andPosY are int's of the postion of the object:**Int**</br >
Width and Height is the size of the object:**Int**
### Radius
#### Check if the Cursor is in a certain *radius* and pressing a mouse button(Type). Can be used for making buttons etc
```lua
CursorFunctions.IsClicked(Type,posX,posY,Radius)
```

# Joystick
```lua
function love.update()
CursorFunctions.UpdateCursor()
end
```
Make sure to add this in love.update or a while True loop


# License

```
MIT License

Copyright (c) 2021 Ballance100

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.


THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
