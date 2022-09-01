---
translation: true
template: /templates/_template-encoder-child.md
title: Convert ICO to Base64 in C# code
description: Convert ICO to Base64 in C# and use an encoded string for data URI. Embed it into HTML, CSS, XML, JSON and others.
url: /net/ico-to-base64/
family: svg
platformtag: net
feature: encode
informat: ICO
outformat: Base64
---

{{<section banner>}}
---
h1: Convert ICO to Base64 via C#
h2: Encode ICO to Base64 string in C# and use it for examples for data URI
---

{{<section overview>}}
---
h2: About URI Scheme
---

Data URI is a method of embedding images and other files in web pages as a string of text based on Base64 encoding. Data URI scheme allows you to include any binary data in HTML, CSS, JSON, or SVG documents. For example, you can embed images in a web page as if they were loaded from an external resource, but instead of specifying the URL of the file, you insert the Base64 encoded contents of the image. The data URI scheme was defined in RFC 2397, and as of 2022, it is fully supported by most major browsers. The main advantage of data URI use is a speed-up of page loading because the browser does not need to make an additional web request to retrieve the file since the image is already embedded in the HTML document.

The syntax of data URI is the following: `data:[<mime type>][;charset=<charset>][;base64],<encoded data>`.

Because the size of Base64-encoded data increases by 33%, it is recommended to use data URI only for small images. Large Base64 images produce a lot of code in the HTML, which results in a loss of performance benefits. An ICO image contains an icon generally used to represent a Windows program, file, or folder. Windows ICO files typically store images ranging from 16x16 to 256x256 pixels. If you need to convert ICO to Base64 and use encoded string to embed ICO image into a text file, please learn all pros and cons.

{{<section code-text>}}
---
h2: How to convert ICO to Base64 in C#
title: C# code to convert ICO to Base64 string and embed it into SVG file
---

In order to convert ICO to Base64 string, we use [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API, which is a feature-rich, powerful, easy-to-use document manipulation API for the C# platform. We consider the example of ICO to Base64 encoding and embedding Base64 string as data URI into an SVG document. These operations can be done with a few lines of code:

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open a binary file - ICO image
    var bytes = File.ReadAllBytes(@"image.ico");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert ICO to Base64
    img.Href.BaseVal = "data:image/ico;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: Steps to Convert ICO to Base64 in C#
---

1. Open a ICO image to convert. Use the ReadAllBytes(`path`) method to open the ICO image and read the contents of the file into a byte array. 
1. Initialize a new instance of the [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor) class. 
1. Use the [CreateElementNS(`namespaceURI, qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) method of the SVGDocument class to create an image instance. The `namespaceURI` sets the reference to W3C SVG specification. The `qualifiedName` must contain the string tag name of the image element.
1. Convert ICO to Base64. Call The ToBase64String(bytes) method to convert an array of 8-bit integers to its equivalent string representation encoded in base64 digits.
1. Add the image element into the SVG document using [AppendChild(`node`)](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/) method.
1. Call the [Save(`path`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/) method to save the SVG document.


{{<section online-encoder>}}
---
h2: Online Base64 Encoders
---

{{<section examples>}}
---
h2: Base64 Encoding Usage Examples
svg: SVG code to embed Base64 ICO image into an SVG document
html: HTML code to embed Base64 ICO image
css: CSS code to embed Base64 ICO image as a background image
xml: XML code to embed Base64 ICO image into an XML document
json: JSON code to embed Base64 ICO image into JSON document
---

{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/x-icon;charset=utf-8;base64,Qk04DAAAAAAAADYAAAAoAAAAIAAAACAAAAABABgAAAAAAAIMAAASCwAAEgs..." alt="Blue circle"/>
</svg>
```

{{<section "code-html" i18n-exclude>}}

```cs
<body>
    <div>
        <img src="data:image/x-icon;base64,Qk04DAAAAAAAADYAAAAoAAAAIAAAACAAAAABABgAAAAAAAIMAAASCwAAEgs..." alt="Blue circle">
    </div>
</body>
```

{{<section "code-css" i18n-exclude>}}

```cs
.class {
    background-image: url('data:image/x-icon;base64,Qk04DAAAAAAAADYAAAAoAAAAIAAAACAAAAABABgAAAAAAAIMAAASCwAAEgs...');
}
```

{{<section "code-xml" i18n-exclude>}}

```cs
<?xml version="1.0" encoding="UTF-8"?>
<root>
<image mime = "image/x-icon">Qk04DAAAAAAAADYAAAAoAAAAIAAAACAAAAABABgAAAAAAAIMAAASCwAAEgs...</image>
</root>
```

{{<section "code-json" i18n-exclude>}}

```cs
{
  "image": {
    "mime": "image/x-icon",
    "data": "Qk04DAAAAAAAADYAAAAoAAAAIAAAACAAAAABABgAAAAAAAIMAAASCwAAEgs..."
  }
}
```

{{<section other-encoders>}}
---
title: Other Supported Base64 Encoders
subTitle: "You can convert Image to Base64 string. JPG, PNG, BMP, GIF, TIFF, ICO, and SVG formats are supported:"
---