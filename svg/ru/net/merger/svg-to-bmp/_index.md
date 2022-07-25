---
translation: true
template: ./../_template-child.md
title: Объединение SVG в BMP на C# - Aspose.SVG
description: Объедините SVG в BMP с помощью C# API в Windows, macOS и Linux
url: /net/merger/svg-to-bmp/
family: svg
platformtag: net
feature: merge
informat: SVG
outformat: BMP
otherformats: XPS PDF GIF JPEG PNG TIFF BMP
---

{{<section banner>}}
---
h1: Объединить SVG в BMP на C#
h2: Высокоскоростной .NET API для объединения файлов SVG в Windows, macOS и Linux.
---

{{<section overview>}}
---
h2: Объединение SVG в BMP с помощью C#
---

SVG — один из наиболее часто используемых форматов для создания веб-сайтов и печати графики для обеспечения масштабируемости. Но иногда вам нужно объединить файлы SVG и сохранить их как один документ в другом формате файла. Файлы BMP представляют собой файлы растровых изображений, которые используются для хранения высококачественных растровых цифровых изображений. Формат BMP может хранить данные в виде двумерных цифровых изображений как в монохромном, так и в цветном формате с различной глубиной цвета. С помощью API [Aspose.SVG для .NET](https://products.aspose.com/svg/net/) вы можете программно объединять SVG в BMP. Мощный C# API поможет вам быстро и качественно объединить файлы SVG!

{{<section code-text>}}
---
h2: Пример кода C# для объединения SVG в BMP
title: Объединить SVG в BMP — C#
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
    using var device = new Aspose.Svg.Rendering.Image.ImageDevice("result.bmp");
    // Merge SVG to BMP
    renderer.Render(device, document1, document2, document3);                
}
```

{{<section steps>}}
---
h2: Шаги по слиянию SVG в BMP с помощью C#
---
1. Загрузите документы SVG с помощью одного из конструкторов [SVGDocument()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/).
1. Создайте новый экземпляр класса [SvgRenderer](https://reference.aspose.com/svg/net/aspose.svg.rendering/svgrenderer/).
1. Используйте конструктор [ImageDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/imagedevice/#constructor_5) для инициализации нового экземпляра класса ImageDevice.
1. Вызовите метод [Render()](https://reference.aspose.com/svg/net/aspose.svg.rendering/renderer-1/), чтобы объединить файлы SVG в BMP.
1. Несколько файлов SVG будут сохранены в виде изображения BMP по указанному пути.



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