This is an example based on the littlefs Zephyr test code.

It attempts to mount two littlefs file systems defined in the external flash on a nRF52840DK.

The master branch works when built with NCS 2.6.1 or 2.7.0 but fails when built with 2.8.0 or later.

It also fails to work as expected if mcuboot is enabled for any build.  There are two branches, mcuboot.2.6.1 and mcuboot.3.2.1 that demonstrate this.

To build, open the project in VS Code with the nRF Connect for VS Code extension pack.  Then open a VCOM0 connection to the nRF52840DK and reset the board.