# vuetify-dialog-virtual-keyboard

This simple example shows how a Vuetify Dialog does not reposition itself on mobile to accomodate the virtual keyboard that shows up when focusing on a text element.

To see this problem in action, build and view this app on a mobile phone. Open the dialog and you should see that the virtual keyboard shows up, blocking part of the dialog. The effect is worse in full-screen mode if you have card actions, as they are always hidden at the bottom of the screen, under the virtual keyboard.

The showing of the virtual keyboard also make the page underneath the scrim scrollable.
