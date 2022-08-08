---
translation: true
template: /templates/_template-merger-child.md
title: Merge SVG to XPS via C# - Aspose.SVG
description: Merge SVG to XPS using C# on Windows, macOS & Linux
url: /net/merger/svg-to-xps/
family: svg
platformtag: net
feature: merge
informat: SVG
outformat: XPS
otherformats: XPS PDF GIF JPEG PNG TIFF BMP
---

{{<section banner>}}
---
h1: Merge SVG to XPS via C#
h2: High-speed .NET API to combine SVG files on Windows, macOS & Linux
---

{{<section overview>}}
---
h2: Merge SVG to XPS in C#
---

SVG is one of the most used formats for website building and print graphics to achieve scalability. But sometimes, you need to merge SVG files and save them as one document in another file format. XPS format has a set of advantages that support security features and more. With [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API, you can merge SVG to XPS programmatically. Powerful C# API helps you to combine SVG files quickly and in high quality!

{{<section code-text>}}
---
h2: C# code example to merge SVG to XPS
title: Merge SVG to XPS - C#
---

A high-speed C# library allows .NET developers to merge SVG files and convert the combined result into other popular formats such as PDF, XPS, JPEG, PNG, BMP, GIF, and TIFF quickly and efficiently. Documents merging can be done with a few lines of code:

{{<section "code-snippet" i18n-exclude>}}

```cs
// Initialize SVG documents from files to merge 
using (var document1 = new SVGDocument("document1.svg"))
using (var document2 = new SVGDocument("document2.svg"))
using (var document3 = new SVGDocument("document3.svg"))
{
    // Create an instance of SvgRenderer
    using var renderer = new Aspose.Svg.Rendering.SvgRenderer();	
    // Create an instance of XpsDevice
    using var device = new Aspose.Svg.Rendering.Xps.XpsDevice("result.xps");
    // Merge SVG to XPS
    renderer.Render(device, document1, document2, document3);                
}
```

{{<section steps>}}
---
h2: Steps to Merge SVG to XPS using C#
---

1.  Load an SVG document using one of the [SVGDocument()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/) constructors.
1.  Create a new instance of the [SvgRenderer](https://reference.aspose.com/svg/net/aspose.svg.rendering/svgrenderer/) class.
1.  Use the [XpsDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.xps/xpsdevice/xpsdevice/#constructor_5) constructor to initialize a new instance of the XpsDevice class.
1.  Call the [Render()](https://reference.aspose.com/svg/net/aspose.svg.rendering/renderer-1/) method to merge SVGs into a single XPS file.
1.  Multiple SVG files will be saved into one XPS file at the specified path.

{{<section documentation>}}

The [Aspose.Svg.Rendering](https://reference.aspose.com/svg/net/aspose.svg.rendering/) namespace implements easy access to Render() methods. You can quickly perform SVG merge and export the combining result to popular formats, such as PDF, XPS, JPEG, PNG, BMP, TIFF, and GIF. Please visit <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">our documentation</a> to learn more about using Aspose.SVG API functions. In the documentation article <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target="_blank">How to Merge SVG Files</a>, you can consider C# examples of how to merge SVG.

{{<section online-merger>}}
---
h2: Online SVG Merger
---

Aspose.SVG offers a free online <a href="https://products.aspose.app/svg/merger/svg" target="_blank">Merge SVG</a> app that combines multiple SVGs into a single file. You can choose a kind of SVG Merger for different output files such as SVG, JPG or PNG. Our application is multifunctional. You can create image collages, edit and manipulate SVG images before merging. SVG Merger allows you to freely add images, rotate, scale, add backgrounds, filters and move each image until you are happy with the end result of your design.

{{<section get-started>}}
---
h2: Get Started with .NET SVG API
---

Install from command line as ```nuget install Aspose.SVG``` or via Package Manager Console of Visual Studio with ```Install-Package Aspose.SVG```.
Alternatively, get the offline MSI installer or DLLs in a ZIP file from [downloads](https://releases.aspose.com/svg/net/). Aspose.SVG for .NET API is a standalone library and does not depend on any software for SVG document processing.
 For more details about C# library installation and system requirements, please refer to [Aspose.SVG Documentation](https://docs.aspose.com/svg/net/getting-started/).

{{<section other-mergers>}}
---
title: Other Supported Mergers
subTitle: "You can merge SVG & Images into other file formats:"
---