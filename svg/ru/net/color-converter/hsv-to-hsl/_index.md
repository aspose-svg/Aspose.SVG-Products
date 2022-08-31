---
translation: true
template: /templates/_template-color-child.md
title: Конвертировать HSV в HSL - C# код, Онлайн Конвертер
description: Работа с цветовыми кодами и преобразование HSV в HSL в C#
url: /net/color-converter/hsv-to-hsl/
family: svg
platformtag: net
feature: color converter
informat: HSV
outformat: HSL
otherformats: RGB HEX HWB CMYK LAB LCH XYZ OKLAB OKLCH NCOL
---

{{<section banner>}}
---
h1: Конвертировать HSV в HSL на C#
h2: Используйте высокоскоростной API .NET для преобразования цветов HSV в HSL в Windows, macOS и Linux.
---

{{<section overview>}}
---
h2: Преобразование HSV в HSL с помощью C#
---

[Aspose.SVG для .NET API](https://products.aspose.com/svg/net/) предлагает высокоскоростную библиотеку C#, которую можно использовать для различных задач анализа SVG. Одной из особенностей API является легкий доступ к работе с несколькими цветовыми пространствами. Пространство имен Aspose.Svg.Converters реализует простой доступ к классу [ColorConverter,](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/) который анализирует цвета (RGB, HEX, HSL, HWB, CMYK, NCOL, LCH, OKLCH, LAB, OKLAB) из строки и возвращает интерфейс IConvertibleColor для преобразования в различные цветовые пространства.<br>
Цветовые коды или цветовые форматы тесно связаны с методами описания и определения цветов и широко используются в вебе, дизайне, полиграфии, фотографии, искусстве и т. д. И для разных задач предпочтительны разные цветовые форматы. Поэтому иногда вам может понадобиться преобразовать цветовые коды.

{{<section input-color>}}
---
title: Что такое цвет HSV?
---

{{<section output-color>}}
---
title: Что такое цвет HSL?
---

{{<section code-text>}}
---
h2: Онлайн Конвертер Цветов
title: Преобразование HSV в HSL — C#
---

Если вам нужно преобразовать цвета из одной цветовой модели в другую, воспользуйтесь нашим бесплатным онлайн Конвертером! Он поддерживает различные цветовые пространства, включая HEX, RGB, CMYK, HSL, LAB, XYZ и т. д. Вам просто нужно ввести значение цвета для преобразования! Щелкните внутри области цвета, чтобы выбрать нужный вам цвет, или введите цветовой код в текстовом поле ввода. Вы сразу же увидите другие цветовые коды для выбранного цвета в разделе «Output».

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/color id=1 input="HSV" output="HSL">}}
// Parse HSV color from a string
var color = ColorConverter.ConvertFrom("hsv(223.0,82%,85%)");

// Convert HSV to HSL 
string hslColor = color.ToHslString();

// Print the result into console
Console.WriteLine(hslColor);
//result should be: hsl(223,69.91%,50.15%)

{{< /app/svg/color>}}

{{<section steps>}}
---
h2: Действия по преобразованию HSV в HSL с помощью C#
---

Если вы хотите использовать функции преобразования в своем продукте или программно конвертировать цветовые коды, пожалуйста, рассмотрите приведенный выше  C# пример. Конвертацию между цветовыми кодами можно выполнить с помощью нескольких строк кода:

1. Вызовите метод [ConvertFrom()](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/convertfrom/) класса ColorConverter и передайте шестнадцатеричный код в виде строки.
1. Метод ConvertFrom() анализирует цвет из строкового представления и возвращает интерфейс [IConvertibleColor](https://reference.aspose.com/svg/net/aspose.svg.drawing/iconvertiblecolor/) для преобразования его в требуемый цвет.
1. Метод IConvertibleColor.ToHslString() преобразует цвет HSV в цвет HSL в формате: hsl(0,0%,0%).

{{<section documentation>}}

Ознакомьтесь с нашей документацией, чтобы узнать больше об использовании функций API Aspose.SVG и рассмотреть примеры C# для наиболее распространенных сценариев обработки SVG. В статье документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-change-svg-color/" target= "_blank">Как изменить цвет SVG</a>, вы можете посмотреть, как изменить цвет элементов и фона в изображениях SVG, используя библиотеку Aspose.SVG .NET. В статье <a href="https://docs.aspose.com/svg/net/drawing-basics/svg-color/" target="_blank">Цвет SVG</a> подробно рассматривается, как Текст и фигуры SVG можно раскрашивать.

{{<section online-color-converter>}}

[Конвертеры цветов](https://products.aspose.app/svg/color-converter) — это бесплатные онлайн-приложения, которые позволяют преобразовывать цвета между различными цветовыми кодами, такими как RGB, HEX, HSL, HSV, HWB, LAB, CMYK, LCH, XYZ, OKLAB, OKLCH, RGBA, HSLA и т.д. на лету. Конвертеры цветов просты в использовании и работают в любом браузере и операционной системе. Вы получаете результат сразу после ввода кода цвета, который нужно преобразовать.

{{<section get-started>}}
---
h2: Начало работы с .NET SVG API
---

Установите из командной строки ```nuget install Aspose.SVG``` или через консоль диспетчера пакетов Visual Studio с ```Install-Package Aspose.SVG```.
Кроме того, вы можете получить автономный установщик MSI или библиотеки DLL в ZIP-файле из [загрузки.](https://releases.aspose.com/svg/net/) Aspose.SVG API — это автономный API, который можно использовать для обработки и анализа документов SVG в приложениях.
Дополнительные сведения об установке библиотеки C# и системных требованиях см. в [Документации Aspose.SVG.](https://docs.aspose.com/svg/net/getting-started/)

{{<section other-color-converters>}}
---
title: Другие поддерживаемые Конвертеры цветов
---