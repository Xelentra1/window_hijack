# Window Hijack
Rendering on external windows via hijacking thread contexts.
You can read a full write-up at: https://secret.club/2020/05/12/abusing-compositions.html

## Usage
If you plan on manual mapping this driver, or using it on a game with an anti-cheat then you'll need to make some modifications, these are left for you to do.

To use the project as-is:

1. Enable test-signing mode
2. Compile in Release x64
3. Load the driver using any traditional driver loader
4. Start window_hijack_cli using the following pattern: `window_hijack_cli.exe [window_class_name]`

## Credits
paracord (yousif), IChooseYou

## Changes
Added notes to what is necessary for this to work inside of a manually mapped driver, and describes why it only works in the IOCTL handler.

The notes can be located in window_hijack\includes\dispatch\control.cpp.
