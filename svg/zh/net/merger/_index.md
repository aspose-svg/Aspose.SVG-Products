---
translation: true
template: /templates/_template-merger.md
title: 使用 C# 将 SVG 组合成流行格式
url: /net/merger/
description: 使用几行 C# 代码将图像或 SVG 组合为 PDF、XPS、PNG、JPEG 等。
---

{{<section banner>}}
---
h1: 使用 C# 组合 SVG、JPEG、PNG 或其他图像
h2: 使用 C# 将 SVG 或图像文件合并在一起，并将结果保存为流行的格式，包括 PDF、XPS、BMP、JPEG、PNG、GIF 和 TIFF
---

{{<section overview>}}
---
h2: 如何使用 C# 合并 SVG 和图像
---

您需要将多个 SVG 或图像组合到一个文档中的原因有很多。要合并 SVG 文件，我们将使用 <a href="https://products.aspose.com/svg/net/" target="_blank">Aspose.SVG for .NET API</a> 这是一个功能-用于 C# 平台的丰富、强大且易于使用的文档操作和合并 API。我们的 C# 库提供了用于渲染和合并 SVG 的 <a href="https://reference.aspose.com/svg/net/aspose.svg.rendering/svgrenderer/" target="_blank">SvgRenderer </a>类文件。 Render() 方法使您能够一次将多个文档发送到输出渲染设备并合并它们。

{{<section demos>}}
---
h2: 将 SVG 组合为 PDF 的 C# 示例
---

高速 C# 库允许 .NET 开发人员合并 SVG 文件，并将合并后的结果以高质量和高效率转换为多种流行格式，例如 PDF、XPS、JPEG、PNG、BMP、GIF 和 TIFF。文档合并可以用几行代码来完成：

{{<section code-text>}}
---
title: 将 SVG 合并为 PDF - C#
---

{{<section "code-snippet" i18n-exclude>}}

```cs
// Initialize SVG documents from files to merge 
using (var document1 = new SVGDocument("document1.svg"))
using (var document2 = new SVGDocument("document2.svg"))
using (var document3 = new SVGDocument("document3.svg"))
{
    // Create an instance of SvgRenderer
    using var renderer = new Aspose.Svg.Rendering.SvgRenderer();	
    // Create an instance of SvgRenderer
    using var device = new Aspose.Svg.Rendering.Pdf.PdfDevice("result.pdf");
    //Merge all SVG documents to PDF
    renderer.Render(device, document1, document2, document3);                
}
```

{{<section documentation>}}
---
h2: 文档中的 SVG 合并
---

Aspose.SVG for .NET 库允许您使用 C# 以编程方式创建、编辑、读取、转换和合并 SVG 文件。 [Aspose.Svg.Rendering](https://reference.aspose.com/svg/net/aspose.svg.rendering/) 命名空间实现了对转换和合并方法的轻松访问。此外，它还提供将 SVG 文件组合成流行格式的功能，例如 PDF、XPS、JPEG、PNG、BMP、TIFF 和 GIF。请访问文档章节 <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" 目标="_blank">如何合并 SVG 文件</a>，了解有关 SVG C# API 合并功能的更多信息。

{{<section installing>}}
---
h2: 为 .NET 库安装 Aspose.SVG
---

Aspose.SVG for .NET 是一个跨平台的灵活库，旨在为处理和呈现 SVG 文档提供广泛的功能。它无缝集成到您的 .NET 应用程序中，无需安装任何第三方软件即可处理 SVG 文件。我们的 SVG .NET API 可以与任何 .NET 语言一起使用，例如 C#、VB.NET、ASP.NET 等。它同样适用于任何可以安装 Mono（.NET 4.0 框架支持）或使用 .NET 的操作系统核。这包括 Windows、Linux 和 macOS。

通过 NuGet 安装 <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG for .NET</a>：
1. 使用包管理器控制台。
2. 使用 NuGet 包管理器 GUI。</br>



  有关 C# 库安装的更多详细信息，请参阅 [Aspose.SVG 文档](https://docs.aspose.com/svg/net/getting-started/installation/)。

{{<section other-mergers>}}
---
h2: 其他支持的合并
---

您可以将 SVG 文件组合成许多其他文件格式，包括下面列出的几种文件格式：