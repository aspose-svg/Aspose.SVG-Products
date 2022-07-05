---
translation: true
template: ./../_template-child.md
title: 通过 C# 将 SVG 合并到 XPS - Aspose.SVG
description: 在 Windows、macOS 和 Linux 上使用 C# 将 SVG 合并到 XPS
url: /net/merger/svg-to-xps/
family: svg
platformtag: net
feature: merge
informat: SVG
outformat: XPS
otherformats: XPS PDF GIF JPEG PNG TIFF BMP
---

{{<section banner>}}
---
h1: 通过 C# 将 SVG 合并到 XPS
h2: 用于在 Windows、macOS 和 Linux 上组合 SVG 文件的高速 .NET API
---

{{<section overview>}}
---
h2: 在 C# 中将 SVG 合并到 XPS
---

SVG 是用于网站构建和打印图形以实现可扩展性的最常用格式之一。但有时，您需要合并 SVG 文件并将它们另存为另一种文件格式的文档。 XPS 格式具有支持安全功能等的一系列优势。使用 [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API，您可以通过编程方式将 SVG 合并到 XPS。强大的 C# API 可帮助您快速、高质量地组合 SVG 文件！

{{<section code-text>}}
---
h2: 将 SVG 合并到 XPS 的 C# 代码示例
title: 将 SVG 合并到 XPS - C#
---

高速 C# 库允许 .NET 开发人员合并 SVG 文件并将合并后的结果快速有效地转换为其他流行格式，例如 PDF、XPS、JPEG、PNG、BMP、GIF 和 TIFF。文档合并可以用几行代码来完成：

{{<section "code-snippet" i18n-exclude>}}

```cs
// Initialize SVG documents from files to merge 
using (var document1 = new SVGDocument("document1.svg"))
using (var document2 = new SVGDocument("document2.svg"))
using (var document3 = new SVGDocument("document3.svg"))
{
    // Create an instance of SvgRenderer
    using var renderer = new Aspose.Svg.Rendering.SvgRenderer();	
    // Create an instance of XpsDevice
    using var device = new Aspose.Svg.Rendering.Xps.XpsDevice("result.xps");
    // Merge SVG to XPS
    renderer.Render(device, document1, document2, document3);                
}
```

{{<section steps>}}
---
h2: 使用 C# 将 SVG 合并到 XPS 的步骤
---
1. 使用 [SVGDocument()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/) 构造函数之一加载 SVG 文档。
1.创建[SvgRenderer](https://reference.aspose.com/svg/net/aspose.svg.rendering/svgrenderer/)类的新实例。
1.使用[XpsDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.xps/xpsdevice/xpsdevice/#constructor_5)构造函数初始化XpsDevice类的新实例。
1. 调用 [Render()](https://reference.aspose.com/svg/net/aspose.svg.rendering/renderer-1/) 方法将 SVG 合并为单个 XPS 文件。
1. 多个 SVG 文件将被保存到指定路径的一个 XPS 文件中。



{{<section documentation>}}

[Aspose.Svg.Rendering](https://reference.aspose.com/svg/net/aspose.svg.rendering/) 命名空间实现了对 Render() 方法的轻松访问。您可以快速执行 SVG 合并并将合并结果导出为流行格式，例如 PDF、XPS、JPEG、PNG、BMP、TIFF 和 GIF。请访问<a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">我们的文档</a>了解更多关于使用 Aspose.SVG API 函数的信息。在文档文章 <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target= "_blank">如何合并 SVG 文件</a>，您可以考虑如何合并 SVG 的 C# 示例。

{{<section online-merger>}}
---
h2: 在线 SVG 合并
---

Aspose.SVG 提供免费的在线 <a href="https://products.aspose.app/svg/merger/svg" target="_blank">Merge SVG</a> 应用程序，可将多个 SVG 合并到一个文件中。您可以为不同的输出文件（例如 SVG、JPG 或 PNG）选择一种 SVG Merger。我们的应用程序是多功能的。您可以在合并之前创建图像拼贴、编辑和操作 SVG 图像。 SVG Merger 允许您自由地添加图像、旋转、缩放、添加背景、过滤器和移动每个图像，直到您对设计的最终结果感到满意为止。

{{<section get-started>}}
---
h2: .NET SVG API 入门
---

从命令行安装为 ```nuget install Aspose.SVG``` 或通过 Visual Studio 的 Package Manager Console 使用 ```Install-Package Aspose.SVG``` 安装。
或者，从 [下载](https://downloads.aspose.com/svg/net) 获取 ZIP 文件中的离线 MSI 安装程序或 DLL。 Aspose.SVG for .NET API 是一个独立的库，不依赖于任何软件来处理 SVG 文档。
 有关 C# 库安装和系统要求的更多详细信息，请参阅 [Aspose.SVG 文档](https://docs.aspose.com/svg/net/getting-started/)。

{{<section other-mergers>}}
---
title: 其他支持的合并
subTitle: "您可以将 SVG 和图像合并为其他文件格式："
---