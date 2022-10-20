[toc]

# HDR

## 色域 Color Gamut

所谓色域就是显示设备能够正确显示颜色的范围，色域越广，显示的颜色就越多。

目前的主流电视设备支持的色域通常是 BT.709 色域，而 HDR 的颜色标准通常是 P3，甚至是 BT.2020，从下图就可以看到这三个色域之间的差距。

色域的标准定义是对一种颜色进行编码的方法，也指一个技术系统能够产生的颜色的总和。当然这个颜色总和是一个理想值，现实中我们只能达到这个颜色总和的一部分，因此就有了不同的色彩标准。

![image](http://dev-qiyun.club/images/%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A120220211-111445.png)

[祁云技术博客分享](http://www.dev-qiyun.club/2022/02/11/%E5%A6%82%E4%BD%95%E6%B8%B2%E6%9F%93HDR%E5%9B%BE%E5%83%8F%E6%88%96%E8%A7%86%E9%A2%91%EF%BC%9F/)

## 伽玛曲线
参考：
[什么是伽玛曲线](http://www.52rd.com/News/APP/Detail/?ID=121527)

伽玛就是成像物件形成画面的“反差系数”，如果伽玛曲线比较陡，则输出的画面反差比较高，如果伽马曲线比较缓，则输出的画面反差比较低。

所谓伽玛，其实就是一个“成像物件”对入射光线做出的“反应”。然后根据不同亮度下的不同反应值获得的曲线，就是伽马曲线。人眼作为一个“成像物件”，其伽玛曲线不是一条直线，说明人眼对光线的反应是非线性的。

![image](https://user-images.githubusercontent.com/8341724/196832705-2b3e6226-eaf6-4113-8c5d-dd8d0447d015.png)


## HDR 发展历史

以下讲解了HDR10 和 DolbyVision，以及PQ和HLG曲线的渊源，很容易就理解了这些标准产生的背景。[HDR的四种标准](https://tieba.baidu.com/p/6136703352?red_tag=1231589841)

这篇讲解了HDR的发展历史，以及基本的元素[如何渲染HDR图像或视频](http://www.dev-qiyun.club/2022/02/11/%E5%A6%82%E4%BD%95%E6%B8%B2%E6%9F%93HDR%E5%9B%BE%E5%83%8F%E6%88%96%E8%A7%86%E9%A2%91%EF%BC%9F/)

通过调节背光亮度来加强SDR画面的动态范围，这可以被视为“模拟HDR”，真正的HDR要等到2015年8月27日才算诞生，那一天美国消费者技术协会（Consumer Technology Association）公布了HDR10标准，提供17.6档的动态范围。今天，所有的HDR电视均支持这一标准。

## HDR vs SDR

|特性|SDR|HDR|
| :----: | :----: | :----: |
|最大分辨率|1920*1080|7680*4320|
|最大位深|8bit or 10bit| 10bit or 12bit|
|色域|Rec.709| P3 or Rec.2020|

## HDR 要素

HDR 之所以称之为HDR，至少包含以下三个能力：
- 高动态范围
- 高色域 (Color Gamut)
- 高位深

### 高动态

### 高色域

### 高位深

### Tone Mapping

色调映射的目的是使高动态范围HDR图像能够适应低动态范围SDR显示器。

### 元数据

不同的HDR标准有不同的元数据设计要求，总体来说，包括静态和动态两种。

### 电光转换函数 EOTF

作用：EOTF 是将电子信号转换为所需光信号的数学函数（即数字到模拟函数）。
与伽玛的不同之处在于，伽玛告诉显示器发射其最大亮度的一定**百分比**，而 EOTF 告诉它要产生多少尼特的**亮度**。1nit=1 cd/m²（卡特拉每平方米）；

1. PQ

Perceptual Quantizer感知量化，是由杜比设立的HDR转换方式。其本质是将亮度等级以绝对的数值进行记录，用杜比实验室多屏视频副总裁Roland Vlaicu的话来说“这能体现内容创作者的创作意图”。
PQ曲线基于人类视觉感知的特征，并且最适合于在互联网上制作电影或串流视频的内容，其中再现准确性是关键。

Perceptual Quantizer（也叫SMTPE ST2084）是由杜比开发的，包括随后的HDR标准也由杜比参与制定.

![image](https://user-images.githubusercontent.com/8341724/196834766-1431edb4-dffc-45b6-970e-61494223d6e0.png)


2. HLG

BBC与NHK合作开发了另一项HDR技术HLG（Hybrid Log-Gamma），并认为这是针对电视广播信号的最佳HDR技术。

HLG曲线最高亮度与显示设备的最高亮度无关（这也从另一方面说明了为什么HLG曲线不用配置元数据）。
它与PQ系统的不同之处在于，HLG可以在摄像机内直接完成HDR的编码，这被称为“场景参考”；而PQ需要在之后对信号进行处理，以适配监视器的亮度等级，这叫“显示参考”。

![image](https://user-images.githubusercontent.com/8341724/196834794-ae66c887-8d6a-4d64-81bc-6cfacd2d12a6.png)

## HDR 渲染


## Android 平台的HDR实现参考

[Android HDR技术说明](https://source.android.com/docs/core/display/hdr#technologies)


## HDR Vivid 标准

[联盟官网](http://www.theuwa.com/code)

