---
title: Convert SVG to BMP with .NET Core 
description: Load, Save and Convert SVG files using .NET Core API on Windows, macOS & Linux
url: /net/conversion/svg-to-bmp/
family: svg
platformtag: net
feature: conversion
informat: SVG
outformat: BMP
otherformats: GIF JPEG PNG TIFF 
---

{{< blocks/products/pf/main-wrap-class isAutogenPage="true" >}}
{{< blocks/products/pf/agp/upper-banner-autogen h1="Convert SVG to BMP via C#" h2="Convert SVG files to XPS, PDF & Image formats like BMP on Windows, macOS & Linux">}}
{{< blocks/products/pf/main-container >}}
{{< blocks/products/pf/agp/feature-section isGrey="true" >}}

{{% blocks/products/pf/agp/feature-section-col title="SVG to BMP Conversion on .NET Core" %}}
1. Initialize [SVGDocument](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument) with your SVG file
1. Initialize [ImageRenderingOptions](https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions) class and set output format
1. Initialize [ImageDevice](https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice) class and specify the output file name to render
1. Call [SVGDocument.RenderTo](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto) method & pass the instance of ImageDevice
{{% /blocks/products/pf/agp/feature-section-col %}}

{{% blocks/products/pf/agp/feature-section-col title="Get Started with .NET SVG API" %}}
Install from command line as ```nuget install Aspose.SVG``` or via Package Manager Console of Visual Studio with ```Install-Package Aspose.SVG```.

Alternatively, get the offline MSI installer or DLLs in a ZIP file from [downloads](https://products.aspose.com/svg/net).
{{% /blocks/products/pf/agp/feature-section-col %}}

{{% blocks/products/pf/agp/code-autogen title=".NET C# Code for SVG to BMP Conversion" gistPath="" %}}
```cs
using (var document = new SVGDocument("template.svg"))
{
	var options = new ImageRenderingOptions(ImageFormat.Bmp);
	using (IDevice device = new ImageDevice(options, "output.bmp"))
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