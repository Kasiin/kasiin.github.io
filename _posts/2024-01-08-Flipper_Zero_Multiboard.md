---
layout:     post   		# 使用的布局（不需要改）
title:      Fliper Zero Multiboard		# 标题 
subtitle:   Flipper Zero 模块使用说明 #副标题
date:       2023-01-08			# 时间
author:     Kasiin 				# 作者
header-img: img/post-bg-2015.jpg 	#这篇文章标题背景图片
catalog: true 						# 是否归档
tags:								#标签
    - DIY
---
# Flipper Zero Multiboard

>注意：所有模块均在第三方固件中测试，推荐使用unleashed固件，链接：[https://github.com/DarkFlippers/unleashed-firmware]

## Author: [Dr.B0rk](https://github.com/DrB0rk/Flipper-Zero-Boards)（作者：[mDr.B0rk](https://github.com/DrB0rk/Flipper-Zero-Boards)）

## 一. 产品外观
Multiboard由两个模块构成，NRF24模块和ESP32模块，NRF24模块可以使用sniffer和mousejacker，ESP32模块烧录Marauder固件之后可以用于WiFi安全测试。
不同外观仅原件和模块封装不同，功能相同，使用方法也一致。  

![multiboard 2.0](https://raw.githubusercontent.com/Kasiin/images/main/multiboard%202.0.jpg)  

![multiboard 3.0](https://raw.githubusercontent.com/Kasiin/images/main/multiboard%203.0.jpg)  

![multiboard 2.5](https://raw.githubusercontent.com/Kasiin/images/main/multiboard%202.5.jpg)
## 二. 固件更新
Multiboard

### 方法1

使用Dr.B0rk仓库中的multiboard flasher更新：[https://github.com/DrB0rk/Flipper-Zero-Boards/tree/main/Multiboard%20flasher]

操作方法：
1. 将Dr.B0rk的仓库完整下载到本地
2. 从[这里](https://github.com/justcallmekoko/ESP32Marauder/releases)下载最新的Marauder固件，记得选择以flipper结尾的bin文件
3. 把下载到的bin文件改名为esp32_marauder.bin并放到Flipper-Zero-Boards/Multiboard flasher/Marauder文件夹中
4. 把multiboard插到flipper zero上，在flipper zero主界面选择GPIO->USB-UART Bridge，将flipper zero连接到电脑
5. 按住multiboard上的boot键不松开，按一下reset键使ESP32进入bootloader
6. 按WIN+X键后选择设备管理器，查看端口（COM & LPT）内对应的端口号（一般是COMX，X是数字）
7. 回到上个文件夹双击Flash.bat，填入端口号
8. 看到无报错的finish界面，刷写成功（模块不会自行退出bootloader模式，需要拔掉再插上才能使用，或者按reset）

### 方法2

使用ESP32官方的烧录工具flash_download_tool进行烧录

操作方法：
1. 从官网下载[flash_download_tool](https://www.espressif.com.cn/sites/default/files/tools/flash_download_tool_3.9.5_0.zip)
2. 从[这里](https://github.com/justcallmekoko/ESP32Marauder/releases)下载最新的Marauder固件，记得选择以flipper结尾的bin文件
3. 从Dr.B0rk仓库的Flipper-Zero-Boards/Multiboard flasher/Marauder文件夹中获取bootloader.bin和partitions.bin两个文件，这两个文件与上一步下载到的Marauder固件放在一起
4. 打开flash_download_tool软件，并按照下图设置  
   ![20240107234143](https://raw.githubusercontent.com/Kasiin/images/main/20240107234143.png)  

   ![20240107234420](https://raw.githubusercontent.com/Kasiin/images/main/20240107234420.png)  

5. 按方法1中的步骤将multiboard通过flipper zero或者其他你熟悉的串口工具连接到电脑并进入bootloader
6. 在flash_download_tool右下角选择你的设备的COM号
7. 点击开始，等待刷写完成


## 三. 使用


### ESP32部分
1. 将multiboard插入flipper zero并打开APP->GPIO->[ESP32]WiFi Marauder
   
   ![20240107234953](https://raw.githubusercontent.com/Kasiin/images/main/20240107234953.png)
2. Marauder的具体使用方法，参照Marauder WiKi：https://github.com/justcallmekoko/ESP32Marauder/wiki


### NRF24部分
参考NRF24模块说明：[https://kasiin.top/2023/01/08/Flipper_Zero_NRF24/]





## Warning
These apps are for **educational purposes** only. Please use this code responsibly and only use these apps on your own equipment.  
本模块和软件只能用作教育和学习用途，一切使用责任请自负，请仅在您拥有的设备上使用
