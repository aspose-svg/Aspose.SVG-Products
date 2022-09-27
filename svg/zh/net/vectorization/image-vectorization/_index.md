---
translation: true
template: /templates/_template-image-vectorization.md
title: 图像矢量化 - C# 代码和在线矢量化器
description: 在线或在 C# 中矢量化图像！图像矢量化为您提供矢量图形的所有优点。免费试用在线图像矢量化器！
url: /net/image-vectorization/
family: svg
platformtag: net
feature: vectorization
informat: Image
outformat: SVG
---

{{<section banner>}}
---
h1: 图像矢量化 - C# 代码和在线矢量化器
h2: 你准备好继续矢量绘图了吗？
---

{{<section overview>}}
---
h2: 什么是图像矢量化？
---

图像矢量化是将位图图像转换为矢量图形的过程 - 贝塞尔曲线、样条曲线和直线。矢量化很有帮助，因为放大图像时图像不会像素化。缩放而不损失质量、小文件大小和动画支持 - 只是矢量化图像的几个优点。无论您是从事绘画、设计、艺术、印刷、建筑还是网络开发，矢量图都是该专业的重要组成部分。另一方面，您可以尝试图像并获得一些有趣的矢量化效果。在本文中，我们将了解如何在 C# 中或使用在线 Image Vectorizer 将 Image 转换为矢量图形。


{{<section plugin-text>}}
---
h2: 在线图像矢量化器
---

你准备好从用像素绘画到用矢量绘画了吗？ Image Vectorizer 旨在将光栅图像转换为基于由贝塞尔曲线和线条组成的几何形状的矢量图形。矢量化后，所有矢量图形元素都保存为 SVG 文件。 Image Vectorizer 支持 JPEG、JPG、PJP、PJPEG、PNG、BMP、ICO、GIF、TIFF、WEBP、XBM 等位图格式。您可以使用与适当的矢量化选项链接的控件以交互方式管理矢量化 SVG 文件。立即将您的图像转换为可缩放且清晰的矢量艺术！

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: C# 中的图像矢量化
---

 [Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) 提供了一个高速 C# 库，可用于不同的 SVG 解析任务. [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) 命名空间包括用于实现图像矢量化过程的类和接口，并在保存图像之前使用各种预处理选项矢量格式。处理涉及控制以下矢量化选项：TraceSimplifier、TraceSmoother、PathBuilder 等。

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
title: 在 C# 中矢量化图像的步骤
---

1. 初始化[ImageVectorizer](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/)类的一个实例。使用 ImageVectorizer() 构造函数之一并指定配置属性。
    - [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) 属性设置跟踪更平滑。它用于平滑轮廓的碎片。
    - [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) 属性设置跟踪简化。因此，轨迹曲线将由具有更少(或更大)点的线段组成。
    - [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) 属性设置 SVG 路径段构建器并影响曲线在控制点处弯曲的剧烈程度。
1. 从指定文件矢量化图像。 [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) 方法获取图像文件的路径并返回一个 SVGDocument。
1. 将矢量化图像保存为 SVG 文件。使用 [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) 方法并将输出路径传递给它。

  

{{<section documentation>}}
---
h2: 文档中的图像矢量化
---

Scalable Vector Graphics 目前广泛用于渲染 Web 图形。与位图相比，矢量图形可以创建缩放到任何大小的清晰图像，它们非常适合绘制任何类型的 Web 插图，包括图标、图表、图表等。在文档章节 [Vectorization - Basic Overview,](https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/) 您将找到对图像矢量化过程。 <br>
- [图像矢量化工作流程](https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/image-vectorization-workflow/) - 您将找到图像矢量化信息，图像矢量化过程和矢量化选项的描述，了解如何将光栅图像(例如 PNG、JPG、BMP、TIFF、GIF、ICO)矢量化为 SVG 文档。
- [图像矢量化示例](https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/image-vectorization-examples/) - 您将考虑一些 C# 示例演示 ImageVectorization 功能和配置属性对矢量化结果的影响。

{{<section other-vectorizers>}}
---
title: 其他支持的矢量化器
subTitle: 节省您的时间并检查这些图像矢量化器以获得矢量图形的所有好处！
---