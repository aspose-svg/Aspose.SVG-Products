---
translation: true
template: /templates/_template-conversion-child.md
title: Convert SVG to PNG in C# - Online Converter
description: Convert SVG to PNG using .NET Core API on Windows, macOS & Linux. Try online SVG to PNG Converter for free!
url: /net/conversion/svg-to-png/
family: svg
platformtag: net
feature: conversion
informat: SVG
outformat: PNG
otherformats: GIF JPEG PNG TIFF PDF XPS BMP
---

{{<section banner>}}
---
h1: Convert SVG to PNG via C#
h2: High-speed .NET API for converting SVG to PNG on Windows, macOS & Linux
---

{{<section overview>}}
---
h2: SVG to PNG Conversion via .NET Core
---

SVG is one of the most used formats for website building and print graphics to achieve scalability. But sometimes, you need to convert SVG and save it in a common raster image format. With [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API, you can transform SVG to PNG programmatically with full control over a wide range of conversion parameters. Powerful C# API allows you to convert SVG to other popular formats with high speed and high quality.


{{<section demos>}}
---
h2: Free Online Converter Live Demos
---

Test the quality of SVG to PNG conversion right in your browser! The following C# example demonstrates how to convert an SVG document using ConvertSVG() method. We describe the source code for reading SVG from a file and then converting SVG to PNG with default saving options. Please load SVG from the local file system, select the output format and run the example. You will immediately get the result as a separate file.

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/converter SVG PNG "JPG|JPEG" BMP XPS TIFF PDF GIF >}}
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

Please visit <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">our documentation</a> to learn more about using Aspose.SVG API conversion functions and to consider C# examples for the most common SVG conversion scenarios. In the documentation article <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/convert-svg-to-image/" target="_blank">Convert SVG to Image</a>, you can consider C# examples of how to convert SVG to images in different ways. Let's consider some of them: 

{{<section steps1>}}
---
h2: Steps to Convert SVG to PNG using ConvertSVG() Method
---

1.  Load an SVG file using one of the SVGDocument() constructors of the [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/) class.
1.  Create a new  [ImageSaveOptions](https://reference.aspose.com/svg/net/aspose.svg.saving/imagesaveoptions/) object. By default, the `Format` property is PNG.
1.  Use the [ConvertSVG()](https://reference.aspose.com/svg/net/aspose.svg.converters/converter/convertsvg/) method to save SVG as a PNG image. You need to pass the SVGDocument, ImageSaveOptions, and output file path to the ConvertSVG() method.
1.  The PNG file will be saved to the specified path.

{{<section steps2>}}
---
h2: Steps to Convert SVG to PNG using RenderTo() Method
---

1. Initialize [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/) with your SVG file.
1. Create an object of the ImageRenderingOptions class. Use the [ImageRenderingOptions()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/imagerenderingoptions/) constructor and specify the `Format` property of the document.
1. Initialize [ImageDevice](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/) class and specify the output file name to render. 
1. Call [RenderTo()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/) method & pass the instance of the ImageDevice.

{{<section code-text>}}
---
title: Convert SVG to PNG
---

{{<section "code-snippet" i18n-exclude>}}

```cs
using (var document = new SVGDocument("input.svg"))
{
	var options = new ImageRenderingOptions(ImageFormat.Png);
	using (IDevice device = new ImageDevice(options, "output.png"))
	{
		document.RenderTo(device);                    
	}
}
```

{{<section other-conversions>}}
---
title: Other Supported SVG Conversions
subTitle: "You can also convert SVG to many other file formats:"
---