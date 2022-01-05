---
layout:     post   		# 使用的布局（不需要改）
title:      计算机网路学习资料汇总 		# 标题 
subtitle:   Computer Networking Learning #副标题
date:       2022-01-05 			# 时间
author:     Kasiin 				# 作者
header-img: img/post-bg-2015.jpg 	#这篇文章标题背景图片
catalog: true 						# 是否归档
tags:								#标签
    - 计算机网络
---

# 计算机网路学习资料汇总

## 书籍推荐
首先是基础书籍推荐:

**网络是怎样连接的**
![图 1](https://cdn.jsdelivr.net/gh/Kasiin/images/c2db514acb8ea7f55d9c21d004d681e2d21e238a47be7796a9fd3ea1ce908ca9.png)  


这本书是日本人写的，它和《程序是怎样运行的》、《计算机是怎样跑起来的》统称为图解入门系列，最大的特点就是风趣幽默，简单易懂。这本书通过多图来解释浏览器中从输入网址开始，一路追踪了到显示出网页内容为止的整个过程，以图配文，讲解了网络的全貌，并重点介绍了实际的网络设备和软件是如何工作的。

本书图文并茂，通俗易懂，非常适合计算机、网络爱好者及相关从业人员阅读。
所以如果大家是新手的话，强烈推荐一下这本书。
日本人就爱图解，同样图解系列的入门书籍还有《图解 HTTP》、《图解 TCP/IP》。

**图解 HTTP**
![图 2](https://cdn.jsdelivr.net/gh/Kasiin/images/25d91a091adc56c7b9f712e72723043084f4e72dea0033344a4b91f3a7212c46.png)  


《图解 HTTP》是 HTTP 协议的入门书籍，当然 HTTP 也是属于计算机网络的范畴，这本书适合于想要对 HTTP 有基本认知的程序员，同样也适合查漏补缺。

这类书看起来就毫无难度了，不得不说图解系列是给小白的圣经，它能增强你的自信，让你觉得计算机其实没那么难，这是非常重要的。初学者，最怕的就是劝退了。

**图解 TCP/IP**
![图 3](https://cdn.jsdelivr.net/gh/Kasiin/images/48ecdf00675a534b1412534fcd2eda1c387800604ec103877221e91055a37abc.png)  

上面的图解 HTTP 是针对 HTTP 协议的，那么《图解 TCP/IP》就是针对 TCP/IP 协议簇中的协议了，这本书我已经看了 80% 了，还是比较系统的一本书，基本上涵盖了 TCP/IP 协议簇中的所有协议知识了，这本书看完了完全就可以直接深入理解 TCP/IP 协议簇了。

对于新手来说，最重要的一点就是帮助你理解，怎么简单怎么来，这样才能快速入门，对于快餐式的社会来说，快速理解当然是当仁不让的首选了。

如果上面这几本书你都搞定了的话，那你就可以读一下 《计算机网络：自顶向下方法》这本书了，这本书可以作为基础书籍也可以作为进阶书籍，这里我归为了进阶书籍，因为里面有一些章节不是那么好理解，比如介绍网络层的时候，会分为数据平面和控制平面，介绍 TCP 和 UDP 的时候，也会聊到一些原理性问题。

**计算机网络：自顶向下方法**
![图 4](https://cdn.jsdelivr.net/gh/Kasiin/images/62797049e2b47224c9ab27d5fa8d0bcaf1ea263a010f5cd41f8d9a83f6214a33.png)  


这本书是一本计算机网络的**圣经**书籍，圣经就在于人人都应该读一下这本书，原著非常经典，翻译也很不错，我自己也马上就看完了，这本书会从顶层也就是网络层逐步下探到物理层，一层一层的带你入门，解释各层之间的协议，主要特征是什么，一个数据包的发送历程。这本书并不局限于某个具体的协议，而是从宏观的角度来看待计算机网络到底是什么，里面有一些专业名词，理解并掌握后会对深入学习计算机网络非常有用。

**计算机网络：谢希仁版**
![图 5](https://cdn.jsdelivr.net/gh/Kasiin/images/9fcb98d6f573df577da87efd45a76c81b5c69e8fa431f59808697394093e93ea.png)  


这本书是很多大学的教材，也是一本非常好的进阶书籍，这本书相对于自顶向下方法更多是对于通信网络的阐述。

这本书的特点是突出基本原理和基本概念的阐述，同时力图反映计算机网络的一些最新发展。本书可供电气信息类和计算机类专业的大学本科生和研究生使用，对从事计算机网络工作的工程技术人员也有参考价值

---
现在我们接着聊，如果上面这两本书随便一本看完了，那么恭喜你已经是一个老手了，你的网络基础能打败 90% 以上的人了，如果你还不满足的话，那你就需要继续深入，继续深入也是我推荐给你的提高书籍。

**HTTP 权威指南**
![图 6](https://cdn.jsdelivr.net/gh/Kasiin/images/1a664b62570dcce6d03f5db255204f57446600a5e0fa8cdc017a0b966d15e6b3.png)  

HTTP 权威指南是深入 HTTP 非常值得一看的书，这本书写的非常全了。

此书第一部分是 HTTP 的概述，如果你没有时间，通读第一部分就能让你应付普通的日常开发工作。

第二部分主要讲现实世界中 HTTP 的架构，也可以看作 HTTP 的全景图，包括 Web Server/Cache/Proxy/Gateway，是全书中精华的部分。

第三部分主要是 HTTP 安全，其中 Basic 和 Digest 概略看下即可，现实世界中用的应该不多。看 HTTPS 最好有一些计算机安全基础，这样会顺畅很多。

第四部分主要是关于 HTTP Message Body 的部分，包括 Content Negotiation，MIME Type，chunked encoding等，概略看下即可。

第五部分的内容，Web Hosting 可以认真看下，了解下 Virtual Host(话说我上学的时候一直搞不懂 Virtual Host，一个 IP 怎么能同时 Host 两个不同域名的 Web 页面呢)。

剩下三章已经过时，基本可以忽略。最后的附录，可以用作边用边学的字典，如果你自己来写 Web Server，那么这一部分是极有价值的参考。

总而言之，无论你是前端还是后端，只要是 Web 相关的，那么此书就是必读的。

**TCP/IP 详解**
![图 7](https://cdn.jsdelivr.net/gh/Kasiin/images/f2b20f11e2fa49f6705a4ea9d50d9481298e8412a8747c706509edebba992ada.png)  


这是一本被翻译耽误的经典书，两个硬核作者 Kevin R. Fall 和 W. Richard Stevens 被南开大学的某计算机系的译者给毁了。我第一开始读这本书以为是自己智商不够，原来是翻译瞎TM翻啊。语句不通且不说，您好歹走点心，改点措辞也行啊，纯粹是生搬硬套谷歌翻译啊，哎。


不过这本书确实是一本非常好的书，这本书的关注点在于 TCP/IP 协议栈上，可以说把 TCP/IP 讲透讲细了，比如讲 TCP 就会分别从连接管理、TCP 超时重传、TCP 拥塞控制、TCP 保活机制来讲起，不管你是从事哪个技术栈的研究，不管你是程序员还是网络工程师，这本书都是你值得一读的一本，不过要读最好还是读英文版。

TCP/IP 详解有三本，第二本是
![图 8](https://cdn.jsdelivr.net/gh/Kasiin/images/6db9aa13cca3a27b85993e474375e9e46bb877a62f35dbb8363a8d4774f8dde7.png)  


这本黑皮书主要是介绍如何实现 TCP/IP 协议的，这本书很难入门。书中给出了约 500 个图例，15000 行实际操作的 C 代码，采用举例教学的方法帮助你掌握 TCP/IP 实现。

本书不仅说明了插口 API 和协议族的关系以及主机实现与路由器实现的差别。还介绍了 4.4BSD-Lite 版的新的特点。本书适用于希望理解 TCP/IP 协议如何实现的人，包括编写网络应用程序的程序员以及利用 TCP/IP 维护计算机网络的系统管理员。

第三卷是 tcp 事务协议、http、nntp 和 unix 域协议
![图 9](https://cdn.jsdelivr.net/gh/Kasiin/images/8bd9ed511d4111cb413db2132ab3d2881586a3a9598874383d0d6000cc60c669.png)  


这本书看的人就更少了。

第 3 卷详细介绍了当今 TCP/IP 程序员和网络管理员必须非常熟悉的四个基本主题：TCP 的扩展、Hyper 文本传输协议、网络新闻传输协议和 UNIX 域协议。与前两卷一样，本书介绍了 4.4BSD-Lite 网络代码中的示例和实现细节。

---

上面都是一些理论书籍，下面是稍微偏实战一些的书籍了。

计算机网络实战最有效的当然就属于抓包了，有很多抓包工具比如 wireshark、sniffer、httpwatch、iptool、fiddle 等，但是我用的和使用频率最高的应该就是 wireshark 了，关于 wireshark 还有几本实战方面的书你需要知道

**wireshark 数据包分析实战**
![图 10](https://cdn.jsdelivr.net/gh/Kasiin/images/f921c4ff8c7a89bbb9526101684c0f8c4b4e32afae6078e07a53cdf9f9b3e923.png)  


初学者必备，介绍了 wireshark 安装，嗅探网络流量，wireshark 的基本使用，用 wireshark 分析了一圈常用的TCP，UDP 协议，也简要分析了 HTTP 等应用层协议，概要介绍了一些 TCP 重传的机制，最后是无线分析。

整个书定位应该是入门级别的，基本上每章都是简要介绍，并没有特别深入大张阔斧地进行描述。文章行文思路清晰，译者的翻译水平也不错。总的来说，是初步认识和了解 wireshark 的好书。

**wireshark 网络分析就是这么简单**
![图 11](https://cdn.jsdelivr.net/gh/Kasiin/images/6b6a32577e3ea3a99b18ffaff185e07b6377109ceedd568c58633094866dce63.png)  


读的时候你会忍不住笑的，区别于《Wireshark数据包分析实战》，本书就像一本侦探小说集，以幽默风趣的语言风格，借助wireshark以理性的思考来不断探险，根据蛛丝马迹来侦破案情。总结，读完数据包分析实战来读这本。

**Wireshark网络分析实战**
![图 12](https://cdn.jsdelivr.net/gh/Kasiin/images/933ccce8349ae2dd794b499018f66f530c19b18e4fa424473912b9d061bcd01c.png)  

其内容涵盖了 Wireshark 的基础知识，抓包过滤器的用法，显示过滤器的用法，基本/高级信息统计工具的用法，Expert Info 工具的用法，Wiresahrk 在 Ethernet、LAN 及无线 LAN 中的用法，ARP 和 IP 故障分析，TCP/UDP故障分析，HTTP 和 DNS 故障分析，企业网应用程序行为分析，SIP 多媒体和 IP电话，排除由低带宽或高延迟所引发的故障，认识网络安全等知识。

书籍推荐大概就是上面那些，除了书之外，还有一些视频、博客、官网网站可以学习

**视频推荐**
1. 计算机网络微课堂（有字幕无背景音乐版）（陆续更新中......）_哔哩哔哩 (゜-゜)つロ 干杯~-bilibili
![图 13](https://cdn.jsdelivr.net/gh/Kasiin/images/014e2f84391ea8475f20318927a06a0f78db31e067ce1ef3607c9053a59f6469.png)  

学习计算机网络，首先推荐 UP 主湖科大教书匠，他讲的计算机网络十分通俗易懂，重点的地方讲的十分细致，并且还有一些实验，更好的是有考研 408 的难题的讲解，也是非常适合考研党，除了课程内容外还有很多习题讲解视频，特别赞的一点是每天动态里都会更新一道考研题，播放量也非常的多。


2. 2019 王道考研 计算机网络_哔哩哔哩 (゜-゜)つロ 干杯~-bilibili
![图 1](https://cdn.jsdelivr.net/gh/Kasiin/images/4ebbbe5387758bbbd68be8ab89f57b4d81e1ed92c23990f58293e64c5119c05a.png)  

既然说到了考研，那我就不得不提一下王道考研了，恭喜你发现了宝藏。王道考研的计算机网络视频，播放量非常多，而且老师是一位小姐姐，声音十分动听，声音这么好听的老师给你讲课，妈妈再也不用担心我的学习了呢，总之，这个视频的质量也非常高，弹幕全是对小姐姐的高度评价。（王道考研其他的视频也不错哦，暗示一下：操作系统，数据结构等等）


3. 韩立刚计算机网络 谢希仁 第7版 2020年12月_哔哩哔哩 (゜-゜)つロ 干杯~-bilibili
![图 2](https://cdn.jsdelivr.net/gh/Kasiin/images/656f9129d6e2aa8cab625f848750770517c4741aae0d06b42a96bb2503be5295.png)  

韩立刚老师所讲的计算机网络视频，内容比较多，但是讲解的通俗易懂，并且老师讲课的经验也十分的丰富。配套的教材是谢希仁老师的计算机网络教材，韩老师的最近的一个视频视频比较新，播放量还比较少，但是他讲的是真的不错，相比于王道考研所讲的计算机网络，韩老师更加细致一些。


4. 计算机网络（谢希仁第七版）-方老师_哔哩哔哩 (゜-゜)つロ 干杯~-bilibili
![图 3](https://cdn.jsdelivr.net/gh/Kasiin/images/39b44dcb007a459df4f4d3a7ccbd3b003be0aacf388fb06e0f1f4323d0509327.png)  

在计算机网络方面，我还想推荐的一位老师就是方老师，也是一位小姐姐老师。她的视频配套的教材也是谢老师的网络教材，在线看的小伙伴也超多，弹幕都是对方老师的评价。


**博客推荐**

推荐几个不错的学习博客。

互联网协议入门-阮一峰：http://www.ruanyifeng.com/blog/2012/05/internet_protocol_suite_part_i....

网络协议-兰亭风雨：http://blog.csdn.net/ns_code/article/category/1805481

HTTP协议：http://www.cnblogs.com/TankXiao/category/415412.html

Unix 网络编程：http://blog.csdn.net/chenhanzhun/article/category/2767131/2

TCP/IP详解：http://blog.csdn.net/chenhanzhun/article/category/2734921/1

计算机网络面试题：http://blog.csdn.net/shadowkiss/article/details/6552144

国外优秀计算机网络站点：http://www.tcpipguide.com/free/t_TCPSlidingWindowAcknowledgmentSystemForDataTranspo-6.htm

当然最硬核的就是 RFC 文档了 https://tools.ietf.org/rfc/index

学习 HTTP ，必须要看一下 MDN 官网 https://developer.mozilla.org/zh-CN/docs/Web/HTTP

学习计算机网络，Cloudflare 你必须要去看 https://www.cloudflare.com/zh-cn/learning/

GeeksforGeeks 学习计算机网络也非常不错 https://www.geeksforgeeks.org/basics-computer-networking/

Tutorialspoint 系统学习计算机，不仅仅局限于计算机网络 https://www.tutorialspoint.com/computer_fundamentals/computer_networking.htm

国外优秀的学习网站不能少了 javapoint https://www.javatpoint.com/types-of-computer-network