# openHASP-unofficial-firmwares
OpenHasp firmware for some boards not included in official releases page

I found out these affordable esp32 powered boards from Sunton, with a big size screen, touch interface, audio and sensors connectors...

Seller included some technical documentation and a few simple code samples. They worked but I wanted to use it for my Open Assistant installation.

Then, I discovered [the amazing OpenHASP project](https://github.com/HASwitchPlate/openHASP). 

OpenHasp releases a powerful firmware for some (quite expensive) smart screens with touchable interfaces. After some tests, author kindly included specific configuration files for Sunton boards, ~~but you need to download the source code, make a few adjustments and compile it in order to have your firmware ready to upload~~ and added these to the nightly builds. 

~~As some people asked me about this firmware, I have uploaded a ready to flash version to the releases page~~. 

https://github.com/HASwitchPlate/openHASP/actions/runs/3381121807#artifacts

Just dowload the needed *artifact*, and flash your board with your favourite tool.

For example:

esptool.py --port COM1 --baud 460800 write_flash 0x0 esp32-3248s035r_full_4MB_v0.6.3-dev_72224eb.bin
