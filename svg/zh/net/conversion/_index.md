---
translation: true
template: _template.md
title: 使用 C# 将 SVG 转换为流行格式 - 在线 SVG 转换器
url: /net/conversion/
description: 通过 .NET 库使用几行 C# 代码将 SVG 转换为 PDF、XPS 和图像。免费在线查看 SVG 转换器！
---

{{<section banner>}}
---
h1: 通过 C# 进行 SVG 转换
h2: 将 SVG 转换为 PDF、XPS 和图像，包括 BMP、JPEG、PNG、TIFF，以构建跨平台的 .NET 应用程序
---

{{<section overview>}}
---
h2: 如何使用 C# 转换 SVG
---

SVG（可缩放矢量图形）是一种基于 XML 的二维图形图像格式。它是一种主要用于 Web 的矢量图形格式。 SVG 的主要优点是它无与伦比的缩放到任何大小的能力，而不会出现任何质量下降。所有现代浏览器都支持 SVG，看起来 Web 应该已经切换到矢量图形了。但是，SVG 的使用有一些限制，有时您需要将 SVG 转换为其他格式。
 
 - 静态 [Converter 类](https://reference.aspose.com/svg/net/aspose.svg.converters/converter/) 是一个共享外观，它提供 SVG 文件到流行格式的转换并允许进行这些操作方便又容易。

 - [RenderTo()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/) 方法用于将 SVG 渲染为另一种格式并将文档发送到输出设备。 Aspose.SVG API 提供以下输出设备实现：PdfDevice、XpsDevice 和 ImageDevice 类，它们分别执行 PDF、XPS 和 Image 文件格式的渲染。

<a href="https://products.aspose.com/svg/net/" target="_blank">Aspose.SVG for .NET API</a> 使开发人员的转换过程更容易。可以使用几种不同的方法在格式之间进行转换：

{{<section demos>}}
---
h2: SVG 转换器现场演示
---

您可以将 SVG 与 Aspose.SVG 实时转换为 .NET API。以下 C# 示例演示了如何转换 SVG 文档。请从本地文件系统加载文件，选择输出格式并运行示例。您将立即将结果作为单独的文件获得。

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/converter SVG PDF BMP "JPG|JPEG" PNG GIF TIFF XPS>}}
using Aspose.Svg;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;

    using var document = new SVGDocument("input.{{input lower}}");
{{#if_output 'PDF'}}
    var options = new PdfSaveOptions();
{{/if_output}}
{{#if_output 'DOCX'}}
    var options = new DocSaveOptions();
{{/if_output}}
{{#if_output 'XPS'}}
    var options = new XpsSaveOptions();
{{/if_output}}
{{#if_output 'MD'}}
    var options = new MarkdownSaveOptions();
{{/if_output}}
{{#if_output 'BMP' 'JPG' 'GIF' 'PNG' 'TIFF'}}
    var options = new ImageSaveOptions(ImageFormat.{{output camel}});
{{/if_output}}
    Converter.ConvertSVG(document, options, "output.{{output lower}}");
{{< /app/svg/converter>}}

{{<section documentation>}}
---
h2: 文档中流行的 SVG 转换
---

Aspose.SVG for .NET 库允许您使用 C# 以编程方式创建、编辑、读取和转换 SVG 文件。 SVG C# API 的主要亮点是转换功能。 [Aspose.SVG.Converters](https://reference.aspose.com/svg/net/aspose.svg.converters/) 命名空间实现了对转换方法的轻松访问。它提供广泛的 SVG 到流行格式的转换，例如 PDF、XPS、JPEG、PNG、BMP、TIFF 和 GIF。请访问文档章节 <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">如何转换SVG 文件</a> 以了解有关 SVG C# API 转换功能的更多信息。

<div>
	<ul>
		<li><a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/convert-svg-to-pdf/" target="_blank">Convert SVG to PDF</a></li>
		<li><a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/convert-svg-to-xps/" target="_blank">Convert SVG to XPS</a></li>
		<li><a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/convert-svg-to-image/" target="_blank">Convert SVG to Image</a></li>							
	</ul>
</div>

{{<section installing>}}
---
h2: 为 .NET 库安装 Aspose.SVG
---

Aspose.SVG for .NET 是一个跨平台的灵活库，旨在为处理和呈现 SVG 文档提供广泛的功能。它无缝集成到您的 .NET 应用程序中，无需安装任何第三方软件即可处理 SVG 文件。我们的 SVG .NET API 可以与任何 .NET 语言一起使用，例如 C#、VB.NET、ASP.NET 等。它同样适用于任何可以安装 Mono（.NET 4.0 框架支持）或使用 .NET 的操作系统核。这包括 Windows、Linux 和 macOS。

通过 NuGet 安装 <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG for .NET</a>：
1. 使用包管理器控制台。
1. 使用 NuGet 包管理器 GUI。



有关 C# 库安装的更多详细信息，请参阅 [Aspose.SVG 文档](https://docs.aspose.com/svg/net/getting-started/installation/)。

{{<section other-conversions>}}
---
h2: 其他支持的转换
---

您还可以将 SVG 文件转换为许多其他文件格式，包括下面列出的几种文件格式：