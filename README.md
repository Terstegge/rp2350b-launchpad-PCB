# RP2350B-Launchpad PCB

This repository contains the KiCad design files for a TI-style Launchpad board
with the RP2350B microcontroller. The board features a build-in picoprobe
debugger, which signals UART RX/TX and SWD activity with 3 LEDs. The unused
GPIO pins of the picoprobe are connected to a header, which could be used
in the future for more functionality like a simple logic analyzer etc.

The target RP2350B controller has 2 connected pushbuttons, one normal LED and
8 WS2812-2020 LEDs as input/output. Some signals are also available on a
horizonal header at the lower end of the PCB, which is used to connect WLAN or
Bluetooth boards like WifiTick. The RP2350B uses a 8 MiB flash chip and an
additional 8 MiB PSRAM chip. The board also has a button to enable programming
via the target USB port (mass storage device). Normally this button is
not needed, because all programming and debugging of the target is performed
via the picoprobe using openocd and gdb.

The board also contains a LiPo-charger to enable battery-powered projects.

Why was this board designed? I have been using the MSP432 Launchpad from TI for
quite a while in university classes teaching microcontroller technology.
Unfortunately TI has stopped producing all MSP432-related products. Still we
have purchased lots of TI boosterpack-boards like the Educational Boosterpack MK II.
The be able to used these Boosterpacks also in the future, a new Launchpad had
to be found. The RP2350B is a very interesting microcontroller, and, what is
quite important for educational purposes, it has excellent documentation.
So this board came to life. As far as I know this is the only RP2350 board
which includes a picoprobe debugger.

There are no pictures yet because the boards has not been produced so far.
