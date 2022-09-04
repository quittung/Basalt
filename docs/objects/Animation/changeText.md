## changeText
Changes the text while animation is running

#### Parameters: 
1. `table` multiple text strings - example: {"i", "am", "groot"}
2. `number` duration in seconds
3. `number` time - time when this part should begin (offset to when the animation starts - default 0)

#### Returns: 
1. `animation` Animation in use

#### Usage:

```lua
local mainFrame = basalt.createFrame()
local testButton = mainFrame:addButton("buttonToAnimate")
local aAnimation = mainFrame:addAnimation():setObject(testButton):changeText({"i", "am", "groot"}, 2):play()
```
```xml
<animation object="buttonToAnimate" play="true">
    <text>
        <text>i</text>
        <text>am</text>
        <text>groot</text>
        <duration>2</duration>
    </text>
</animation>
```