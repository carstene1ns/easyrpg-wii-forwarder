# easyrpg-wii-forwarder
Loader part of the Wii EasyRPG Player Channel

## What it does / should do

- Initializes the Wii console and specifically GX (Video Output)
- Displays a nice background image with fadein
- Searches for connected devices (SD/USB)
- Tries to load the boot.dol/.elf from the devices in descending order:
  - /apps/easyrpg/
  - /easyrpg/
- fades to black and executes the found Player executable
- returns to the Homebrew Channel/System Menu if loading failed

## Compiling

- Setup DevkitPro, DevkitPPC, libogc, libfat and the png and z portlibs like usual
- execute `make`

The resulting boot.dol can be embedded in the loader channel's .wad using CustomizeMii.
