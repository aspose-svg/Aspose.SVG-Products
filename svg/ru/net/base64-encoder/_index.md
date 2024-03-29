﻿---
translation: true
template: /templates/_template-encoder.md
title: Кодировать изображение в Base64 - C# код и Онлайн Конвертер
url: /net/base64-encoder/
description: Преобразование изображения в Base64 онлайн или на C#. Используйте изображения Base64 в виде URI данных, чтобы встроить их в HTML, CSS или JSON.
---

{{<section banner>}}
---
h1: Кодировать изображение в Base64 онлайн или на С#
h2: Преобразование изображения в кодированную Base64 строку. Поддерживаются форматы JPG, PNG, BMP, GIF, TIFF, WEBP, SVG и др.
---

{{<section text-plugin>}}
---
h2: Конвертируйте изображения в Base64 онлайн!
---

{{<section "app-plugin" i18n-exclude>}}

{{< app/svg/base64 inputFormat="Image" sourceImage="/svg/images/encoder/flower.jpg">}}
{{< /app/svg/base64>}} 

{{<section base64>}}
---
h2: Как кодировать изображения с помощью C#
title: Кодирование Base64
---

Base64 — это схема кодирования для преобразования двоичных данных в текстовый формат ASCII. Обычно он используется для передачи данных через Интернет. Результат преобразования изображения в Base64 — это просто набор латинских букв, цифр и двух символов — «+» и «/». Любой браузер знает, что с ними делать. Другими словами, Base64 — это разновидность кодирования двоичного кода в текст.

 Base64 особенно распространен в Интернете, где его использование включает возможность встраивания файлов изображений или других двоичных ресурсов в текстовые ресурсы, такие как файлы HTML и CSS. Включение данных изображения в HTML-файл означает, что браузеру не нужно делать дополнительный веб-запрос для извлечения файла, поскольку изображение уже встроено в HTML-документ. Кодировку Base64 рекомендуется использовать только для небольших изображений. Большие изображения Base64 приводят к большому количеству кода в HTML, что влечет потерю преимуществ в производительности. 

{{<section demos>}}
---
h2: Кодировать изображение в Base64 на С#
title: Код С# для преобразования изображения PNG в Base64
---

В этой статье рассматривается, как кодировать файл изображения в строку Base64 с помощью функций Aspose.SVG .NET API. В следующем примере C# показано, как преобразовать изображение PNG в строку Base64 и встроить его в файл SVG. Метод ReadAllBytes(string) используется для открытия изображения (двоичного файла) и чтения содержимого файла в массив байтов. Метод ToBase64String(bytes) преобразует массив 8-разрядных целых чисел в его эквивалентное строковое представление, кодированное цифрами с основанием 64. Затем метод AppendChild() добавляет изображение в кодировке Base64 в документ SVG.

{{<section "code" i18n-exclude>}}

```cs
    // Open a binary file - PNG image
    var bytes = File.ReadAllBytes(@"image.png");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert image to base64
    img.Href.BaseVal = "data:image/png;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section html>}}
---
h2: Встроить изображение Base64 в HTML
title: Код HTML для встраивания изображения Base64 в виде URI данных
text: Изображения в кодировке Base64 можно встраивать в HTML с помощью тега `<img>`. Просто вставьте данные изображения непосредственно в файл HTML, используя схему URI данных. Кодировка Base64 и использование схемы данных URI уменьшают количество HTTP-запросов, необходимых браузеру для отображения веб-страницы. Этот фрагмент кода демонстрирует, как можно встраивать изображения Base64 в HTML.
---

URI данных состоит из двух частей, разделенных запятой. Первая часть указывает изображение в кодировке Base64, а вторая часть указывает строку изображения в кодировке Base64:
1. `data:image/jpeg;base64` — это заголовок схемы URI данных.
1. `iVBORw0KGgoAAAANSUhEUg...` — это данные, кодированные в формате Base64.


{{<section css>}}
---
h2: Встроить изображение Base64 в CSS код
title: Код CSS для встраивания изображения Base64 в виде URI данных
---

Еще один способ уменьшить количество HTTP-запросов к изображениям — использование CSS-свойства `background-image`. Свойство `background-image` определяет изображения как фон элемента. Каждое изображение для свойства background-image может быть указано как URL-адрес или как URI данных изображения. Разница в том, что в первом случае браузер отправляет HTTP-запрос на получение внешнего изображения, а во втором случае изображение в формате Base64 встраивается непосредственно в документ и не указывает на другие источники. Поэтому браузеру не нужно загружать HTTP-запросы для его доставки.

{{<section encoder-online>}}
---
h2: Онлайн Кодировщики Base64
---

Онлайн <a href="https://products.aspose.app/svg/{{lang}}/encoding" target="_blank">Кодировщики Base64</a> преобразуют содержимое документов SVG или файлов изображений в их эквивалент строковое представление, кодированное цифрами с основанием 64. Они также предоставляют примеры для данных URI, JSON, XML и других. Инструменты кодирования помогают избежать различных проблем с кодированием данных, которые делают содержимое веб-сайта или сообщения электронной почты нечитаемыми. Кодировщики Base64 безопасны, просты в использовании и совершенно бесплатны. Приложения работают в любом браузере и на любой операционной системе.

{{<section installing>}}
---
h2: Установка библиотеки Aspose.SVG для .NET
---

Aspose.SVG для .NET — это кроссплатформенная библиотека, предназначенная для предоставления широкого спектра функций для обработки и рендеринга документов SVG. Он легко интегрируется в ваши приложения .NET для работы с файлами SVG без установки какого-либо стороннего программного обеспечения. Наш SVG .NET API можно использовать с любым языком .NET, таким как C#, VB.NET, ASP.NET и т. д. Он одинаково хорошо работает на любой ОС, которая может установить Mono (поддержка .NET 4.0 Framework) или использовать .NET Сore. Сюда входят Windows, Linux и macOS.

Установка <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG для .NET через NuGet</a>:
1. Использование консоли диспетчера пакетов.
1. Использование графического интерфейса диспетчера пакетов NuGet.

Дополнительные сведения об установке библиотеки C# вы найдете в [документации Aspose.SVG.](https://docs.aspose.com/svg/net/getting-started/installation/)

{{<section other-encoders>}}
---
h2: Другие поддерживаемые Кодировщики
---

Вы также можете кодировать файлы SVG или изображения в Base64:

{{<section "svg">}}
---
title: Код SVG для встраивания изображения Base64
---

Фрагмент получившегося файла image-base64.svg показан ниже. Строка Base64 была обрезана, чтобы не загромождать пример кода SVG. Формат для встраивания изображения Base64 в качестве данных URI следующий:

`data:[<mime type>][;charset=<charset>][;base64],<кодированные данные>`

{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/png;charset=utf-8;base64,iVBORw0KGgoAAAANSUhEUg..." alt="Red border"/>
</svg>
```

{{<section "code-html" i18n-exclude>}}

```cs
<body>
    <div>
        <img src="data:image/jpeg;base64,iVBORw0KGgoAAAANSUhEUg..." alt="Red border">
    </div>
</body>
```

{{<section "code-css" i18n-exclude>}}

```cs
body {
    background-image: url('data:image/jpeg;base64,iVBORw0KGgoAAAANSUhEUg...');
}
```