---
layout:     post   		# 使用的布局（不需要改）
title:      Fliper Zero NRF24		# 标题 
subtitle:   Flipper Zero 模块使用说明 #副标题
date:       2023-01-08			# 时间
author:     Kasiin 				# 作者
header-img: img/post-bg-2015.jpg 	#这篇文章标题背景图片
catalog: true 						# 是否归档
tags:								#标签
    - DIY
---
# Flipper Zero NRF24

>注意：所有模块均在第三方固件中测试，推荐使用unleashed固件，链接：[https://github.com/DarkFlippers/unleashed-firmware]

## Author: [mothball187](https://github.com/mothball187/flipperzero-nrf24/tree/main/mousejacker)（作者：[mothball187](https://github.com/mothball187/flipperzero-nrf24/tree/main/mousejacker)）


## How to use 使用方法
- Connect NRF24 to flipper using provided pinouts   
  将NRF24模块插入到Flipper Zero
- Open NRF24: Sniffer, and scan channels, switch between modes/channels using buttons   
  打开APP->GPIO->[NRF24]sniffer，扫描频道，可以使用按钮在模式/频道间切换
- When you got address -> Open NRF24: Mouse Jacker   
  扫描到地址之后，打开APP->GPIO->[NRF24]Mouse Jacker
- Select Address and open badusb file   
  选择地址并打开BadUSB文件（关于badUSB的使用请自行学习）
- Done  
  结束

## Demo (YouTube)
[![YouTube](https://img.youtube.com/vi/C5hbyAjuU4k/0.jpg)](https://www.youtube.com/watch?v=C5hbyAjuU4k)

## Mouse Jack affected devices
just for reference  

https://www.bastille.net/research/vulnerabilities/mousejack/affected-devices


## Warning
These apps are for **educational purposes** only. Please use this code responsibly and only use these apps on your own equipment.  
本模块和软件只能用作教育和学习用途，一切使用责任请自负，请仅在您拥有的设备上使用

## Acknowledgments
The NRF24 sniffing technique was discovered and shared by Travis Goodspeed in [his blog](http://travisgoodspeed.blogspot.com/2011/02/promiscuity-is-nrf24l01s-duty.html).

The mousejack vulnerabilities were discovered and reported by Marc Newlin, see [the blog](https://www.bastille.net/research/vulnerabilities/mousejack/technical-details) for technical details.

Much of the driver code was inspired by [RadioHead's Arduino library](https://www.airspayce.com/mikem/arduino/RadioHead/classRH__NRF24.html).
Much of the mousejack code was inspired by the [Jackit project](https://github.com/insecurityofthings/jackit).

