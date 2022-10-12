---
translation: true
template: /templates/_template-vectorization-child.md
title: Image stenciling - C# code and Online Stencil Maker 
description: Convert Image to SVG and apply stencil transformation in C#. Vectorize and stenciling Images and get all advantages of vector graphics. Try Online Stencil Maker for free!
url: /net/vectorization/stencil/
family: svg
platformtag: net
feature: vectorization, stencil
informat: Image
outformat: SVG
---

{{<section banner>}}
---
h1: Stancil drawing - C# code and Stencil Maker
h2: Make stancil form images online or programmatically.
---

{{<section overview>}}
---
h2:  What is an image stenciling?
---

The image stenciling is a process that turns an ordinary photo into an outline image that can be used as a stencil for graffiti-like effects. 

There are several basic steps for turning a photo or image into a stencil:

* Convert a photo or image to grayscale, this step is optional, as you can reduce the number of colors to quantize instead.
* Quantize the image to get the stancil, after that you can download the result or vectorize it and get the stancil shape lines.
* There are three options for drawing stencils. The first is "None" when all the vectorized shapes are filled, the second is "Auto" when the shapes are not filled and the borders have the "original" color, and the last is "MonoСolor" when the shapes are also not filled, but the borders have the predefined color. 
<br>
[Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) offers a high-speed C# library that you can use for different SVG parsing tasks. The [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) Namespace includes classes and interfaces for implementing the image vectorization process with stenciling options.

{{<section output-file>}}
---
title: What is SVG File Format?
---

{{<section plagin-text>}}
---
h2: Online Stencil Maker
---

If you need to turn your photos or images into stencils, use our free online tool! It allows not only to get raster stencils, but also to vectorize them and work with scalable and clear vectors. Stencil Maker supports JPEG, JPG, PJP, PJPEG, PNG, BMP, ICO, GIF, TIFF, WEBP, XBM and other bitmap formats!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image" sourceImage="/svg/images/vectorization/fish.png" colors="3" scale="1" grayscale="true" stencil="monocolor" extent="1" stencilColor="#00ff00">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Convert PNG to SVG in C#
---

Aspose.SVG for the .NET API provides classes and methods that allow you to implement the image vectorization process and work with stenciling options.

{{<section "code" i18n-exclude>}}

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
            ColorsLimit = 10,
            LineWidth = 1,
            Stencil = new StencilConfiguration { Type = StencilType.MonoColor, Color = Aspose.Svg.Drawing.Color.FromRgb(0,0,255) }
        }
    };
    // Vectorize PNG from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.png");
    // Save vectorized PNG as SVG file 
	document.Save(OutputFolder + "image.svg");
```

{{<section steps>}}
---
h2: How to vectorize PNG in C#
title: Steps to Convert PNG to SVG in C#
---

To vectorize PNG image with Aspose.SVG, you should follow a few steps:

1. Initialize an instance of the [ImageVectorizer](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/) class. Use one of ImageVectorizer() constructors and specify configuration properties.
    - [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) property gets or sets the SVG path segments builder. 
    - [ColorsLimit](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/colorslimit/) property gets or sets the maximum number of colors used to quantize an image.
    - [Stencil](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/stencil/) property gets or sets stencil effect configuration. By default, no stencil effect is applied.
1. Vectorize an image from the specified file. The [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) method takes the path to the image file and returns an SVGDocument.
1. Save the vectorized PNG to SVG. Use the [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) method and pass to it the output path.

{{<section documentation>}}

In the documentation chapter <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Vectorization - Basic Overview</a>, you will find image vectorization info, a description of the image vectorization process and vectorization options, learn how to vectorize raster images such as PNG, JPG, BMP, TIFF, GIF, ICO into an SVG document. You will consider a few C# examples that demonstrate the [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) functionalities and the effect of configuration properties on the vectorization result.

{{<section other-vectorizers>}}
---
title: Other Supported Vectorizers
---