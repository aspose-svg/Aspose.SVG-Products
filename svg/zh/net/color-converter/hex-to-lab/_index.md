---
translation: true
template: ./../_template-child.md
title: C# 中的 HEX 到 LAB 转换
description: 在 C# 中使用颜色代码并将 HEX 转换为 LAB
url: /net/color-converter/hex-to-lab/
family: svg
platformtag: net
feature: color converter
informat: HEX
outformat: LAB
otherformats: HSL RGB HWB CMYK HSV LCH XYZ OKLAB OKLCH NCOL
---

{{<section banner>}}
---
h1: 通过 C# 将 HEX 转换为 LAB
h2: 在 Windows、macOS 和 Linux 上使用高速 .NET API 将 HEX 转换为 LAB 颜色
---

{{<section overview>}}
---
h2: 使用 C# 将 HEX 转换为 LAB
---

[Aspose.SVG for .NET API](https://products.aspose.com/svg/net/) 提供了一个高速 C# 库，可用于不同的 SVG 解析任务。 API 功能之一是可以轻松访问多个颜色空间。 Aspose.Svg.Converters 命名空间实现对 [ColorConverter](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/) 类（RGB、HEX、HSL、HWB、CMYK、NCOL、LCH、OKLCH、LAB、OKLAB）的解析颜色的轻松访问，并返回一个 IConvertibleColor 接口用于转换为不同的颜色空间.<br>
颜色代码或颜色格式与描述和定义颜色的方法密切相关，广泛应用于网页、设计、测绘、摄影、艺术等领域。针对不同的任务，首选不同的颜色格式。因此，有时您可能需要转换颜色代码。

{{<section input-color>}}
---
title: 什么是十六进制颜色？
---

{{<section output-color>}}
---
title: 什么是实验室颜色？
---

{{<section code-text>}}
---
h2: 在线颜色转换器
title: 将 HEX 转换为 LAB - C#
---

如果您需要将颜色从一种颜色模型转换为另一种颜色，请使用我们的免费在线工具！ 它支持各种颜色空间，包括HEX、RGB、CMYK等，您只需输入颜色值进行转换！ 在颜色区域内单击以选择颜色，或在输入文本框中输入颜色代码。 您将立即在输出部分看到所选颜色的其他颜色代码。

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/color id=1 input="HEX" output="LAB">}}
// Parse HEX color from a string
var color = ColorConverter.ConvertFrom("#DEB487");

// Convert HEX to LAB 
string labColor = color.ToLabString();

// Print the result into console
Console.WriteLine(labColor);
//result should be: lab(76.339%, 9.034%, 23.226%)
{{< /app/svg/color>}}

{{<section steps>}}
---
h2: 使用 C# 将 HEX 转换为 LAB 的步骤
---

如果您想在产品中使用转换功能或以编程方式转换颜色代码，请参阅上面的 C# 代码示例。 几行代码就可以完成颜色转换：

1. 调用ColorConverter类的[ConvertFrom()](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/convertfrom/)方法，将HEX码作为字符串传递。
1. ConvertFrom()方法从字符串表示中解析颜色，返回[IConvertibleColor](https://reference.aspose.com/svg/net/aspose.svg.drawing/iconvertiblecolor/)接口转换成需要的颜色空格。
1. IConvertibleColor.ToLabString() 方法将 HEX 转换为 LAB 颜色，格式为：lab(0%,0%,0%)。

{{<section documentation>}}

请访问我们的文档以了解有关使用 Aspose.SVG API 函数的更多信息，并考虑最常见的 SVG 处理场景的 C# 示例。在文档文章 <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-change-svg-color/" target= "_blank">如何更改 SVG 颜色</a>，您可以查看如何使用 Aspose.SVG .NET 库更改 SVG 图像中元素和背景的颜色。文章 <a href="https://docs.aspose.com/svg/net/drawing-basics/svg-color/" target="_blank">SVG 颜色</a> 深入探讨了如何SVG 文本和形状可以着色。

{{<section online-color-converter>}}

[颜色转换器](https://products.aspose.app/svg/color-converter) 是免费的在线 Web 应用程序，可让您在 RGB、HEX、HSL、HSV、HWB、LAB、CMYK 等不同颜色代码之间转换颜色、LCH、XYZ、OKLAB、OKLCH、RGBA、HSLA 等。颜色转换器易于使用，适用于任何浏览器和操作系统。输入需要转换的颜色代码后立即得到结果。

{{<section get-started>}}
---
h2: .NET SVG API 入门
---

从命令行安装为 ```nuget install Aspose.SVG``` 或通过 Visual Studio 的 Package Manager Console 使用 ```Install-Package Aspose.SVG``` 安装。
或者，从 [下载](https://downloads.aspose.com/svg/net) 获取 ZIP 文件中的离线 MSI 安装程序或 DLL。 Aspose.SVG API 是一个独立的 API，可用于应用程序中的 SVG 文档操作和解析。
有关 C# 库安装和系统要求的更多详细信息，请参阅 [Aspose.SVG 文档](https://docs.aspose.com/svg/net/getting-started/)。

{{<section other-color-converters>}}
---
title: 其他支持的颜色转换器
---