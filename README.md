# Keyboard-Firmware

## Setup

Clone vial-qmk and run QMK setup.
Clone this repo and cd into it.

```bash

# Get firmware directory
export $(qmk env | grep QMK_FIRMWARE | tr -d \")

# Create symlink
ln -s $(realpath .)/ $QMK_FIRMWARE/keyboards/custom

```

Firmware can now be compiled with `qmk compile -kb custom/<keyboard name> -km vial`
