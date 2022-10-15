# av_lab
av实验室，用于音视频领域的资料学习分享，立志于让所有人都能入门、学习、理解音视频领域。

内容大多来自网络，也有个人完成的一些文章，分门别类的加以整理总结；网上的内容以链接形式提供，如有版权要求，可以联系删除。

个人建议的学习思路：

1. 先通读某一大类的专栏文章和书籍，这些专栏文章和书籍一般都是完整的介绍某一类知识提下，能够以较好的条理性从头阐述，对于系统理解脉络知识很有帮助；
当然，通读的时候肯定会遇到各种问题，这个没有关系，多读几遍这样的专栏，就大概理解了知识脉络，后续就是针对性的加以精读和实践。
2. 音视频领域很广，业务知识门槛不低，虽然本身技术发展演进不如互联网迅速，但是对于理论知识的要求较高，再加以软件、硬件的综合要求，如对编解码算法的掌握和优化，对于音频器件的控制，电路的调试等等，不亚于一个全栈工程师。整个行业分解的也很大，依据个人的兴趣和行业的热度，来选择细分领域加以钻研。但是无论哪个细分行业，基础知识都是必备的，建议都要加以牢固掌握。
3. 基础知识包括：
 - 音频的声学基础，声音的基本要素，数字信号处理的基本方法
 - 编解码的基础，最好以某个格式做到精通，如AAC和H264
 - 流媒体基础，分包、拆包、传输的基本流程，以RTP和RTCP为精通，对照互联网的tcp/udp要求，要理解过程
 - 常见硬件平台的驱动调试、硬件开发，了解概貌，知道如何做bringup，如linux版本的驱动调试（根据需要，这个是BSP工程师的范畴）
 - 常见开源软件的掌握，如ffmpeg，这个掌握要到什么程度？动手写demo，分析demux，decode，encode的代码流程，知道代码结构，如何进行编译，裁减，优化等，可以结合网上的一些面试题做自我考试，或者针对一个场景做完整工程
 - 常见开源客户端的使用，如ijkplayer，基于ffmpeg如何实现的完整播放器，自己能不能看懂
 - 常见问题的分析思路，如音频的卡顿、延时，视频的丢帧，不同步，流媒体的起播，卡顿
4. 为了多长见识，需要多学习了解行业的动态，随时更新自己的技术栈，理解一个新兴的业务，如AI编码背后的逻辑，虽然对数学要求很高，但是可以慢慢尝试。

总体包括：

- 专栏文章和书籍
- 音频技术
- 视频技术
- 流媒体技术
- 图片技术
- Android系统音视频
- linux系统音视频
- 开源软件
- 技术规范
- 参考工具
- 面试资源

## 专栏文章和书籍

- 专栏总结

