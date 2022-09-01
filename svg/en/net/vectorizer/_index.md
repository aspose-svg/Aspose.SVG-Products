---
translation: true
template: /templates/_template-vectorizer.md
title: Vectorize Image or Text - C# code and Online Vectorizer 
url: /net/vectorizer/
description: Vectorizer converts raster images or SVG text to vector graphics and saves the output to SVG file
---

{{<section banner>}}
---
h1: Vectorize Image or Text in C# 
h2: Convert Image to vector in C#. JPG, PNG, BMP, GIF, TIFF, and ICO formats are supported.
---

{{<section overview>}}
---
title: Image Vectorization
---

A raster image is a collection of pixels - dots or grains - on film, paper or screen. Image vectorization is a way to represent an image in vector form. The vector image will have all the advantages of vector graphics, and will not be pixelated when scaled.

Scaling a raster image leads to noise and blurring appearing on it. To avoid such artefacts, you can convert a bitmap image into a vector format, for example, into SVG graphics.

A raster image is a map of pixels, each pixel having it’s own color. A vector image is an image based upon a formula—it is not based upon pixels.
 

{{<section image-vectorization>}}
---
h2: How to Vectorize Image Using C#
title: C# code to convert PNG image to vector
---

Converting an image to a vector is very easy with the Aspose.SVG API. The ImageVectorization Namespace includes classes and interfaces for implementing an image vectorization process. The following code snippet demonstrates the use of the ImageVectorizer class to vectorize an image:

{{<section "code-image" i18n-exclude>}}

```cs       
	// Initialize an instance of the ImageVectorizer class
    var vectorizer = new ImageVectorizer
    {
        Configuration = 
		{
			TraceSmoother =   new ImageTraceSmoother(1),
			TraceSimplifier = new ImageTraceSimplifier(0.5f),
			ColorsLimit = 3
		}
    };
    // Vectorize image from the specified file
	using var document = vectorizer.Vectorize("image.png"));
    // Save vectorized image as SVG file 
	document.Save("image.svg"));
```

{{<section text-vectorization>}}
---
title: Text to Vector
h2: How to Vectorize Text in C#
title-code: C# code to convert SVG text to vector
---

Text Vectorization is the process of converting text into digital graphics. In the vectorized SVG text, all font glyphs are replaced with the combination of path, use, mask, g elements, etc. Thus, vectorization promotes text protection from simple copying, unwanted using, borrowing, and modification.

{{<section "code-text" i18n-exclude>}}

```cs
// Load an SVG document from a file
var document = new SVGDocument("text.svg"));
// Set text elements vectorization 
var saveOptions = new SVGSaveOptions
{
    VectorizeText = true
};    
// Save the SVG document with specified saveOptions
document.Save("text_vectorized.svg", saveOptions);
```

{{<section online>}}
---
h2: Online Image Vectorizer
---

Online <a href="https://products.aspose.app/svg/{{lang}}/encoding" target="_blank">Base64 Encoders</a> convert the content of SVG documents or image files to its equivalent string representation that is encoded with base-64 digits. They also provide examples for for data URI, JSON, XML, and others. Encoding tools help you avoid various data encoding issues that make website content or email messages unreadable. Base64 Encoders are secure, easy to use and completely free. They work in any browser and on any operating system. Convert Image to Base64 for free just now!

{{<section installing>}}
---
h2: Installing Aspose.SVG for .NET library
---

Aspose.SVG for .NET is a cross-platform flexible library that is designed to provide a wide range of features for processing and rendering SVG documents. It seamlessly integrates into your .NET Apps to work with SVG files without installing any 3rd party software.  Our SVG .NET API can be used with any .NET language, such as C#, VB.NET, ASP.NET, etc. It works equally well on any OS that can install Mono (.NET 4.0 Framework support) or use .NET core.  This includes Windows, Linux, and macOS.

Installing <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG for .NET through NuGet</a>:

1. Using the Package Manager Console. 
1. Using the NuGet Package Manager GUI.  

For more details about C# library installation, please refer to [Aspose.SVG Documentation.](https://docs.aspose.com/svg/net/getting-started/installation/)

{{<section other-vectorizers>}}
---
h2: Other Supported Vectorizers
---

You can convert Image to Vector - JPG, PNG, BMP, GIF, TIFF, and ICO formats are supported: