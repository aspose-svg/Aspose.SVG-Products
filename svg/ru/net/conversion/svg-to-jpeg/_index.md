---
translation: true
template: ./../_template-child.md
title: Преобразование SVG в JPEG с помощью C# Core - Онлайн-конвертер SVG в JPEG
description: Загружайте и конвертируйте SVG в JPEG с помощью .NET Core API в Windows, macOS и Linux. Попробуйте онлайн-конвертер SVG в JPEG бесплатно!
url: /net/conversion/svg-to-jpeg/
family: svg
platformtag: net
feature: conversion
informat: SVG
outformat: JPEG
otherformats: GIF JPEG PNG TIFF BMP PDF XPS
---

{{<section banner>}}
---
h1: Преобразование SVG в JPEG через C#
h2: Высокоскоростной .NET API для преобразования SVG в JPEG в Windows, macOS и Linux.
---

{{<section overview>}}
---
h2: Преобразование SVG в JPEG через .NET Core
---

SVG — один из наиболее часто используемых форматов для создания веб-сайтов и печати графики для обеспечения масштабируемости. Но иногда вам нужно преобразовать SVG и сохранить его в распространенном формате растрового изображения. С помощью API [Aspose.SVG для .NET](https://products.aspose.com/svg/net/) вы можете программно преобразовать SVG в JPEG с полным контролем над широким диапазоном параметров преобразования. Мощный C# API позволяет конвертировать SVG в популярные форматы с высокой скоростью и высоким качеством.


{{<section demos>}}
---
h2: Бесплатные онлайн-демонстрации конвертера
---

Проверьте качество преобразования SVG в JPEG прямо в браузере! В следующем примере C# показано, как преобразовать документ SVG с помощью метода ConvertSVG(). Мы описываем исходный код для чтения SVG из файла и последующего преобразования SVG в JPEG с параметрами сохранения по умолчанию. Пожалуйста, загрузите SVG из локальной файловой системы, выберите выходной формат и запустите пример. Вы сразу получите результат в виде отдельного файла.

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/converter SVG "JPG|JPEG" BMP XPS TIFF PNG PDF GIF >}}
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

Посетите <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">нашу документацию</a>. чтобы узнать больше об использовании функций преобразования Aspose.SVG API и рассмотреть примеры C# для наиболее распространенных сценариев преобразования SVG. В статье документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/convert-svg-to-image/" target="_blank ">Преобразовать SVG в изображение</a>, вы можете рассмотреть примеры C# того, как конвертировать SVG в изображения различными способами. Рассмотрим некоторые из них:

{{<section steps1>}}
---
h2: Шаги для преобразования SVG в JPEG с использованием метода ConvertSVG()
---
1. Загрузите файл SVG с помощью одного из конструкторов SVGDocument() класса [SVGDocument](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument).
1. Создайте новый объект [ImageSaveOptions](https://apireference.aspose.com/svg/net/aspose.svg.saving/imagesaveoptions) с JPEG ImageFormat. По умолчанию свойство «Формат» имеет значение PNG.
1. Используйте метод [ConvertSVG()](https://apireference.aspose.com/svg/net/aspose.svg.converters/converter/convertsvg/), чтобы сохранить SVG как изображение JPEG. Вам необходимо передать SVGDocument, ImageSaveOptions и путь к выходному файлу методу ConvertSVG().
1. Файл JPEG будет сохранен по указанному пути.



{{<section steps2>}}
---
h2: Шаги для преобразования SVG в JPEG с использованием метода RenderTo()
---
1. Инициализируйте [SVGDocument](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument) с помощью файла SVG.
1. Создайте объект класса ImageRenderingOptions. Используйте конструктор [ImageRenderingOptions()](https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/constructors/1) и укажите свойство «Формат» документа.
1. Инициализируйте класс [ImageDevice](https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice) и укажите имя выходного файла для рендеринга.
1. Вызовите метод [RenderTo()](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto) и передайте экземпляр ImageDevice.



{{<section code-text>}}
---
title: Конвертировать SVG в JPEG
---

{{<section "code-snippet" i18n-exclude>}}

```cs
using (var document = new SVGDocument("input.svg"))
{
	var options = new ImageRenderingOptions(ImageFormat.Jpeg);
	using (IDevice device = new ImageDevice(options, "output.jpg"))
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
Кроме того, вы можете получить автономный установщик MSI или библиотеки DLL в ZIP-файле из [загрузки](https://downloads.aspose.com/svg/net). Aspose.SVG для .NET API является автономной библиотекой и не зависит от какого-либо программного обеспечения для обработки документов SVG.
 Дополнительные сведения об установке библиотеки C# и системных требованиях см. в [Документации Aspose.SVG](https://docs.aspose.com/svg/net/getting-started/).

 {{<section other-conversions>}}
---
title: Другие поддерживаемые преобразования SVG
subTitle: "Вы также можете конвертировать SVG во многие другие форматы файлов:"
---