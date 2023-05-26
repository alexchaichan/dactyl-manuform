This ist a fork of [abstracthat/dactyl-manuform](https://github.com/abstracthat/dactyl-manuform) while this is a fork of [adereth/dactyl-keyboard](https://github.com/adereth/dactyl-keyboard)


## Hot Swap Sockets

https://github.com/stingray127/handwirehotswap/tree/main/Matrix

# Switches [GAMAKAY MECHANICAL SILENT SWITCHES (Pegasus)](https://gamakay.com/products/gamakay-35pcs-pack-gamakay-switch-linear-mechanical-phoenix-crystal-bumblebee-switch-prelubricate-keyboard-switch-for-diy-mechanical-gaming-keyboards?variant=42678166683837)



# Keycaps

# Material List

# Flashing

[qmk](https://qmk.fm/)

[Online Configurator](https://config.qmk.fm/)

```
# installing qmk
if [[ "$(uname)" == "Darwin" ]]; then
    brew tap qmk/qmk
    brew install qmk
elif [[ "$(expr substr $(uname -s) 1 5)" == "Linux" ]]; then
    sudo pacman -S qmk
fi

# creating the firmware-repositorie
qmk setup
# git clone https://github.com/qmk/qmk_firmware

# navigate into firmware-directory
cd ~/qmk_firmware

# compile the firmware .hex file
qmk compile -kb handwired/dactyl_manuform/5x6 -km custom
```

- Plug the USB cable into the left half of the Dactyl.
- Push the hardware *reset* button.
- Run `qmk flash -kb handwired/dactyl_manuform/5x6 -km custom`
- Unplug the cable, and plug it into the right half. Follow the same instructions above.
- Unplug the cable, and plug it back into the left half. You’re done!

___

[keyboard tester](https://www.keyboardtester.com/tester.html)

# License

Copyright © 2015-2017 Matthew Adereth and Tom Short

The source code for generating the models (everything excluding the [things/](things/) and [resources/](resources/) directories is distributed under the [GNU AFFERO GENERAL PUBLIC LICENSE Version 3](LICENSE).

The generated models and PCB designs are distributed under the [Creative Commons Attribution-NonCommercial-ShareAlike License Version 3.0](LICENSE-models).

