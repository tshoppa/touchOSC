ColorPicker comes in 4 variations:

-**colorpicker.tosc** the vanilla version with the most common functionality
-**colorpicker swatches.tosc** colorpicker with an additional history of previously selected colors
-**colorpicker small.tosc** a small sized colorpicker
-**colorpicker min.tosc** super compact colorpicker (but least comfortable to use)

Each tosc file will contain the according colorpicker component as well as a usage demo

# Instalation
To use the colorpicker in your layout, open the .tosc file and copy the 'ColorPicker' group to your project (it is locked by default, so you will have to unlock it before copying)
Make sure the colorpicker group is in front of all other controls to make it appear as a modal dialog when activated.

The group also contains a dialog pane that greys out the user interface  while the dialog is in use. Therefore resizeand move the ColorPicker to cover your complete document.
Finally, enter the group and move the dialog to where it should appear (usually in the center).

# Usage
ColorPicker is activated by script

```
ColorPicker:notify( 'pickColor', {
    receiver:   receiveingControl,
    callback:   aCallbackControl,
    initial:    anInitialColor
})
```

you can either sepcify a **receiver** control, which will directly receive the selected color when the dialog is closed with "ok".
Alternatively, you can set a **callback** component that will be notified with "colorPicked" and the new color, or with "colorPickCanceled" when the dialog is closed with "cancel".

You can optionally specify an **initial** color that will be set as the current color when the dialog is shown.

**Note**: Clicking the dialog pane will also close the dialog (as "cancel")
