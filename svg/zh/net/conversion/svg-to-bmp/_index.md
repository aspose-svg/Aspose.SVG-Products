﻿---
translation: true
template: /templates/_template-conversion-child.md
title: 使用 C# Core 将 SVG 转换为 BMP - 在线 SVG 到 BMP 转换器
description: 在 Windows、macOS 和 Linux 上使用 .NET Core API 加载 SVG 并将其转换为 BMP。免费试用在线 SVG 到 BMP 转换器！
url: /net/conversion/svg-to-bmp/
family: svg
platformtag: net
feature: conversion
informat: SVG
outformat: BMP
otherformats: GIF BMP JPEG PNG TIFF PDF XPS
---

{{<section banner>}}
---
h1: 通过 C# 将 SVG 转换为 BMP
h2: 用于在 Windows、macOS 和 Linux 上将 SVG 转换为 BMP 的高速 .NET API
---

{{<section overview>}}
---
h2: 通过 .NET Core 将 SVG 转换为 BMP
---

SVG 是用于网站构建和打印图形以实现可扩展性的最常用格式之一。但有时，您需要转换 SVG 并将其保存为常见的光栅图像格式。使用 [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API，您可以以编程方式将 SVG 转换为 BMP 图像，并完全控制各种转换参数。强大的 C# API 允许您将 SVG 转换为高速和高质量的流行格式。


{{<section demos>}}
---
h2: 免费在线转换器现场演示
---

在您的浏览器中测试 SVG 到 BMP 转换的质量！以下 C# 示例演示如何使用 ConvertSVG() 方法转换 SVG 文档。我们描述了从文件中读取 SVG 并使用默认保存选项将 SVG 转换为 BMP 的源代码。请从本地文件系统加载 SVG，选择输出格式并运行示例。您将立即将结果作为单独的文件获得。

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/converter SVG BMP XPS TIFF PNG PDF "JPG|JPEG" GIF>}}
using Aspose.Svg;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;
using Aspose.Svg.Rendering.Image;

    using var document = new SVGDocument("image.svg");
{{#if_output 'PDF'}}
    var options = new PdfSaveOptions();
{{/if_output}}
{{#if_output 'XPS'}}
    var options = new XpsSaveOptions();
{{/if_output}}
{{#if_output 'BMP' 'JPG' 'GIF' 'PNG' 'TIFF'}}
    var options = new ImageSaveOptions(ImageFormat.{{output param2 camel}});
{{/if_output}}
    Converter.ConvertSVG(document, options, "output.{{output lower}}");   
{{< /app/svg/converter>}} 

{{<section documentation>}}

请访问<a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">我们的文档</a>了解有关使用 Aspose.SVG API 转换函数的更多信息，并考虑最常见的 SVG 转换场景的 C# 示例。在文档文章 <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/convert-svg-to-image/" target="_blank ">Convert SVG to Image</a>，您可以考虑如何以不同方式将 SVG 转换为图像的 C# 示例。让我们考虑其中的一些：

{{<section steps1>}}
---
h2: 使用 ConvertSVG() 方法将 SVG 转换为 BMP 的步骤
---
1. 使用 [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/) 类的 SVGDocument() 构造函数之一加载 SVG 文件。
1. 使用 BMP ImageFormat 创建一个新的 [ImageSaveOptions](https://reference.aspose.com/svg/net/aspose.svg.saving/imagesaveoptions/) 对象。默认情况下，“格式”属性为 PNG。
1. 使用[ConvertSVG()](https://reference.aspose.com/svg/net/aspose.svg.converters/converter/convertsvg/)方法将SVG保存为BMP图像。您需要将 SVGDocument、ImageSaveOptions 和输出文件路径传递给 ConvertSVG() 方法。
1. BMP文件将保存到指定路径。

{{<section steps2>}}
---
h2: 使用 RenderTo() 方法将 SVG 转换为 BMP 的步骤
---
1. 使用您的 SVG 文件初始化 [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/)。
1. 创建 ImageRenderingOptions 类的对象。使用 [ImageRenderingOptions()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/imagerenderingoptions/) 构造函数并指定文档的 `Format` 属性。
1. 初始化[ImageDevice](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/)类并指定要渲染的输出文件名。
1. 调用[RenderTo()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/)方法并传递ImageDevice的实例。

{{<section code-text>}}
---
title: 将 SVG 转换为 BMP
---

{{<section "code-snippet" i18n-exclude>}}

```cs
using (var document = new SVGDocument("input.svg"))
{
	var options = new ImageRenderingOptions(ImageFormat.Bmp);
	using (IDevice device = new ImageDevice(options, "output.bmp"))
	{
		document.RenderTo(device);                    
	}
}
```

{{<section other-conversions>}}
---
title: 其他支持的 SVG 转换
subTitle: "您还可以将 SVG 转换为许多其他文件格式："
---