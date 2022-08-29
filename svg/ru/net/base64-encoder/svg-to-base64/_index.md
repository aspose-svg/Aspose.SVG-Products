---
translation: true
template: /templates/_template-encoder-child.md
title: Конвертировать SVG в Base64 на C#
description: Преобразуйте SVG в Base64 на C# и используйте кодированную строку для URI данных. Встраивайте его в HTML, CSS, XML, JSON и др.
url: /net/svg-to-base64/
family: svg
platformtag: net
feature: encode
informat: SVG
outformat: Base64
---

{{<section banner>}}
---
h1: Преобразование SVG в Base64 на C#
h2: Кодируйте изображение SVG в строку Base64 на C# и используйте его в качестве примеров для URI данных.
---

{{<section overview>}}
---
h2: О схеме URI
---

URI данных — это метод встраивания изображений и других файлов в веб-страницы в виде текстовой строки на основе кодировки Base64. Схема URI данных позволяет включать любые двоичные данные в документы HTML, CSS, JSON или SVG. Например, вы можете вставлять изображения в веб-страницу, как если бы они были загружены из внешнего ресурса, но вместо указания URL-адреса файла вы вставляете содержимое изображения в кодировке Base64. Основным преимуществом использования URI данных является ускорение загрузки страницы, поскольку браузеру не нужно делать дополнительный веб-запрос для извлечения файла, поскольку изображение уже встроено в HTML-документ.

Синтаксис URI данных следующий: `data:[<MIME type>][;charset=<charset>][;base64],<кодированные данные>`.

Файлы SVG могут содержать «небезопасные» символы. Векторные изображения могут иметь растровое содержимое или атрибуты, значения которых заключены в одинарные или двойные кавычки. Поэтому требуется предварительная обработка (нормализация) этого формата. Вы можете использовать изображение SVG в HTML или CSS кодированное в виде URI данных. Если SVG изображение кодировано с использованием URI данных, оно будет работать в любом браузере.

{{<section code-text>}}
---
h2: Как преобразовать SVG в Base64 на С#
title: Код С# для преобразования строки SVG в строку Base64 и встраивания ее в файл SVG
---

Чтобы преобразовать изображение SVG в строку Base64, мы используем API [Aspose.SVG для .NET](https://products.aspose.com/svg/net/), который представляет собой многофункциональный, мощный и простой в использовании -использовать API для работы с документами для платформы C#. Мы рассматриваем пример преобразования изображения SVG в кодировку Base64 и встраивания строки Base64 в качестве URI данных в документ SVG. Эти операции можно выполнить с помощью нескольких строк кода:

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open an SVG image
    var bytes = File.ReadAllBytes(@"flower.svg");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert SVG image to Base64
    img.Href.BaseVal = "data:image/svg+xml;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: Шаги по преобразованию SVG в Base64 в C#
---
1. Откройте изображение SVG для преобразования. Используйте метод ReadAllBytes(`path`), чтобы открыть изображение SVG и прочитать содержимое файла в массив байтов.
1. Инициализируйте новый экземпляр класса [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor).
1. Используйте метод [CreateElementNS(`namespaceURI,qualName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) класса SVGDocument для создания экземпляр изображения. `namespaceURI` устанавливает ссылку на спецификацию W3C SVG. `qualifiedName` должно содержать имя строкового тега элемента изображения.
1. Преобразуйте SVG в Base64. Вызовите метод ToBase64String(bytes) для преобразования массива 8-разрядных целых чисел в его эквивалентное строковое представление, кодированное в цифрах base64.
1. Добавьте элемент изображения в документ SVG, используя метод [AppendChild(`node`)](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/).
1. Используйте метод [Save(`path`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/) для сохранения документа SVG.

{{<section online-encoder>}}
---
h2: Онлайн-кодировщики Base64
---

{{<section examples>}}
---
h2: Примеры использования кодировки Base64
svg: Код SVG для встраивания изображения SVG Base64 в документ SVG
html: HTML-код для встраивания изображения Base64 SVG
css: Код CSS для встраивания изображения Base64 SVG в качестве фонового изображения
xml: Код XML для встраивания изображения SVG Base64 в документ XML
json: Код JSON для встраивания изображения SVG Base64 в документ JSON
---

{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/svg+xml;charset=utf-8;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..." alt="Blue flower"/>
</svg>
```

{{<section code-html>}}

```cs
<body>
    <div>
        <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..." alt="Blue flower">
    </div>
</body>
```

{{<section code-css>}}

```cs
.class {
    background-image: url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna...');
}
```

{{<section code-xml>}}

```cs
<?xml version="1.0" encoding="UTF-8"?>
<root>
<image mime = "image/svg+xml">PHN2ZyB3aWR0aD0iNDUwIiBoZWlna...</image>
</root>
```

{{<section code-json>}}

```cs
{
  "image": {
    "mime": "image/svg+xml",
    "data": "PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..."
  }
}
```

{{<section other-encoders>}}
---
title: Другие поддерживаемые кодировщики Base64
subTitle: "Вы можете преобразовать изображение в строку Base64 — поддерживаются форматы JPG, PNG, BMP, GIF, TIFF, ICO и SVG:"
---