|分类|内容|
| :----: | :----: |
|音视频|[音视频基础知识：流媒体核心技术梳理](https://mp.weixin.qq.com/s?__biz=MzI0NTMxMjA1MQ==&mid=2247483830&idx=1&sn=60bea3eb935eafcb81d0701908a822f6&chksm=e9513eeade26b7fc1cafd9ca3384f9bfa9a3ac329a58fbc625d963944036fd99ffebbf86f6d0&scene=21#wechat_redirect)|
||[Microsoft的媒体基础](https://docs.microsoft.com/zh-cn/windows/win32/medfound/media-foundation-programming-guide)|
|个人专栏|[0voice-audio_video_streaming](https://github.com/0voice/audio_video_streaming)|
||[AvStackDocs](https://github.com/ty6815/AvStackDocs)|

- 关于书籍
基础的通用知识书籍：
有一个关于书籍的推荐链接：

## 音频技术
### 格式

|格式|内容|
| :----: | :----: |
|mp3|[mp3格式解析](https://blog.csdn.net/sunshine1314/article/details/2514322)|
||[mp3 tech-外国小哥自己弄的mp3、aac介绍](http://www.mp3-tech.org/)|
||[ID3 org](https://id3.org/)|
|midi|[midi org](https://www.midi.org/)|


### 蓝牙音频
|分类|内容|
| :----: | :----: |
||[LHDC](https://www.hwa-lhdc.org/how-it-works)|
||[aptx](https://www.aptx.com/which-aptx)|


### 测试资源 

## 视频技术
### 文件封装

|分类|内容|
| ---- | ---- |
|HDR|[HEVC的VUI](https://zhuanlan.zhihu.com/p/522169996)|
||[HDR编码总结](https://zhuanlan.zhihu.com/p/536673560)|

### 测试资源
[xiph视频测试资源](https://media.xiph.org/video/derf/)

## 显示技术

|分类|内容|
| :----: | :----: |
|色彩管理|[Color Management](https://www.bgteach.com/article/291)|
||[Color Gamut: Understanding Rec.709, DCI-P3, and Rec.2020](https://www.benq.com/en-us/business/resource/trends/understanding-color-gamut.html)|

## 流媒体技术

## 图片技术
### 图片基础

|分类|内容|
| :----: | :----: |
||[Exif orientation](https://jdhao.github.io/2019/07/31/image_rotation_exif_info/)|
||[Exif file format](https://www.media.mit.edu/pia/Research/deepview/exif.html)|
||[各类图片加载框架](https://edward7zhang.github.io/2019/03/04/Android%E7%AB%AF%E5%90%84%E7%B1%BB%E5%9B%BE%E7%89%87%E5%8A%A0%E8%BD%BD%E6%A1%86%E6%9E%B6%E5%AF%B9%E6%AF%94/)|
||[iOS的image介绍](https://tenloy.github.io/2021/09/15/graphics-processing.html)|


### heif
|分类|内容|
| :----: | :----: |
||[nokia heif官网](https://nokiatech.github.io/heif/examples.html)|
||[libheif开源库](https://github.com/strukturag/libheif)|

### 测试资源

|分类|内容|
| :----: | :----: |
||[图片测试资源RAISE](http://loki.disi.unitn.it/RAISE/download.html)|
||[图片测试资源Kodak](https://r0k.us/graphics/kodak/)|
||[图片测试资源Clic](http://compression.cc/tasks/)|

## Android系统音视频
|分类|内容|
| :----: | :----: |
|音频|[AudioPatch分析](https://blog.csdn.net/yzhang8703/article/details/47660803)|
|视频|[深入理解Android音视频同步](https://blog.csdn.net/nonmarking/article/details/78745646)|

## linux系统音视频
|分类|内容|
| :----: | :----: |
||[ALSA](https://www.alsa-project.org/wiki/Main_Page)|
||[PulseAudio](https://gavv.github.io/articles/pulseaudio-under-the-hood/)|
|pipewire|[pipewire under hood](https://venam.nixers.net/blog/unix/2021/06/23/pipewire-under-the-hood.html)|

## 开源软件
|分类|内容|
| :----: | :----: |
|vlc|[vlc 播放器](https://github.com/videolan/vlc)|
|ffmpeg|[雷神的ffmpeg学习总结](https://blog.csdn.net/leixiaohua1020/article/details/15811977)|

## 技术规范
各类标准规范：
|分类|内容|
| :----: | :----: |
|TIFF||
|H264||

## 参考工具
### 格式解析类：
|分类|内容|
| :----: | :----: |
|mp4|[mp4 creator](http://mp4creator.sourceforge.net/)|
|avi|[AVIDemux](https://www.fosshub.com/Avidemux.html)|

### 视频流解析类：

|分类|内容|
| :----: | :----: |
|收费|[CodecVisa](http://www.codecian.com/)|
||[Elecard](http://www.elecard.com/en/download/products.html)|
||[Intel VideoPro Analyzer](https://software.intel.com/content/www/us/en/develop/articles/video-pro-analyzer.html)|
||[Adobe 工具](https://www.adobe.com/?faas_unique_submission_id={44411BF3-B7E5-44FB-3ED7-2F9F480102C1}&s_cid=null)|
||[Vega (目前也没在市面上见到过破解版的)](http://lazybing.github.io/blog/2015/11/01/hevc-analyse-tool/)|
|免费|[雷神的VideoEye](https://blog.csdn.net/leixiaohua1020/article/details/34553607)|


### 在线转码工具
有一些很方便的在线工具，小巧而实用：

## 面试资源
|分类|内容|
| :----: | :----: |
||[audio_video_streaming](https://github.com/0voice/audio_video_streaming)|
