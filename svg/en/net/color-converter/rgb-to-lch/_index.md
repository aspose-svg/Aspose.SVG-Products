---
translation: true
template: ./../_template-child.md
title: RGB to LCH Conversion in C#
description: Work with color codes and convert RGB to LCH in C#
url: /net/color-converter/rgb-to-lch/
family: svg
platformtag: net
feature: color converter
informat: RGB
outformat: LCH
otherformats: HEX HSV HSL HWB CMYK LAB XYZ OKLAB OKLCH NCOL
---

{{<section banner>}}
---
h1: Convert RGB to LCH via C#
h2: Use High-speed .NET API to Convert RGB to LCH color on Windows, macOS & Linux
---

{{<section overview>}}
---
h2: Convert RGB to LCH Using C#
---

[Aspose.SVG for .NET API](https://products.aspose.com/svg/net/) offers a high-speed C# library that you can use for different SVG parsing tasks. One of the API features is easy access to work with several color spaces. The Aspose.Svg.Converters namespace implements easy access to [ColorConverter](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/) class that parses colors (RGB, HEX, HSL, HWB, CMYK, NCOL, LCH, OKLCH, LAB, OKLAB) from a string and returns the IConvertibleColor interface for converting to various color spaces.<br><br>
Colors codes or color formats are closely linked to the methods of describing and defining colors and are widely used in the web, design, polygraphy, photography, arts, etc. And for different tasks, different color formats are preferred. So, sometimes you may need to convert color codes.

{{<section input-color>}}
---
title: What is RGB Color?
---

{{<section output-color>}}
---
title: What is LCH Color?
---

{{<section code-text>}}
---
h2: C# code example to convert RGB to LCH
title: Convert RGB to LCH - C#
---

The high-speed C# library allows .NET developers to quickly and efficiently convert RGB to LCH color. Color conversion can be done with a few lines of code:

{{<section "code-snippet" i18n-exclude>}}

```cs

// Parse RGB color from a string
var color = ColorConverter.ConvertFrom("rgb(222, 180, 135)");
// Convert RGB to LCH 
string lchColor = color.ToLchString();
// Print the result into console
Console.WriteLine(lchColor);
//result should be: lch(76.339%, 20.768%, 68.746%)

```

{{<section steps>}}
---
h2: Steps to convert RGB to LCH using C#
---

1. Call the [ConvertFrom()](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/convertfrom/) method of the ColorConverter class and pass the RGB code as a string. 
1. The ConvertFrom() method parses color from string representation and returns the [IConvertibleColor](https://reference.aspose.com/svg/net/aspose.svg.drawing/iconvertiblecolor/) interface to convert it to the required color spaces.
1. The IConvertibleColor.ToLchString() method converts RGB to LCH color in the format: lch(0%,0%,0%).

{{<section documentation>}}

Please visit our documentation to learn more about using Aspose.SVG API functions and consider C# examples for the most common SVG processing scenarios. In the documentation article <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-change-svg-color/" target="_blank">How to Change SVG Color</a>, you can view how to change the color of elements and background in SVG images using Aspose.SVG .NET library. The article <a href="https://docs.aspose.com/svg/net/drawing-basics/svg-color/" target="_blank">SVG Color</a> takes an in-depth look at how SVG text and shapes can be colorized.

{{<section online-color-converter>}}
---
h2: Online Color Converter
---

[Color Converters](https://products.aspose.app/svg/color-converter) are free online web applications that allow you to convert colors between different color codes like RGB, HEX, HSL, HSV, HWB, LAB, CMYK, LCH, XYZ, OKLAB, OKLCH, RGBA, HSLA, etc. on the fly. Color Converters are easy-to-use and work on any browser and operating system. You get the result immediately after entering the color code you need to convert.

{{<section get-started>}}
---
h2: Get Started with .NET SVG API
---

Install from command line as ```nuget install Aspose.SVG``` or via Package Manager Console of Visual Studio with ```Install-Package Aspose.SVG```.
Alternatively, get the offline MSI installer or DLLs in a ZIP file from [downloads](https://downloads.aspose.com/svg/net). Aspose.SVG API is a standalone API and can be used for SVG document manipulation and parsing within applications. 
For more details about C# library installation and system requirements, please refer to [Aspose.SVG Documentation](https://docs.aspose.com/svg/net/getting-started/).

{{<section other-color-converters>}}
---
title: Other Supported Color Converters
---