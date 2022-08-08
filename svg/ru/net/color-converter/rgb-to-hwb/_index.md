---
translation: true
template: /templates/_template-color-child.md
title: Конвертировать RGB в HWB - C#
description: Работа с цветовыми кодами и преобразование RGB в HWB в C#
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
h1: Конвертировать RGB в HWB с помощью C#
h2: Используйте высокоскоростной .NET API для преобразования цветов RGB в HWB в Windows, macOS и Linux.
---

{{<section overview>}}
---
h2: Преобразование RGB в HWB с помощью C#
---

[Aspose.SVG для .NET API](https://products.aspose.com/svg/net/) предлагает высокоскоростную библиотеку C#, которую можно использовать для различных задач анализа SVG. Одной из особенностей API является легкий доступ к работе с несколькими цветовыми пространствами. Пространство имен Aspose.Svg.Converters реализует простой доступ к классу [ColorConverter,](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/) который анализирует цвета (RGB, HEX, HSL, HWB, CMYK, NCOL, LCH, OKLCH, LAB, OKLAB) из строки и возвращает интерфейс IConvertibleColor для преобразования в различные цветовые пространства.<br>
Цветовые коды или цветовые форматы тесно связаны с методами описания и определения цветов и широко используются в вебе, дизайне, полиграфии, фотографии, искусстве и т. д. И для разных задач предпочтительны разные цветовые форматы. Поэтому иногда вам может понадобиться преобразовать цветовые коды.

{{<section input-color>}}
---
title: Что такое цвет RGB?
---

{{<section output-color>}}
---
title: Что такое цвет HWB?
---

{{<section code-text>}}
---
h2: Онлайн Конвертер Цветов
title: Преобразование RGB в HWB — C#
---

Если вам нужно преобразовать цвета из одной цветовой модели в другую, воспользуйтесь нашим бесплатным онлайн Конвертером! Он поддерживает различные цветовые пространства, включая HEX, RGB, CMYK, HSL, LAB, XYZ и т. д. Вам просто нужно ввести значение цвета для преобразования! Щелкните внутри области цвета, чтобы выбрать нужный вам цвет, или введите цветовой код в текстовом поле ввода. Вы сразу же увидите другие цветовые коды для выбранного цвета в разделе «Output».

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/color id=1 input="RGB" output="HWB">}}
// Parse RGB color from a string
var color = ColorConverter.ConvertFrom("rgb(222, 180, 135)");

// Convert RGB to HWB 
string hwbColor = color.ToHwbString();

// Print the result into console
Console.WriteLine(hwbColor);
//result should be: hwb(31.034, 53%, 13%)
{{< /app/svg/color>}}

{{<section steps>}}
---
h2: Действия по преобразованию RGB в HWB с помощью C#
---

Если вы хотите использовать функции преобразования в своем продукте или программно конвертировать цветовые коды, пожалуйста, рассмотрите приведенный выше  C# пример. Конвертацию между цветовыми кодами можно выполнить с помощью нескольких строк кода:

1. Вызовите метод [ConvertFrom()](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/convertfrom/) класса ColorConverter и передайте код RGB в виде строки.
1. Метод ConvertFrom() анализирует цвет из строкового представления и возвращает интерфейс [IConvertibleColor](https://reference.aspose.com/svg/net/aspose.svg.drawing/iconvertiblecolor/) для преобразования его в требуемый цвет.
1. Метод IConvertibleColor.ToHwbString() преобразует цвет RGB в цвет HWB в формате: hwb(0,0%,0%).

{{<section documentation>}}

Ознакомьтесь с нашей документацией, чтобы узнать больше об использовании функций API Aspose.SVG и рассмотреть примеры C# для наиболее распространенных сценариев обработки SVG. В статье документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-change-svg-color/" target= "_blank">Как изменить цвет SVG</a>, вы можете посмотреть, как изменить цвет элементов и фона в изображениях SVG, используя библиотеку Aspose.SVG .NET. В статье <a href="https://docs.aspose.com/svg/net/drawing-basics/svg-color/" target="_blank">Цвет SVG</a> подробно рассматривается, как Текст и фигуры SVG можно раскрашивать.

{{<section online-color-converter>}}
---
h2: Онлайн-конвертер цвета
---

[Конвертеры цветов](https://products.aspose.app/svg/color-converter) — это бесплатные онлайн-приложения, которые позволяют преобразовывать цвета между различными цветовыми кодами, такими как RGB, HEX, HSL, HSV, HWB, LAB, CMYK, LCH, XYZ, OKLAB, OKLCH, RGBA, HSLA и т.д. на лету. Конвертеры цветов просты в использовании и работают в любом браузере и операционной системе. Вы получаете результат сразу после ввода кода цвета, который нужно преобразовать.

{{<section get-started>}}
---
h2: Начало работы с .NET SVG API
---

Установите из командной строки ```nuget install Aspose.SVG``` или через консоль диспетчера пакетов Visual Studio ```Install-Package Aspose.SVG```.
Кроме того, вы можете получить автономный установщик MSI или библиотеки DLL в ZIP-файле из [загрузки.](https://releases.aspose.com/svg/net/) Aspose.SVG API — это автономный API, который можно использовать для обработки и анализа документов SVG в приложениях.
Дополнительные сведения об установке библиотеки C# и системных требованиях см. в [Документации Aspose.SVG.](https://docs.aspose.com/svg/net/getting-started/)

{{<section other-color-converters>}}
---
title: Другие поддерживаемые Конвертеры цветов
---