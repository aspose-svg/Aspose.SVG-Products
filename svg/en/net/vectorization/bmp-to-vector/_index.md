---
translation: true
template: /templates/_template-vectorization-child.md
title: Vectorize BMP - C# code and Online Vectorizer 
description: BMP to vector in C#. Convert BMP to SVG and get all advantages of vector graphics. Try Online Image Vectorizer for free!
url: /net/vectorization/bmp-to-svg/
family: svg
platformtag: net
feature: vectorization
informat: BMP
outformat: SVG
---

{{<section banner>}}
---
h1: BMP to Vector - C# code and Online Vectorizer
h2: Convert BMP to SVG vector format online or programmatically.
---

{{<section overview>}}
---
h2: Vectorize Bitmap
---

Under vectorization, we mean the process of replacing bitmaps with mathematic curves, and geometric shapes made up of path elements and saved as SVG. You may want to vectorize bitmaps for a number of reasons. Vector graphics have a set of advantages: scaling, small file size, animation support, etc, or you just want to experiment with images and get some fun vectorizing effects. In any case, bitmap vectorization is a good experience if you are interested in photography, painting, design, arts, and web development.<br>
[Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) offers a high-speed C# library that you can use for different SVG parsing tasks. The [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) Namespace includes classes and interfaces for implementing the image vectorization process. In this article, we'll look at how to convert BMP to vector graphics in C# using the Aspose.SVG API. What's more, we provide an online Image Vectorizer for you to try real-time image to vector conversion.

{{<section input-file>}}
---
title: What is BMP File Format?
---

{{<section output-file>}}
---
title: What is SVG File Format?
---

{{<section plagin-text>}}
---
h2: Online Image Vectorizer
---

If you need to vectorize images, use our free online tool! Image Vectorizer supports JPG, PNG, BMP, ICO, GIF, and TIFF formats. It offers various options for preprocessing bitmaps before saving them to SVG format. Convert your images into scalable and clear vector art just now!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="JPG">}}

{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Convert BMP to SVG in C#
h2: How to use Image Vectorizer?
---

1. First, load the raster image from a local file system in PNG, JPG, GIF, BMP, TIFF, or ICO format. You will see three windows - Source, Quantized and Vectorized - with the preview of initial, color-quantized and vectorized images.
1. Image Vectorizer converts BMP to vector with default settings and you can download vectorized BMP as an SVG file. But for getting a better result, you can handle the quantization and vectorization processes with two settings sidebars. Click "Quantize" button to apply quantization settings, click "Vectorize" button to apply vectorization settings and convert BMP to SVG.
1. Click the "Download Result" button to get the resultant. 

 Image Vectorizer converts raster bitmap images into vector artwork constructed from outlines. The vectorization algorithm includes the next steps: color quantization, contour tracing, trace smoothing, trace simplification, and building SVG path elements from the traces. Apply custom settings to get the best BMP vectorization result.

<b>Quantization sidebar</b>
 - Color quantization is a process of selecting the limited number of colors to use in an image. It is applied when the color information of an image is to be reduced. Color quantization is a very complex process involving a number of factors. This can be implemented using different algorithms. Each of the algorithms determines which colors from the larger set of colors remain in the new image and how the discarded colors are mapped to the remaining ones.
 - <b>colors</b> - desired palette size;
 - <b>method</b> - histogram methods that implement various color quantization algorithms;
 - <b>minHueCols</b> - is a parameter that works with color gradients;
 - <b>scale</b> - or scaling factor is adjusted for a finer or coarser sampling of the colors in the plane.


<b>Vectorization sidebar</b>
- <b>tolerance</b> -  is responsible for reducing the number of points in a curve that is approximated by a series of trace points and determines the maximum error tolerance allowed for a point to be eliminated from the trace. The default value is 0.3;
- <b>tension</b> -  is responsible for building path segments from the list of trace points. The tension value determines how sharply the curve bends at the control points;
- <b>severity</b> - affects contours' smoothing and determines the extent of the region considered by query point the Nearest Neighbor approach.

Vector graphics are the best for creating logos, icons, page layouts, maps, graphs, line arts, illustrations, technical drawings and more. It is not the most suitable format for continuous-tone images with blends of color or editing photographs. However, vectorizing photos can result in impressive artistic effects that can be interesting and useful.

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
    // Vectorize BMP from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.bmp");
    // Save vectorized BMP image as SVG file 
	document.Save(OutputFolder + "image.svg"));
```

{{<section steps>}}
---
h2: How to vectorize BMP in C#
title: Steps to Convert BMP to SVG in C#
text: "Aspose.SVG for the .NET API provides classes and methods that allow you to implement the image vectorization process and work with various pre-processing options for images before saving them in vector format. Processing involves controlling the following vectorization options: TraceSimplifier, TraceSmoother, PathBuilder, etc."
---

To vectorize BMP with Aspose.SVG, you should follow a few steps:

1. Initialize an instance of the [ImageVectorizer](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/) class. Use one of ImageVectorizer() constructors and specify configuration properties.
    - [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) property sets the trace smoother. It is used to smooth out fragments of contours. 
    - [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) property sets the trace simplified. As a result, the trace curve will be built composed of line segments with fewer (or bigger) points.
    - [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) property sets the SVG path segments builder and affects how sharply the curve bends at the control points.
1. Vectorize BMP from the specified file. Use the [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) method that returnes an SVGDocument.
1. Save the vectorized BMP image as an SVG file.

{{<section documentation>}}
---
h2: Basics of Vectorization in Documentation 
---

 In the documentation chapter <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Vectorization - Basic Overview</a>, you will find image vectorization info, a description of the image vectorization process and vectorization options, learn how to vectorize raster images such as PNG, JPG, BMP, TIFF, GIF, ICO into an SVG document. You will consider a few C# examples that demonstrate the [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) functionalities and the effect of configuration properties on the vectorization result.

{{<section online-vectorizer>}}

Aspose.SVG offers a Free Online [Image Vectorizer](https://products.aspose.app/svg/image-vectorization) allows you to convert JPG, PNG, BMP, TIFF, ICO, and GIF bitmap images to vector graphics. Using this App, you may apply a set of options for obtaining the perfect result. Save your time and check this Image Vectorizer to get all the benefits of vector graphics!

{{<section other-vectorizers>}}
---
title: Other Supported Vectorizers
---