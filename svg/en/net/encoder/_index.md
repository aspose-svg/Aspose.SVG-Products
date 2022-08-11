---
translation: true
template: /templates/_template-encoder.md
title: Encode Image to Base64 - C# Examples
url: /net/encoder/
description: Learn how to encode images to Base64, JSON, XML, URI, and CSS in C# code. Check online Base64 Encoder for free!
---

{{<section banner>}}
---
h1: Encode Image to Base64 in C# 
h2: Convert JPG, PNG, BMP, GIF, TIFF, ICO, or SVG to Base64 encoded string in C#
---

{{<section overview>}}
---
h2: How to Encode Images or SVG Using C#
---

SVG (Scalable Vector Graphics) is an XML-based image format for two-dimensional graphics. It is a vector graphics format intended primarily for the Web. The main excellence of SVG is its unmatched ability to be scaled to any size without any shred of quality degradation. All modern browsers support SVG, and it would seem that the Web should already switch to vector graphics. However, there are some restrictions on the use of SVG and sometimes you need to convert SVG to other formats.
 
<a href="https://products.aspose.com/svg/net/" target="_blank">Aspose.SVG for .NET API</a> makes the conversion process easier for developers. Converting between formats can perform by using a few different approaches:
 - The static [Converter class](https://reference.aspose.com/svg/net/aspose.svg.converters/converter/) is a shared facade that provides SVG file conversions to the popular formats and allows to make these operations convenient and easy. 

 - The [RenderTo()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/) method is used to render SVG to another format and send a document to the output device. Aspose.SVG API provides the following output devices implementation: the PdfDevice, XpsDevice,  and ImageDevice classes, which perform rendering to PDF, XPS, and Image file formats respectively.

{{<section demos>}}
---
h2: Encoder Live Demos
---

You can encode SVG with Aspose.SVG for .NET API in real-time. The following C# example demonstrates how to encode an SVG document. Please load a file from the local file system, select the output format and run the example. You will immediately get the result as a separate file.

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/converter SVG PDF BMP "JPG|JPEG" PNG GIF TIFF XPS>}}
using Aspose.Svg;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;

    using var document = new SVGDocument("input.{{input lower}}");
{{#if_output 'PDF'}}
    var options = new PdfSaveOptions();
{{/if_output}}
{{#if_output 'DOCX'}}
    var options = new DocSaveOptions();
{{/if_output}}
{{#if_output 'XPS'}}
    var options = new XpsSaveOptions();
{{/if_output}}
{{#if_output 'MD'}}
    var options = new MarkdownSaveOptions();
{{/if_output}}
{{#if_output 'BMP' 'JPG' 'GIF' 'PNG' 'TIFF'}}
    var options = new ImageSaveOptions(ImageFormat.{{output camel}});
{{/if_output}}
    Converter.ConvertSVG(document, options, "output.{{output lower}}");
{{< /app/svg/converter>}}

{{<section encoder-online>}}
---
h2: Online Base64 Encoders
---

Online Base64 Encoders convert the content of SVG documents or image files to its equivalent string representation that is encoded with base-64 digits. They also provide examples for for data URI, JSON, XML, and others. You can choose the output format that you need: Plain Base64, Data URI, JSON, CSS, or XML.

{{<section installing>}}
---
h2: Installing Aspose.SVG for .NET library
---

Aspose.SVG for .NET is a cross-platform flexible library that is designed to provide a wide range of features for processing and rendering SVG documents. It seamlessly integrates into your .NET Apps to work with SVG files without installing any 3rd party software.  Our SVG .NET API can be used with any .NET language, such as C#, VB.NET, ASP.NET, etc. It works equally well on any OS that can install Mono (.NET 4.0 Framework support) or use .NET core.  This includes Windows, Linux, and macOS.

Installing <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG for .NET through NuGet</a>:

1. Using the Package Manager Console. 
1. Using the NuGet Package Manager GUI.  

For more details about C# library installation, please refer to [Aspose.SVG Documentation.](https://docs.aspose.com/svg/net/getting-started/installation/)

{{<section other-conversions>}}
---
h2: Other Supported Encoders
---

You can also encode SVG or Image files into other output formats including few listed below: