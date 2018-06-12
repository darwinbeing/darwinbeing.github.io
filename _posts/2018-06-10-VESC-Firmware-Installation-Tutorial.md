---
layout: post
title:  "VESC/VESC6 Firmware Installation Tutorial"
permalink: /:title
date:   2018-06-10 00:00:00
author: LI Tao
images:
  - assets/images/vesc/vesc.jpg
excerpt:
  "This article is simply a straight forward tutorial on how to install firmware onto a VESC under macOS."

categories: [VESC]
tags: [VESC]
---

[//]: # (Image References)
[image1]: assets/images/vesc/stlink.jpg "stlink"
[image2]: assets/images/vesc/stlink2.jpg "stlink2"
[image3]: assets/images/vesc/vesc.jpg "vesc"
[image4]: assets/images/vesc/vesc-setup.jpg "vesc setup"

This thread is simply a straight forward tutorial on how to install firmware onto a VESC. I have bought a clone of [VESC6 on taobao/aliexpress](https://item.taobao.com/item.htm?id=568914049411), but it should work for any VESC that does not have firmware installed.

**Prepare STLINK**  
Purchase a ST-Link V2 and a 6-pin JST-PH 2mm female header and cables, i have soldered a micro-jst cable, connect the JST and ST-Link together like in the image below.
![alt text][image1]
![alt text][image2]

**Connect USB**  
Plug the ST Link into a USB port of my MacBook Pro. The NiMH/LiPo Battery is NOT connected during the entire process of flashing firmware.
![alt text][image3]
![alt text][image4]

**PREPARATIONS**  
Downloading ARM GCC and installing openocd  
Mac OS X 64-bit
File:[gcc-arm-none-eabi-6-2017-q1-update-mac.tar.bz2](https://developer.arm.com/-/media/Files/downloads/gnu-rm/6_1-2017q1/gcc-arm-none-eabi-6-2017-q1-update-mac.tar.bz2?revision=ae959db1-d164-4f18-be04-771bdf152cd5?product=Downloads,64-bit,,Mac%20OS%20X,6-2017-q1-update)

```
brew install openocd
tar -xvjf gcc-arm-none-eabi-7-2017-q4-major-mac.tar.bz2 -C ~
export PATH=~/gcc-arm-none-eabi-7-2017-q4-major/bin:$PATH
```

**DOWNLOAD, COMPILE AND UPLOAD THE FIRMWARE**  
First, connect a programmer as described in this post. Then, download the latest firmware from github, compile and upload it:

```
git clone https://github.com/vedderb/bldc.git
```

compile default
```
cd bldc
touch conf_general.h
make -j8 build_args="-DHW_VERSION_60"
make upload
```

compile servoout
```
cd bldc
touch conf_general.h
make -j8 build_args="-DSERVO_OUT_ENABLE=1 -DHW_VERSION_60"
make upload
```
If you want to skip downloading and compiling the bootloader and firmware from sources I prepared prebuilt images. You can download these [VESC_default.bin](assets/uploads/VESC_default.bin) [VESC_servoout.bin](assets/uploads/VESC_servoout.bin) and skip to the flashing section of this post.

**reference**  
* [vesc-open-source-esc](http://vedder.se/2015/01/vesc-open-source-esc/)
