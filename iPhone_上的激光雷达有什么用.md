# iPhone 上的激光雷达有什么用

今天凌晨的苹果发布会上，iPhone 12 正式面世。与基本机型相比，iPhone 12 Pro 和 iPhone 12 Pro Max 的后置摄像头除了多一枚长焦镜头，还增加了一颗 LiDAR，激光雷达扫描仪。



这颗激光雷达是什么？它能为你的手机带来什么新体验？



![img](https://mmbiz.qpic.cn/mmbiz_png/SlOqFKqEO4EniaQs7KibNSz661R0ibB29ccGkFjoAjF7lSZObPcF2o33xSpicwzG2MFOIlUOO8QaPniaOHKjJqyHOfw/640?wx_fmt=png)



在这块圆形黑色区域之下，LiDAR 主要由两部分组成：发射端和接收端。垂直腔面发射激光器（VCSEL）作为发射端，向物体发射一束红外光，经反射被 CMOS 图像传感器接收，光束经历的这一段时间被称为飞行时间（ToF）。



![img](https://mmbiz.qpic.cn/mmbiz_png/SlOqFKqEO4EniaQs7KibNSz661R0ibB29ccWbmrfCUCyOjfKw5XhpF2okMzV6icUr7hQXJEmiaeJZGx8NTTZY9ep4iaA/640?wx_fmt=png)



飞行时间又分为直接飞行时间（dToF）和间接飞行时间（iToF）。前者向目标发射一个光脉冲信号，直接测量光子从出发到返回的用时；后者发射一连串经过调制的光波，通过检测来回光波间的相位差测量飞行时间。



![img](https://mmbiz.qpic.cn/mmbiz_gif/SlOqFKqEO4Gbp10icPSn6Ijxicn0YkI9da2iaIic7g0S8TLBmPPBA36AOUnxgkGvvjgficItNUj05KoZWibjtBwMw0jQ/640?wx_fmt=gif)



已知光速，通过简单的计算我们就能得到与目标物体之间的距离。这样的测距原理与雷达类似，不过，LiDAR 基于的是脉冲激光，比雷达利用的无线电波波长更短、频率更高，可以得到分辨率更高的图像，精度可达厘米甚至毫米级别。



![img](https://mmbiz.qpic.cn/mmbiz_png/SlOqFKqEO4Gbp10icPSn6Ijxicn0YkI9davNhr5mu9k4tgX1ZodVNxfm04iag12NDpVGVia0FAApDopC8lMe2FtEXA/640?wx_fmt=png)



因此，LiDAR 也被应用在地图测绘、自动驾驶、文物保护等领域。而到了手机，它又能做些什么呢？



这不是苹果第一次在它的产品里引入激光雷达。早在今年 3 月，2020 款 iPad Pro 就配备了 LiDAR 扫描功能，采用直接飞行时间技术（dToF），相比 iToF，功耗较低且不易受环境光的干扰，可以做到大范围测量。



使用时，发射器投射出 9 * 64 大小的矩阵光束，捕捉并绘制最远 5 米范围内的位置深度图。改变，首先发生在你拍摄的照片里。



![img](https://mmbiz.qpic.cn/mmbiz_gif/SlOqFKqEO4Gbp10icPSn6Ijxicn0YkI9da7HlsGFiaJuLHwkILk3c8vEX9TIpFFK3g4wrKKsZQWagSLJG8V0zHduw/640?wx_fmt=gif)



一张出色的浅景深照片，是通过调大相机光圈并对焦在距离相机较近的地方实现的。今天，通过多个摄像头和机器学习算法的帮助，用手机也能轻而易举拍出这种背景虚化的效果。



首先，神经网络和机器学习技术可以让手机知道我们在拍什么，以及目标距离我们有多远。对于普通人来说，从一张照片中判断物体层次和远近关系是一件非常容易的事，但对于机器，则需要大量的资源来学习，比如颜色分布、明暗程度和物体尺寸。



![img](https://mmbiz.qpic.cn/mmbiz_png/SlOqFKqEO4Gbp10icPSn6Ijxicn0YkI9da0mXriaBgTEz7Ee7fodRdEm85M7IN8P7xyqGUbloVNl2DojAXhTdtzww/640?wx_fmt=png)



就像上面这张照片，曝光度均匀且主题明显，机器很容易分析出距离镜头较近的点以及距离镜头较远的点。



可一旦照片中有更复杂的关系，事情就变得棘手了。



人类或者动物的毛发、丰富的色彩、以及与背景颜色接近的衣服等，都很容易被机器误判为背景，尤其是主体的边缘区域，呈现出不自然的模糊效果。



LiDAR 的加入能带来更精准的深度信息，以便于让 iPhone 理解物体之间的前后关系，通过算法绘制出一张空间位图，并将照片做切片处理。iPhone 会在几纳秒内根据深度信息图将照片切分成多份，距离越远的图层，模糊程度越高，制作出一张以假乱真的浅景深人像照片。



![img](https://mmbiz.qpic.cn/mmbiz_png/SlOqFKqEO4Gbp10icPSn6Ijxicn0YkI9daMsvO1UibLa31AD0jSycGUeceXbic4Uo08qicCV4YeLh1mEgMticvsoSFicg/640?wx_fmt=png)



同时，在低光照条件下，iPhone 的对焦速度也将大幅提升，并且可以在黑暗中准确找到画面中的人物，为夜间模式下的人像照片打下基础。



当然，LiDAR 对 iPhone 12 Pro 的拍照提升实际上还得看实拍测试。你可以期待另一个让它真正大放异彩的领域—— AR。



2017 年开始，苹果公司推出 AR 软件开发套件 ARKit，开发者们可以使用它制作出精致的 AR 应用，比如下面这个能让你随时随地打保龄球的游戏。



![img](https://mmbiz.qpic.cn/mmbiz_gif/SlOqFKqEO4Gbp10icPSn6Ijxicn0YkI9dalY0hUguhvbiaB6xzCNzib5Aruwd5ficJico9xxY2Suc37Ixt7FcvN6xUsw/640?wx_fmt=gif)



游戏场景中的这两人保持运动状态，且是前后移动，在没有深度信息的辅助下，机器难以判断出两个人的位置关系，把球放置在二人中央。所以你会看到，球时不时从人体内「穿」过的诡异画面。



![img](https://mmbiz.qpic.cn/mmbiz_gif/SlOqFKqEO4Gbp10icPSn6Ijxicn0YkI9daaBb8dg8J6HgQBJv8skjHeN4VuxvNPpxaHwqZNoVFuzEHuwuLsdnzjA/640?wx_fmt=gif)



而加入了 LiDAR 之后，通过测量出照片的深度系统，将游戏里的 3D 模型附着在地面、桌面等平面上，并分析整个摄像头视野内的空间位置关系来动态调节模型的光照和阴影，使游戏体验更加真实。



当这些人物从你面前跑过，将带来身临其境的体验，并且通过机器学习算法的加持，AR 应用能更清楚地知道摄像机视野里的是你家的沙发还是地面，从而将草地附着到沙发脚的位置，与你所处的位置达到前所未有的契合。



你可能意识到了，手机前置的 Face ID 也能构建 3D 图像，它与 LiDAR 有什么区别？



![img](https://mmbiz.qpic.cn/mmbiz_png/SlOqFKqEO4Gbp10icPSn6Ijxicn0YkI9da7RfZBRBtDffAYU5de6iaFphvyWZ70JFeCzSLJEQG4rSibpNeicdMSjic6Q/640?wx_fmt=png)



从红外摄像机拍摄到的光斑可以看出，Face ID 的结构光传感器通过点阵投影发射出超过 3 万个不可见的光斑，利用扭曲建模，制作出一张准确的面部深度图，从而将 2D 的图像转换为带有深度信息的 3D 图像。受距离所限，只能进行小范围的 3D 绘制，用于人脸识别。



![img](https://mmbiz.qpic.cn/mmbiz_png/SlOqFKqEO4Gbp10icPSn6Ijxicn0YkI9dal8VZqcmQ3t3rEXLiaftQeGNic0IE8EZjbkUuF0VK7n2C5jk6aDrJniaAA/640?wx_fmt=png)



而 LiDAR 的光斑较大且疏，更适合用来对整个房间进行扫描和建模。



![img](https://mmbiz.qpic.cn/mmbiz_gif/SlOqFKqEO4Gbp10icPSn6Ijxicn0YkI9daoupJtvYJPGwdkSMhGcstGr1QUW7eY9XPQr7ok0606iaOfgBym6OMqAg/640?wx_fmt=gif)



LiDAR 能让你的手机在 AR 应用中获得更好的体验，在家里放一把椅子，它比你的双目还要更精准地知道椅子离地面多远、离墙壁多远。



椅子嵌进墙里或是立在墙面的画面，再也不会出现了。



\-



> 封面图来源：
>
> Apple
>
> 
>
> 参考资料：
>
> [1] Foix, S., et al. (2011). Lock-in Time-of-Flight (ToF) Cameras: A Survey. IEEE Sensors Journal, 11: 1917-1926.
