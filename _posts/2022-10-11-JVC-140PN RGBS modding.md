---
layout:     post   		# 使用的布局（不需要改）
title:      【怀旧游戏之旅】CRT彩监折腾—JVC-H140PN改装RGB输入 		# 标题 
subtitle:   JVC-H140PN RGB Modding #副标题
date:       2022-10-11 			# 时间
author:     Kasiin 				# 作者
header-img: img/post-bg-2015.jpg 	#这篇文章标题背景图片
catalog: true 						# 是否归档
tags:								#标签
    - 折腾
---









# 【怀旧游戏之旅】CRT彩监折腾—JVC-H140PN改装RGB输入
## 一、背景

一直比较喜欢玩FC游戏，之前是在各种掌机和模拟器平台玩，后来中了油管“高清马赛克”的毒，陆续购买了RGB FC和OSSC来玩FC游戏，既然玩老游戏，绕不过的就是老显示设备了，彩监肯定是会接触到的。
前阵子闲逛咸鱼发现一台缺门牙的JVC-H140PN，750线的14寸彩监，价格不错，直接拿下了，回来用DC主机AV输入测试一下没有问题。
![20221011145550](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011145550.png)

## 二、起因

彩监买回来了，高线数确实很舒服，这机器有个缺点，只有AV和S端子输入，既然要玩游戏机怎能没有RGB输入呢，于是网上冲浪搜索一番发现国外大佬（感谢大佬：Martin Hejnfelt, [主页](https://immerhax.com/)）有[改装教程](https://immerhax.com/?p=558)，需要用到一片arduino刷个固件，i2c搭个桥打开芯片的RGB输入功能，看了一下改造教程并不复杂，根据资料画了片板子直接开搞！
![20221011145621](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011145621.png)

## 三、过程

打的板子和零件都到齐就开干了，费了一番劲之后焊好，测试一下，成功点亮！
![20221011145648](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011145648.png)
![20221011145710](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011145710.png)
![20221011145730](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011145730.png)
下一步就是画个外壳打印一下固定到机子后面了。
![20221011145753](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011145753.png)

## 四、插曲

改完开机，我用dc主机接入，声音画面都OK，但是用RGB FC接入，只有声音没有画面，难道还是翻车了？研究了一会无果，睡觉了。

第二天睡了一觉起来，突然灵光乍现，想到了可能的问题点，我用了scart接口，彩监的消隐脚直接接到scart的16脚，dc的scart可以正常输出消隐的5v电压，但是RGB FC这个脚是悬空的，没有输出5v，所以解码芯片的RGB根本没有打开，想到这里一整天都神清气爽。

下班回家赶紧操作，从板子上其他地方加了5V到芯片的消隐，并且增加了一个物理开关以方便切换不同主机的时候使用，解决了消隐的问题，RGB FC可以正常输入显示了，顺便3d打印了外壳，利用散热孔固定在后盖，这不就妥了吗！
![20221011150330](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011150330.png)
![20221011150602](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011150602.png)
![20221011150353](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011150353.png)
![20221011150408](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011150408.png)
![20221011150443](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011150443.png)


## 五、总结
RGB输入得到的画面还是提升很大的，咸鱼闲逛又收到一台jvc-h150cg，这台直接可以插卡RGB，更方便，收拾了小房间，把飘窗位置作为游戏角了。
![FB78D6C8-7888-414D-A0C6-548498A14A55](https://cdn.jsdelivr.net/gh/Kasiin/images@main/FB78D6C8-7888-414D-A0C6-548498A14A55.jpeg)
最后，其实玩这些设备，打游戏是第二的，各种改装各种Mod才是第一的乐趣，比如下面这个，也是开源的项目，给老游戏机增加蓝牙手柄支持，根据国外大佬资料打了板子验证成功，正在画缩小的板子更美观一些，这就是下一个话题了。
![20221011151103](https://cdn.jsdelivr.net/gh/Kasiin/images@main/20221011151103.png)
![2FA9FC41-E237-4886-A42B-47176E92E5CF](https://cdn.jsdelivr.net/gh/Kasiin/images@main/2FA9FC41-E237-4886-A42B-47176E92E5CF.jpeg)
![CF6DF71B-E3A7-478E-8E9A-FE2A59759AC7](https://cdn.jsdelivr.net/gh/Kasiin/images@main/CF6DF71B-E3A7-478E-8E9A-FE2A59759AC7.jpeg)