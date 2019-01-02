# Notes CC3100 related IT products

## Uniflash 3.4

Uniflash 3.4 is tools to program CC3100 flash memory.

- [Uniflash Download page](http://www.ti.com/tool/UniFlash)
- [CC3100 & CC3200 UniFlash Quick Start Guide](http://processors.wiki.ti.com/index.php/CC3100_%26_CC3200_UniFlash_Quick_Start_Guide)
- [CC3100 & CC3200 UniFlash Full User Guide](http://processors.wiki.ti.com/index.php/CC3100_%26_CC3200_UniFlash)
- Uniflash 3.4 + CC3100, correct the 3d COM port ([ti thread](https://e2e.ti.com/support/wireless-connectivity/wifi/f/968/p/758725/2803061#2803061))

## Definitions

**SimpleLink** (a.k.a SimpleLink Driver) - the driver for controlling CC3100 by SPI interface. Its hardware-independent code is placed `C:\TI\CC3100SDK_X.X.X\cc3100-sdk\simplelink`. In the `include\simplelink.h` there is variable `SL_DRIVER_VERSION`, which defined version of driver.

**SimpleLink Studio** - the porting of SimpleLink Driver on Windows OS (Windows 7/8/10 tested) to test examples with `CC3100BOOST+CC31XXEMUBOOST+(PC as MCU)` configuration.

**Service Pack** - CC3100 firmware. Closed TI binary, updating with UniFlash 3.4 (for CC3100)

## ServicePack version schema

The last versions of ServicePack have the schema `X.X.X.X-B.B.B.B`, where
- `X.X.X.X` is `SL_HOST_DRIVER_VERSION` from `simplelink.h`
- `B.B.B.B` is actual version of NWP firmware

Inside the `readme.txt` of ServicePAck there is example results of `sl_DevGet() + SL_DEVICE_GENERAL_VERSION` with corresponding SDK.

- **More detailed version see on the [separate page](./versions.md)**