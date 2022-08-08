---
translation: true
template: /templates/_template-merger-child.md
title: Объединение нескольких SVG в XPS с помощью C# - Aspose.SVG
description: Объединение SVG в XPS с помощью C# в Windows, macOS и Linux
url: /net/merger/svg-to-xps/
family: svg
platformtag: net
feature: merge
informat: SVG
outformat: XPS
otherformats: XPS PDF GIF JPEG PNG TIFF BMP
---

{{<section banner>}}
---
h1: Объединить SVG в XPS на C#
h2: Высокоскоростной .NET API для объединения файлов SVG в Windows, macOS и Linux.
---

{{<section overview>}}
---
h2: Объединение SVG в XPS в C#
---

SVG — один из наиболее часто используемых форматов для создания веб-сайтов и печати графики для обеспечения масштабируемости. Но иногда вам нужно объединить файлы SVG и сохранить их как один документ в другом формате файла. Формат XPS имеет ряд преимуществ, включая поддержку функций безопасности и многое другое. С помощью API [Aspose.SVG для .NET](https://products.aspose.com/svg/net/) вы можете программно объединять SVG в XPS. Мощный C# API поможет вам быстро и качественно объединить файлы SVG!

{{<section code-text>}}
---
h2: Пример кода C# для объединения SVG в XPS
title: Объединение SVG в XPS — C#
---

Высокоскоростная библиотека C# позволяет разработчикам .NET быстро и эффективно объединять файлы SVG и преобразовывать объединенный результат в другие популярные форматы, такие как PDF, XPS, JPEG, PNG, BMP, GIF и TIFF. Слияние документов можно выполнить с помощью нескольких строк кода:

{{<section "code-snippet" i18n-exclude>}}

```cs
// Initialize SVG documents from files to merge 
using (var document1 = new SVGDocument("document1.svg"))
using (var document2 = new SVGDocument("document2.svg"))
using (var document3 = new SVGDocument("document3.svg"))
{
    // Create an instance of SvgRenderer
    using var renderer = new Aspose.Svg.Rendering.SvgRenderer();	
    // Create an instance of XpsDevice
    using var device = new Aspose.Svg.Rendering.Xps.XpsDevice("result.xps");
    // Merge SVG to XPS
    renderer.Render(device, document1, document2, document3);                
}
```

{{<section steps>}}
---
h2: Шаги по слиянию SVG в XPS с помощью C#
---
1. Загрузите документы SVG с помощью одного из конструкторов [SVGDocument()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/).
1. Создайте новый экземпляр класса [SvgRenderer](https://reference.aspose.com/svg/net/aspose.svg.rendering/svgrenderer/).
1. Используйте конструктор [XpsDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.xps/xpsdevice/xpsdevice/#constructor_5) для инициализации нового экземпляра класса XpsDevice.
1. Вызовите метод [Render()](https://reference.aspose.com/svg/net/aspose.svg.rendering/renderer-1/), чтобы объединить SVG в один файл XPS.
1. Несколько файлов SVG будут сохранены в один файл XPS по указанному пути.



{{<section documentation>}}

Пространство имен [Aspose.Svg.Rendering](https://reference.aspose.com/svg/net/aspose.svg.rendering/) реализует простой доступ к методам Render(). Вы можете быстро выполнить слияние SVG и экспортировать результат объединения в популярные форматы, такие как PDF, XPS, JPEG, PNG, BMP, TIFF и GIF. Посетите <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">нашу документацию</a>, чтобы узнать подробнее об использовании функций API Aspose.SVG. В статье документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target= "_blank">Как объединить файлы SVG</a>, вы можете рассмотреть примеры C# того, как объединить файлы SVG.

{{<section online-merger>}}
---
h2: Объединение SVG онлайн
---

Aspose.SVG предлагает бесплатное онлайн-приложение <a href="https://products.aspose.app/svg/merger/svg" target="_blank">Merge SVG</a>, которое объединяет несколько SVG в один файл. Вы можете выбрать тип слияния SVG для различных выходных файлов, таких как SVG, JPG или PNG. Наше приложение многофункционально. Вы можете создавать коллажи изображений, редактировать и манипулировать изображениями SVG перед объединением. SVG Merger позволяет свободно добавлять изображения, вращать, масштабировать, добавлять фоны, фильтры и перемещать каждое изображение до тех пор, пока вы не будете довольны конечным результатом своего дизайна.

{{<section get-started>}}
---
h2: Начало работы с .NET SVG API
---

Установите из командной строки как ```nuget install Aspose.SVG``` или через консоль диспетчера пакетов Visual Studio с ```Install-Package Aspose.SVG```.
Кроме того, вы можете получить автономный установщик MSI или библиотеки DLL в ZIP-файле из [загрузки](https://releases.aspose.com/svg/net/). Aspose.SVG для .NET API является автономной библиотекой и не зависит от какого-либо программного обеспечения для обработки документов SVG.
 Дополнительные сведения об установке библиотеки C# и системных требованиях см. в [документации Aspose.SVG](https://docs.aspose.com/svg/net/getting-started/).

{{<section other-mergers>}}
---
title: Другие поддерживаемые слияния
subTitle: "Вы можете объединить изображения и сохранить результат в другие форматы файлов:"
---