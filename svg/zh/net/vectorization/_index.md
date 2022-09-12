---
translation: true
template: /templates/_template-vectorization.md
title: 矢量化图像或文本 - C# 代码和在线矢量化器
url: /net/vectorization/
description: 将图像或 SVG 文本转换为矢量图形并将输出保存为 SVG 文件。在线或在 C# 中矢量化图像或文本！
---

{{<section banner>}}
---
h1: 在 C# 中矢量化图像或文本
h2: 在 C# 中将图像转换为矢量。支持JPG、JPEG、PNG、BMP、GIF、TIFF、ICO、IFIF、WEBP等位图格式。
---

{{<section overview>}}
---
title: 图像矢量化
---

光栅图像是胶片、纸张或屏幕上的像素图(点或颗粒)。每个像素都有自己的颜色。缩放光栅图像会导致其上出现噪点和模糊。为避免此类伪影，您可以将位图图像转换为矢量格式，例如，转换为 SVG 图形。图像矢量化是一种以矢量形式表示图像的方法。矢量图像基于一个公式——它不是基于像素，而是基于诸如点、线、曲线之类的图元，这些图元由数学表达式表示。此类图像中的线条和填充的彩色区域表示为数学曲线，这些曲线由通过路径连接形成它们的笛卡尔点定义。矢量图像将具有矢量图形的所有优点，并且在缩放时不会像素化。
 
您可以使用 Aspose.SVG for .NET API 实时矢量化图像。试试我们的免费图像矢量化器，将像素颜色信息转换为简单的几何对象！请选择要矢量化的图像。支持JPG、JPEG、PJP、PJPEG、PNG、BMP、XBM、GIF、TIFF、ICO、IFIF、WEBP等位图格式。

{{<section "app-pluging" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}}

{{<section plugin-use>}}
---
h2: 如何使用图像矢量化器？
---

Image Vectorizer 具有三个区域：Source Image、Quantized Image 和 Vectorized Image。

<b>Source Image</b> - 此区域包含用于矢量化的源光栅图像。

<b>Quantized Image</b> - 此区域包含应用颜色量化后的光栅图像。颜色量化是选择有限数量的颜色以在图像中使用的过程。当要减少图像的颜色信息时应用它。颜色量化是一个非常复杂的过程，涉及许多因素。这可以使用不同的算法来实现。每个算法都确定较大颜色集中的哪些颜色保留在新图像中，以及丢弃的颜色如何映射到剩余的颜色。 <br>您可以在边栏中手动选择<b>颜色</b>的数量和其他颜色量化设置。

<b>Vectorized Image</b> - 此区域包含矢量化图像和设置侧边栏。您可以设置公差、严重性、张力和线宽值。有关图像矢量化选项的更多详细信息，请参阅文档文章 <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/image-vectorization-examples/" target="_blank">图像矢量化示例。</a>

{{<section image-vectorization>}}
---
h2: 如何使用 C# 对图像进行矢量化
title: 将JPG图像转换为矢量的C#代码
---

使用 <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/" target="_blank">Aspose.SVG for .NET API</a> 将图像转换为矢量非常简单。 ImageVectorization 命名空间包括用于实现图像矢量化过程的类和接口。以下代码片段演示了如何使用 <a href="https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/" target="_blank">ImageVectorizer</a> 类矢量化图像：

{{<section "code-image" i18n-exclude>}}

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
	using var document = vectorizer.Vectorize(InputFolder + "image.jpg");
    // Save vectorized image as SVG file 
	document.Save(OutputFolder + "example.svg");
```

{{<section link-image>}}

您可以通过单击链接了解更多关于图像矢量化的信息 - <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/vectorization/image-to-svg/">图像转 SVG。</a>


{{<section text-vectorization>}}
---
title: 文字转矢量
h2: 如何在 C# 中矢量化文本
title-code: 将 SVG 文本转换为矢量的 C# 代码
text: "我们想与您分享一个用于对 SVG 文档中的文本元素进行矢量化的功能。文本矢量化是将文本转换为数字图形的过程。在矢量化的 SVG 文本中，所有字体字形都被替换为 `path`、`use`、`mask`、`g` 元素等的组合。因此，矢量化促进了文本保护，防止简单复制、不必要的使用、借用和修改。"
---

如果您对可扩展矢量图形及其应用程序的开发感兴趣，请查看我们灵活、高速的 Aspose.SVG for .NET API，它具有一组用于 C# 和其他 .NET 编程语言的强大接口。 <a href="https://reference.aspose.com/svg/net/aspose.svg.saving/" target="_blank">Aspose.Svg.Saving</a> 命名空间包括 <a href=" https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/" target="_blank">SVGSaveOptions</a> 类，它允许您实现文本矢量化过程。要矢量化文本，请将 SVGSaveOptions 类的 `VectorizeText` 属性设置为 true：

{{<section "code-text" i18n-exclude>}}

```cs
// Load an SVG document from a file
var document = new SVGDocument("text.svg");
// Set text elements vectorization 
var saveOptions = new SVGSaveOptions
{
    VectorizeText = true
};    
// Save the SVG document with specified saveOptions
document.Save("text_vectorized.svg", saveOptions);
```

{{<section link-text>}}

您可以通过单击链接了解有关文本矢量化的更多信息 - <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/vectorization/text-to-vector/">文本到矢量。</a>

{{<section installing>}}
---
h2: 为 .NET 库安装 Aspose.SVG
---

<a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/" target="_blank">Aspose.SVG for .NET</a> 是一个跨平台的灵活的库，旨在为处理和呈现 SVG 文档提供广泛的功能。它无缝集成到您的 .NET 应用程序中，无需安装任何 3rd 方建模或渲染软件即可提供 SVG 文件的处理和渲染。 Aspose.SVG for .NET 让开发人员可以使用其与官方 SVG 规范完全兼容的 DOM。我们的 API 可以与任何 .NET 语言一起使用，例如 C#、VB.NET、ASP.NET 等。它同样适用于任何可以安装 Mono(.NET 4.0 框架支持)或使用 .NET 核心的操作系统。这包括 Windows、Linux 和 macOS。

通过 NuGet 安装 <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG for .NET</a>：
1. 使用包管理器控制台。从菜单中打开 Microsoft Visual Studio 和包管理器控制台以打开包管理器控制台。然后输入命令“Install-Package Aspose.SVG”并回车安装。
2. 使用 NuGet 包管理器 GUI。打开 Microsoft Visual Studio 并从菜单中管理 NuGet 包以打开包管理器。搜索“Aspose.SVG”，选择并单击“安装”。 </br>



有关 C# 库安装的更多详细信息，请参阅 [Aspose.SVG 文档。](https://docs.aspose.com/svg/net/getting-started/installation/)

{{<section other-vectorizers>}}
---
h2: 其他支持的矢量化器
---

您可以将图像转换为矢量 - 支持 JPG、PNG、BMP、GIF、TIFF 和 ICO 格式：