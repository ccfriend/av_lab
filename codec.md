# 编解码综述

参考：https://www.jianshu.com/p/c2b4f65895b9

## 文件格式

文件格式这个概念应该是我们比较熟悉的，比如我们常见的 Word 文档的文件格式是 .doc，JPG 图片的文件格式是 .jpg 等等。
那对于视频来说，我们常见的文件格式则有：.mov、.avi、.mpg、.vob、.mkv、.rm、.rmvb等等。

## 封装格式

视频封装格式，简称视频格式，相当于一种储存视频信息的容器，它里面包含了封装视频文件所需要的视频信息、音频信息和相关的配置信息(比如：视频和音频的关联信息、如何解码等等)。一种视频封装格式的直接反映就是对应着相应的视频文件格式。

列举一些文件封装格式：

- AVI 格式，对应的文件格式为 .avi，英文全称 Audio Video Interleaved，是由 Microsoft 公司于 1992 年推出。这种视频格式的优点是图像质量好，无损 AVI 可以保存 alpha 通道。缺点是体积过于庞大，并且压缩标准不统一，存在较多的高低版本兼容问题。
- DV-AVI 格式，对应的文件格式为 .avi，英文全称 Digital Video Format，是由索尼、松下、JVC 等多家厂商联合提出的一种家用数字视频格式。常见的数码摄像机就是使用这种格式记录视频数据的。它可以通过电脑的 IEEE 1394 端口传输视频数据到电脑，也可以将电脑中编辑好的的视频数据回录到数码摄像机中。
- WMV 格式，对应的文件格式是 .wmv、.asf，英文全称 Windows Media Video，是微软推出的一种采用独立编码方式并且可以直接在网上实时观看视频节目的文件压缩格式。在同等视频质量下，WMV 格式的文件可以边下载边播放，因此很适合在网上播放和传输。
- MPEG 格式，对应的文件格式有 .mpg、.mpeg、.mpe、.dat、.vob、.asf、.3gp、.mp4 等等，英文全称 Moving Picture Experts Group，是由运动图像专家组制定的视频格式，该专家组于 1988 年组建，专门负责视频和音频标准制定，其成员都是视频、音频以及系统领域的技术专家。MPEG 格式目前有三个压缩标准，分别是 MPEG-1、MPEG-2、和 MPEG-4。MPEG-4 是现在用的比较多的视频封装格式，它为了播放流式媒体的高质量视频而专门设计的，以求使用最少的数据获得最佳的图像质量。
- Matroska 格式，对应的文件格式是 .mkv，Matroska 是一种新的视频封装格式，它可将多种不同编码的视频及 16 条以上不同格式的音频和不同语言的字幕流封装到一个 Matroska Media 文件当中。
- Real Video 格式，对应的文件格式是 .rm、.rmvb，是 Real Networks 公司所制定的音频视频压缩规范称为 Real Media。用户可以使用 RealPlayer 根据不同的网络传输速率制定出不同的压缩比率，从而实现在低速率的网络上进行影像数据实时传送和播放。
- QuickTime File Format 格式，对应的文件格式是 .mov，是 Apple 公司开发的一种视频格式，默认的播放器是苹果的 QuickTime。这种封装格式具有较高的压缩比率和较完美的视频清晰度等特点，并可以保存 alpha 通道。
- Flash Video 格式，对应的文件格式是 .flv，是由 Adobe Flash 延伸出来的一种网络视频封装格式。这种格式被很多视频网站所采用。

更多详细格式介绍可以参考：

## 视频编解码

- H.26X 系列
由国际电传视讯联盟远程通信标准化组织(ITU-T)主导，包括 H.261、H.262、H.263、H.264、H.265。

H264更多详细参考：https://www.vcodex.com/an-overview-of-h264-advanced-video-coding/

- MPEG 系列
由国际标准组织机构(ISO)下属的运动图象专家组(MPEG)开发。

## 音频编解码

视频中除了画面通常还有声音，所以这就涉及到音频编解码。在视频中经常使用的音频编码方式有：
- AAC，英文全称 Advanced Audio Coding，是由 Fraunhofer IIS、杜比实验室、AT&T、Sony等公司共同开发，在 1997 年推出的基于 MPEG-2 的音频编码技术。2000 年，MPEG-4 标准出现后，AAC 重新集成了其特性，加入了 SBR 技术和 PS 技术，为了区别于传统的 MPEG-2 AAC 又称为 MPEG-4 AAC。
- MP3，英文全称 MPEG-1 or MPEG-2 Audio Layer III，是当曾经非常流行的一种数字音频编码和有损压缩格式，它被设计来大幅降低音频数据量。它是在 1991 年，由位于德国埃尔朗根的研究组织 Fraunhofer-Gesellschaft 的一组工程师发明和标准化的。MP3 的普及，曾对音乐产业造成极大的冲击与影响。
- WMA，英文全称 Windows Media Audio，由微软公司开发的一种数字音频压缩格式，本身包括有损和无损压缩格式。
