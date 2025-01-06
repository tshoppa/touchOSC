TextInputDialog.tosc contains the actual keyboard component and a demo.

![image of keyboard](https://github.com/tshoppa/touchOSC/blob/main/modules/TextInputDialog/img/Screenshot%20Keyboard.png)

# Instalation
To use the TextInputDialog in your touchOSC layout, open TextInputDialog.tosc and copy the group "TextInput" to your project (The group is locked by default, so you will have to unlock it)
Make sure the TextInput is in front of all other control elements so that will appear as a modal dialog when activated. 

# Usage
TextInput is activated by script:
```
TextInput:notify( 'showTextDialog', {
    receiver:      receiveingControl,
    callback:      aCallbackControl,
    initialText:   anInitialText,
    maxTextLength: aTextLengthInteger,
    advice:        anAdviceString
})
```
There are 2 ways to process the result of a TextInput operation. You can either specify a receiver or a callback.

**receiver** a label or text control that will directly receive the text when the dialog is closed with "ok".\
**callback** a control, that will be notified with "heresYourText" and the text value when the dialog is closed with "ok". If the dialog is closed with "cancel", the control will be nitified with "textDialogCanceled".

You can also use both methods at once (e.g. if you just want to react on cancel in the script)

other (optional) parameters:\
**initialText** will be shown in the textbox of the TextInput\
**maxTextLength** max number of characters the TextInput will accept\
**advice** the advice string at the top of the dialog ("please enter a text")\
