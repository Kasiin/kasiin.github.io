---
layout:     post   		# 使用的布局（不需要改）
title:      Fliper Zero GPS		# 标题 
subtitle:   Flipper Zero 模块使用说明 #副标题
date:       2023-02-20			# 时间
author:     Kasiin 				# 作者
header-img: img/post-bg-2015.jpg 	#这篇文章标题背景图片
catalog: true 						# 是否归档
tags:								#标签
    - DIY
---
# Flipper Zero GPS

>注意：所有模块均在第三方固件中测试，推荐使用unleashed固件，链接：[https://github.com/DarkFlippers/unleashed-firmware]

## Author: [ezod](https://github.com/ezod/flipperzero-gps)（作者：[ezod](https://github.com/ezod/flipperzero-gps)）

![module](https://cdn.jsdelivr.net/gh/Kasiin/images@main/IMG_0406.32rt4gbnaw80.webp)




## How to use 使用方法

### Hardware
- Connect GPS module to flipper using provided pinouts   
  将GPS模块插入到Flipper Zero
  ![1](https://cdn.jsdelivr.net/gh/Kasiin/images@main/IMG_0405.394xneqtpfq0.webp)
- Open [NMEA] GPS, wait for 5 seconds and press reset button on GPS module   
  打开APP->GPIO->[NMEA] GPS，等待5s，然后按一下GPS模块上的reset按钮
- Time To First Fix (TTFF) takes about 30 seconds, keep your Flipper next to an open window or outside.   
  首次定位大概需要30秒，使用时尽量靠近窗口或者户外
  ![2](https://cdn.jsdelivr.net/gh/Kasiin/images@main/IMG_0404.5pko444eavs0.webp)
- Done  
  结束
### Software （by ezod）
This is a single-screen app, and a few interactions are provided via the hardware buttons:  
这是一款单屏应用程序，通过硬件按钮进行一些交互：
- Long press the up button to change the baud rate. The default baud rate is 9600, but 4800, 19200, 38400, 57600, and 115200 baud are also supported.  
  长按向上按钮可更改波特率。默认波特率为 9600，但也支持 4800、19200、38400、57600 和 115200
- Long press the right button to change speed units from knots to kilometers per hour.  
  长按右键可将速度单位从海里每小时改为公里每小时
- Press the OK button to set the backlight to always on mode. Press it again to disable.  
  按确定按钮将背光设置为常亮模式。再次按下则禁用。
- Long press the back button to exit the app.  
  长按返回键退出应用




## Warning
These apps are for **educational purposes** only. Please use this code responsibly and only use these apps on your own equipment.  
本模块和软件只能用作教育和学习用途，一切使用责任请自负，请仅在您拥有的设备上使用

