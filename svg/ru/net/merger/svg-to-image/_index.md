---
translation: true
template: /templates/_template-merger-child.md
title: Объединить нескольго SVG в файл расторового изображения с помощью C# - Aspose.SVG
description: Объединение нескольких SVG документов в формат файла растрового изображения с помощью C# в Windows, macOS и Linux
url: /net/merger/svg-to-image/
family: svg
platformtag: net
feature: merge
informat: SVG
outformat: GIF JPEG PNG TIFF BMP
otherformats: GIF JPEG PNG TIFF BMP PDF XPS
---

{{<section banner>}}
---
h1: Объединить SVG в файл растрового изображения на C#
h2: Высокоскоростной .NET API для объединения файлов SVG в Windows, macOS и Linux.
---

{{<section overview>}}
---
h2: Объединение SVG в формат файла растрового изображения с использованием C#
---

SVG — один из наиболее часто используемых форматов векторных изображений для создания веб-сайтов и печатной графики для обеспечения масштабируемости. Но иногда вам нужно объединить файлы SVG и сохранить их как одно растровое изображение. Растровое изображение представляет собой двумерную сетку пикселей; он может хранить данные в несжатом или сжатом формате. Изображения широко используются для передачи изображений по сети и отображения фотографий и графики на веб-страницах и в облачных хранилищах. С помощью API [Aspose.SVG для .NET](https://products.aspose.com/svg/net/) вы можете программно объединять несколько SVG файлов в одно растровое изображение. Мощный C# API поможет вам быстро и качественно объединить файлы SVG!

{{<section code-text>}}
---
h2: Пример кода C# для объединения SVG в PNG
title: Объединить SVG в PNG — C#
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
    // Create an instance of ImageDevice
    using var device = new Aspose.Svg.Rendering.Image.ImageDevice("result.png");
    // Merge SVG to PNG
    renderer.Render(device, document1, document2, document3);                
}
```

{{<section steps>}}
---
h2: Шаги по объединению нескольких SVG в изображение с помощью C#
---
1. Загрузите документы SVG с помощью одного из конструкторов [SVGDocument()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/).
1. Создайте новый экземпляр класса [SvgRenderer](https://reference.aspose.com/svg/net/aspose.svg.rendering/svgrenderer/).
1. Используйте конструктор [ImageDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/imagedevice/#constructor_5) для инициализации нового экземпляра класса ImageDevice.
1. Вызовите метод [Render()](https://reference.aspose.com/svg/net/aspose.svg.rendering/renderer-1/), чтобы объединить SVG в требуемый формат изображения.
1. Несколько файлов SVG будут сохранены в растровое изображение по указанному пути.



{{<section documentation>}}

Пространство имен [Aspose.Svg.Rendering](https://reference.aspose.com/svg/net/aspose.svg.rendering/) реализует простой доступ к методам Render(). Вы можете быстро выполнить слияние SVG и экспортировать результат объединения в популярные форматы, такие как PDF, XPS, JPEG, PNG, BMP, TIFF и GIF. Посетите <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">нашу документацию</a>, чтобы узнать подробнее об использовании функций API Aspose.SVG. В статье документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target= "_blank">Как объединить файлы SVG</a>, вы можете рассмотреть примеры C# того, как объединить файлы SVG.

{{<section online-merger>}}
---
h2: Объединение изображений онлайн
---

Aspose.SVG предлагает бесплатное онлайн-приложение <a href="https://products.aspose.app/svg/merger" target="_blank">Image Merger</a>, которое объединяет несколько изображений в один файл. Вы можете выбрать тип объединения изображений для различных исходных файлов, таких как SVG, JPG, PNG, BMP, ICO, GIF или TIFF, и сохранить результат в одном из следующих выходных форматов: JPG, PNG или SVG. Наше приложение многофункционально. Вы можете создавать коллажи изображений, редактировать и манипулировать изображениями перед объединением. Image Merger позволяет свободно добавлять изображения, вращать, масштабировать, добавлять фоны, фильтры и перемещать каждое изображение, пока вы не будете довольны конечным результатом своего дизайна.

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