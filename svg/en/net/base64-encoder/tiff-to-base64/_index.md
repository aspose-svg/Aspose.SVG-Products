---
translation: true
template: /templates/_template-encoder-child.md
title: Convert TIFF to Base64 in C# 
description: Convert TIFF to Base64 in C# and use an encoded string for data URI. Embed it into HTML, CSS, XML, JSON and others.
url: /net/tiff-to-base64/
family: svg
platformtag: net
feature: encode
informat: TIFF
outformat: Base64
---

{{<section banner>}}
---
h1: Convert TIFF to Base64 in C#
h2: Encode TIFF to Base64 string in C# and use it for examples for data URI
---

{{<section overview>}}
---
h2: About URI Scheme
---

Data URI is a method of embedding images and other files in web pages as a string of text based on Base64 encoding. Data URI scheme allows you to include any binary data in HTML, CSS, JSON, or SVG documents. For example, you can embed images in a web page as if they were loaded from an external resource, but instead of specifying the URL of the file, you insert the Base64 encoded contents of the image. The data URI scheme was defined in RFC 2397, and as of 2022, it is fully supported by most major browsers. The main advantage of data URI use is a speed-up of page loading because the browser does not need to make an additional web request to retrieve the file since the image is already embedded in the HTML document.

The syntax of data URI is the following: `data:[<mime type>][;charset=<charset>][;base64],<encoded data>`.

Because the size of Base64-encoded data increases by 33%, it is recommended to use data URI only for small images. Large Base64 images produce a lot of code in the HTML, which results in a loss of performance benefits. If you need to convert TIFF to Base64 and use encoded string to embed into an HTML, CSS, JSON, or SVG file, please learn all pros and cons first. 

{{<section code-text>}}
---
h2: How to convert TIFF to Base64 in C#
title: C# code to convert TIFF to Base64 string and embed it into SVG file
---

In order to convert TIFF to Base64 string, we use [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API, which is a feature-rich, powerful, easy-to-use document manipulation API for the C# platform. We consider the example of TIFF to Base64 encoding and embedding Base64 string as data URI into an SVG document. These operations can be done with a few lines of code:

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open a binary file - TIFF image
    var bytes = File.ReadAllBytes(@"image.tiff");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert TIFF to Base64
    img.Href.BaseVal = "data:image/tiff;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: Steps to Convert TIFF to Base64 in C#
---

1. Open a TIFF image to convert. Use the ReadAllBytes(`path`) method to open the TIFF image and read the contents of the file into a byte array. 
1. Initialize a new instance of the [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor) class. 
1. Use the [CreateElementNS(`namespaceURI, qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) method of the SVGDocument class to create an image instance. The `namespaceURI` sets the reference to W3C SVG specification. The `qualifiedName` must contain the string tag name of the image element.
1. Convert TIFF to Base64. Call The ToBase64String(bytes) method to convert an array of 8-bit integers to its equivalent string representation encoded in base64 digits.
1. Add the image element into the SVG document using [AppendChild(`node`)](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/) method.
1. Use the [Save(`path`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/) method to save the SVG document.


{{<section online-encoder>}}
---
h2: Online Base64 Encoders
---

{{<section examples>}}
---
h2: Base64 Encoding Usage Examples
svg: SVG code to embed Base64 TIFF image into an SVG document
html: HTML code to embed Base64 TIFF image
css: CSS code to embed Base64 TIFF image as a background image
xml: XML code to embed Base64 TIFF image into an XML document
json: JSON code to embed Base64 TIFF image into JSON document
---

{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/tiff;charset=utf-8;base64,SUkqAAgAAAAUAP4ABAABAAAAAAAAAAABAw..." alt="Blue circle"/>
</svg>
```

{{<section code-html>}}

```cs
<body>
    <div>
        <img src="data:image/tiff;base64,SUkqAAgAAAAUAP4ABAABAAAAAAAAAAABAw..." alt="Blue circle">
    </div>
</body>
```

{{<section code-css>}}

```cs
.class {
    background-image: url('data:image/tiff;base64,SUkqAAgAAAAUAP4ABAABAAAAAAAAAAABAw...');
}
```

{{<section code-xml>}}

```cs
<?xml version="1.0" encoding="UTF-8"?>
<root>
<image mime = "image/tiff">SUkqAAgAAAAUAP4ABAABAAAAAAAAAAABAw...</image>
</root>
```

{{<section code-json>}}

```cs
{
  "image": {
    "mime": "image/tiff",
    "data": "SUkqAAgAAAAUAP4ABAABAAAAAAAAAAABAw..."
  }
}
```

{{<section other-encoders>}}
---
title: Other Supported Base64 Encoders
subTitle: "You can convert Image to Base64 string - JPG, PNG, BMP, GIF, TIFF, ICO, and SVG formats are supported:"
---