---
translation: true
template: /templates/_template-conversion.md
title: Преобразование SVG в популярные форматы с помощью C# - онлайн Конвертер SVG
url: /net/conversion/
description: Конвертируйте SVG в PDF, XPS и изображения с помощью нескольких строк кода C#. Проверьте онлайн Конвертер SVG бесплатно!
---

{{<section banner>}}
---
h1: Конвертировать SVG на C#
h2: Преобразование SVG в PDF, XPS, JPEG, PNG, TIFF, BMP, GIF c помощью высокоскоростной .NET библиотеки
---

{{<section overview>}}
---
h2: Как конвертировать SVG с помощью C#
---

SVG (Scalable Vector Graphics) — это основанный на XML формат изображения для двумерной графики. Это формат векторной графики, предназначенный в первую очередь для Интернета. Главным преимуществом SVG является его непревзойденная способность масштабироваться до любого размера без малейшего ухудшения качества. Все современные браузеры поддерживают SVG, и, казалось бы, Сеть уже должна перейти на векторную графику. Однако существуют некоторые ограничения на использование SVG, и иногда вам нужно конвертировать SVG в другие форматы.
 
 - Статический [Converter class](https://reference.aspose.com/svg/net/aspose.svg.converters/converter/) представляет собой общий фасад, который обеспечивает преобразование файлов SVG в популярные форматы и позволяет выполнять эти операции. удобно и легко.

 - Метод [RenderTo()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/) используется для рендеринга SVG в другой формат и отправки документа на устройство вывода. Aspose.SVG API обеспечивает реализацию следующих устройств вывода: классы PdfDevice, XpsDevice и ImageDevice, которые выполняют рендеринг в файлы форматов PDF, XPS и Image соответственно.

<a href="https://products.aspose.com/svg/net/" target="_blank">Aspose.SVG для .NET API</a> упрощает процесс преобразования для разработчиков. Преобразование между форматами может выполняться с использованием нескольких различных подходов:

{{<section demos>}}
---
h2: Демонстрация Конвертера SVG
---

Вы можете конвертировать SVG с помощью Aspose.SVG для .NET API в режиме реального времени. В следующем примере C# показано, как преобразовать документ SVG. Пожалуйста, загрузите файл из локальной файловой системы, выберите выходной формат и запустите пример. Вы сразу получите результат в виде отдельного файла.

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/converter SVG PDF BMP "JPG|JPEG" PNG GIF TIFF XPS>}}
using Aspose.Svg;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;

    using var document = new SVGDocument("input.{{input lower}}");
{{#if_output 'PDF'}}
    var options = new PdfSaveOptions();
{{/if_output}}
{{#if_output 'DOCX'}}
    var options = new DocSaveOptions();
{{/if_output}}
{{#if_output 'XPS'}}
    var options = new XpsSaveOptions();
{{/if_output}}
{{#if_output 'MD'}}
    var options = new MarkdownSaveOptions();
{{/if_output}}
{{#if_output 'BMP' 'JPG' 'GIF' 'PNG' 'TIFF'}}
    var options = new ImageSaveOptions(ImageFormat.{{output camel}});
{{/if_output}}
    Converter.ConvertSVG(document, options, "output.{{output lower}}");
{{< /app/svg/converter>}}

{{<section documentation>}}
---
h2: Статьи документации о конвертации SVG файлов
---

Библиотека Aspose.SVG для .NET позволяет программно создавать, редактировать, читать и конвертировать файлы SVG с помощью C#. Главной изюминкой SVG C# API является функция преобразования. Пространство имен [Aspose.SVG.Converters](https://reference.aspose.com/svg/net/aspose.svg.converters/) реализует простой доступ к методам конвертации. Оно обеспечивает широкий спектр преобразований SVG в популярные форматы, такие как PDF, XPS, JPEG, PNG, BMP, TIFF и GIF. Пожалуйста, посетите главу документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">Как конвертировать SVG файлы</a>, чтобы узнать больше о функциях преобразования SVG C# API.

<div>
	<ul>
		<li><a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/convert-svg-to-pdf/" target="_blank">Convert SVG to PDF</a></li>
		<li><a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/convert-svg-to-xps/" target="_blank">Convert SVG to XPS</a></li>
		<li><a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/convert-svg-to-image/" target="_blank">Convert SVG to Image</a></li>							
	</ul>
</div>

{{<section installing>}}
---
h2: Как установить библиотеку Aspose.SVG для .NET
---

Aspose.SVG для .NET — это кроссплатформенная гибкая библиотека, предназначенная для предоставления широкого спектра функций для обработки и рендеринга документов SVG. Она легко интегрируется в ваши приложения .NET для работы с файлами SVG без установки какого-либо стороннего программного обеспечения. Наш SVG .NET API можно использовать с любым языком .NET, таким как C#, VB.NET, ASP.NET и т. д. Он одинаково хорошо работает на любой ОС, которая может установить Mono (поддержка .NET 4.0 Framework) или использовать .NET Сore. Сюда входят Windows, Linux и macOS.

Установка <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG для .NET через NuGet</a>:
1. Использование консоли диспетчера пакетов.
1. Использование графического интерфейса диспетчера пакетов NuGet.



Дополнительные сведения об установке библиотеки C# вы найдете в [документации Aspose.SVG](https://docs.aspose.com/svg/net/getting-started/installation/).

{{<section other-conversions>}}
---
h2: Другие поддерживаемые Конвертеры
---

Вы можете конвертировать файлы SVG во многие другие форматы файлов, включая некоторые из перечисленных ниже: