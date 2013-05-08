---
layout: post
title: 我和OpenCV的故事，兼译者序
---

{{ page.title }}
================

我翻译的《OpenCV 2 Computer Vision Application Programming Cookbook》将于近期面世，本文是译者序

================

一切的起源是 OpenCV_1.0.exe 的安装包，那时我电脑中安装的还是 VC++ 6.0 绿色版，我以为计算机视觉只是图像处理的别名。当我运行samples/facedetect时惊呆了，笔记本自带的摄像头居然实时地识别出我的脸。后来我意识到这句话说错了，其实是检测到了我的脸。人脸识别指的是计算机知道我是谁，这个功能在当时的OpenCV是不支持的的。另一个让我震惊的是samples/inpaint.exe，字面意识是图像修补，即智能地填补缺失的像素信息，那会儿我想这可以用来去马赛克。后来想明白了信息是不会凭空出现的，如果你事先不知道马赛克背后可能是什么，那么无法去恢复它。

2008年的上海的双年展上，我看到了一款摄像头互动的艺术作品《上海，我能邀你跳支舞吗？》，参展者在摄像头前通过身体来影响投影屏幕中的虚拟建筑。这是我从没想象过的人机交互方式，我意识到程序的操控设备可以脱离鼠标键盘，进入到现实的空间中。回来后我用OpenCV自制了一个用双手控制的虚拟打鼓游戏，录好视频在放在优酷上，启发了一些人。这便是最原始的体感，在硬件上只依赖一个摄像头。一年后的E3展上，Kinect以Project Natal的名称为世人所知。

提到摄像头互动，自然不能不说基于CCV的多点触摸，国内外不少公司都在凭借这款开源的软件接活。而CCV最核心的摄像头跟踪模块完全依赖OpenCV，所做的无非是阈值化加上寻找连通区域。因为打开了OpenCV这扇门，我接触到截然不同的编程世界。研究CCV的间隙我还学习了 openFrameworks 和 Processing，今年我还有一本 Processing 的翻译书籍要出版，这是另外一个故事。

之后从事了游戏行业，基本没机会用OpenCV，直到一个游戏项目中的字体贴图丢失了坐标信息，需要通过肉眼手动定位。这很不科学，于是我拾起OpenCV，阈值化加上寻找连通区域，输入一副图像，输出字体的包围盒坐标，同事纷纷觉得不可思议。计算机视觉的魅力便在此，从看似无关的像素中能够提取信息。这不是唯一一次在工作中使用OpenCV，之后我得到了一份增强现实、图像检索等领域的开发工作，可以全职地进行OpenCV的开发。共事的有国内著名CV网站 cvchina.info 的站长张小军，本书的第二章也是由他翻译的，对于他在工作中的指点在此一并感谢。

OpenCV的用途很广，除了上述提到的，还有视频监控、双目视觉、机器学习、Kinect深度信息处理、照片美化、图像拼接、GPU加速等等功能。但是OpenCV的书籍并不多，在本书面世前市场上只有一本讲述1.0接口的Learning OpenCV。本书的意义在于，讲述了2.0后出现的 C++ 接口以及大量的新功能。如果你看过 Learning OpenCV，想学习新接口使用，那么推荐你阅读这本书。如果你没有接触过 OpenCV，想直接跳过 C 接口的函数，那么更加推荐你阅读本书。

最后，感谢陪伴我鼓励我的妻子 M，如果没有你，我和OpenCV的故事到第二段就结束了，译者序也必定由他人撰写。

张静<br>
2013年4月25日<br>
上海<br>
