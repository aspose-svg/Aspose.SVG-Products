---
translation: true
template: /templates/_template-text-vectorization.md
title: Convert text to vector paths in C# - Aspose.SVG
description: Vectorize text in SVG files using C#. Convert text to vector graphics and save it as SVG.
url: /net/vectorization/text-to-vector/
family: svg
platformtag: net
feature: vectorization
informat: SVG
outformat: SVG
---

{{<section banner>}}
---
h1: Text to Vector in C#
h2: Vectorize text in SVG documents and save it as vector graphics 
---

{{<section overview>}}
---
h2: Convert Text to Vector Paths
---

Text vectorization is the process of converting text into a variety of vector paths and geometrical forms. You can use different fonts and then convert them into vector outlines creating your own vector fonts. Such a text become a vector drawing and cannot be edited in the text editor. But you can edit and customize the vector characters by manipulating of `<path>`, `<use>`, `<mask>`, `<g>` elements in SVG code. You can apply the “filter”, “mask”, “opacity”, and other effects to the vectorized SVG text customizing its features such as opacity, lighting effects, etc. In addition to this, you can transform borders, strokes, shadows, glows, and other SVG aspects that can help you to design text. You can play with all these SVG features to get the best results. The vectorized text, being vector graphics, allows fonts usage without installation on the client computer and retains its style when used in any computer environment. Thus, converting text to vector forms is very helpful for use in logos, icons, banners, advertisements, etc.

[Aspose.SVG for .NET](https://products.aspose.com/svg/{{lang.url-fragment}}net/) API provides the feature of text vectorization in SVG documents. Check out our C# library so you can convert SVG text to vector graphics with ease!

{{<section code-text>}}
---
h2: C# code example to vectorize text in an SVG document
title: Convert text to vector - C#
---

In the vectorized SVG text, all font glyphs are replaced to a combination of graphics elements. Aspose.SVG for .NET API provides the feature of vectorizing text elements in SVG documents. To vectorize text, set the [VectorizeText](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/vectorizetext/) property of the SVGSaveOptions class to `true`. Text vectorization can be done with a few lines of code:

{{<section "code-snippet" i18n-exclude>}}

```cs
// Load an SVG document from a file
var document = new SVGDocument(InputFolder + "text.svg");
// Create a Save Options object 
var saveOptions = new SVGSaveOptions
{
    VectorizeText = true
};    
// Save the SVG document with specified saveOptions
document.Save((OutputFolder + "text-vectorized.svg"), saveOptions);
```

{{<section steps>}}
---
h2: Steps to vectorize SVG text in C#
---

1.  Load an SVG document using one of the [SVGDocument()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/) constructors.
1.  Create a new instance of the [SVGSaveOptions](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/) class. Use the [SVGSaveOptions()](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/svgsaveoptions/) constructor and set the [VectorizeText](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/vectorizetext/) property as `true`. It points to replacing text elements with paths.
1.  Call the [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_8) method and pass to it the output path and save options object.

{{<section documentation>}}

In the documentation chapter <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Vectorization - Basic Overview</a>, you will find text vectorization info, learn how to vectorize text in SVG document and consider C# examples. In the documentation article <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/text-vectorization/" target="_blank">Text Vectorization & Text Security</a>, you will know about text vectorization advantages.

{{<section online-vectorizer>}}
---
h2: Online Text Vectorizer
---

Aspose.SVG offers a free online <a href="https://products.aspose.app/svg/text-to-vector" target="_blank">Text to Vector</a> App that converts text in SVG file into vector forms. Text to Vector works from any device, any platform. No registration, plugin or additional software installation is required for you. Convert your SVG text to vector and get all advantages of vector graphics!

{{<section other-vectorizers>}}
---
title: Other Supported Vectorizers
---