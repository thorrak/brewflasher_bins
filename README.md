# brewflasher_bins - Cached, compiled bootloaders for ESP32

These are cached versions of the bootloader binaries as compiled by Espressif in conjunction with each release of the
Arduino package. These binaries are only included in the tagged "release" versions of the Arduino package, and are not
included in the master branch. 

These binaries can be found, for example, here: https://github.com/espressif/arduino-esp32/tree/2.0.14/tools/sdk

The .elf files are available in each controller's folder: https://github.com/espressif/arduino-esp32/tree/2.0.14/tools/sdk/esp32s3/bin

The .elf files then need to be converted to bin files using esptool: `esptool.py --chip ESP32S3 elf2image bootloader_dio_80m.elf`

The resulting bin files are then included in this repo.

