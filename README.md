# TyK380v2 - A Logitech K380s based custom membrane keyboard

This project uses the Logitech Pebble Keys 2 K380s (further on called K380v2)
keyboard as a hardware platform to build a custom programmable wireless membrane
keyboard based on ZMK.

This is the upgraded revision from my [original TyK380][original-git] using the
newest revision of the K380 by Logitech.

## Features

- Bluetooth
- LEDs
- 2x AAA batteries
- ZMK
  - multiple device profiles
  - long-lasting battery
  - custom keyboard layout (i.e. Dvorak, …)
  - and all the other features that ZMK provides

## Do we need custom hardware?

This time around the answer is luckily no. The K380v2 upgrades the internal
microcontroller to an nRF52832, which can intentionally be unlocked / repurposed. Now
we only require attaching an SWD debugger (i.e. STLink Clones) to the internal PCB
and can flash our own firmware on there.

Although note that this keyboard doesn't support the extended features of the
original TyK380 replacement PCB like LiPo charging or USB. So give that project a
visit if you want that.

## The mod

This time around the mod is only software based, but it still requires us to open up
the keyboard in order to attach our debugger to the specified ports.

> [!WARNING]
> This section is still ToDo. See the `PROGRAMMING.md` document for information how to 
> unlock the chip. Better documentation will arrive over time.


[original-git]: https://github.com/tyalie/TyK380-keyboard
