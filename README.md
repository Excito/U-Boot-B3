This is adapted 2013.01.01 U-Boot sources for the Excito B3 board.

Please note that this release changes the color used during u-boot phase (bootloader) of the B3 :

* White is used during normal startup
* Yellow is used during usb (install/rescue) startup with power button pressed

This allows easier boot problem identification.

To compile it issue the following commands on the cloned repository directly on the B3 (do not try to cross-compile) :

```
make bubba3_config
make -j2 u-boot.kwb
```
