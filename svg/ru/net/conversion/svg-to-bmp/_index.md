---
translation: true
template: ./../_template-child.md
title: Конвертировать SVG в BMP с помощью C# Core - Онлайн-конвертер SVG в BMP
description: Загружайте и конвертируйте SVG в BMP с помощью .NET Core API в Windows, macOS и Linux. Попробуйте онлайн Конвертер SVG в BMP бесплатно!
url: /net/conversion/svg-to-bmp/
family: svg
platformtag: net
feature: conversion
informat: SVG
outformat: BMP
otherformats: GIF BMP JPEG PNG TIFF PDF XPS
---

{{<section banner>}}
---
h1: Конвертировать SVG в BMP на C#
h2: Высокоскоростной .NET API для преобразования SVG в BMP в Windows, macOS и Linux.
---

{{<section overview>}}
---
h2: Преобразование SVG в BMP с помощью .NET Core
---

SVG — один из наиболее часто используемых форматов для создания веб-сайтов и печати графики для обеспечения масштабируемости. Но иногда вам нужно преобразовать SVG и сохранить его в распространенном формате растрового изображения. С помощью API [Aspose.SVG для .NET](https://products.aspose.com/svg/net/) вы можете программно преобразовать изображение SVG в BMP с полным контролем над широким диапазоном параметров преобразования. Мощный C# API позволяет конвертировать SVG в популярные форматы с высокой скоростью и высоким качеством.


{{<section demos>}}
---
h2: Бесплатное приложение для конвертации SVG
---

Проверьте качество преобразования SVG в BMP прямо в браузере! В следующем примере C# показано, как преобразовать документ SVG с помощью метода ConvertSVG(). Мы описываем исходный код для чтения SVG из файла и последующего преобразования SVG в BMP с параметрами сохранения по умолчанию. Пожалуйста, загрузите SVG из локальной файловой системы, выберите выходной формат и запустите пример. Вы сразу получите результат в виде отдельного файла.

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/converter SVG BMP XPS TIFF PNG PDF "JPG|JPEG" GIF>}}
using Aspose.Svg;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;
using Aspose.Svg.Rendering.Image;

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

Посетите <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">нашу документацию</a> чтобы узнать больше об использовании функций преобразования Aspose.SVG API и рассмотреть примеры C# для наиболее распространенных сценариев преобразования SVG. В статье документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/convert-svg-to-image/" target="_blank ">Преобразовать SVG в изображение</a>, вы можете рассмотреть примеры C# того, как конвертировать SVG в изображения различными способами. Рассмотрим некоторые из них:

{{<section steps1>}}
---
h2: Шаги для преобразования SVG в BMP с использованием метода ConvertSVG()
---
1. Загрузите файл SVG с помощью одного из конструкторов SVGDocument() класса [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument).
1. Создайте новый объект [ImageSaveOptions](https://reference.aspose.com/svg/net/aspose.svg.saving/imagesaveoptions) с форматом изображения BMP. По умолчанию свойство «Формат» имеет значение PNG.
1. Используйте метод [ConvertSVG()](https://reference.aspose.com/svg/net/aspose.svg.converters/converter/convertsvg/), чтобы сохранить SVG как изображение BMP. Вам необходимо передать SVGDocument, ImageSaveOptions и путь к выходному файлу методу ConvertSVG().
1. Файл BMP будет сохранен по указанному пути.



{{<section steps2>}}
---
h2: Шаги по преобразованию SVG в BMP с использованием метода RenderTo()
---
1. Инициализируйте [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument) с помощью файла SVG.
1. Создайте объект класса ImageRenderingOptions. Используйте конструктор [ImageRenderingOptions()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/constructors/1) и укажите свойство «Формат» документа.
1. Инициализируйте класс [ImageDevice](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice) и укажите имя выходного файла для рендеринга.
1. Вызовите метод [RenderTo()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto) и передайте экземпляр ImageDevice.



{{<section code-text>}}
---
title: Конвертировать SVG в BMP
---

{{<section "code-snippet" i18n-exclude>}}

```cs
using (var document = new SVGDocument("input.svg"))
{
	var options = new ImageRenderingOptions(ImageFormat.Bmp);
	using (IDevice device = new ImageDevice(options, "output.bmp"))
	{
		document.RenderTo(device);                    
	}
}
```

{{<section get-started>}}
---
h2: Начало работы с .NET SVG API
---

Установите из командной строки как ```nuget install Aspose.SVG``` или через консоль диспетчера пакетов Visual Studio с ```Install-Package Aspose.SVG```.
Кроме того, вы можете получить автономный установщик MSI или библиотеки DLL в ZIP-файле из [загрузки](https://releases.aspose.com/svg/net/). Aspose.SVG для .NET API является автономной библиотекой и не зависит от какого-либо программного обеспечения для обработки документов SVG.
 Дополнительные сведения об установке библиотеки C# и системных требованиях вы найдете в [документации Aspose.SVG](https://docs.aspose.com/svg/net/getting-started/).

{{<section other-conversions>}}
---
title: Другие поддерживаемые SVG Конвертеры
subTitle: "Вы также можете конвертировать SVG во многие другие форматы файлов:"
---