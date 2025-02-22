# Retro Segment and Dot display
A 7 segment display and a 5x7 dot display for the retro charme of hardware devices in your touchOSC template. 

# Segment display
https://github.com/user-attachments/assets/d02941ce-0ade-4721-b964-2d1d904c736a

## usage
copy one of the 'Display' groups to your projects. To add more characters, enter the group and copy one of the 'Char' groups to the end of the display.
(make sure to always append new Chars to the very right, it's important for the order in which characters are set).

## api
strings and properties are set by calling 'notify(key,val)' on the Display via script. 

| Key   |      Val      |  Description | Example |
|-------|---------------|-------------|---------|
| set |  string or number | sets text | display:notify('set', 100)<br>display:notify('set', 'hello')|
| color | Color | sets color | display:notify('color', Colors.red) |
| setSize | 'x', 's', 'm', 'l' | sets one of 4 fixed sizes to match different layout dimensions | display:notify('setSize', 's') |
| scrollIn | {text = string, speed = number } | scrolls in a text from the right | display:notify('scrollIn', {text = 'hello', speed = 100}) |
| runText | {text = string, speed = number } | scrolls a text repeatedly through the display | display:notify('runText', {text = 'hello', speed = 100}) |
| haltRunText | boolean | stops (true) or continues(false) a running text | display:notify('haltRunText', true) |
| speed | number | sets the speed of a running text | display:notify('speed', 80) |

# Dot display
https://github.com/user-attachments/assets/afd843cd-16c9-4058-ba14-b191283386a3


