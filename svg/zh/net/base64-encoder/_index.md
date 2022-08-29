---
translation: true
template: /templates/_template-encoder.md
title: 在 C# 代码中将图像编码为 Base64
url: /net/base64-encoder/
description: 在 C# 代码中将图像转换为 Base64。使用编码为数据 URI 的 Base64 图像将它们嵌入 HTML、CSS 或 JSON。
---

{{<section banner>}}
---
h1: 在 C# 中将图像编码为 Base64
h2: 在 C# 中将图像转换为 Base64 编码的字符串。支持 JPG、PNG、BMP、GIF、TIFF、ICO 和 SVG 格式。
---

{{<section base64>}}
---
h2: 如何使用 C# 对图像进行编码
title: Base64 编码
---

Base64 是一组类似的编码方案，用于将二进制数据转换为 ASCII 文本格式。 Base64 通常用于通过 Internet 传输数据。将图像转换为 Base64 的结果只是一组拉丁字母、数字和两个字符——“+”和“/”。任何浏览器都知道如何处理它们。换句话说，Base64 是一种二进制到文本的编码。 Base64 编码字符串用于各种输出格式：普通 Base64、JSON、XML、数据 URI 或 CSS。

 Base64 在 Web 上特别常见，它的用途包括将图像文件或其他二进制资源嵌入文本资源(如 HTML 和 CSS 文件)中的能力。在 HTML 文件中包含图像数据意味着浏览器不需要发出额外的 Web 请求来检索文件，因为图像已经嵌入在 HTML 文档中。建议仅对小图像使用 base64 编码。大型 base64 图像会导致 HTML 中的大量代码，从而导致性能优势的损失。还应该注意的是，base64 图像永远不会被 Google 索引，因为它不会出现在图像搜索中。

{{<section demos>}}
---
h2: 在 C# 中将图像转换为 Base64
title: 将PNG图像转换为Base64的C#代码
---

本文介绍如何使用 Aspose.SVG .NET API 功能将图像文件编码为 Base64 字符串。以下 C# 示例演示了如何将 PNG 图像转换为 Base64 字符串并将其嵌入到 SVG 文件中。 ReadAllBytes(string) 方法用于打开图像(二进制文件)并将文件内容读入字节数组。 ToBase64String(bytes) 方法将 8 位整数数组转换为其等效的以 64 位数字编码的字符串表示形式。 AppendChild() 方法然后将 base64 编码图像添加到 SVG 文档。

{{<section "code" i18n-exclude>}}

```cs
    // Open a binary file - PNG image
    var bytes = File.ReadAllBytes(@"image.png");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert image to base64
    img.Href.BaseVal = "data:image/png;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section html>}}
---
h2: 在 HTML 中嵌入 Base64 图像
title: 将 Base64 图像嵌入为数据 URI 的 HTML 代码
text: 为什么需要将 Image 转换为 Base64？ Base64 编码的图像可以使用 `<img>` 标签嵌入到 HTML 中。只需使用数据 URI 将图像数据直接粘贴到 HTML 文件中。 Base64 编码和数据 URI 方案的使用减少了浏览器呈现网页所需的 HTTP 请求数量。此代码片段演示了如何在 HTML 中嵌入 Base64 图像。
---

数据 URI 由用逗号分隔的两部分组成。第一部分指定 Base64 编码的图像，第二部分指定 Base64 编码的图像字符串：
1. `data:image/jpeg;base64`，是数据URI方案头。
1. `iVBORw0KGgoAAAANSUhEUg...`是Base64编码数据。

{{<section css>}}
---
h2: 嵌入 Base64 图像作为 CSS 背景代码的示例
title: 将 Base64 图像嵌入为数据 URI 的 CSS 代码
---

减少对图像的 HTTP 请求数量的另一种方法是使用 CSS `background-image` 属性。 `background-image` 属性将图像定义为元素的背景。 background-image 属性的每个图像都可以指定为 URL 或图像数据 URI。不同的是，第一种情况浏览器发送HTTP请求获取外部图片，而第二种情况base64图片直接嵌入到文档中，不指向其他来源。因此，浏览器不需要加载 HTTP 请求来传递输出。

{{<section svg>}}
---
title: 用于嵌入 Base64 图像的 SVG 代码
---

生成的 image-base64.svg 文件的片段如下所示。 Base64 字符串被剪掉，以免弄乱 SVG 代码示例。将 Base64 图像嵌入为 URI 数据的格式如下，具体如下：

`data:[<mime type>][;charset=<charset>][;base64],<encoded data>`


{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/png;charset=utf-8;base64,iVBORw0KGgoAAAANSUhEUg..." alt="Red border"/>
</svg>
```

{{<section "code-html" i18n-exclude>}}

```cs
<body>
    <div>
        <img src="data:image/jpeg;base64,iVBORw0KGgoAAAANSUhEUg..." alt="Red border">
    </div>
</body>
```

{{<section "code-css" i18n-exclude>}}

```cs
body {
    background-image: url('data:image/jpeg;base64,iVBORw0KGgoAAAANSUhEUg...');
}
```

{{<section encoder-online>}}
---
h2: 在线 Base64 编码器
---

在线 <a href="https://products.aspose.app/svg/{{lang}}/encoding" target="_blank">Base64 Encoders</a> 将 SVG 文档或图像文件的内容转换为其等价物用 base-64 数字编码的字符串表示形式。它们还提供了数据 URI、JSON、XML 等的示例。编码工具可帮助您避免使网站内容或电子邮件消息无法读取的各种数据编码问题。 Base64 编码器安全、易于使用且完全免费。它们适用于任何浏览器和任何操作系统。立即免费将 Image 转换为 Base64！

{{<section installing>}}
---
h2: 为 .NET 库安装 Aspose.SVG
---

Aspose.SVG for .NET 是一个跨平台的灵活库，旨在为处理和呈现 SVG 文档提供广泛的功能。它无缝集成到您的 .NET 应用程序中，无需安装任何第三方软件即可处理 SVG 文件。我们的 SVG .NET API 可以与任何 .NET 语言一起使用，例如 C#、VB.NET、ASP.NET 等。它同样适用于任何可以安装 Mono(.NET 4.0 框架支持)或使用 .NET 的操作系统核。这包括 Windows、Linux 和 macOS。

通过 NuGet 安装 <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG for .NET</a>：
1. 使用包管理器控制台。
1. 使用 NuGet 包管理器 GUI。

有关 C# 库安装的更多详细信息，请参阅 [Aspose.SVG 文档。](https://docs.aspose.com/svg/net/getting-started/installation/)

{{<section other-encoders>}}
---
h2: 其他支持的编码器
---

您可以将图像编码为 Base64 - 支持 JPG、PNG、BMP、GIF、TIFF、ICO 和 SVG 格式：