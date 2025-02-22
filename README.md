# touchOSC
These are tools and modules I developed for the [TouchOSC](https://hexler.net/touchosc) app. TouchOSC is a powerful surface builder with a LUA scripting api to process Midi and OSC messages.

## Animator
A tool to create animated layout transitions! You can setup up to 20 different layouts in your template and choose from a variety of animations to transit between them.
This is useful to support user preferences (layout mirroring, easy/advanced settings, vetical vs. horizontal layout etc.) but also to just make you template more vivid.
The Animator panel provides a simple visual interface to add and remove layouts and animations.    
For more details see the [description in the module folder](https://github.com/tshoppa/touchOSC/blob/main/modules/animator/).

<video src="https://github.com/user-attachments/assets/8604f81a-bb3c-431e-8af3-2e9240db9685" width = "66%"></video>
<img src="modules/animator/img/Animator.png" alt="TouchOSC Layout Animator" width="66%"/>

## Retro Segment and Dot display
A 7 segment display and a 5x7 dot display to bring the retro charme to your touchOSC template. 
For more details see the [description in the module folder](https://github.com/tshoppa/touchOSC/blob/main/modules/SegmentDisplay/).

<video src="https://github.com/user-attachments/assets/afd843cd-16c9-4058-ba14-b191283386a3"></video>
<video src="https://github.com/user-attachments/assets/d02941ce-0ade-4721-b964-2d1d904c736a"></video>

## Text Input
A dialog to edit text for labels, text controls or OSC messages.
It features lower and uppercase characters as well as a range of symbols. The keyboard layout is QUERTY (for characters, the symbols are more or less random).
For more details see the [description in the module folder](https://github.com/tshoppa/touchOSC/blob/main/modules/TextInputDialog/).

<img src="modules/TextInputDialog/img/Screenshot%20Keyboard.png" alt="Keyboard" width="66%"/>

## Color Picker
A dialog to select colors from an RGB color space representation (similar to the color selector in the touchOSC editor itself). 
I wanted colors in an app to be configurable by the user, but picking a color by changing individual RGB channels (e.g. by 3 separate faders) is quite tedious.
The color picker provides an intuitive WYSIWYG color selection aproach, faders for opacity and fine adjustment, a history of last selected colors and a grascale switch.  
For more details see the [description in the module folder](https://github.com/tshoppa/touchOSC/blob/main/modules/ColorPicker/).

<img src="modules/ColorPicker/img/Screenshot%20color%20picker%20history.png" alt="Color Picker" width="66%"/>

