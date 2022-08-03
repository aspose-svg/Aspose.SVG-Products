---
translation: true
template: /templates/_template-conversion-child.md
title: Конвертировать SVG в PDF на C# Core
description: Загружайте и конвертируйте SVG в PDF с помощью .NET Core API в Windows, macOS и Linux. Попробуйте онлайн-конвертер SVG в PDF бесплатно!
url: /net/conversion/svg-to-pdf/
family: svg
platformtag: net
feature: conversion
informat: SVG
outformat: PDF
otherformats: GIF JPEG PNG TIFF BMP PDF XPS
---

{{<section banner>}}
---
h1: Конвертировать SVG в PDF на C#
h2: Высокоскоростной .NET API для преобразования SVG в PDF в Windows, macOS и Linux.
---

{{<section overview>}}
---
h2: Преобразование SVG в PDF с помощью .NET Core
---

SVG — один из наиболее часто используемых форматов для создания веб-сайтов и печати графики для обеспечения масштабируемости. Но иногда вам нужно преобразовать SVG и сохранить его в другом формате файла. С помощью API [Aspose.SVG для .NET](https://products.aspose.com/svg/net/) вы можете программно преобразовать SVG в PDF с полным контролем над широким диапазоном параметров преобразования. Мощный C# API позволяет конвертировать SVG в популярные форматы с высокой скоростью и высоким качеством.


{{<section demos>}}
---
h2: Бесплатное приложение для конвертации SVG
---

Проверьте качество преобразования SVG в PDF прямо в браузере! В следующем примере C# показано, как преобразовать документ SVG с помощью метода ConvertSVG(). Мы описываем исходный код для чтения SVG из файла и последующего преобразования SVG в PDF с параметрами сохранения по умолчанию. Пожалуйста, загрузите SVG из локальной файловой системы, выберите выходной формат и запустите пример. Вы сразу получите результат в виде отдельного файла.

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/converter SVG PDF "JPG|JPEG" BMP XPS TIFF PNG GIF >}}
using Aspose.Svg;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;

    using var document = new SVGDocument("image.svg");
{{#if_output 'PDF'}}
    var options = new PdfSaveOptions();
{{/if_output}}
{{#if_output 'XPS'}}
    var options = new XpsSaveOptions();
{{/if_output}}
{{#if_output 'BMP' 'JPG' 'GIF' 'PNG' 'TIFF'}}
    var options = new ImageSaveOptions(ImageFormat.{{output param2 camel}});
{{/if_output}}
    Converter.ConvertSVG(document, options, "output.{{output lower}}");   
{{< /app/svg/converter>}} 

{{<section documentation>}}

Посетите <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">нашу документацию</a> чтобы узнать больше об использовании функций преобразования Aspose.SVG API и рассмотреть примеры C# для наиболее распространенных сценариев преобразования SVG. В главе документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">Как конвертировать SVG Файлы</a>, вы можете рассмотреть примеры C# того, как конвертировать SVG в PDF разными способами. Рассмотрим некоторые из них:

{{<section steps1>}}
---
h2: Шаги для преобразования SVG в PDF с использованием метода ConvertSVG()
---
1. Загрузите файл SVG с помощью одного из конструкторов SVGDocument() класса [SVGDocument.](https://reference.aspose.com/svg/net/aspose.svg/svgdocument)
1. Создайте новый объект [PdfSaveOptions](https://reference.aspose.com/svg/net/aspose.svg.saving/pdfsaveoptions).
1. Используйте метод [ConvertSVG(),](https://reference.aspose.com/svg/net/aspose.svg.converters/converter/convertsvg/) чтобы сохранить SVG в виде файла PDF. Вам необходимо передать SVGDocument, PdfSaveOptions и путь к выходному файлу методу ConvertSVG().
1. Файл PDF будет сохранен по указанному пути.

{{<section steps2>}}
---
h2: Шаги по преобразованию SVG в PDF с использованием метода RenderTo()
---
1. Инициализируйте [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument) с помощью файла SVG.
1. Создайте объект класса PdfRenderingOptions. Используйте конструктор [PdfRenderingOptions()](https://reference.aspose.com/svg/net/aspose.svg.rendering.pdf/pdfrenderingoptions/constructors/1) и укажите свойство «Формат» документа.
1. Инициализируйте класс [PdfDevice](https://reference.aspose.com/svg/net/aspose.svg.rendering.pdf/pdfdevice) и укажите имя выходного файла для рендеринга.
1. Вызовите метод [RenderTo()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto) и передайте экземпляр PdfDevice.

{{<section code-text>}}
---
title: Конвертировать SVG в PDF
---

{{<section "code-snippet" i18n-exclude>}}

```cs
using (var document = new SVGDocument("input.svg"))
{
	var options = new PdfRenderingOptions();
	using (IDevice device = new PdfDevice(options, "output.pdf"))
	{
		document.RenderTo(device);                    
	}
}
```

{{<section other-conversions>}}
---
title: Другие поддерживаемые преобразования SVG
subTitle: "Вы также можете конвертировать SVG во многие другие форматы файлов:"
---