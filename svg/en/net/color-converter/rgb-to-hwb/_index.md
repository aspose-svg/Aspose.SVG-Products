---
translation: true
template: /templates/_template-color-child.md
title: Convert RGB to HWB - C# code and Online Converter
description: Work with color codes and convert RGB to HWB in C#. Try Online Color Converter for free!
url: /net/color-converter/rgb-to-hwb/
family: svg
platformtag: net
feature: color converter
informat: RGB
outformat: HWB
otherformats: HEX HSV HSL LAB CMYK LCH XYZ OKLAB OKLCH NCOL
---

{{<section banner>}}
---
h1: Convert RGB to HWB via C#
h2: Use High-speed .NET API to Convert RGB to HWB color on Windows, macOS & Linux
---

{{<section overview>}}
---
h2: Convert RGB to HWB Using C#
---

[Aspose.SVG for .NET API](https://products.aspose.com/svg/net/) offers a high-speed C# library that you can use for different SVG parsing tasks. One of the API features is easy access to work with several color spaces. The Aspose.Svg.Converters namespace implements the [ColorConverter](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/) class that parses colors (RGB, HEX, HSL, HWB, CMYK, NCOL, LCH, OKLCH, LAB, OKLAB) from a string and returns the IConvertibleColor interface for converting to various color spaces.<br>
Colors codes or color formats are closely linked to the methods of describing and defining colors and are widely used in the web, design, polygraphy, photography, arts, etc. And for different tasks, different color formats are preferred. So, sometimes you may need to convert color codes.

{{<section input-color>}}
---
title: What is RGB Color?
---

{{<section output-color>}}
---
title: What is HWB Color?
---

{{<section code-text>}}
---
h2: Online Color Converter
title: Convert RGB to HWB - C#
---
If you need to convert colors from one color model to another, use our free online tool! It supports various color spaces, including HEX, RGB, CMYK, etc. You simply need to enter the color value for conversion! Click inside the color area to select a color, or enter a color code in the Input text box. You will immediately see other color codes for chosen color in the Output section.

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/color id=1 input="RGB" output="HWB">}}
// Parse RGB color from a string
var color = Color.FromRgb(222, 180, 135);

// Convert RGB to HWB 
string hwbColor =  color.Convert(ColorModel.Hwb).ToString(false, false, 3);

// Print the result into console
Console.WriteLine(hwbColor);
//result should be: hwb(31.034, 53%, 13%)
{{< /app/svg/color>}}

{{<section steps>}}
---
h2: How to convert RGB to HWB using C#
---

If you want to use the conversion functions in your product or programmatically convert RGB to HWB, see the C# code example above. Color conversion can be done with a few lines of code:

1. Call the [ConvertFrom()](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/convertfrom/) method of the ColorConverter class and pass the RGB code as a string. 
2. The ConvertFrom() method parses color from string representation and returns the [IConvertibleColor](https://reference.aspose.com/svg/net/aspose.svg.drawing/iconvertiblecolor/) interface to convert it to the required color spaces.
3. The IConvertibleColor.ToHwbString() method converts RGB to HWB color in the format: hwb(0,0%,0%).

{{<section documentation>}}

Please visit our documentation to learn more about using Aspose.SVG API functions and consider C# examples for the most common SVG processing scenarios. In the documentation article <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-change-svg-color/" target="_blank">How to Change SVG Color</a>, you can view how to change the color of elements and background in SVG images using Aspose.SVG .NET library. The article <a href="https://docs.aspose.com/svg/net/drawing-basics/svg-color/" target="_blank">SVG Color</a> takes an in-depth look at how SVG text and shapes can be colorized.

{{<section online-color-converter>}}

[Color Converters](https://products.aspose.app/svg/color-converter) are free online web applications that allow you to convert colors between different color codes like RGB, HEX, HSL, HSV, HWB, LAB, CMYK, LCH, XYZ, OKLAB, OKLCH, RGBA, HSLA, etc. on the fly. Color Converters are easy-to-use and work on any browser and operating system. You get the result immediately after entering the color code you need to convert.

{{<section other-color-converters>}}
---
title: Other Supported Color Converters
---