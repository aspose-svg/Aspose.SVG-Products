---
translation: true
template: /templates/_template-text-vectorization.md
title: 在 C# 中将文本转换为矢量路径 - Aspose.SVG
description: 使用 C# 对 SVG 文件中的文本进行矢量化。将文本转换为矢量图形并将其保存为 SVG。
url: /net/vectorization/text-to-vector/
family: svg
platformtag: net
feature: vectorization
informat: SVG
outformat: SVG
---

{{<section banner>}}
---
h1: C#中的文本到向量
h2: 将 SVG 文档中的文本矢量化并将其保存为矢量图形
---

{{<section overview>}}
---
h2: 将文本转换为矢量路径
---

文本矢量化是将文本转换为各种矢量路径和几何形式的过程。您可以使用不同的字体，然后将它们转换为创建自己的矢量字体的矢量轮廓。这样的文本成为矢量图，无法在文本编辑器中进行编辑。但是您可以通过在 SVG 代码中操作 `<path>`、`<use>`、`<mask>`、`<g>` 元素来编辑和自定义矢量字符。您可以将“过滤器”、“蒙版”、“不透明度”和其他效果应用于矢量化 SVG 文本，自定义其不透明度、灯光效果等功能。除此之外，您还可以变换边框、描边、阴影、发光，以及其他可以帮助您设计文本的 SVG 方面。您可以使用所有这些 SVG 功能来获得最佳效果。矢量化文本是矢量图形，无需在客户端计算机上安装即可使用字体，并且在任何计算机环境中使用时都保持其风格。因此，将文本转换为矢量形式对于在徽标、图标、横幅、广告等中的使用非常有帮助。

[Aspose.SVG for .NET](https://products.aspose.com/svg/{{lang.url-fragment}}net/) API 提供了 SVG 文档中文本矢量化的功能。查看我们的 C# 库，以便您可以轻松地将 SVG 文本转换为矢量图形！

{{<section code-text>}}
---
h2: 用于矢量化 SVG 文档中的文本的 C# 代码示例
title: 将文本转换为矢量 - C#
---

在矢量化 SVG 文本中，所有字体字形都被替换为图形元素的组合。 Aspose.SVG for .NET API 提供了矢量化 SVG 文档中文本元素的功能。要矢量化文本，请将 SVGSaveOptions 类的 [VectorizeText](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/vectorizetext/) 属性设置为 `true`。文本向量化可以用几行代码完成：

{{<section "code-snippet" i18n-exclude>}}

```cs
// Load an SVG document from a file
var document = new SVGDocument(InputFolder + "text.svg");
// Create a Save Options object 
var saveOptions = new SVGSaveOptions
{
    VectorizeText = true
};    
// Save the SVG document with specified saveOptions
document.Save((OutputFolder + "text-vectorized.svg"), saveOptions);
```

{{<section steps>}}
---
h2: 在 C# 中矢量化 SVG 文本的步骤
---
1. 使用 [SVGDocument()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/) 构造函数之一加载 SVG 文档。
1. 创建 [SVGSaveOptions](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/) 类的新实例。使用 [SVGSaveOptions()](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/svgsaveoptions/) 构造函数并设置 [VectorizeText](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/vectorizetext/) 属性为 `true`。它指向用路径替换文本元素。
1. 调用 [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_8) 方法并将输出路径和保存选项对象传递给它。



{{<section documentation>}}

在文档章节中 <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">矢量化 - 基本概述</a>，您将找到文本矢量化信息，学习如何对 SVG 文档中的文本进行矢量化并考虑 C# 示例。在文档文章 <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/text-vectorization/" target="_blank">文本矢量化& Text Security</a>，您将了解文本矢量化的优势。

{{<section online-vectorizer>}}
---
h2: 在线文本矢量化器
---

Aspose.SVG 提供免费的在线<a href="https://products.aspose.app/svg/text-to-vector" target="_blank">文本到矢量</a>应用程序，可以将文本转换为SVG文件成矢量形式。 Text to Vector 适用于任何设备、任何平台。您无需注册、插件或其他软件安装。将您的 SVG 文本转换为矢量并获得矢量图形的所有优势！

{{<section other-vectorizers>}}
---
title: 其他支持的矢量化器
---