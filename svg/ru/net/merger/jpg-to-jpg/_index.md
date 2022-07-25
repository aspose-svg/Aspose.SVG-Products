---
translation: true
template: ./../_template-child.md
title: Объединение JPG в JPG на C# - Aspose.SVG
description: Объединение JPG в JPG с помощью .NET Core API в Windows, macOS и Linux
url: /net/merger/jpg-to-jpg/
family: svg
platformtag: net
feature: merge
informat: JPG
outformat: JPG
otherformats: GIF PNG TIFF BMP
---

{{<section banner>}}
---
h1: Объединить JPG в JPG на C#
h2: Высокоскоростной .NET API для объединения файлов JPG в Windows, macOS и Linux.
---

{{<section overview>}}
---
h2: Объединение JPG в JPG с помощью C#
---

JPEG — это стандартный формат изображения, разработанный Объединенной группой экспертов по фотографии. Технология сжатия файлов JPEG хорошо разработана и продумана. Он удаляет избыточные данные о цвете и обеспечивает чрезвычайно высокую степень сжатия. Тем не менее, JPEG может отображать яркие и красочные изображения и обеспечивать лучшее качество изображения при наименьшем размере изображения. Во многих случаях вам может понадобиться объединить изображения JPG. С помощью API [Aspose.SVG для .NET](https://products.aspose.com/svg/net/) вы можете программно объединить JPG в JPG. Мощный C# API поможет вам быстро и качественно объединить файлы JPG!

{{<section code-text>}}
---
h2: Пример кода C# для объединения JPG в JPG
title: Объединение JPG в JPG — C#
---

Объедините несколько файлов JPG и легко сохраните результат в виде одного файла JPG! Объединение изображений можно выполнить с помощью нескольких строк кода:

{{<section "code-snippet" i18n-exclude>}}

```cs
// Images to merge 
var images = new string[] { @"image1.jpg", "image2.jpg" };
// Initialize a new instance of SVGDocument
using (var document = new SVGDocument())
{
    // Declare an image function
    SVGImageElement CreateThumbnail(string imagePath, int width, int height)
    {
        var image = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
        image.Href.BaseVal = imagePath;
        image.Width.BaseVal.Value = width;
        image.Height.BaseVal.Value = height;
        return image;
    }
    // Set a thumbnail size
    const int thumbnailWidth = 200;
    const int thumbnailHeight = 200;
    const int thumbnailMargin = 10;
    // Create thumbnails merging loop
    for (var i = 0; i < images.Length; i++)
    {
        // Create a thumbnail
        var thumbnail = CreateThumbnail(images[i], thumbnailWidth, thumbnailHeight);
        // Define coordinates 
        thumbnail.X.BaseVal.Value = 0;
        thumbnail.Y.BaseVal.Value = (thumbnailHeight + thumbnailMargin) * i;
        // Append the thumbnail to the document
        document.DocumentElement.AppendChild(thumbnail);
    }
    // Define saving options
    var options = new ImageRenderingOptions
    {
        Format = ImageFormat.Jpeg,
        PageSetup =
        {
            Sizing = SizingType.FitContent
        }
    };    
    // Render document 
    document.RenderTo(new ImageDevice(options, "merged.jpg"));
}
```

{{<section steps>}}
---
h2: Шаги по слиянию JPG в JPG с помощью C#
---
1. Определите изображения JPG для объединения.
1. Инициализируйте новый экземпляр класса [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor).
1. Объявите функцию изображения. Для создания экземпляр изображения. `namespaceURI` устанавливает ссылку на спецификацию W3C SVG. `qualifiedName` должно содержать имя строкового тега элемента изображения.
1. Вызовите функцию изображения, чтобы создать объект-миниатюру.
1. Чтобы добавить миниатюры в документ, используйте метод [AppendChild()](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/#appendchild).
1. Используйте один из конструкторов [ImageRenderingOptions()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/) для инициализации нового экземпляра класса ImageRenderingOptions. Вы можете настроить процесс рендеринга, указав размер страницы, формат изображения и т. д. В качестве формата изображения по умолчанию используется PNG.
1. Создайте экземпляр ImageDevice с помощью конструктора [ImageDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/imagedevice/#constructor_3).
1. Вызовите метод [RenderTo(`device`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/#renderto), чтобы отправить текущий документ на выходное устройство рендеринга.
1. Несколько изображений JPG будут сохранены в один файл JPG по указанному пути.



{{<section documentation>}}

Высокоскоростная библиотека C# позволяет разработчикам .NET быстро и эффективно объединять файлы JPG в одно изображение. Пространство имен [Aspose.Svg.Rendering.Image](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/) предоставляет определенные классы устройств, а также несколько классов параметров рендеринга, отвечающих за рендеринг в растровые форматы: JPEG, PNG, BMP, GIF и TIFF. Посетите <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">нашу документацию</a>, чтобы узнать подробнее об использовании функций API Aspose.SVG.

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
Кроме того, вы можете получить автономный установщик MSI или библиотеки DLL в ZIP-файле из [загрузки](https://downloads.aspose.com/svg/net). Aspose.SVG для .NET API является автономной библиотекой и не зависит от какого-либо программного обеспечения для обработки документов SVG.
 Дополнительные сведения об установке библиотеки C# и системных требованиях см. в [документации Aspose.SVG](https://docs.aspose.com/svg/net/getting-started/).

{{<section other-mergers>}}
---
title: Другие поддерживаемые слияния
subTitle: "Вы можете объединять изображения с файлами других форматов:"
---