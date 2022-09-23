---
translation: true
template: /templates/_template-encoder-child.md
title: Конвертировать GIF в Base64 - Онлайн Конвертер и C# код
description: Преобразуйте GIF в Base64 онлайн или на C# и используйте кодированную строку для схемы URI данных. Встраивайте в HTML, CSS, JSON, XML.
url: /net/gif-to-base64/
family: svg
platformtag: net
feature: encode
informat: GIF
outformat: Base64
---

{{<section banner>}}
---
h1: Конвертируйте GIF в Base64
h2: Кодируйте GIF в строку Base64 онлайн или на C# и используйте ее в качестве примеров для URI данных.
---

{{<section overview>}}
---
h2: О схеме URI
---

URI данных — это метод встраивания изображений и других файлов в веб-страницы в виде текстовой строки на основе кодировки Base64. Схема URI данных позволяет включать любые двоичные данные в документы HTML, CSS, JSON или SVG. Например, вы можете вставлять изображения в веб-страницу, как если бы они были загружены из внешнего ресурса, но вместо указания URL-адреса файла вы вставляете содержимое изображения в кодировке Base64. Схема URI данных была определена в RFC 2397, и по состоянию на 2022 год она полностью поддерживается большинством основных браузеров. Основным преимуществом использования URI данных является ускорение загрузки страницы, поскольку браузеру не нужно делать дополнительный веб-запрос для извлечения файла, поскольку изображение уже встроено в HTML-документ.

Синтаксис URI данных следующий: `data:[<MIME type>][;charset=<charset>][;base64],<кодированные данные в виде строки Base64>`.

Поскольку размер данных в кодировке Base64 увеличивается на 33 %, рекомендуется использовать URI данных только для небольших изображений. Большие изображения Base64 создают много кода в HTML, что приводит к потере преимуществ в производительности. Файлы GIF имеют небольшой размер, что делает их идеальными для использования в качестве URI данных на веб-сайтах для логотипов, значков, штриховых рисунков и многого другого.

{{<section code-text>}}
---
h2: Как конвертировать GIF в Base64 на С#
title: Код С# для преобразования GIF в строку Base64 и встраивания ее в файл SVG
---

Чтобы преобразовать GIF в строку Base64, мы используем API [Aspose.SVG для .NET,](https://products.aspose.com/svg/net/) который является многофункциональным, мощным и простым в работе с документами для платформы C#. Рассмотрим пример кодирования GIF в Base64 и встраивания строки Base64 в качестве URI данных в документ SVG. Эти операции можно выполнить с помощью нескольких строк кода:

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open a binary file - GIF image
    var bytes = File.ReadAllBytes(@"image.gif");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert GIF to Base64
    img.Href.BaseVal = "data:image/gif;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: Шаги по преобразованию GIF в Base64 на C#
---
1. Откройте изображение GIF для конвертации. Используйте метод ReadAllBytes(`path`), чтобы открыть изображение GIF и прочитать содержимое файла в массив байтов.
1. Инициализируйте новый экземпляр класса [SVGDocument.](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor)
1. Используйте метод [CreateElementNS(`namespaceURI,qualName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) класса SVGDocument для создания экземпляр изображения. `namespaceURI` устанавливает ссылку на спецификацию W3C SVG. `qualifiedName` должно содержать строковое имя тега элемента изображения.
1. Конвертируйте GIF в Base64. Вызовите метод ToBase64String(bytes) для преобразования массива 8-разрядных целых чисел в его эквивалентное строковое представление, кодированное в цифрах Base64.
1. Добавьте элемент изображения в документ SVG, используя метод [AppendChild(`node`).](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/)
1. Используйте метод [Save(`path`,)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/) чтобы сохранить документ SVG.

{{<section online-encoder>}}
---
h2: Онлайн Кодировщик Base64
---

{{<section examples>}}
---
h2: Примеры использования кодировки Base64
html: HTML-код для встраивания GIF-изображения в кодировке Base64
css: Код CSS для встраивания изображения Base64 GIF в качестве фонового изображения
xml: Код XML для встраивания GIF-изображения Base64 в XML-документ
json: Код JSON для встраивания GIF-изображения Base64 в документ JSON
---

{{<section code-html>}}

```cs
<body>
    <div>
        <img src="data:image/gif;base64,R0lGODlhMgAyAPMMAA1dKxdkNC90STV4TkWCXFWNamGVdIaulZe..." alt="Green circle">
    </div>
</body>
```

{{<section code-css>}}

```cs
.class {
    background-image: url('data:image/gif;base64,R0lGODlhMgAyAPMMAA1dKxdkNC90STV4TkWCXFWNamGVdIaulZe...');
}
```

{{<section code-xml>}}

```cs
<?xml version="1.0" encoding="UTF-8"?>
<root>
 <image mime = "image/gif">R0lGODlhMgAyAPMMAA1dKxdkNC90STV4TkWCXFWNamGVdIaulZe...</image>
</root>
```

{{<section code-json>}}

```cs
{
  "image": {
    "mime": "image/gif",
    "data": "R0lGODlhMgAyAPMMAA1dKxdkNC90STV4TkWCXFWNamGVdIaulZe..."
  }
}
```

{{<section other-encoders>}}
---
title: Другие поддерживаемые Кодировщики Base64
subTitle: "Вы можете преобразовать изображение в строку Base64. Поддерживаются форматы JPG, PNG, BMP, GIF, TIFF, ICO и SVG:"
---