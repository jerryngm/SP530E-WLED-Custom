WLED Build For SP530E

Download custom_build.bin  
Download ESPtool [Here](https://github.com/espressif/esptool/releases)  
Download C3_bootloader.bin and C3_partitions_4M.bin  
  
Use this Command below.  

esptool.py write_flash --encrypt 0x0 C3_bootloader.bin 0x8000 C3_partitions_4M.bin 0x10000 custom_build.bin
