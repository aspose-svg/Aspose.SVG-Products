---
translation: true
template: _template.md
title: Объединение нескольких SVG файлов в один файл PDF, JPEG, PNG и т.д. на C#
url: /net/merger/
description: Объединяйте изображения или SVG в один файл и сохраняйте результат в PDF, XPS, PNG, JPEG, BMP, GIF, TIFF с помощью C#.
---

{{<section banner>}}
---
h1: Объединить SVG, JPEG, PNG или другие изображения вместе с помощью C#
h2: Объединяйте файлы SVG или файлы изображений вместе и сохраняйте результат в PDF, XPS, BMP, JPEG, PNG, GIF и TIFF, используя C#.
---

{{<section overview>}}
---
h2: Как объединить несколько файлов изображений на C#
---

Есть много причин, по которым вам нужно объединить несколько SVG или изображений в один документ. Чтобы объединить файлы SVG, мы будем использовать <a href="https://products.aspose.com/svg/net/" target="_blank">Aspose.SVG для .NET API</a>, который представляет собой многофункциональный, мощный и простой в использовании API для работы с документами и слияния для платформы C#. Наша библиотека C# предоставляет класс <a href="https://reference.aspose.com/svg/net/aspose.svg.rendering/svgrenderer/" target="_blank">SvgRenderer </a> для рендеринга и слияния SVG документов. Метод Render() дает вам возможность одновременно отправлять несколько документов на выходное устройство рендеринга и объединять их.

{{<section demos>}}
---
h2: Пример С# кода для объединения SVG файлов в один PDF
---

Высокоскоростная библиотека C# позволяет разработчикам .NET объединять файлы SVG и преобразовывать объединенный результат во многие популярные форматы, такие как PDF, XPS, JPEG, PNG, BMP, GIF и TIFF, с высоким качеством и эффективностью. Слияние документов можно выполнить с помощью нескольких строк кода:

{{<section code-text>}}
---
title: Объединить SVG в PDF — C#
---

{{<section "code-snippet" i18n-exclude>}}

```cs
// Initialize SVG documents from files to merge 
using (var document1 = new SVGDocument("document1.svg"))
using (var document2 = new SVGDocument("document2.svg"))
using (var document3 = new SVGDocument("document3.svg"))
{
    // Create an instance of SvgRenderer
    using var renderer = new Aspose.Svg.Rendering.SvgRenderer();	
    // Create an instance of SvgRenderer
    using var device = new Aspose.Svg.Rendering.Pdf.PdfDevice("result.pdf");
    //Merge all SVG documents to PDF
    renderer.Render(device, document1, document2, document3);                
}
```

{{<section documentation>}}
---
h2: Объединение SVG в документации
---

Библиотека Aspose.SVG для .NET позволяет программно создавать, редактировать, читать, преобразовывать и объединять файлы SVG с помощью C#. Пространство имен [Aspose.Svg.Rendering](https://reference.aspose.com/svg/net/aspose.svg.rendering/) реализует простой доступ к методам конвертации и объединения. Кроме того, оно обеспечивает объединение файлов SVG в популярные форматы, такие как PDF, XPS, JPEG, PNG, BMP, TIFF и GIF. Пожалуйста, посетите главу документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target="_blank">Как объединить файлы SVG</a>, чтобы узнать больше о функциях объединения SVG C# API.

{{<section installing>}}
---
h2: Установка библиотеки Aspose.SVG для .NET
---

Aspose.SVG для .NET — это кроссплатформенная гибкая библиотека, предназначенная для предоставления широкого спектра функций для обработки и рендеринга документов SVG. Он легко интегрируется в ваши приложения .NET для работы с файлами SVG без установки какого-либо стороннего программного обеспечения. Наш SVG .NET API можно использовать с любым языком .NET, таким как C#, VB.NET, ASP.NET и т. д. Он одинаково хорошо работает на любой ОС, которая может установить Mono (поддержка .NET 4.0 Framework) или использовать .NET Core. Сюда входят Windows, Linux и macOS.

Установка <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG для .NET через NuGet</a>:
1. Использование консоли диспетчера пакетов.
2. Использование графического интерфейса диспетчера пакетов NuGet.</br>



  Дополнительные сведения об установке библиотеки C# вы найдете в [документации Aspose.SVG](https://docs.aspose.com/svg/net/getting-started/installation/).

{{<section other-mergers>}}
---
h2: Другие поддерживаемые Объединения
---

Вы можете объединить несколько файлов SVG и сохранить результат в другом формате: