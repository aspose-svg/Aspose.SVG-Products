---
title: Merge JPG to JPG via C# - Aspose.SVG
description: Merge JPG to JPG using .NET Core API on Windows, macOS & Linux
url: /net/merger/jpg-to-jpg/
family: svg
platformtag: net
feature: merge
informat: JPG
outformat: JPG
---
{{< blocks/products/pf/main-wrap-class isAutogenPage="true" >}}
{{< blocks/products/pf/main-wrap-class >}}
{{< blocks/products/pf/upper-banner h1="Merge JPG to JPG via C#" h2="High-speed .NET API to combine JPG files on Windows, macOS & Linux" logoImageSrc="https://www.aspose.cloud/templates/aspose/img/products/svg/headers/aspose_svg-for-net.svg" pfName="Aspose.SVG " subTitlepfName="for .NET" downloadUrl="https://downloads.aspose.com/svg/net" >}}

{{< blocks/products/pf/main-container >}}

{{% blocks/products/pf/agp/content h2="Merge JPG to JPG Using C#" %}}

JPEG is a standard image format developed by the Joint Photographic Experts Group. The JPEG file compression technology is well designed and thought out. It removes redundant color data and provides an extremely high compression ratio. Still, JPEG can display vivid and colourful images and achieve better image quality with the smallest image size. In many cases, you may need to combine JPG images. With [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API, you can merge JPG to JPG programmatically. Powerful C# API allows you to transform your JPG files quickly and in high quality.</br></br>

<h2> C# code example to merge JPG to JPG </h2>
<p> A high-speed C# library allows .NET developers to merge JPG files into one image quickly and efficiently. Documents merging can be done with a few lines of code:</p></br>

{{% blocks/products/pf/agp/code-block title="Merge JPG to JPG  - C#" offSpacer="true" %}}

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
        Format = ImageFormat.Jpeg,
        PageSetup =
        {
            Sizing = SizingType.FitContent
        }
    };    
    // Render document 
    document.RenderTo(new ImageDevice(options, "merged.jpg"));
}
```
<p></p></br></br>
{{% /blocks/products/pf/agp/code-block %}}

<h2> Steps to Merge JPG to JPG using C# </h2>

1. Define images to merge. 
1. Initialize a new instance of the [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor) class. 
1. Declare an image function. You should use the [CreateElementNS(`namespaceURI, qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) method of the SVGDocument class to create an image instance. The `namespaceURI` sets the reference to W3C SVG specification. The `qualifiedName` must contain the string tag name of the image element.
1. Call the image function to create a thumbnail object.
1. To add thumbnails to the document, use [AppendChild()](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/#appendchild) method.
1. Use one of the [ImageRenderingOptions()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/) constructor to initialize a new instance of the ImageRenderingOptions class. You can customize the rendering process by specifying the page size, image format, etc. PNG is used as the default image format.
1. Create an instans of ImageDevice using the [ImageDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/imagedevice/#constructor_3) constructor.
1. Call the [RenderTo(`device`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/#renderto) method to send the current document to the output rendering device.
1. Multiple JPG images will be saved to the one JPG file on the specified path.</br></br>

The [Aspose.Svg.Rendering.Image](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/) namespace provides specific device classes as well as a few rendering options classes responsible for rendering to raster formats: JPEG, PNG, BMP, GIF, and TIFF. Please visit <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">our documentation</a> to learn more about using Aspose.SVG API functions. </br></br>
<h2>Online Image Merger</h2>
Aspose.SVG offers a free online <a href="https://products.aspose.app/svg/merger" target="_blank">Image Merger</a> App that combines multiple images into a single file. You can choose a kind of Image Merger for different source files such as SVG, JPG, PNG, BMP, ICO, GIF, or TIFF, and save the merging result to one of the following output formats: JPG, PNG or SVG. Our application is multifunctional. You can create image collages, edit and manipulate images before merging. Image Merger allows you to freely add images, rotate, scale, add backgrounds, filters and move each image until you are happy with the end result of your design.</br>

{{% /blocks/products/pf/agp/content %}}

{{% blocks/products/pf/agp/content h2="Get Started with .NET SVG API" %}}

Install from command line as ```nuget install Aspose.SVG``` or via Package Manager Console of Visual Studio with ```Install-Package Aspose.SVG```.</br>
Alternatively, get the offline MSI installer or DLLs in a ZIP file from [downloads](https://downloads.aspose.com/svg/net). Aspose.SVG for .NET API is a standalone library and does not depend on any software for SVG document processing.</br>
 For more details about C# library installation and system requirements, please refer to [Aspose.SVG Documentation](https://docs.aspose.com/svg/net/getting-started/).
{{% /blocks/products/pf/agp/content %}}

{{< blocks/products/pf/agp/other-supported-section title="Other Supported Mergers" >}}

{{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/svg/net/merger/jpg-to-jpg/" name="JPG TO JPG" description="JPEG Image" >}}
{{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/svg/net/merger/png-to-png/" name="PNG TO PNG" description="Portable Network Graphics" >}}
{{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/svg/net/merger/svg-to-pdf/" name="SVG TO PDF" description="Portable Document Format" >}}
{{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/svg/net/merger/svg-to-xps/" name="SVG TO XPS" description="XML Paper Specifications" >}}
{{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/svg/net/merger/svg-to-bmp/" name="SVG TO BMP" description="Bitmap Image" >}}
{{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/svg/net/merger/svg-to-image/" name="SVG TO IMAGE" description="Image formats" >}}
{{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/svg/net/merger/svg-to-jpeg/" name="SVG TO JPEG" description="JPEG Image" >}}
{{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/svg/net/merger/svg-to-gif/" name="SVG TO GIF" description="Graphical Interchange Format" >}}
{{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/svg/net/merger/svg-to-png/" name="SVG to PNG" description="Portable Network Graphics" >}}
{{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/svg/net/merger/svg-to-tiff/" name="SVG TO TIFF" description="Tagged Image Format" >}}

{{< /blocks/products/pf/agp/other-supported-section >}}
{{< /blocks/products/pf/main-container >}}
{{< /blocks/products/pf/main-wrap-class >}}