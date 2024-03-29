﻿---
translation: true
deploy: false
---

{{<section RGB>}}

RGB（红、绿、蓝）颜色空间由所有可能的颜色组成，这些颜色可以通过混合红、绿和蓝获得。这种颜色模型在摄影、电视和计算机图形学中很流行。 RGB 值指定为 0 到 255 之间的整数。因此，例如，rgb(255,0,0) 显示为红色。红色参数设置为最高值 (255)，其余设置为 0。<br>
Aspose.SVG C# 库支持 RGB 百分比（从 0% 到 100%）。例如，rgb(100%,0,0) 显示为红色。


{{<section HEX>}}

十六进制代码是最常用的颜色代码。这是因为它们简单易懂。 HEX 代码只不过是 RGB 的十六进制表示。六位数的颜色编号分为三组，每组两位数指定加色中红色、绿色和蓝色的数量。每个两位数的十六进制对可以有一个从 00 到 FF 的值。这提供了超过 1600 万种可能的颜色。如果这三个组中的每一个都包含字符，例如#RRGGBB，那么它们可以写成#RGB。所有浏览器都支持十六进制颜色值。

{{<section HSL>}}

HSL（色相、饱和度、亮度）是 RGB 颜色模型在柱坐标中的表示。色调是色轮上的任何颜色；它是色轮上从 0 到 360 的度数。所以，0 是红色，120 是绿色，240 是蓝色。饱和度是颜色的强度或纯度。它决定了颜色的鲜艳程度。例如，0% 是灰色，100% 是完全饱和的颜色。亮度是颜色的亮度或光量。亮度决定了颜色有多少黑色或白色。例如，50% 没有色调，0% 是全黑，100% 是全白。

{{<section HSV>}}

HSV 代表 Hue、Saturation 和 Value（亮度值）。 HSV 与 HSL 类似，但它们是两种不同的颜色模型。它们都基于圆柱几何形状，但 HSV 是基于“六角锥”模型，而 HSL 是基于“双六角锥”模型。选择 HSV 颜色首先要选择一种可用的色调，然后调整阴影和亮度值。色调设置颜色在色轮上的位置（从 0 到 360）。饱和度是一个饱和度百分比值（从 0% 到 100%）。亮度是亮度百分比（从 0% 到 100%）。

{{<section LAB>}}

就像地理坐标——经度、纬度和高度——颜色值 LAB 为我们提供了一种检测颜色的方法。 LAB 使用三个轴：L - 亮度，a* - 从红色到绿色值，b* - 从蓝色到黄色值。亮度以百分比表示，可以超过 100%。 a 和 b 轴的值可以从正到负。它通常被限制在 -128 到 127 的范围内，用于整数代码值。如果您希望屏幕上的颜色与打印在纸上时的颜色相同，建议使用 LAB 颜色空间和 LAB 颜色代码。

{{<section LCH>}}

LCH 代表亮度、色度和色调。与 LAB 一样，亮度可以是超过 100% 的百分比。 LCH 颜色模型中的颜色分量松散地对应于 HSL。与 HSL 类似，色调可以是 0 到 360 之间的范围。但是，LCH 色调角度并不完全对应于相同 HSL 的色调值。色度表示颜色的量，我们可以把它想象成类似于 HSL 中的饱和度。但是色度可以超过 100 - 事实上，理论上它是无界的。 LCH 颜色空间作为 LAB 是感知均匀的，这意味着颜色空间中坐标的精确数值变化给出了颜色之间相同的感知差异。


{{<section HWB>}}

HWB 代表色相、白度和黑度。 HWB 与颜色模型 HSV（Hue、Saturation、Value）和 HSL（Hue、Saturation、Lightness）非常相似，只是 HSV 和 HSL 都不提供白色饱和度。与 HSL 和 HSV 一样，色调可以在 0 到 360 范围内的任何位置。另外两个参数控制有多少白色或黑色混合到该色调中，最高 100%（这将导致完全白色或黑色） . HWB 对于创建单色调色板特别有用。 HTML 尚不支持 HWB，但建议将其作为 CSS4 中的新标准。


{{<section XYZ>}}

XYZ 颜色模型 (CIE 1931 XYZ) 是基于人眼 CIE RGB 版本结果的纯数学空间。与 RGB、CMYK 和其他模型不同，在 XYZ 中，主要成分是假设的，这意味着您不能将 X、Y 和 Z 映射到要混合的任何颜色集。这些颜色不对应于任何真实的光波长。 XYZ 是一种颜色空间的加法方案，因为它定义了提供给眼睛的三种刺激（三种原色）的量。 XYZ 广泛应用于科学工作和技术领域。其他颜色空间中的颜色描述通常与它们在该空间中的表示有关。


{{<section RGBA>}}

RGBA（红色、绿色、蓝色和 Alpha）颜色值是 RGB 颜色值的扩展，带有决定颜色不透明度的 Alpha 通道。 alpha 参数是一个介于 0.0 和 1.0 之间的数字，用于指定透明度。例如，rgba(255, 0, 0) 显示为纯红色，rgba(255, 0, 0, 0.5) 显示为不透明度为 50% 的红色。对于 RGBA 值，与 RGB 值不同，它没有十六进制表示法。

{{<section HSLA>}}

与 RGB/RGBA 类似，HSL 具有 HSLA 模式，支持 alpha 通道来指定颜色不透明度。 HSLA (Hue, Saturation, Lightness, Alpha) 颜色值由色调、饱和度、亮度和 alpha 指定，其中 alpha 参数指定不透明度。 alpha 参数是介于 0.0（表示“完全透明”）和 1.0（表示“完全不透明”）之间的数字。例如，hsla(0, 100%, 50%, 1) 显示为纯红色，hsla(0, 100%, 50%, 0.5) 显示为不透明度为 50% 的红色。

{{<section CMYK>}}

CMYK 颜色是青色、品红色、黄色和黑色的组合。这种模型被称为减法，因为墨水从白色中减去颜色。 CMYK 是最流行的颜色模型之一。 CMYK 颜色模型用于纸张的印刷油墨。该模型包含多种颜色，但与 RGB 相比，颜色数量有限。 CMYK 在创建打印设计时被广泛使用，以确保所需的颜色是准确的，而不是用于样式表或 HTML。 HTML 不支持 CMYK，但建议将其作为 CSS4 中的新标准。