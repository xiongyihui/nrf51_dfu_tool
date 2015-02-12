nRF51 DFU Tool
==============

The tool is for nRF51822 OTA (Over The Air, SoftDevice 7.0.0).
It's based on https://bitbucket.org/glennrub/nrf51_dfu_linux/src.

## Requirements
+ [DFU bootloader](https://github.com/Seeed-Studio/nrf51_dfu_bootloader)
+ Bluez (tested with V4.101)
+ python intelhex library


## Usage
```
sudo hcitool lescan -i hci0   # Get target's address
python dfu.py -f new_firmware.hex -a F9:6C:59:06:AF:27
```
