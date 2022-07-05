---
translation: true
template: ./../_template-child.md
title: Преобразование HSL в HEX в C#
description: Работа с цветовыми кодами и преобразование HSL в HEX в C#
url: /net/color-converter/hsl-to-hex/
family: svg
platformtag: net
feature: color converter
informat: HSL
outformat: HEX
otherformats: RGB HWB CMYK LAB LCH XYZ OKLAB OKLCH NCOL
---

{{<section banner>}}
---
h1: Преобразование HSL в HEX через C#
h2: Используйте высокоскоростной .NET API для преобразования цветов HSL в HEX в Windows, macOS и Linux.
---

{{<section overview>}}
---
h2: Преобразование HSL в HEX с помощью C#
---

[Aspose.SVG для .NET API](https://products.aspose.com/svg/net/) предлагает высокоскоростную библиотеку C#, которую можно использовать для различных задач анализа SVG. Одной из особенностей API является легкий доступ к работе с несколькими цветовыми пространствами. Пространство имен Aspose.Svg.Converters реализует простой доступ к классу [ColorConverter](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/), который анализирует цвета (RGB, HEX, HSL, HWB). , CMYK, NCOL, LCH, OKLCH, LAB, OKLAB) из строки и возвращает интерфейс IConvertibleColor для преобразования в различные цветовые пространства.<br><br>
Цветовые коды или цветовые форматы тесно связаны с методами описания и определения цветов и широко используются в вебе, дизайне, полиграфии, фотографии, искусстве и т. д. И для разных задач предпочтительны разные цветовые форматы. Поэтому иногда вам может понадобиться преобразовать цветовые коды.

{{<section input-color>}}
---
title: Что такое цвет HSL?
---

{{<section output-color>}}
---
title: Что такое шестнадцатеричный цвет?
---

{{<section code-text>}}
---
h2: Пример кода C# для преобразования HSL в HEX
title: Преобразование HSL в HEX — C#
---

Высокоскоростная библиотека C# позволяет разработчикам .NET быстро и эффективно преобразовывать цвета HSL в HEX. Преобразование цвета можно выполнить с помощью нескольких строк кода:

{{<section "code-snippet" i18n-exclude>}}

```cs

// Parse HSL color from a string
var color = ColorConverter.ConvertFrom("hsl(31.034, 57%, 70%)");
// Convert HSL to HEX 
string hexColor = color.ToHexString();
// Print the result into console
Console.WriteLine(hexColor);
//result should be: #DEB486

```

{{<section steps>}}
---
h2: Действия по преобразованию HSL в HEX с помощью C#
---
1. Вызовите метод [ConvertFrom()](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/convertfrom/) класса ColorConverter и передайте код HSL в виде строки.
1. Метод ConvertFrom() анализирует цвет из строкового представления и возвращает интерфейс [IConvertibleColor](https://reference.aspose.com/svg/net/aspose.svg.drawing/iconvertiblecolor/) для преобразования его в требуемый цвет. пространства.
1. Метод IConvertibleColor.ToHexString() преобразует цвет HSL в HEX в формате: #000000.



{{<section documentation>}}

Ознакомьтесь с нашей документацией, чтобы узнать больше об использовании функций API Aspose.SVG и рассмотреть примеры C# для наиболее распространенных сценариев обработки SVG. В статье документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-change-svg-color/" target= "_blank">Как изменить цвет SVG</a>, вы можете посмотреть, как изменить цвет элементов и фона в изображениях SVG, используя библиотеку Aspose.SVG .NET. В статье <a href="https://docs.aspose.com/svg/net/drawing-basics/svg-color/" target="_blank">Цвет SVG</a> подробно рассматривается, как Текст и фигуры SVG можно раскрашивать.

{{<section online-color-converter>}}
---
h2: Онлайн-конвертер цвета
---

[Преобразователи цветов](https://products.aspose.app/svg/color-converter) — это бесплатные онлайн-приложения, которые позволяют преобразовывать цвета между различными цветовыми кодами, такими как RGB, HEX, HSL, HSV, HWB, LAB, CMYK. , LCH, XYZ, OKLAB, OKLCH, RGBA, HSLA и т.д. на лету. Преобразователи цветов просты в использовании и работают в любом браузере и операционной системе. Вы получаете результат сразу после ввода кода цвета, который нужно преобразовать.

{{<section get-started>}}
---
h2: Начало работы с .NET SVG API
---

Установите из командной строки как ```nuget install Aspose.SVG``` или через консоль диспетчера пакетов Visual Studio с ```Install-Package Aspose.SVG```.
Кроме того, вы можете получить автономный установщик MSI или библиотеки DLL в ZIP-файле из [загрузки](https://downloads.aspose.com/svg/net). Aspose.SVG API — это автономный API, который можно использовать для обработки и анализа документов SVG в приложениях.
Дополнительные сведения об установке библиотеки C# и системных требованиях см. в [Документации Aspose.SVG](https://docs.aspose.com/svg/net/getting-started/).

{{<section other-color-converters>}}
---
title: Другие поддерживаемые преобразователи цветов
---