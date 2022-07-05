---
translation: true
template: ./../_template-child.md
title: 通过 C# 将 JPG 合并到 PNG - Aspose.SVG
description: 在 Windows、macOS 和 Linux 上使用 .NET Core API 将 JPG 合并到 PNG
url: /net/merger/jpg-to-png/
family: svg
platformtag: net
feature: merge
informat: JPG
outformat: PNG
otherformats: GIF JPG TIFF BMP
---

{{<section banner>}}
---
h1: 通过 C# 将 JPG 合并为 PNG
h2: 用于在 Windows、macOS 和 Linux 上组合 JPG 文件的高速 .NET API
---

{{<section overview>}}
---
h2: 使用 C# 将 JPG 合并为 PNG
---

JPEG 是由联合图像专家组开发的标准图像格式。 JPEG可以显示生动多彩的图像，并以最小的图像尺寸获得更好的图像质量。 PNG是指一种使用无损压缩的光栅图像文件格式，因此在用户中很受欢迎。每种图像格式都有其优点和缺点，在许多情况下，您可能需要组合 JPG 图像并将它们保存为一个 PNG 文件。使用 [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API，您可以以编程方式将 JPG 合并到 PNG。强大的 C# API 帮助您快速、高质量地合并 JPG 文件！

{{<section code-text>}}
---
h2: 将 JPG 合并为 PNG 的 C# 代码示例
title: 将 JPG 合并为 PNG - C#
---

合并多个 JPG 文件并将结果轻松保存为单个 PNG！合并图像可以用几行代码完成：

{{<section "code-snippet" i18n-exclude>}}

```cs
// Images to merge 
var images = new string[] { @"image1.jpg", "image2.jpg" };
// Initialize a new instance of SVGDocument
using (var document = new SVGDocument())
{
    // Declare an image function
    SVGImageElement CreateThumbnail(string imagePath, int width, int height)
    {
        var image = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
        image.Href.BaseVal = imagePath;
        image.Width.BaseVal.Value = width;
        image.Height.BaseVal.Value = height;
        return image;
    }
    // Set a thumbnail size
    const int thumbnailWidth = 200;
    const int thumbnailHeight = 200;
    const int thumbnailMargin = 10;
    // Create thumbnails merging loop
    for (var i = 0; i < images.Length; i++)
    {
        // Create a thumbnail
        var thumbnail = CreateThumbnail(images[i], thumbnailWidth, thumbnailHeight);
        // Define coordinates 
        thumbnail.X.BaseVal.Value = 0;
        thumbnail.Y.BaseVal.Value = (thumbnailHeight + thumbnailMargin) * i;
        // Append the thumbnail to the document
        document.DocumentElement.AppendChild(thumbnail);
    }
    // Define saving options
    var options = new ImageRenderingOptions
    {
        Format = ImageFormat.Png,
        PageSetup =
        {
            Sizing = SizingType.FitContent
        }
    };    
    // Render document 
    document.RenderTo(new ImageDevice(options, "merged.png"));
}
```

{{<section steps>}}
---
h2: 使用 C# 将 JPG 合并为 PNG 的步骤
---
1. 定义要合并的 JPG 图片。
1.初始化[SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor)类的新实例。
1.声明一个图像函数。您应该使用 SVGDocument 类的 [CreateElementNS(`namespaceURI,qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) 方法创建一个图像实例。 `namespaceURI` 设置对 W3C SVG 规范的引用。 `qualifiedName` 必须包含图像元素的字符串标签名称。
1.调用image函数创建缩略图对象。
1. 要将缩略图添加到文档中，请使用 [AppendChild()](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/#appendchild) 方法。
1. 使用 [ImageRenderingOptions()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/) 构造函数之一初始化 ImageRenderingOptions 类的新实例。您可以通过指定页面大小、图像格式等来自定义渲染过程。PNG 用作默认图像格式。
1. 使用 [ImageDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/imagedevice/#constructor_3) 构造函数创建 ImageDevice 的实例。
1.调用[RenderTo(`device`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/#renderto)方法将当前文档发送到输出渲染设备。
1. 多张JPG图片将被保存到指定路径的一个PNG文件中。



{{<section documentation>}}

高速 C# 库允许 .NET 开发人员快速有效地将 JPG 文件合并为一个 PNG 图像。 [Aspose.Svg.Rendering.Image](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/) 命名空间提供了特定的设备类以及一些负责渲染的渲染选项类光栅格式：JPEG、PNG、BMP、GIF 和 TIFF。请访问<a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">我们的文档</a>了解更多关于使用 Aspose.SVG API 函数的信息。

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
或者，从 [下载](https://downloads.aspose.com/svg/net) 获取 ZIP 文件中的离线 MSI 安装程序或 DLL。 Aspose.SVG for .NET API 是一个独立的库，不依赖于任何软件来处理 SVG 文档。
 有关 C# 库安装和系统要求的更多详细信息，请参阅 [Aspose.SVG 文档](https://docs.aspose.com/svg/net/getting-started/)。

{{<section other-mergers>}}
---
title: 其他支持的合并
subTitle: "您可以将图像合并为其他文件格式："
---