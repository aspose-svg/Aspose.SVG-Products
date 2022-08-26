---
translation: true
template: /templates/_template-encoder-child.md
title: 在 C# 中将 BMP 转换为 Base64
description: 在 C# 中将 BMP 转换为 Base64，并将编码字符串用于数据 URI。将其嵌入 HTML、CSS、XML、JSON 等。
url: /net/bmp-to-base64/
family: svg
platformtag: net
feature: encode
informat: BMP
outformat: Base64
---

{{<section banner>}}
---
h1: 通过 C# 将 BMP 转换为 Base64
h2: 在 C# 中将 BMP 编码为 Base64 字符串并将其用作数据 URI 的示例
---

{{<section overview>}}
---
h2: 关于 URI 方案
---

数据 URI 是一种基于 Base64 编码将图像和其他文件作为文本字符串嵌入网页中的方法。数据 URI 方案允许您在 HTML、CSS、JSON 或 SVG 文档中包含任何二进制数据。例如，您可以将图像嵌入到网页中，就好像它们是从外部资源加载的一样，但不是指定文件的 URL，而是插入图像的 Base64 编码内容。数据 URI 方案在 RFC 2397 中定义，截至 2022 年，它被大多数主流浏览器完全支持。使用数据 URI 的主要优点是加快了页面加载速度，因为图像已经嵌入到 HTML 文档中，因此浏览器不需要发出额外的 Web 请求来检索文件。

数据 URI 的语法如下：`data:[<mime type>][;charset=<charset>][;base64],<encoded data>`。

由于 Base64 编码数据的大小增加了 33%，因此建议仅对小图像使用数据 URI。大型 Base64 图像会在 HTML 中生成大量代码，这会导致性能优势的损失。

{{<section code-text>}}
---
h2: 如何在 C# 中将 BMP 转换为 Base64
title: 将 BMP 转换为 Base64 字符串并将其嵌入到 SVG 文件中的 C# 代码
---

为了将 BMP 转换为 Base64 字符串，我们使用 [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API，它是一个功能丰富、功能强大、易于使用的 API。使用 C# 平台的文档操作 API。我们考虑 BMP 到 Base64 编码并将 Base64 字符串作为数据 URI 嵌入到 SVG 文档中的示例。只需几行代码即可完成这些操作：

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open a binary file - BMP image
    var bytes = File.ReadAllBytes(@"image.bmp");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert BMP to Base64
    img.Href.BaseVal = "data:image/bmp;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: 在 C# 中将 BMP 转换为 Base64 的步骤
---
1. 打开要转换的 BMP 图像。使用 ReadAllBytes(`path`) 方法打开 BMP 图像并将文件内容读入字节数组。
1.初始化[SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor)类的新实例。
1.使用SVGDocument类的[CreateElementNS(`namespaceURI,qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns)方法创建一个图像实例。 `namespaceURI` 设置对 W3C SVG 规范的引用。 `qualifiedName` 必须包含图像元素的字符串标签名称。
1. 将 BMP 转换为 Base64。调用 ToBase64String(bytes) 方法将 8 位整数数组转换为以 base64 数字编码的等效字符串表示形式。
1. 使用 [AppendChild(`node`)](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/) 方法将图像元素添加到 SVG 文档中。
1.调用[Save(`path`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/)方法保存SVG文档。




{{<section online-encoder>}}
---
h2: 在线 Base64 编码器
---

{{<section examples>}}
---
h2: Base64 编码使用示例
html: 嵌入 Base64 BMP 图像的 HTML 代码
css: 将 Base64 BMP 图像嵌入为背景图像的 CSS 代码
xml: 将 Base64 BMP 图像嵌入 XML 文档的 XML 代码
json: 将 Base64 BMP 图像嵌入 JSON 文档的 JSON 代码
---

{{<section code-html>}}

```cs
<body>
    <div>
        <img src="data:image/bmp;base64,Qk04DAAAAAAAADYAAAAoAAA...=" alt="Blue circle">
    </div>
</body>
```

{{<section code-css>}}

```cs
.class {
    background-image: url('data:image/bmp;base64,Qk04DAAAAAAAADYAAAAoAAA...=');
}
```

{{<section code-xml>}}

```cs
<?xml version="1.0" encoding="UTF-8"?>
<root>
 <image mime = "image/bmp">Qk04DAAAAAAAADYAAAAoAAA...=</image>
</root>
```

{{<section code-json>}}

```cs
{
  "image": {
    "mime": "image/bmp",
    "data": "Qk04DAAAAAAAADYAAAAoAAA...="
  }
}
```

{{<section other-encoders>}}
---
title: 其他支持的 Base64 编码器
subTitle: "您可以将 Image 转换为 Base64 字符串。支持 JPG、PNG、BMP、GIF、TIFF、ICO 和 SVG 格式："
---