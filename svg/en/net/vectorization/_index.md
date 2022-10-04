---
translation: true
template: /templates/_template-vectorization.md
title: Vectorize Image or Text - C# code and Online Vectorizer
url: /net/vectorization/
description: Convert images or SVG text to vector graphics and save the output to an SVG file. Vectorize images or text online or in C#!
---

{{<section banner>}}
---
h1: Vectorize Image or Text in C# 
h2: Convert Image to vector in C#. JPG, JPEG, PNG, BMP, GIF, TIFF, ICO, IFIF, WEBP and other bitmap formats are supported.
---

{{<section overview>}}
---
title: Image Vectorization
---

A raster image is a map of pixels - dots or grains - on film, paper or screen. Each pixel has its own color. Scaling a raster image leads to noise and blurring appearing on it. To avoid such artefacts, you can convert a bitmap image into a vector format, for example, into SVG graphics. Image vectorization is a way to represent an image in vector form. A vector image is based upon a formula — it is not based upon pixels but on primitives such as points, lines, curves, which are represented by mathematical expressions. Lines and filled colored areas in such images are represented as mathematical curves that are defined by Cartesian points connected by paths to form them. A vector image will have all the benefits of vector graphics and will not be pixelated when scaled.
 
You can vectorize image with Aspose.SVG for .NET API in real-time. Try our free Image Vectorizer and convert pixel color information into simple geometric objects! Please select an image to vectorize. JPG, JPEG, PJP, PJPEG, PNG, BMP, XBM, GIF, TIFF, ICO, IFIF, WEBP and other bitmap formats are supported.

{{<section "app-pluging" i18n-exclude>}}
{{<app/svg/imagevectorizer id="1" inputFormat="Image"  sourceImage="/svg/images/encoder/flower.jpg">}}{{</app/svg/imagevectorizer>}}

{{<section plugin-use>}}
---
h2: How to Use Image Vectorizer?
---

The Image Vectorizer has three areas: Source Image, Quantized Image and Vectorized Image.

<b>Source Image</b> - this area contains the source raster image for vectorization.

<b>Quantized Image</b> - this area contains a raster image after applying color quantization. Color quantization is a process of selecting the limited number of colors to use in an image. It is applied when the color information of an image is to be reduced. Color quantization is a very complex process involving a number of factors. This can be implemented using different algorithms. Each of the algorithms determines which colors from the larger set of colors remain in the new image and how the discarded colors are mapped to the remaining ones. <br>You can manually select the number of <b>colors</b> and other color quantization settings in the sidebar.

<b>Vectorized Image</b> - this area contains the vectorized image and a settings sidebar. You can set a tolerance, severity, tension, and line-width valies. For more details about image vectorization options, please learn the documentation article <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/image-vectorization-examples/" target="_blank">Image Vectorization Examples.</a>

{{<section image-vectorization>}}
---
h2: How to Vectorize Image Using C#
title: C# code to convert JPG image to vector
---

Converting an image to vector is very easy with <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/" target="_blank">Aspose.SVG for .NET API</a>. The ImageVectorization Namespace includes classes and interfaces for implementing an image vectorization process. The following code snippet demonstrates the use of the <a href="https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/" target="_blank">ImageVectorizer</a> class to vectorize an image:

{{<section "code-image" i18n-exclude>}}

```cs       
	// Initialize an instance of the ImageVectorizer class
	var vectorizer = new ImageVectorizer
    {
		//optionally set configuration
        Configuration =
        {
			//optionally set path builder
            PathBuilder = new BezierPathBuilder {
			//optionally set trace smoother
            TraceSmoother = new ImageTraceSmoother(1),
                ErrorThreshold =  30,
                MaxIterations = 30
            },
            ColorsLimit = 25,
            LineWidth = 1
        }
    };
    // Vectorize image from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.jpg");
    // Save vectorized image as SVG file 
	document.Save(OutputFolder + "example.svg");
```

{{<section link-image>}}

You can learn more about image vectorization by clicking on the link - <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/vectorization/image-to-svg/">Image to SVG.</a>


{{<section text-vectorization>}}
---
title: Text to Vector
h2: How to Vectorize Text in C#
title-code: C# code to convert SVG text to vector
text: "We would like to share with you a feature for vectorising text elements inside an SVG document. Text Vectorization is the process of converting text into digital graphics. In the vectorized SVG text, all font glyphs are replaced with the combination of `path`, `use`, `mask`, `g` elements, etc. Thus, vectorization promotes text protection from simple copying, unwanted using, borrowing, and modification."
---

In case you are interested in the development of scalable vector graphics and their application, have a look at our flexible, high-speed Aspose.SVG for .NET API with a powerful set of interfaces for C# and other .NET programming languages. The <a href="https://reference.aspose.com/svg/net/aspose.svg.saving/" target="_blank">Aspose.Svg.Saving</a> Namespace includes the <a href="https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/" target="_blank">SVGSaveOptions</a> class, which allows you to implement the text vectorization process. To vectorize text, set the `VectorizeText` property of the SVGSaveOptions class to true:

{{<section "code-text" i18n-exclude>}}

```cs
// Load an SVG document from a file
var document = new SVGDocument("text.svg");
// Set text elements vectorization 
var saveOptions = new SVGSaveOptions
{
    VectorizeText = true
};    
// Save the SVG document with specified saveOptions
document.Save("text_vectorized.svg", saveOptions);
```

{{<section link-text>}}

You can learn more about text vectorization by clicking on the link - <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/vectorization/text-to-vector/">Text to Vector.</a>

{{<section installing>}}
---
h2: Installing Aspose.SVG for .NET library
---

<a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/" target="_blank">Aspose.SVG for .NET</a> is a cross-platform flexible library that is designed to provide a wide range of features for processing and rendering SVG documents. It seamlessly integrates into your .NET Apps to provide processing and rendering of SVG files without installing any 3rd party modeling or rendering software. Aspose.SVG for .NET offers developers to work with its DOM that is fully compatible with the official SVG specifications.  Our  API can be used with any .NET language, such as C#, VB.NET, ASP.NET, etc. It works equally well on any OS that can install Mono (.NET 4.0 Framework support) or use .NET core.  This includes Windows, Linux, and macOS.

Installing <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG for .NET through NuGet</a>: 

1. Using the Package Manager Console. Open Microsoft Visual Studio and Package Manager Console from the menu to open package manager console. Then type the command `Install-Package Aspose.SVG` and press Enter to install. 
2. Using the NuGet Package Manager GUI. Open Microsoft Visual Studio and Manage NuGet Packages from the menu to open package manager. Search for "Aspose.SVG", select and click "Install". </br>  

For more details about C# library installation, please refer to [Aspose.SVG Documentation.](https://docs.aspose.com/svg/net/getting-started/installation/)

{{<section other-vectorizers>}}
---
h2: Other Supported Vectorizers
---

You can convert Image to Vector - JPG, PNG, BMP, GIF, TIFF, and ICO formats are supported: