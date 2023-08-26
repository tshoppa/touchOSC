# touchOSC
These are 2 dialogs I developed for an application that needed more user interaction than touchOSC surfaces usually do.

## Text Input
A dialog to enter a text. I needed it to name sound patches to be saved in an external synth.
It features lower and uppercase characters as well as a range of symbols. The keyboard layout is QUERTY (for characters, the symbols are more or less random).
For more details see the [description in the module folder](https://github.com/tshoppa/touchOSC/blob/main/modules/TextInputDialog/README.md).

<img src="modules/TextInputDialog/img/Screenshot%20Keyboard.png" alt="Keyboard" width="66%"/>

## Color Picker
A dialog to select colors from an RGB color space representation (similar to the color selector in the touchOSC editor itself). 
I wanted colors in an app to be configurable by the user, but picking a color by changing individual RGB channels (e.g. by 3 separate faders) is quite tedious.
The color picker provides an intuitive WYSIWYG color selection aproach, faders for opacity and fine adjustment, a history of last selected colors and a grascale switch.  
For more details see the [description in the module folder](https://github.com/tshoppa/touchOSC/blob/main/modules/ColorPicker/README.md).

<img src="modules/ColorPicker/img/Screenshot%20color%20picker%20history.png" alt="Color Picker" width="66%"/>
