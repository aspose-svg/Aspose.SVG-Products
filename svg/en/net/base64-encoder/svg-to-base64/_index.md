---
translation: true
template: /templates/_template-encoder-child.md
title: Convert SVG to Base64 in C# 
description: Convert SVG to Base64 in C# and use an encoded string for data URI. Embed it into HTML, CSS, XML, JSON and others.
url: /net/svg-to-base64/
family: svg
platformtag: net
feature: encode
informat: SVG
outformat: Base64
---

{{<section banner>}}
---
h1: Convert SVG to Base64 in C#
h2: Encode SVG image to Base64 string in C# and use it for examples for data URI
---

{{<section overview>}}
---
h2: About URI Scheme
---

Data URI is a method of embedding images and other files in web pages as a string of text based on Base64 encoding. Data URI scheme allows you to include any binary data in HTML, CSS, JSON, or SVG documents. For example, you can embed images in a web page as if they were loaded from an external resource, but instead of specifying the URL of the file, you insert the Base64 encoded contents of the image. The main advantage of data URI use is a speed-up of page loading because the browser does not need to make an additional web request to retrieve the file since the image is already embedded in the HTML document.

The syntax of data URI is the following: `data:[<mime type>][;charset=<charset>][;base64],<encoded data>`.

SVG files may contain “unsafe” characters. Vector images can have raster as embedded content or attributes whose values are enclosed in single or double quotes. Therefore, preliminary processing (normalization) of this format is required. You can use SVG in HTML or CSS via data URI. If SVG is encoded using data URI, it will work in any browser. 

{{<section code-text>}}
---
h2: How to convert SVG to Base64 in C#
title: C# code to convert SVG to Base64 string and embed it into SVG file
---

In order to convert SVG image to Base64 string, we use [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) API, which is a feature-rich, powerful, easy-to-use document manipulation API for the C# platform. We consider the example of SVG image to Base64 encoding and embedding Base64 string as data URI into an SVG document. These operations can be done with a few lines of code:

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open an SVG image
    var bytes = File.ReadAllBytes(@"flower.svg");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert SVG image to Base64
    img.Href.BaseVal = "data:image/svg+xml;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: Steps to Convert SVG to Base64 in C#
---

1. Open an SVG image to convert. Use the ReadAllBytes(`path`) method to open the SVG image and read the contents of the file into a byte array. 
1. Initialize a new instance of the [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor) class. 
1. Use the [CreateElementNS(`namespaceURI, qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) method of the SVGDocument class to create an image instance. The `namespaceURI` sets the reference to W3C SVG specification. The `qualifiedName` must contain the string tag name of the image element.
1. Convert SVG to Base64. Call The ToBase64String(bytes) method to convert an array of 8-bit integers to its equivalent string representation encoded in base64 digits.
1. Add the image element into the SVG document using [AppendChild(`node`)](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/) method.
1. Use the [Save(`path`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/) method to save the SVG document.


{{<section online-encoder>}}
---
h2: Online Base64 Encoders
---

{{<section examples>}}
---
h2: Base64 Encoding Usage Examples
svg: SVG code to embed Base64 SVG image into an SVG document
html: HTML code to embed Base64 SVG image
css: CSS code to embed Base64 SVG image as a background image
xml: XML code to embed Base64 SVG image into an XML document
json: JSON code to embed Base64 SVG image into JSON document
---

{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/svg+xml;charset=utf-8;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..." alt="Blue flower"/>
</svg>
```

{{<section code-html>}}

```cs
<body>
    <div>
        <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..." alt="Blue flower">
    </div>
</body>
```

{{<section code-css>}}

```cs
.class {
    background-image: url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna...');
}
```

{{<section code-xml>}}

```cs
<?xml version="1.0" encoding="UTF-8"?>
<root>
<image mime = "image/svg+xml">PHN2ZyB3aWR0aD0iNDUwIiBoZWlna...</image>
</root>
```

{{<section code-json>}}

```cs
{
  "image": {
    "mime": "image/svg+xml",
    "data": "PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..."
  }
}
```

{{<section other-encoders>}}
---
title: Other Supported Base64 Encoders
subTitle: "You can convert Image to Base64 string - JPG, PNG, BMP, GIF, TIFF, ICO, and SVG formats are supported:"
---