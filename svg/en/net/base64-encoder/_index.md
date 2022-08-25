---
translation: true
template: /templates/_template-encoder.md
title: Encode Image to Base64 in C# code
url: /net/base64-encoder/
description: Convert image to Base64 in C# code. Use Base64 images encoded as data URIs to embed them in HTML, CSS, or JSON.
---

{{<section banner>}}
---
h1: Encode Image to Base64 in C# 
h2: Convert Image to Base64 encoded string in C#. JPG, PNG, BMP, GIF, TIFF, ICO, and SVG formats are supported.
---

{{<section base64>}}
---
h2: How to Encode Images Using C#
title: Base64 Encoding
---

Base64 is an encoding scheme to convert binary data into an ASCII text format. It is generally used to transfer data over the Internet. The result of converting an image to Base64 is just a set of Latin letters, numbers and two characters - “+” and “/”. Any browser knows what to do with them. In other words, Base64 is a kind of binary-to-text encoding.

 Base64 is especially common on the Web, where its use includes the ability to embed image files or other binary resources within text resources such as HTML and CSS files. Including the image data in the HTML file means the browser does not need to make an additional web request to retrieve the file because the image is already embedded in the HTML document. It is recommended to use base64 encoding only for small images. Large base64 images result in a lot of code in HTML, which results in a loss of performance benefits. It should also be noted that a base64 image will never be indexed by Google because it doesn't show up in image searches.

{{<section demos>}}
---
h2: Convert Image to Base64 in C#
title: C# code to convert PNG image to Base64
---

This article considers how to encode an image file to a Base64 string using Aspose.SVG .NET API features. The following C# example demonstrates how to convert a PNG image to a Base64 string and embed it into an SVG file. The ReadAllBytes(string) method is used to open an image  (binary file) and read the contents of the file into a byte array. The ToBase64String(bytes) method converts an array of 8-bit integers to its equivalent string representation encoded in base 64 digits. The AppendChild() method then adds the base64 encoded image to the SVG document.

{{<section "code" i18n-exclude>}}

```cs
    // Open a binary file - PNG image
    var bytes = File.ReadAllBytes(@"image.png");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert image to base64
    img.Href.BaseVal = "data:image/png;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section html>}}
---
h2: Embed a Base64 Image in HTML
title: HTML code to embed Base64 Image as data URI
text: Base64 encoded images can be embedded in HTML using the `<img>` tag. Just paste the image data directly into the HTML file using the data URI. Base64 encoding and data URI scheme usage reduce the number of HTTP requests a browser needs to render a web page. This code snippet demonstrates how you can embed Base64 images in HTML.
---

The data URI consists of two parts separated by a comma. The first part specifies a Base64 encoded image, and the second part specifies a Base64 encoded image string:

1. `data:image/jpeg;base64`, is the data URI scheme header. 
1. `iVBORw0KGgoAAAANSUhEUg...` is the encoded Base64 data.

{{<section css>}}
---
h2: Example of embedded a Base64 image as CSS background code
title: CSS code to embed Base64 Image as data URI
---

One more way to reduce the number of HTTP requests for images - is the CSS `background-image` property usage. The `background-image` property defines images as the background of an element. Each image for the background-image property can be specified as a URL or as an image data URI. The difference is that in the first case the browser sends an HTTP request to get the external image, while in the second case the base64 image is directly embedded in the document and does not point out other sources. Therefore, the browser doesn’t need to load HTTP requests to deliver the output.

{{<section svg>}}
---
title: SVG code to embed Base64 Image
---

The fragment of the resulting image-base64.svg file is shown below. The Base64 string was cut so as not to clutter up the SVG code example. The format to embed Base64 image as URI data is the following, to be specific:

`data:[<mime type>][;charset=<charset>][;base64],<encoded data>`


{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/png;charset=utf-8;base64,iVBORw0KGgoAAAANSUhEUg..." alt="Red border"/>
</svg>
```

{{<section "code-html" i18n-exclude>}}

```cs
<body>
    <div>
        <img src="data:image/jpeg;base64,iVBORw0KGgoAAAANSUhEUg..." alt="Red border">
    </div>
</body>
```

{{<section "code-css" i18n-exclude>}}

```cs
body {
    background-image: url('data:image/jpeg;base64,iVBORw0KGgoAAAANSUhEUg...');
}
```

{{<section encoder-online>}}
---
h2: Online Base64 Encoders
---

Online <a href="https://products.aspose.app/svg/{{lang}}/encoding" target="_blank">Base64 Encoders</a> convert the content of SVG documents or image files to its equivalent string representation that is encoded with base-64 digits. They also provide examples for for data URI, JSON, XML, and others. Encoding tools help you avoid various data encoding issues that make website content or email messages unreadable. Base64 Encoders are secure, easy to use and completely free. They work in any browser and on any operating system. 

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

You can also encode SVG or Image files to Base64: