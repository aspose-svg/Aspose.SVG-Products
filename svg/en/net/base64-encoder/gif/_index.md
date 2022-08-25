---
translation: true
template: /templates/_template-encoder-child.md
title: Convert GIF to Base64 via C# 
description: Convert GIF to Base64 in C# and use an encoded string for examples for data URI. Embed it into HTML, CSS, JavaScript and others.
url: /net/base64-encoder/gif/
family: svg
platformtag: net
feature: encode
informat: GIF
outformat: Base64
---

{{<section banner>}}
---
h1: Convert GIF to Base64 via C#
h2: Encode GIF to Base64 string in C# and use it for examples for data URI
---

{{<section overview>}}
---
h2: About URI Scheme
---

Data URI is based on Base64 encoding use. Data URI scheme allows you to include any binary data in web pages, in CSS, JSON, or SVG. For example, you can embed images in an HTML page as if they were loaded from an external resource. But instead of specifying the URL of the file, you insert the encoded contents of the image. To embed binary data into a text document you should encode it to Base64. The data URI scheme was defined in RFC 2397, and as of 2022, it is fully supported by most major browsers. The main advantage of data URI use is a speed-up of page loading because the browser does not need to make an additional web request to retrieve the file since the image is already embedded in the HTML document.

The syntax of data URI is the following: `data:[<mime type>][;charset=<charset>][;base64],<encoded data>`.

Because the size of Base64-encoded data increases by 33%,  it is recommended to use data URI only for small images. Large Base64 images produce a lot of code in the HTML, which results in a loss of performance benefits. GIF files are small in size, making them ideal for use as data URI on websites for logos, icons, line art, and more.

{{<section code-text>}}
---
h2: How to convert GIF to Base64 in C#
title: C# code to convert GIF to Base64 string and embed it into SVG file
---

In order to convert GIF to Base64 string, we use [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API, which is a feature-rich, powerful, easy-to-use document manipulation API for the C# platform. We consider the example of GIF to Base64 encoding and embedding Base64 string as data URI into an SVG document. These operations can be done with a few lines of code:

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open a binary file - GIF image
    var bytes = File.ReadAllBytes(@"image.gif");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert GIF to Base64
    img.Href.BaseVal = "data:image/gif;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: Steps to Convert GIF to Base64 in C#
---

1. Open a GIF image to convert. Use the ReadAllBytes(`path`) method to open the GIF image and read the contents of the file into a byte array. 
1. Initialize a new instance of the [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor) class. 
1. Use the [CreateElementNS(`namespaceURI, qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) method of the SVGDocument class to create an image instance. The `namespaceURI` sets the reference to W3C SVG specification. The `qualifiedName` must contain the string tag name of the image element.
1. Convert GIF to Base64. Call The ToBase64String(bytes) method to convert an array of 8-bit integers to its equivalent string representation encoded in base64 digits.
1. Add the image element into the SVG document using [AppendChild(`node`)](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/) method.
1. Call the [Save(`path`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/) method to save the SVG document.

{{<section online-encoder>}}
---
h2: Online Base64 Encoders
---

{{<section examples>}}
---
h2: Base64 Encoding Examples
---

{{<section get-started>}}
---
h2: Get Started with .NET SVG API
---

Install from command line as ```nuget install Aspose.SVG``` or via Package Manager Console of Visual Studio with ```Install-Package Aspose.SVG```.
Alternatively, get the offline MSI installer or DLLs in a ZIP file from [downloads.](https://releases.aspose.com/svg/net/) Aspose.SVG for .NET API is a standalone library and does not depend on any software for SVG document processing.
 For more details about C# library installation and system requirements, please refer to [Aspose.SVG Documentation.](https://docs.aspose.com/svg/net/getting-started/)

{{<section other-encoders>}}
---
title: Other Supported Base64 Encoders
subTitle: "You can convert Image to Base64 string.  JPG, PNG, BMP, GIF, TIFF, ICO, and SVG formats are supported:"
---