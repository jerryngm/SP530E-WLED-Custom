###WLED Build For SP530E

Download custom_build.bin  
Download ESPtool [Here](https://github.com/espressif/esptool/releases)  
Download C3_bootloader.bin and C3_partitions_4M.bin [Here](https://github.com/Aircoookie/WLED/releases/tag/v0.15.0-b2)  
  
  
Connect UART Cable to board reverse side  
#Use this Command below to backup the original firmware.  

#Use this Command below to flash the firmware.  
esptool.py write_flash --encrypt 0x0 C3_bootloader.bin 0x8000 C3_partitions_4M.bin 0x10000 custom_build.bin
