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

## Animator
A tool to create animated layout transitions! You can setup up to 20 different layouts in your template and choose from a variety of animations to transit between them.
This is usefull to support user preferences (layout mirroring, easy/advanced settings, vetical vs. horizontal layout etc.) but also to just make you template more vivid.
For more details see the [description in the module folder](https://github.com/tshoppa/touchOSC/blob/main/modules/animator/Readme.md).

<video src="https://github.com/user-attachments/assets/8604f81a-bb3c-431e-8af3-2e9240db9685"></video>
<img src="modules/animator/img/Animator.png" alt="TouchOSC Layout Animator" width="66%"/>
