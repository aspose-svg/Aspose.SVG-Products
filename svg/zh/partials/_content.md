---
translation: true
deploy: false
---

{{<section encode-plugin>}}
---
h2: 在线编码图像
---

使用 [Aspose.SVG for .NET](https://products.aspose.com/svg/{{lang.url-fragment}}net/) API 实时编码图像！ 请从本地文件系统加载图像，您将立即获得数据 URI、Base64 图像源和 Base64 CSS 背景源的结果。 支持JPG、JPEG、PJP、PJPEG、PNG、BMP、XBM、GIF、TIFF、ICO、IFIF、WEBP等图片格式。

{{<section "app-plugin" i18n-exclude>}}

{{< app/svg/base64 sourceImage="/svg/images/encoder/tulip.jpg">}}
{{< /app/svg/base64>}} 

{{<section encode-online>}}

Aspose.SVG 提供免费的在线应用程序来编码和解码二进制数据：

 - [Base64 编码器](https://products.aspose.app/svg/encoding) 是一组工具，可让您以各种输出格式对二进制数据进行编码：Plain Base64、JSON、XML、URI 或 CSS。
 - [图像 Base64 解码器](https://products.aspose.app/svg/image-base64-decoder) 通过在输入控件中粘贴 URI 字符串，将包含 Base64 字符串的数据 URI 转换为图像。
 
我们基于浏览器的应用程序适用于所有平台，包括 Windows、Linux、Mac OS、Android 和 iOS。您无需注册、插件或软件安装。开始安全、可靠、轻松地使用我们的在线 Base64 编码/解码工具！

{{<section encode-uri>}}
---
h2: 数据 URI 的优缺点
---

数据 URI 为我们提供了一种在网页上嵌入图像的明智方法。 URI 方案可以以多种方式使用。但无论如何，有利有弊。

- 加快页面加载。浏览器不需要发出额外的 Web 请求来检索文件，因为图像已经嵌入到 HTML 文档中。
- 性能改进。浏览器需要更少的 CPU 时间。
- 网页变得独立于外部文件，即使离线也可以轻松共享。

<b>优点：</b>

- Base64 编码数据的大小比二进制图像大 1/3。
- 编码的图像不会被浏览器缓存，每次访问此类页面时都会下载。
- 编码图像难以编辑，因为需要首先解码 Base64 字符串。
- Base64 图像永远不会被 Google 索引，因为它不会出现在图像搜索结果中。

<b>缺点：</b>

{{<section vectorization-use>}}
---
h2: 如何使用图像矢量化器？
---

1. 首先，从本地文件系统加载 JPEG、JPG、PJP、PJPEG、WEBP、PNG、BMP、ICO、GIF、TIFF、XBM 或其他位图格式的光栅图像。您将看到三个窗口 - 源、量化和矢量化 - 带有初始、颜色量化和矢量化图像的预览。
1. Image Vectorizer 使用默认设置将 {{i18n.informat}} 转换为矢量，您可以将矢量化的 {{i18n.informat}} 下载为 SVG 文件。但是为了获得更好的结果，您可以使用两个设置侧边栏来处理量化和矢量化过程。单击 “Quantize” 按钮应用量化设置，单击 “Vectorize” 按钮应用矢量化设置并将 {{i18n.informat}} 转换为 SVG。
1. 点击 “Download Result” 按钮获取结果。

 Image Vectorizer 将光栅位图图像转换为由轮廓构成的矢量图。矢量化算法包括以下步骤：颜色量化、轮廓跟踪、轨迹平滑、轨迹简化以及从轨迹构建 SVG 路径元素。应用自定义设置以获得最佳的 {{i18n.informat}} 矢量化结果。

<b>量化侧边栏</b>

颜色量化是选择有限数量的颜色以在图像中使用的过程。当要减少图像的颜色信息时应用它。颜色量化是一个非常复杂的过程，涉及许多因素。这可以使用不同的算法来实现。每个算法都确定较大颜色集中的哪些颜色保留在新图像中，以及丢弃的颜色如何映射到剩余的颜色。

 - <b>colors</b> - 所需的调色板大小；
 - <b>method</b> - 实现各种颜色量化算法的直方图方法；
 - <b>minHueCols</b> - 是一个适用于颜色渐变的参数；
 - <b>scale</b> - 或调整比例因子以对平面中的颜色进行更精细或更粗糙的采样。

<b>矢量化侧边栏</b> 

- <b>tolerance</b> - 负责减少由一系列跟踪点近似的曲线中的点数，并确定允许从跟踪中消除的点的最大误差容限。默认值为 0.3；
- <b>tension</b> - 负责从跟踪点列表构建路径段。张力值决定了曲线在控制点处的弯曲程度；
- <b>severity</b> - 影响轮廓的平滑并确定查询点最近邻方法所考虑的区域范围。

矢量图形是创建徽标、图标、页面布局、地图、图表、线条艺术、插图、技术图纸等的最佳选择。对于具有混合颜色或编辑照片的连续色调图像，它不是最合适的格式。但是，矢量化照片可以产生令人印象深刻的艺术效果，这些效果可能有趣且有用。