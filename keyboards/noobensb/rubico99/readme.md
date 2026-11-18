# Rubico99

A 99-key compact full-size keyboard PCB with Vial support.

* Keyboard Maintainer: [Henryk Zaborowski](https://github.com/henryk-zaborowski)
* Hardware Supported: Rubico99 PCB (STM32F072CBT6)

Make example for this keyboard (after setting up your build environment):

    make noobensb/rubico99:vial

Flashing example for this keyboard:

    make noobensb/rubico99:vial:flash

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

Enter the bootloader in 3 ways:

* **Bootmagic reset**: Hold down the key at (0,0) in the matrix (Esc) and plug in the keyboard
* **Physical reset button**: Press the button on the back of the PCB (SW901) - it pulls BOOT0 high and resets the MCU
* **Keycode in layout**: Press the key mapped to `QK_BOOT` (Fn + Esc in the default keymap)
