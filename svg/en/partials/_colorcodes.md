---
translation: true
deploy: false
---

{{<section RGB>}}

The RGB (Red, Green, Blue) color space consists of all possible colors that can be obtained by mixing red, green, and blue. This color model is popular in photography, TV and computer graphics. RGB values are specified as an integer between 0 and 255. So, for example, rgb(255,0,0) is displayed as red. The red parameter is set to its highest value (255), and the rest are set to 0.<br>
Aspose.SVG C# library supports RGB percentages (from 0% to 100%). For example, rgb(100%,0,0) is displayed as red.


{{<section HEX>}}

HEX codes are the most used color codes. This is because they are simple and easy to understand. HEX codes are nothing more than a hexadecimal representation of RGB. The six-digit color number is structured into three groups of two digits which specify the amount of Red, Green, and Blue in the additive color. Each two-digit hex pair can have a value from 00 to FF. This gives over 16 million possible colors. If each of the three groups contains characters, such as #RRGGBB, then they can be written as #RGB. Hexadecimal color values are supported in all browsers.

{{<section HSL>}}

HSL (Hue, Saturation, Lightness) is a representation of the RGB color model in cylindrical coordinates. Hue is any color on the color wheel; it’s a degree on the color wheel from 0 to 360. So, 0 is red, 120 is green, 240 is blue. Saturation is the intensity or purity of a color. It determines how vivid the color will be. For example, zero percent is gray, and 100 percent is a fully saturated color. Lightness is the amount of brightness or light in color. Lightness determines how much black or white tint the color has. For example, 50 percent has no tint, zero percent is entirely black, and 100 percent is fully white.

{{<section HSV>}}

HSV stands for Hue, Saturation and Value (brightness value). HSV  is similar to HSL, but they are two different color models. They are both based on cylindrical geometries, but HSV is based on the "hexcone" model, while HSL is based on the "bi-hexcone" model. Selecting an HSV color begins with picking one of the available hues and then adjusting the shade and brightness values. Hue sets the position of the color on the color wheel (from 0 to 360). Saturation is a saturation percentage value (from 0% to 100%). Brightness is a brightness percentage (from 0% to 100%).

{{<section LAB>}}

Like geographic coordinates - longitude, latitude and height - the color values LAB give us a way to detect colors. LAB uses three axes: L - Lightness, a* - from Red to Green Value, and b* - from Blue to Yellow Value. The Lightness is expressed as a percentage and can exceed 100%. Values for the a and b axes can range from positive to negative. It is commonly clamped to the range of −128 to 127 for use with integer code values. The LAB color space and LAB color codes are recommended to use if you want the color on-screen to look the same as when printed on paper.

{{<section LCH>}}

LCH stands for Lightness, Chroma, and Hue. As with LAB, the Lightness can be a percentage that exceeds 100%. The color components in the LCH color model loosely correspond to HSL's. Similar to HSL, hue can be a range between 0 and 360. However, the LCH Hue angles don't fully correspond to the same HSL's hue values. Chroma represents the amount of color, and we can think of it as similar to saturation in HSL. But chroma can exceed 100 - in fact, it's theoretically unbounded. LCH color space as LAB is perceptual uniform, meaning the exact numerical change of coordinates in the color space gives the same perceptual difference between colors.


{{<section HWB>}}

HWB stands for hue, whiteness and blackness. The HWB is very similar to the color models HSV (Hue, Saturation, Value) and HSL (Hue, Saturation, Lightness), except that neither HSV nor HSL provide white saturation. Like HSL and HSV, the hue can be anywhere within a range of 0 to 360. The other two arguments control how much white or black is mixed into that hue, up to 100% (which would result in a totally white or black color). HWB is especially useful for creating monochrome color palettes. HWB is not supported in HTML yet, but it is suggested as a new standard in CSS4.


{{<section XYZ>}}

The XYZ color model (CIE 1931 XYZ) is a purely mathematical space based on the results of the CIE RGB version of the human eye. Unlike RGB, CMYK, and other models, in XYZ the primary components are hypothetical, meaning you can't map X, Y, and Z to any set of colors to mix. These colors do not correspond to any real light wavelengths. XYZ is an additive scheme of color spaces since it defines the amounts of three stimuli provided to the eye (the three primaries). XYZ is widely used in scientific works and technical fields. Color descriptions in other color spaces are often related to their representation in this space.


{{<section RGBA>}}

RGBA (Red, Green, Blue, and Alpha) color values are an extension of RGB color values with an alpha channel that determines the opacity of the color. The alpha parameter is a number between 0.0 and 1.0 that specifies transparency. For example, rgba(255, 0, 0) is displayed as pure red, rgba(255, 0, 0, 0.5) is displayed as red with 50% opacity. For an RGBA value, unlike RGB values, there is no hexadecimal notation.

{{<section HSLA>}}

Similar to RGB/RGBA, HSL has an HSLA mode with support for an alpha channel to specify the color opacity. The HSLA (Hue, Saturation, Lightness, Alpha) color value is specified with hue, saturation, lightness, and alpha, where the alpha parameter specifies the opacity. The alpha parameter is a number between 0.0, meaning “fully transparent”, and 1.0, meaning “fully opaque”. For example, hsla(0, 100%, 50%, 1) is displayed as pure red, hsla(0, 100%, 50%, 0.5) is displayed as red with 50% opacity.

{{<section CMYK>}}

CMYK colors are a combination of Cyan, Magenta, Yellow, and blacK. This model is known as subtractive, as inks subtract the colors from white. CMYK is one of the most popular color models. The CMYK color model is used in printing inks for paper. This model includes many colors, but the number of colors is limited compared to RGB. CMYK is widely used while creating designs for printing to ensure that the desired colors are accurate and never for style sheets or HTML. CMYK is not supported in HTML, but it is suggested as a new standard in CSS4.