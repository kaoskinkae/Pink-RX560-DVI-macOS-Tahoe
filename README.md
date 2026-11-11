# Pink-RX560-DVI-macOS-Tahoe



##The solution to the Pink DVI output color issue on Radeon RX 560 may work on other Polaris cards.

We need the "patch-edit.rb" script; running it as an administrator will create a folder containing the full configuration for the connected monitors—in my case, LG-DVI and HDMI—within the active user's folder.

Now, for the "DisplayVendorID-xxxx" folder, place it inside your Downloads folder, within a folder you create and name "Overrides."

Run two commands from the terminal, and it will copy this to the correct location.

##sudo mkdir -p /Library/Displays/Contents/Resources/Overrides

##sudo ditto ~/Downloads/Overrides /Library/Displays/Contents/Resources/Overrides

It is important that the folder be placed inside the newly created folder named "Overrides".

Let’s restart. It is important that, throughout the entire process, a monitor or television with a DVI connection remains connected. We can verify this using version 5.0.9 of the Hackintool application.

Once we restart, the monitor or television will no longer have that annoying pink tint.
