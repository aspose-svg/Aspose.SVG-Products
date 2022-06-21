---
translation: true
template: template.md
title: C# .NET SVG files Parsing API - Aspose 
weight: 20
url: /net/ 
description: C# .NET SVG library to load file, read and traverse the elements and convert SVG to PDF, XPS and Image formats
---

{{<section banner>}}
---
h1: .NET APIs to Parse SVG Files
h2: Create, load, parse, render and convert SVG files to popular formats without any software dependencies
---

{{<section overview>}}
---
item1: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/creating-loading-documents/" target="_blank">Create or load SVG documents</a> from a file, URL, string, stream, etc.
item2: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">Convert SVG</a> to PDF, PNG, and other popular formats.
item3: <a href="hhttps://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Vectorize raster images</a> such as PNG, JPG, BMP, TIFF, GIF, and ICO into an SVG document.
item4: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/navigation-inspection/" target="_blank">Navigate SVG documents</a> using XPath Query, CSS Selector, Element and Document Traversal features. 
item5: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-edit-svg-documents/" target="_blank">Edit SVG files</a> by inserting new nodes, removing, or editing the content of existing nodes.
item6: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target="_blank">Render SVG documents</a> with high quality. 
item7: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/text-vectorization/" target="_blank">Vectorize SVG text</a> in a short time and with professional quality and resolution, and more.
---

Aspose.SVG for .NET is a flexible library for SVG file processing and fully compatible with its specifications. API can easily load, save and convert SVG files as well as read and traverse the elements of files through its Document Object Model (DOM). API is independent of any other software and empowers developers to work with SVG files without going into the underlying details of the format.<br><br>
Using Aspose.SVG C# library in your project allows you to perform the following tasks:

{{<section glance>}}
---
h3: At a Glance
description: An overview of Aspose.SVG for .NET API.
---

{{<section platform>}}
---
h3: Platform Independence
description: Aspose.SVG for .NET supports all major platforms including.
---

{{<section formats>}}
---
h3: Supported File Formats
description: Aspose.SVG for .NET supports all popular image file formats and more.
---

{{<section feature>}}
---
title: Advanced .NET SVG Parsing API Features
feature1: Create and read SVG documents
feature2: Edit and Save SVG files
feature3: Convert SVG to popular formats
feature4: Full control over SVG nodes
feature5: Add and remove nodes
feature6: Change the node properties
feature7: Content navigation using XPath Query
feature8: Navigate via CSS Selectors, Element and Document Traversal
feature9: DOM Tree manipulation of official SVG specifications
---

{{<section convert>}}
---
h2: Convert SVG using C#
h3: Convert SVG to PNG - C#
----
   
Aspose.SVG for .NET can read and convert SVG to PDF, XPS and major image formats. The conversion process is simple and reliable, thus making SVG .NET API a perfect choice. You can use API in your C# or any other .NET application to develop converter applications without getting into the details of underlying file formats. Getting conversion functionality is simple and depends on each application requirement. Here are a few lines of code for conversion between formats.

{{<section "code" i18n-exclude>}}
     
using Aspose.Svg;
using System.IO;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;
...
    
    // Initialize an SVG document from a file
    using (var document = new SVGDocument("input.svg"))
    {
        // Create an instance of the ImageSaveOptions class
    	var pngSaveOptions = new ImageSaveOptions();    
    
        // Convert SVG to PNG
    	Converter.ConvertSVG(document, pngSaveOptions, "output.png");
    }

{{<section online-converters>}}

You can try online SVG Converter <a href="https://products.aspose.app/svg/conversion/svg" target="_blank">here.</a>

{{<section other-converters>}}

Other Supported SVG Conversions:

{{<section image-vector>}}
---
h2: Convert Raster Image to Vector Graphic
h3: Convert Image to Vector - C#
---

Converting an image to vector is very easy using Aspose.SVG API. The <a href="https://apireference.aspose.com/svg/net/aspose.svg.imagevectorization/"  target="_blank">ImageVectorization</a> Namespace includes classes and interfaces for implementing the image vectorization process. The following code snippet demonstrates the use of the ImageVectorizer class for image vectorization:

{{<section "code-image" i18n-exclude>}}
     
using Aspose.Svg.ImageVectorization;
using Aspose.Svg.Saving;
...
    
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
	
	// Vectorize raster image from the specified file
	using var document = vectorizer.Vectorize("input.png");
	
	// Save vectorized image as SVG file 
	document.Save("output.svg");

{{<section merge>}}
---
h2: Merge SVG in C#
h3: Merge SVG to PDF - C#
---	
	
The Renderer() method gives you the ability to send multiple documents at once to the output rendering device and merge them. Documents merging can be done with a few lines of code:

{{<section "code-merge" i18n-exclude>}}
     
using Aspose.Svg;
using Aspose.Svg.Rendering;
using Aspose.Svg.Rendering.Pdf;
...   
	
	// Initialize SVG documents from files to merge later
	using (var document1 = new SVGDocument("input1.svg"))
	using (var document2 = new SVGDocument("input2.svg"))
	using (var document3 = new SVGDocument("input3.svg"))
	{
		// Create an instance of SvgRenderer
		using (var renderer = new SvgRenderer())
		{
			// Create an instance of PdfDevice
			using (var device = new PdfDevice("output.pdf"))
			{
				// Merge all SVG documents to PDF
				renderer.Render(device, document1, document2, document3);
			}
		}
	}

{{<section other-mergers>}}	

Other Supported Mergers:  
