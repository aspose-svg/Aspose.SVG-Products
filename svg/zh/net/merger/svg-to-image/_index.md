---
translation: true
template: ./../_template-child.md
title: 使用 C# 将 SVG 合并到图像 - Aspose.SVG
description: 在 Windows、macOS 和 Linux 上使用 C# 将 SVG 合并到图像
url: /net/merger/svg-to-image/
family: svg
platformtag: net
feature: merge
informat: SVG
outformat: GIF JPEG PNG TIFF BMP
otherformats: GIF JPEG PNG TIFF BMP PDF XPS
---

{{<section banner>}}
---
h1: 通过 C# 将 SVG 合并到光栅图像文件
h2: 用于在 Windows、macOS 和 Linux 上组合 SVG 文件的高速 .NET API
---

{{<section overview>}}
---
h2: 使用 C# 将 SVG 合并为光栅图像文件格式
---

SVG 是用于网站建设和打印图形以实现可扩展性的最常用的矢量图像格式之一。但有时，您需要合并 SVG 文件并将它们保存为一个光栅图像。光栅图像表示二维像素网格；它可以以未压缩或压缩格式存储数据。广泛拍摄图像以通过网络传输图片并在网页和云驱动器存储库上显示照片和图形。使用 [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API，您可以通过编程方式将 SVG 合并到 Image。强大的 C# API 可帮助您快速、高质量地组合 SVG 文件！

{{<section code-text>}}
---
h2: 将 SVG 合并为 PNG 的 C# 代码示例
title: 将 SVG 合并为 PNG - C#
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
    // Create an instance of ImageDevice
    using var device = new Aspose.Svg.Rendering.Image.ImageDevice("result.png");
    // Merge SVG to PNG
    renderer.Render(device, document1, document2, document3);                
}
```

{{<section steps>}}
---
h2: 使用 C# 将 SVG 合并到图像的步骤
---
1. 使用 [SVGDocument()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/) 构造函数之一加载 SVG 文档。
1. 创建[SvgRenderer](https://reference.aspose.com/svg/net/aspose.svg.rendering/svgrenderer/)类的新实例。
1. 使用 [ImageDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/imagedevice/#constructor_5) 构造函数初始化 ImageDevice 类的新实例。
1. 调用[Render()](https://reference.aspose.com/svg/net/aspose.svg.rendering/renderer-1/)方法将SVG合并成需要的图片格式。
1. 多个SVG文件将被保存到指定路径的光栅图像中。



{{<section documentation>}}

[Aspose.Svg.Rendering](https://reference.aspose.com/svg/net/aspose.svg.rendering/) 命名空间实现了对 Render() 方法的轻松访问。您可以快速执行 SVG 合并并将合并结果导出为流行格式，例如 PDF、XPS、JPEG、PNG、BMP、TIFF 和 GIF。请访问<a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">我们的文档</a>了解更多关于使用 Aspose.SVG API 函数的信息。在文档文章 <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target= "_blank">如何合并 SVG 文件</a>，您可以考虑如何合并 SVG 的 C# 示例。

{{<section online-merger>}}
---
h2: 在线图像合并
---

Aspose.SVG 提供免费的在线 <a href="https://products.aspose.app/svg/merger" target="_blank">图像合并</a> 应用程序，可将多个图像合并到一个文件中。您可以为不同的源文件（如 SVG、JPG、PNG、BMP、ICO、GIF 或 TIFF）选择一种图像合并，并将结果保存为以下输出格式之一：JPG、PNG 或 SVG。我们的应用程序是多功能的。您可以在合并之前创建图像拼贴、编辑和操作图像。 Image Merger 允许您自由地添加图像、旋转、缩放、添加背景、过滤器和移动每个图像，直到您对设计的最终结果感到满意为止。

{{<section get-started>}}
---
h2: .NET SVG API 入门
---

从命令行安装为 ```nuget install Aspose.SVG``` 或通过 Visual Studio 的 Package Manager Console 使用 ```Install-Package Aspose.SVG``` 安装。
或者，从 [下载](https://releases.aspose.com/svg/net/) 获取 ZIP 文件中的离线 MSI 安装程序或 DLL。 Aspose.SVG for .NET API 是一个独立的库，不依赖于任何软件来处理 SVG 文档。
 有关 C# 库安装和系统要求的更多详细信息，请参阅 [Aspose.SVG 文档](https://docs.aspose.com/svg/net/getting-started/)。

{{<section other-mergers>}}
---
title: 其他支持的合并
subTitle: "您可以将 SVG 和图像合并为其他文件格式："
---