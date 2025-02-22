# Retro Segment and Dot display
A 7 segment display and a 5x7 dot display for the retro charme of hardware devices in your touchOSC template. 

# Segment display
https://github.com/user-attachments/assets/d02941ce-0ade-4721-b964-2d1d904c736a

## usage
copy one of the 'Display' groups to your projects. To add more characters, enter the group and copy one of the 'Char' groups to the end of the display.
(make sure to always append new Chars to the very right, it's important for the order in which characters are set). 
Remove characters also from the right.

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

## usage
copy one of the 'Display' groups to your projects. To add more characters, enter the group and copy one of the 'Char' groups to the end of the display.
(make sure to always append new Chars to the very right, it's important for the order in which characters are set).
Remove characters also from the right.

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
| shape | [shape enumeration](https://hexler.net/touchosc/manual/script-enumerations#shape) | sets the shape of each dot | display:notify('shape', Shape.CIRCLE) |
| invert | boolean | inverts the dot matrix on/off color | display:notify('invert', true) |

## character editor
you can add more characters by expanding the 'codes' table at the top of a Char group script. A character is defined by 5x7 numbers, where 0 represents an off and 1 an on dot.
To expand all Chars of a display, remove all Chars but one, edit the remaining Char and copy and paste it to fill the display again. Remember to always copy to the end of the row.

You can use the Character Editor on the lower right of the template to create the matrix code (note, that this currently only works on desktop versions of touchOSC):  
  - open the log console (Ctrl/Cmd + Shift + L or menu 'View'/'Toggle Log') and switch to Script tab.
  - run the template
  - draw new character by selecting dots in the 5x7 matrix
  - when done, press 'print'
  - copy code from the log console to the codes table
