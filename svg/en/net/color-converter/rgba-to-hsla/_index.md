---
translation: true
template: ./../_template-child.md
title: Convert RGBA to HSLA - C# code and Online Converter
description: Work with color codes and convert RGBA to HSLA in C#. Try Online Color Converter for free!
url: /net/color-converter/rgba-to-hsla/
family: svg
platformtag: net
feature: color converter
informat: RGBA
outformat: HSLA
otherformats: HSVA HWBA NCOLA
---

{{<section banner>}}
---
h1: Convert RGBA to HSLA via C#
h2: Use High-speed .NET API to Convert RGBA to HSLA color on Windows, macOS & Linux
---

{{<section overview>}}
---
h2: Convert RGBA to HSLA Using C#
---

[Aspose.SVG for .NET API](https://products.aspose.com/svg/net/) offers a high-speed C# library that you can use for different SVG parsing tasks. One of the API features is easy access to work with several color spaces. The Aspose.Svg.Converters namespace implements easy access to [ColorConverter](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/) class that parses colors (RGB, HEX, HSL, HWB, CMYK, NCOL, LCH, OKLCH, LAB, OKLAB) from a string and returns the IConvertibleColor interface for converting to various color spaces.<br>
Colors codes or color formats are closely linked to the methods of describing and defining colors and are widely used in the web, design, polygraphy, photography, arts, etc. And for different tasks, different color formats are preferred. So, sometimes you may need to convert color codes.

{{<section input-color>}}
---
title: What is RGBA Color?
---

{{<section output-color>}}
---
title: What is HSLA Color?
---

{{<section code-text>}}
---
h2: Online Color Converter
title: Convert RGBA to HSLA - C#
---
If you need to convert colors from one color model to another, use our free online tool! It supports various color spaces, including HEX, RGB, CMYK, HSL, LAB, NCOL, XYZ, etc. You simply need to enter the color value for conversion! Click inside the color area to select a color, or enter a color code in the Input text box. You will immediately see other color codes for chosen color in the Output section.

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/color id=1 input="RGB" output="HSL">}}
// Parse RGBA color from a string
var color = ColorConverter.ConvertFrom("rgba(222, 180, 135, 0.5)");

// Convert RGBA to HSLA 
string hslaColor = color.ToHslaString();

// Print the result into console
Console.WriteLine(hslaColor);
//result should be: hsla(31.034, 57%, 70%, 0.5)
{{< /app/svg/color>}}


{{<section steps>}}
---
h2: How to convert RGBA to HSLA using C#
---

If you want to use the conversion functions in your product or programmatically convert RGBA to HSLA, see the C# code example above. Color conversion can be done with a few lines of code:

1. Call the [ConvertFrom()](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/convertfrom/) method of the ColorConverter class and pass the RGBA code as a string. 
2. The ConvertFrom() method parses color from string representation and returns the [IConvertibleColor](https://reference.aspose.com/svg/net/aspose.svg.drawing/iconvertiblecolor/) interface to convert it to the required color spaces.
3. The IConvertibleColor.ToHslaString() method converts RGBA to HSLA color in the format: hsla(0,0%,0%,0).

{{<section documentation>}}

Please visit our documentation to learn more about using Aspose.SVG API functions and consider C# examples for the most common SVG processing scenarios. In the documentation article <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-change-svg-color/" target="_blank">How to Change SVG Color</a>, you can view how to change the color of elements and background in SVG images using Aspose.SVG .NET library. The article <a href="https://docs.aspose.com/svg/net/drawing-basics/svg-color/" target="_blank">SVG Color</a> takes an in-depth look at how SVG text and shapes can be colorized.

{{<section online-color-converter>}}

[Color Converters](https://products.aspose.app/svg/color-converter) are free online web applications that allow you to convert colors between different color codes like RGB, HEX, HSL, HSV, HWB, LAB, CMYK, LCH, XYZ, OKLAB, OKLCH, RGBA, HSLA, etc. on the fly. Color Converters are easy-to-use and work on any browser and operating system. You get the result immediately after entering the color code you need to convert.

{{<section get-started>}}
---
h2: Get Started with .NET SVG API
---

Install from command line as ```nuget install Aspose.SVG``` or via Package Manager Console of Visual Studio with ```Install-Package Aspose.SVG```.
Alternatively, get the offline MSI installer or DLLs in a ZIP file from [downloads](https://releases.aspose.com/svg/net/). Aspose.SVG API is a standalone API and can be used for SVG document manipulation and parsing within applications. 
For more details about C# library installation and system requirements, please refer to [Aspose.SVG Documentation.](https://docs.aspose.com/svg/net/getting-started/)

{{<section other-color-converters>}}
---
title: Other Supported Color Converters
---