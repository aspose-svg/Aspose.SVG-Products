---
translation: true
template: /templates/_template-vectorization-child.md
title: Convert Image to SVG - C# code and Online Vectorizer 
description: Image to vector in C#. Convert Image to SVG and get all advantages of vector graphics. Try Online Image Vectorizer for free!
url: /net/vectorization/image-to-svg/
family: svg
platformtag: net
feature: vectorization
informat: Image
outformat: SVG
---

{{<section banner>}}
---
h1: Vectorize Images - C# code and Online Vectorizer
h2: Convert Image to SVG format online or programmatically.
---

{{<section overview>}}
---
h2: Image Vectorization
---

Image vectorization is the process of converting bitmap images into vector graphics - Bezier curves, splines, and lines. Vectorization is helpful because the image will not pixelate when you enlarge it. Scaling without losing quality, small file size, and animation support - are only a few advantages of vectorized images. Whether you are into painting, design, art, printing, architecture or web development, vector images are an essential part of the profession. On the other hand, you just can experiment with images and get some fun vectorizing effects. [Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) offers a high-speed C# library that you can use for different SVG parsing tasks. The [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) Namespace includes classes and interfaces for implementing the image vectorization process. In this article, we'll look at how to convert Image to vector graphics in C# or using an online Image Vectorizer.

{{<section input-file>}}
---
title: What is Image File Format?
---

{{<section output-file>}}
---
title: What is SVG File Format?
---

{{<section plagin-text>}}
---
h2: Online Image Vectorizer
---

If you need to vectorize images, use our free online tool! Image Vectorizer supports JPEG, JPG, PJP, PJPEG, PNG, BMP, ICO, GIF, TIFF, WEBP, XBM and other bitmap formats. It offers various options for preprocessing bitmaps before saving them to SVG format. You are able to interactively manage the vectorized SVG file by using controls linked with proper vectorization options. Convert your images into scalable and clear vector art just now!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Convert Image to SVG in C#
---

Aspose.SVG for the .NET API provides classes and methods that allow you to implement the image vectorization process and work with various pre-processing options for images before saving them in vector format. Processing involves controlling the following vectorization options: TraceSimplifier, TraceSmoother, PathBuilder, etc.

{{<section "code" i18n-exclude>}}

```cs       
	// Initialize an instance of the ImageVectorizer class
    var vectorizer = new ImageVectorizer
    {
        Configuration = 
		{
			// Set severity
			TraceSmoother =   new ImageTraceSmoother(3),
			// Set tolerance
			TraceSimplifier = new ImageTraceSimplifier(0.3f),
			// Set tension
        	PathBuilder = new PathBuilder(0.5f),
		}
    };
    // Vectorize image from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.png");
    // Save vectorized Image as SVG file 
	document.Save(OutputFolder + "image.svg");
```

{{<section steps>}}
---
h2: How to vectorize Image in C#
title: Steps to Convert Image to SVG in C#
---

To vectorize Image with Aspose.SVG, you should follow a few steps:

1. Initialize an instance of the [ImageVectorizer](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/) class. Use one of ImageVectorizer() constructors and specify configuration properties.
    - [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) property sets the trace smoother. It is used to smooth out fragments of contours. 
    - [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) property sets the trace simplified. As a result, the trace curve will be built composed of line segments with fewer (or bigger) points.
    - [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) property sets the SVG path segments builder and affects how sharply the curve bends at the control points.
1. Vectorize Image from the specified file. The [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) method takes the path to the image file and returns an SVGDocument.
1. Save the vectorized Image as an SVG file. Use the [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) method and pass to it the output path.

{{<section documentation>}}

In the documentation chapter <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Vectorization - Basic Overview</a>, you will find image vectorization info, a description of the image vectorization process and vectorization options, learn how to vectorize raster images such as PNG, JPG, BMP, TIFF, GIF, ICO into an SVG document. You will consider a few C# examples that demonstrate the [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) functionalities and the effect of configuration properties on the vectorization result.<br>
Aspose.SVG offers a Free Online [Image Vectorizer](https://products.aspose.app/svg/image-vectorization) allows you to convert JPG, PNG, BMP, TIFF, ICO, and GIF bitmap images to vector graphics. Using this App, you may apply a set of options for obtaining the perfect result. Save your time and check this Image Vectorizer to get all the benefits of vector graphics!

{{<section other-vectorizers>}}
---
title: Other Supported Vectorizers
---