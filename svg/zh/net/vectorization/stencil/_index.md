---
translation: true
template: /templates/_template-vectorization-child.md
title: 图像模板 - C# 代码和在线模板制作工具
description: 将图像转换为 SVG 并在 C# 中应用模板转换。矢量化和模板化图像并获得矢量图形的所有优势。免费试用在线模板制作工具！
url: /net/vectorization/stencil/
family: svg
platformtag: net
feature: vectorization, stencil
informat: Image
outformat: SVG
---

{{<section banner>}}
---
h1: Stancil 绘图 - C# 代码和 Stencil Maker
h2: 在线或以编程方式制作模板图像。
---

{{<section overview>}}
---
h2: 什么是图像模板？
---

图像模板化是将普通照片转换为轮廓图像的过程，该轮廓图像可以用作模板来实现类似涂鸦的效果。

将照片或图像转换为模板有几个基本步骤：
* 将照片或图像转换为灰度，此步骤是可选的，因为您可以减少要量化的颜色数量。
* 量化图像得到stancil，然后你可以下载结果或矢量化它得到stancil的形状线条。
* 绘制模板共有三个选项。第一个是“None”，当所有矢量化形状都被填充时，第二个是“Auto”，当形状没有被填充并且边框具有“原始”颜色时，最后一个是“MonoСolor”，当形状也没有被填充时，但边框具有预定义的颜色。


<br>
[Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) offers a high-speed C# library that you can use for different SVG parsing tasks. The [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) Namespace includes classes and interfaces for implementing the image vectorization process with stenciling options.

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
h2: 在线模板制造商
---

如果您需要将照片或图像转换为模板，请使用我们的免费在线工具！它不仅可以获取光栅模板，还可以将它们矢量化并使用可缩放且清晰的矢量。 Stencil Maker 支持 JPEG、JPG、PJP、PJPEG、PNG、BMP、ICO、GIF、TIFF、WEBP、XBM 等位图格式！

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image" sourceImage="/svg/images/vectorization/fish.png" colors="3" scale="1" grayscale="true" stencil="monocolor" extent="1" stencilColor="#00ff00">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: 在 C# 中将 PNG 转换为 SVG
---

.NET API 的 Aspose.SVG 提供了允许您实现图像矢量化过程和使用模板选项的类和方法。

{{<section "code" i18n-exclude>}}

```cs       
	// Initialize an instance of the ImageVectorizer class
	var vectorizer = new ImageVectorizer
    {
		//optionally set configuration
        Configuration =
        {
			//optionally set path builder
            PathBuilder = new BezierPathBuilder {
			//optionally set trace smoother
            TraceSmoother = new ImageTraceSmoother(1),
                ErrorThreshold =  30,
                MaxIterations = 30
            },
            ColorsLimit = 10,
            LineWidth = 1,
            Stencil = new StencilConfiguration { Type = StencilType.MonoColor, Color = Aspose.Svg.Drawing.Color.FromRgb(0,0,255) }
        }
    };
    // Vectorize PNG from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.png");
    // Save vectorized PNG as SVG file 
	document.Save(OutputFolder + "image.svg");
```

{{<section steps>}}
---
h2: 如何在 C# 中矢量化 PNG
title: 在 C# 中将 PNG 转换为 SVG 的步骤
---

要使用 Aspose.SVG 对 PNG 图像进行矢量化，您应该遵循以下几个步骤：
1.初始化[ImageVectorizer](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/)类的一个实例。使用 ImageVectorizer() 构造函数之一并指定配置属性。
    - [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) 属性获取或设置 SVG 路径段构建器。
    - [ColorsLimit](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/colorslimit/) 属性获取或设置用于量化图像的最大颜色数。
    - [Stencil](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/stencil/) 属性获取或设置模板效果配置。默认情况下，不应用模板效果。
1. 矢量化指定文件中的图像。 [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) 方法获取图像文件的路径并返回一个 SVGDocument。
1. 将矢量化的 PNG 保存为 SVG。使用 [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) 方法并将输出路径传递给它。



{{<section documentation>}}

在文档章节中 <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">矢量化 - 基本概述</a>，您将找到图像矢量化信息，图像矢量化过程和矢量化选项的描述，学习如何将PNG，JPG，BMP，TIFF，GIF，ICO等光栅图像矢量化为SVG文档。您将考虑一些 C# 示例来演示 [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) 功能以及配置属性对矢量化结果的影响。

{{<section other-vectorizers>}}
---
title: 其他支持的矢量化器
---