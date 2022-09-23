---
translation: true
template: /templates/_template-encoder-child.md
title: 将 SVG 转换为 Base64 - 在线编码器和 C# 代码
description: 在线或在 C# 中将 SVG 转换为 Base64，并使用编码字符串作为数据 URI。 将其嵌入 HTML、CSS、XML、JSON 等。
url: /net/svg-to-base64/
family: svg
platformtag: net
feature: encode
informat: SVG
outformat: Base64
---

{{<section banner>}}
---
h1: 在线或使用 C# 将 SVG 转换为 Base64
h2: 将 SVG 编码为 Base64 字符串并将其用于数据 URI。 您可以在线或使用 C# 对图像进行编码。
---

{{<section overview>}}
---
h2: 关于 URI 方案
---

数据 URI 是一种基于 Base64 编码将图像和其他文件作为文本字符串嵌入网页中的方法。数据 URI 方案允许您在 HTML、CSS、JSON 或 SVG 文档中包含任何二进制数据。例如，您可以将图像嵌入到网页中，就好像它们是从外部资源加载的一样，但不是指定文件的 URL，而是插入图像的 Base64 编码内容。使用数据 URI 的主要优点是加快了页面加载速度，因为图像已经嵌入 HTML 文档中，因此浏览器不需要发出额外的 Web 请求来检索文件。

数据 URI 的语法如下：`data:[<mime type>][;charset=<charset>][;base64],<encoded data>`。

SVG 文件可能包含“不安全”字符。矢量图像可以将光栅作为嵌入内容或属性，其值用单引号或双引号括起来。因此，需要对该格式进行初步处理(标准化)。您可以通过数据 URI 在 HTML 或 CSS 中使用 SVG。如果 SVG 是使用数据 URI 编码的，它可以在任何浏览器中工作。

{{<section code-text>}}
---
h2: 如何在 C# 中将 SVG 转换为 Base64
title: 将 SVG 转换为 Base64 字符串并将其嵌入到 SVG 文件中的 C# 代码
---

为了将 SVG 图像转换为 Base64 字符串，我们使用 [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API，它是一个功能丰富、功能强大、易于使用的 API - 使用 C# 平台的文档操作 API。我们考虑将 SVG 图像进行 Base64 编码并将 Base64 字符串作为数据 URI 嵌入到 SVG 文档中的示例。只需几行代码即可完成这些操作：

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open an SVG image
    var bytes = File.ReadAllBytes(@"flower.svg");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert SVG image to Base64
    img.Href.BaseVal = "data:image/svg+xml;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: 在 C# 中将 SVG 转换为 Base64 的步骤
---
1. 打开要转换的 SVG 图像。使用 ReadAllBytes(`path`) 方法打开 SVG 图像并将文件内容读入字节数组。
1. 初始化[SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor)类的新实例。
1. 使用SVGDocument类的[CreateElementNS(`namespaceURI,qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns)方法创建一个图像实例。 `namespaceURI` 设置对 W3C SVG 规范的引用。 `qualifiedName` 必须包含图像元素的字符串标签名称。
1. 将 SVG 转换为 Base64。调用 ToBase64String(bytes) 方法将 8 位整数数组转换为以 base64 数字编码的等效字符串表示形式。
1. 使用 [AppendChild(`node`)](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/) 方法将图像元素添加到 SVG 文档中。
1. 使用[Save(`path`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/)方法保存SVG文档。

{{<section online-encoder>}}
---
h2: 在线 Base64 编码器
---

{{<section examples>}}
---
h2: Base64 编码使用示例
svg: 将 Base64 SVG 图像嵌入 SVG 文档的 SVG 代码
html: 嵌入 Base64 SVG 图像的 HTML 代码
css: 将 Base64 SVG 图像嵌入为背景图像的 CSS 代码
xml: 将 Base64 SVG 图像嵌入 XML 文档的 XML 代码
json: 将 Base64 SVG 图像嵌入 JSON 文档的 JSON 代码
---

{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/svg+xml;charset=utf-8;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..." alt="Blue flower"/>
</svg>
```

{{<section code-html>}}

```cs
<body>
    <div>
        <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..." alt="Blue flower">
    </div>
</body>
```

{{<section code-css>}}

```cs
.class {
    background-image: url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna...');
}
```

{{<section code-xml>}}

```cs
<?xml version="1.0" encoding="UTF-8"?>
<root>
<image mime = "image/svg+xml">PHN2ZyB3aWR0aD0iNDUwIiBoZWlna...</image>
</root>
```

{{<section code-json>}}

```cs
{
  "image": {
    "mime": "image/svg+xml",
    "data": "PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..."
  }
}
```

{{<section other-encoders>}}
---
title: 其他支持的 Base64 编码器
subTitle: "您可以将图像转换为 Base64 字符串 - 支持 JPG、PNG、BMP、GIF、TIFF、ICO 和 SVG 格式："
---