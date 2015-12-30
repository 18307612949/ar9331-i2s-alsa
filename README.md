# ar9331-i2s-alsa
I2S alsa device drivers for the popular MIPS ar9331 SOC (Carambola2, Arduino Yun...)

It is implemented as a openwrt package and can be compiled with Linux Kernel Ver. 3.14.xx.

增加了ar9331对于wm8918(wm8904)的支持
注意：因为ar9331里面没有i2c控制器，所以我修改了mach-ap121.c文件，里面增加gpio-i2c，
SDA = gpio17
SCL = gpio11
