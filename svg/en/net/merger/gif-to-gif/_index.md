---
translation: true
template: ./../_template-child.md
title: Merge GIF to GIF via C# - Aspose.SVG
description: Merge GIF to GIF using .NET Core API on Windows, macOS & Linux
url: /net/merger/gif-to-gif/
family: svg
platformtag: net
feature: merge
informat: GIF
outformat: GIF
otherformats: GIF JPEG PNG TIFF BMP
---

{{<section banner>}}
---
h1: Merge GIF to GIF via C#
h2: High-speed .NET API to combine GIF files on Windows, macOS & Linux
---

{{<section overview>}}
---
h2: Merge GIF to GIF Using C#
---

GIF files have a small file size, which makes them ideal for website usage for logos, line art and simple cartoons. It uploads quickly since these files are usually low resolution. In some cases, you may need to combine GIF images and save them as one file. With [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API, you can merge GIF to GIF programmatically. Powerful C# API helps you to combine GIF files quickly and in high quality!

{{<section code-text>}}
---
h2: C# code example to merge GIF to GIF
title: Merge GIF to GIF - C#
---

Combine multiple GIF files and save the result as a single GIF file easily! Merging images can be done with a few lines of code:

{{<section "code-snippet" i18n-exclude>}}

```cs
// Images to merge 
var images = new string[] { @"image1.gif", "image2.gif" };
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
        Format = ImageFormat.Gif,
        PageSetup =
        {
            Sizing = SizingType.FitContent
        }
    };    
    // Render document 
    document.RenderTo(new ImageDevice(options, "merged.gif"));
}
```

{{<section steps>}}
---
h2: Steps to Merge GIF to GIF using C#
---

1. Define GIF images to merge. 
1. Initialize a new instance of the [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor) class. 
1. Declare an image function. You should use the [CreateElementNS(`namespaceURI, qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) method of the SVGDocument class to create an image instance. The `namespaceURI` sets the reference to W3C SVG specification. The `qualifiedName` must contain the string tag name of the image element.
1. Call the image function to create a thumbnail object.
1. To add thumbnails to the document, use [AppendChild()](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/#appendchild) method.
1. Use one of the [ImageRenderingOptions()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/) constructor to initialize a new instance of the ImageRenderingOptions class. You can customize the rendering process by specifying the page size, image format, etc. PNG is used as the default image format.
1. Create an instans of ImageDevice using the [ImageDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/imagedevice/#constructor_3) constructor.
1. Call the [RenderTo(`device`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/#renderto) method to send the current document to the output rendering device.
1. Multiple GIF images will be saved into one GIF file on the specified path.

{{<section documentation>}}

A high-speed C# library allows .NET developers to merge GIF files into one image quickly and efficiently. The [Aspose.Svg.Rendering.Image](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/) namespace provides specific device classes as well as a few rendering options classes responsible for rendering to raster formats: JPEG, PNG, BMP, GIF, and TIFF. Please visit <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">our documentation</a> to learn more about using Aspose.SVG API functions. 

{{<section online-merger>}}
---
h2: Online Image Merger
---

Aspose.SVG offers a free online <a href="https://products.aspose.app/svg/merger" target="_blank">Image Merger</a> App that combines multiple images into a single file. You can choose a kind of Image Merger for different source files such as SVG, JPG, PNG, BMP, ICO, GIF, or TIFF, and save the result to one of the following output formats: JPG, PNG or SVG. Our application is multifunctional. You can create image collages, edit and manipulate images before merging. Image Merger allows you to freely add images, rotate, scale, add backgrounds, filters and move each image until you are happy with the end result of your design.

{{<section get-started>}}
---
h2: Get Started with .NET SVG API
---

Install from command line as ```nuget install Aspose.SVG``` or via Package Manager Console of Visual Studio with ```Install-Package Aspose.SVG```.
Alternatively, get the offline MSI installer or DLLs in a ZIP file from [downloads](https://downloads.aspose.com/svg/net). Aspose.SVG for .NET API is a standalone library and does not depend on any software for SVG document processing.
 For more details about C# library installation and system requirements, please refer to [Aspose.SVG Documentation](https://docs.aspose.com/svg/net/getting-started/).

{{<section other-mergers>}}
---
title: Other Supported Mergers
subTitle: "You can merge Images into other file formats:"
---