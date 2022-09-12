---
translation: true
template: /templates/_template-vectorization-child.md
title: 将图像转换为 SVG - C# 代码和在线矢量化器
description: 在 C# 中将图像转换为矢量。将图像转换为 SVG 并获得矢量图形的所有优点。免费试用在线图像矢量化器！
url: /net/vectorization/image-to-svg/
family: svg
platformtag: net
feature: vectorization
informat: Image
outformat: SVG
---

{{<section banner>}}
---
h1: 矢量化图像 - C# 代码和在线矢量化器
h2: 在线或以编程方式将图像转换为 SVG 格式。
---

{{<section overview>}}
---
h2: 图像矢量化
---

图像矢量化是将位图图像转换为矢量图形的过程 - 贝塞尔曲线、样条曲线和直线。矢量化很有帮助，因为放大图像时图像不会像素化。缩放而不损失质量、小文件大小和动画支持 - 只是矢量化图像的几个优点。无论您是从事绘画、设计、艺术、印刷、建筑还是网络开发，矢量图都是该专业的重要组成部分。另一方面，您可以尝试图像并获得一些有趣的矢量化效果。 [Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) 提供了一个高速 C# 库，可用于不同的 SVG 解析任务. [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) 命名空间包括用于实现图像矢量化过程的类和接口。在本文中，我们将了解如何在 C# 中或使用在线 Image Vectorizer 将 Image 转换为矢量图形。

{{<section input-file>}}
---
title: 什么是图像文件格式？
---

{{<section output-file>}}
---
title: 什么是 SVG 文件格式？
---

{{<section plagin-text>}}
---
h2: 在线图像矢量化器
---

如果您需要矢量化图像，请使用我们的免费在线工具！ Image Vectorizer 支持 JPEG、JPG、PJP、PJPEG、PNG、BMP、ICO、GIF、TIFF、WEBP、XBM 等位图格式。它提供了各种选项，用于在将位图保存为 SVG 格式之前对其进行预处理。您可以使用与适当的矢量化选项链接的控件以交互方式管理矢量化 SVG 文件。立即将您的图像转换为可缩放且清晰的矢量艺术！

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: 在 C# 中将图像转换为 SVG
---

.NET API 的 Aspose.SVG 提供了类和方法，允许您实现图像矢量化过程，并在以矢量格式保存图像之前使用图像的各种预处理选项。处理涉及控制以下矢量化选项：TraceSimplifier、TraceSmoother、PathBuilder 等。

{{<section "code" i18n-exclude>}}

```cs       
	// Initialize an instance of the ImageVectorizer class
    var vectorizer = new ImageVectorizer
    {
        Configuration = 
		{
			// Set severity
			TraceSmoother =   new ImageTraceSmoother(3),
			// Set tolerance
			TraceSimplifier = new ImageTraceSimplifier(0.3f),
			// Set tension
        	PathBuilder = new PathBuilder(0.5f),
		}
    };
    // Vectorize image from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.png");
    // Save vectorized Image as SVG file 
	document.Save(OutputFolder + "image.svg");
```

{{<section steps>}}
---
h2: 如何在 C# 中矢量化图像
title: 在 C# 中将图像转换为 SVG 的步骤
---

要使用 Aspose.SVG 对图像进行矢量化，您应该遵循以下几个步骤：

1. 初始化[ImageVectorizer](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/)类的一个实例。使用 ImageVectorizer() 构造函数之一并指定配置属性。

    - [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) 属性设置跟踪更平滑。它用于平滑轮廓的碎片。
    - [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) 属性设置跟踪简化。因此，轨迹曲线将由具有更少(或更大)点的线段组成。
    - [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) 属性设置 SVG 路径段构建器并影响曲线在控制点处弯曲的剧烈程度。

1. 从指定文件矢量化图像。 [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) 方法获取图像文件的路径并返回一个 SVGDocument。
1. 将矢量化图像保存为 SVG 文件。使用 [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) 方法并将输出路径传递给它。

{{<section documentation>}}

在文档章节中 <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">矢量化 - 基本概述</a>，您将找到图像矢量化信息，图像矢量化过程和矢量化选项的描述，学习如何将PNG，JPG，BMP，TIFF，GIF，ICO等光栅图像矢量化为SVG文档。您将考虑一些演示 [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) 功能以及配置属性对矢量化结果的影响的 C# 示例。<br>
Aspose.SVG 提供免费在线 [Image Vectorizer](https://products.aspose.app/svg/image-vectorization) 允许您将 JPG、PNG、BMP、TIFF、ICO 和 GIF 位图图像转换为矢量图形。使用此应用程序，您可以应用一组选项来获得完美的结果。节省您的时间并检查此图像矢量化器以获得矢量图形的所有好处！

{{<section other-vectorizers>}}
---
title: 其他支持的矢量化器
---