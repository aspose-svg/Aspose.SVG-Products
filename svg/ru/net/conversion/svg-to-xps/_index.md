---
translation: true
template: ./../_template-child.md
title: Преобразование SVG в XPS с помощью C# Core - Онлайн-конвертер SVG в XPS
description: Преобразование SVG в XPS с помощью .NET Core API в Windows, macOS и Linux. Попробуйте онлайн Конвертер SVG в XPS бесплатно!
url: /net/conversion/svg-to-xps/
family: svg
platformtag: net
feature: conversion
informat: SVG
outformat: XPS
otherformats: GIF JPEG PNG TIFF BMP PDF XPS
---

{{<section banner>}}
---
h1: Преобразование SVG в XPS через C#
h2: Высокоскоростной .NET API для преобразования SVG в XPS в Windows, macOS и Linux.
---

{{<section overview>}}
---
h2: Преобразование SVG в XPS через .NET Core
---

SVG — один из наиболее часто используемых форматов для создания веб-сайтов и печати графики для обеспечения масштабируемости. Но иногда вам нужно преобразовать SVG и сохранить его в другом формате файла. С помощью API [Aspose.SVG для .NET](https://products.aspose.com/svg/net/) вы можете программно преобразовывать SVG в XPS с полным контролем над широким диапазоном параметров преобразования. Мощный C# API позволяет конвертировать SVG в популярные форматы с высокой скоростью и высоким качеством.


{{<section demos>}}
---
h2: Бесплатные онлайн-демонстрации конвертера
---

Проверьте качество преобразования SVG в XPS прямо в браузере! В следующем примере C# показано, как преобразовать документ SVG с помощью метода ConvertSVG(). Мы описываем исходный код для чтения SVG из файла и последующего преобразования SVG в XPS с параметрами сохранения по умолчанию. Пожалуйста, загрузите SVG из локальной файловой системы, выберите выходной формат и запустите пример. Вы сразу получите результат в виде отдельного файла.

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/converter SVG XPS PDF "JPG|JPEG" BMP TIFF PNG GIF >}}
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

Посетите <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">нашу документацию</a>. чтобы узнать больше об использовании функций преобразования Aspose.SVG API и рассмотреть примеры C# для наиболее распространенных сценариев преобразования SVG. В главе документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">Как преобразовать SVG Файлы</a>, вы можете рассмотреть примеры C# того, как конвертировать SVG в XPS разными способами. Рассмотрим некоторые из них:

{{<section steps1>}}
---
h2: Шаги для преобразования SVG в XPS с использованием метода ConvertSVG()
---
1. Загрузите файл SVG с помощью одного из конструкторов SVGDocument() класса [SVGDocument](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument).
1. Создайте новый объект [XpsSaveOptions](https://apireference.aspose.com/svg/net/aspose.svg.saving/xpssaveoptions).
1. Используйте метод [ConvertSVG()](https://apireference.aspose.com/svg/net/aspose.svg.converters/converter/convertsvg/), чтобы сохранить SVG в виде файла XPS. Вам необходимо передать SVGDocument, XpsSaveOptions и путь к выходному файлу методу ConvertSVG().
1. Файл XPS будет сохранен по указанному пути.



{{<section steps2>}}
---
h2: Шаги по преобразованию SVG в XPS с использованием метода RenderTo()
---
1. Инициализируйте [SVGDocument](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument) с помощью файла SVG.
1. Создайте объект класса XpsRenderingOptions. Используйте конструктор [XpsRenderingOptions()](https://apireference.aspose.com/svg/net/aspose.svg.rendering.xps/xpsrenderingoptions/constructors/1) и укажите свойство Format документа.
1. Инициализируйте класс [XpsDevice](https://apireference.aspose.com/svg/net/aspose.svg.rendering.xps/xpsdevice) и укажите имя выходного файла для рендеринга.
1. Вызовите метод [RenderTo()](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto) и передайте экземпляр XpsDevice.



{{<section code-text>}}
---
title: Конвертировать SVG в XPS
---

{{<section "code-snippet" i18n-exclude>}}

```cs
using (var document = new SVGDocument("input.svg"))
{
	var options = new XpsRenderingOptions();
	using (IDevice device = new XpsDevice(options, "output.xps"))
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