---
translation: true
template: /templates/_template-encoder-child.md
title: Конвертировать PNG в Base64 - Онлайн Конвертер и C# код
description: Преобразуйте PNG в Base64 онлайн или на C# и используйте кодированную строку для URI данных. Встраивайте в HTML, CSS, XML, JSON и др.
url: /net/png-to-base64/
family: svg
platformtag: net
feature: encode
informat: PNG
outformat: Base64
---

{{<section banner>}}
---
h1: Преобразование PNG в Base64
h2: Кодируйте строку PNG в Base64 онлайн или на C# и используйте ее в качестве примеров для URI данных.
---

{{<section overview>}}
---
h2: О схеме URI
---

URI данных — это метод встраивания изображений и других файлов в веб-страницы в виде текстовой строки на основе кодировки Base64. Схема URI данных позволяет включать любые двоичные данные в документы HTML, CSS, JSON или SVG. Например, вы можете вставлять изображения в веб-страницу, как если бы они были загружены из внешнего ресурса, но вместо указания URL-адреса файла вы вставляете содержимое изображения в кодировке Base64. Схема URI данных была определена в RFC 2397, и по состоянию на 2022 год она полностью поддерживается большинством основных браузеров. Основным преимуществом использования URI данных является ускорение загрузки страницы, поскольку браузеру не нужно делать дополнительный веб-запрос для извлечения файла, поскольку изображение уже встроено в HTML-документ.

Синтаксис URI данных следующий: `data:[<MIME type>][;charset=<charset>][;base64],<кодированные данные>`.

Поскольку размер данных в кодировке Base64 увеличивается на 33 %, рекомендуется использовать URI данных только для небольших изображений. Большие изображения Base64 создают много кода в HTML, что приводит к потере преимуществ в производительности. Если вам нужно преобразовать PNG в Base64 и использовать кодированную строку для встраивания в текстовый файл, сначала изучите все плюсы и минусы.

{{<section code-text>}}
---
h2: Как преобразовать PNG в Base64 на С#
title: Код С# для преобразования строки PNG в строку Base64 и встраивания ее в файл SVG
---

Чтобы преобразовать строку PNG в строку Base64, мы используем API [Aspose.SVG для .NET,](https://products.aspose.com/svg/net/) который является многофункциональным, мощным и простым в использовании. использовать API для работы с документами для платформы C#. Мы рассматриваем пример кодирования PNG в Base64 и встраивания строки Base64 в качестве URI данных в документ SVG. Эти операции можно выполнить с помощью нескольких строк кода:

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open a binary file - PNG image
    var bytes = File.ReadAllBytes(@"image.png");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert PNG to Base64
    img.Href.BaseVal = "data:image/png;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: Действия по преобразованию PNG в Base64 в C#
---
1. Откройте изображение PNG для преобразования. Используйте метод ReadAllBytes(`path`), чтобы открыть PNG и прочитать содержимое файла в массив байтов.
1. Инициализируйте новый экземпляр класса [SVGDocument.](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor)
1. Используйте метод [CreateElementNS(`namespaceURI,qualName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) класса SVGDocument для создания экземпляр изображения. `namespaceURI` устанавливает ссылку на спецификацию W3C SVG. `qualifiedName` должно содержать имя строкового тега элемента изображения.
1. Конвертируйте PNG в Base64. Вызовите метод ToBase64String(bytes) для преобразования массива 8-разрядных целых чисел в его эквивалентное строковое представление, кодированное в цифрах base64.
1. Добавьте элемент изображения в документ SVG, используя метод [AppendChild(`node`).](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/)
1. Вызовите метод [Save(`path`),](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/) чтобы сохранить документ SVG.

{{<section online-encoder>}}
---
h2: Онлайн-кодировщики Base64
---

{{<section examples>}}
---
h2: Примеры использования кодировки Base64
svg: Код SVG для встраивания изображения Base64 PNG в документ SVG
html: HTML-код для встраивания изображения Base64 PNG
css: Код CSS для встраивания изображения Base64 PNG в качестве фонового изображения
xml: XML-код для встраивания изображения Base64 PNG в XML-документ
json: Код JSON для встраивания изображения PNG Base64 в документ JSON
---

{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/png;charset=utf-8;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAg..." alt="Red circle"/>
</svg>
```

{{<section "code-html" i18n-exclude>}}

```cs
<body>
    <div>
        <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAg..." alt="Red circle">
    </div>
</body>
```

{{<section "code-css" i18n-exclude>}}

```cs
.class {
    background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAg...');
}
```

{{<section "code-xml" i18n-exclude>}}

```cs
<?xml version="1.0" encoding="UTF-8"?>
<root>
<image mime = "image/png">iVBORw0KGgoAAAANSUhEUgAAACAAAAAg...</image>
</root>
```

{{<section "code-json" i18n-exclude>}}

```cs
{
  "image": {
    "mime": "image/png",
    "data": "iVBORw0KGgoAAAANSUhEUgAAACAAAAAg..."
  }
}
```

{{<section other-encoders>}}
---
title: Другие поддерживаемые кодировщики Base64
subTitle: "Вы можете преобразовать изображение в строку Base64. Поддерживаются форматы JPG, PNG, BMP, GIF, TIFF, ICO и SVG:"
---