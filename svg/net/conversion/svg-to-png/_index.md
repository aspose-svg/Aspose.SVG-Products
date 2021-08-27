---
title: Convert SVG to PNG on .NET 
description: Load, Save and Convert SVG files using .NET API
url: /net/conversion/svg-to-png/
family: svg
platformtag: net
feature: conversion
informat: SVG
outformat: PNG
platform: .NET
otherformats: TIFF GIF JPEG PNG 
---

{{< blocks/products/pf/main-wrap-class isAutogenPage="true" >}}
{{< blocks/products/pf/agp/upper-banner-autogen h1="Convert SVG to PNG via C#" h2="Convert SVG files to XPS, PDF & Image formats on .NET">}}
{{< blocks/products/pf/main-container >}}
{{< blocks/products/pf/agp/feature-section isGrey="true" >}}

{{% blocks/products/pf/agp/feature-section-col title="SVG to PNG Conversion on .NET" %}}
1. Initialize [SVGDocument](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument) with your SVG file
1. Initialize [ImageRenderingOptions](https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions) class and set output format
1. Initialize [ImageDevice](https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice) class and specify the output file name to render
1. Call [SVGDocument.RenderTo](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto) method & pass the instance of ImageDevice
{{% /blocks/products/pf/agp/feature-section-col %}}

{{% blocks/products/pf/agp/feature-section-col title="Get Started with .NET SVG API" %}}
Install from command line as ```nuget install Aspose.SVG``` or via Package Manager Console of Visual Studio with ```Install-Package Aspose.SVG```.

Alternatively, get the offline MSI installer or DLLs in a ZIP file from [downloads](https://products.aspose.com/svg/net).
{{% /blocks/products/pf/agp/feature-section-col %}}

{{% blocks/products/pf/agp/code-autogen title=".NET C# Code for SVG to PNG Conversion" gistPath="" %}}
```cs
using (var document = new SVGDocument("template.svg"))
{
	var options = new ImageRenderingOptions(ImageFormat.Png);
	using (IDevice device = new ImageDevice(options, "output.png"))
	{
		document.RenderTo(device);                    
	}
}
```
{{% /blocks/products/pf/agp/code-autogen %}}
{{< /blocks/products/pf/agp/feature-section >}}
{{< blocks/products/pf/agp/about-file-autogen >}}
{{< blocks/products/pf/agp/other-supported-autogen >}}
{{< /blocks/products/pf/main-container >}}
{{< /blocks/products/pf/main-wrap-class >}}