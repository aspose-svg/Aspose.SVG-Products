---
translation: true
template: /templates/_template-vectorization.md
title: Векторизация изображения или текста — код C# и онлайн-векторизатор
url: /net/vectorization/
description: Преобразуйте изображения или текст SVG в векторную графику и сохраните результат в файл SVG. Векторизуйте изображения или текст онлайн или на C#!
---

{{<section banner>}}
---
h1: Векторизовать изображение или текст в C#
h2: Преобразование изображения в вектор в C#. Поддерживаются JPG, JPEG, PNG, BMP, GIF, TIFF, ICO, IFIF, WEBP и другие форматы растровых изображений.
---

{{<section overview>}}
---
title: Векторизация изображения
---

Растровое изображение — это карта пикселей — точек или зерен — на пленке, бумаге или экране. Каждый пиксель имеет свой цвет. Масштабирование растрового изображения приводит к появлению на нем шума и размытия. Чтобы избежать таких артефактов, вы можете преобразовать растровое изображение в векторный формат, например, в графику SVG. Векторизация изображения — это способ представления изображения в векторной форме. Векторное изображение основано на формуле — оно основано не на пикселях, а на примитивах, таких как точки, линии, кривые, которые представлены математическими выражениями. Линии и окрашенные области на таких изображениях представляются как математические кривые, которые определяются декартовыми точками, соединенными образующими их путями. Векторное изображение будет иметь все преимущества векторной графики и не будет пикселизировано при масштабировании.
 
Вы можете векторизовать изображение с помощью Aspose.SVG для .NET API в режиме реального времени. Попробуйте наш бесплатный векторизатор изображений и преобразуйте информацию о цвете пикселей в простые геометрические объекты! Пожалуйста, выберите изображение для векторизации. Поддерживаются JPG, JPEG, PJP, PJPEG, PNG, BMP, XBM, GIF, TIFF, ICO, IFIF, WEBP и другие форматы растровых изображений.

{{<section "app-pluging" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}}

{{<section plugin-use>}}
---
h2: Как использовать векторизатор изображений?
---

Векторизатор изображения имеет три области: Исходный, Квантованный и Векторизованный.

<b>Источник</b> — эта область содержит исходное растровое изображение для векторизации.

<b>Квантованный</b> — эта область содержит растровое изображение после применения цветового квантования. Квантование цвета — это процесс выбора ограниченного количества цветов для использования в изображении. Он применяется, когда информация о цвете изображения должна быть уменьшена. Квантование цвета — очень сложный процесс, включающий ряд факторов. Это может быть реализовано с помощью различных алгоритмов. Каждый из алгоритмов определяет, какие цвета из большего набора цветов остаются в новом изображении и как отброшенные цвета сопоставляются с оставшимися. <br>Вы можете вручную выбрать количество <b>цветов</b> и другие параметры квантования цвета на боковой панели.

<b>Vectorized</b> — эта область содержит векторизованное изображение и боковую панель настроек. Вы можете установить допуск, жесткость, натяжение и ширину линии. Дополнительные сведения о параметрах векторизации изображений см. в статье документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/image-vectorization- examples/" target="_blank">Примеры векторизации изображений.</a>

{{<section image-vectorization>}}
---
h2: Как векторизовать изображение с помощью C#
title: Код С# для преобразования изображения JPG в вектор
---

Преобразование изображения в вектор очень просто с <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/" target="_blank">Aspose.SVG для .NET API</a>. Пространство имен ImageVectorization включает классы и интерфейсы для реализации процесса векторизации изображения. В следующем фрагменте кода показано использование класса <a href="https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/" target="_blank">ImageVectorizer</a> для векторизовать изображение:

{{<section "code-image" i18n-exclude>}}

```cs       
	// Initialize an instance of the ImageVectorizer class
    var vectorizer = new ImageVectorizer
    {
        Configuration = 
		{
			// Set severity
			TraceSmoother =   new ImageTraceSmoother(3),
			// Set tolerance
			TraceSimplifier = new ImageTraceSimplifier(0.3f),
			// Set tension
        	PathBuilder = new PathBuilder(0.5f),
		}
    };
    // Vectorize image from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.jpg");
    // Save vectorized image as SVG file 
	document.Save(OutputFolder + "example.svg"));
```

{{<section link-image>}}

Вы можете узнать больше о векторизации изображений, перейдя по ссылке - <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/vectorization/image-to-svg/" >Изображение в SVG.</a>


{{<section text-vectorization>}}
---
title: Текст в вектор
h2: Как векторизовать текст в C#
title-code: Код С# для преобразования текста SVG в вектор
text: "Мы хотели бы поделиться с вами функцией векторизации текстовых элементов внутри документа SVG. Векторизация текста — это процесс преобразования текста в цифровую графику. В векторизованном тексте SVG все глифы шрифта заменяются комбинацией элементов `path`, `use`, `mask`, `g` и т. д. Таким образом, векторизация способствует защите текста от простого копирования, нежелательного использования, заимствования и модификация."
---

Если вас интересует разработка масштабируемой векторной графики и ее применение, взгляните на наш гибкий, высокоскоростной Aspose.SVG для .NET API с мощным набором интерфейсов для C# и других языков программирования .NET. Пространство имен <a href="https://reference.aspose.com/svg/net/aspose.svg.saving/" target="_blank">Aspose.Svg.Saving</a> включает <a href=" https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/" target="_blank">SVGSaveOptions</a>, который позволяет реализовать процесс векторизации текста. Чтобы векторизовать текст, установите для свойства `VectorizeText` класса SVGSaveOptions значение true:

{{<section "code-text" i18n-exclude>}}

```cs
// Load an SVG document from a file
var document = new SVGDocument("text.svg"));
// Set text elements vectorization 
var saveOptions = new SVGSaveOptions
{
    VectorizeText = true
};    
// Save the SVG document with specified saveOptions
document.Save("text_vectorized.svg", saveOptions);
```

{{<section link-text>}}

Вы можете узнать больше о векторизации текста, перейдя по ссылке - <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/vectorization/text-to-vector/" >Текст в вектор.</a>

{{<section installing>}}
---
h2: Установка библиотеки Aspose.SVG для .NET
---

<a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/" target="_blank">Aspose.SVG для .NET</a> — это кроссплатформенный гибкая библиотека, предназначенная для предоставления широкого спектра возможностей для обработки и рендеринга документов SVG. Он легко интегрируется в ваши приложения .NET для обработки и рендеринга файлов SVG без установки какого-либо стороннего программного обеспечения для моделирования или рендеринга. Aspose.SVG для .NET предлагает разработчикам работать с DOM, полностью совместимым с официальными спецификациями SVG. Наш API можно использовать с любым языком .NET, таким как C#, VB.NET, ASP.NET и т. д. Он одинаково хорошо работает на любой ОС, которая может установить Mono (поддержка .NET 4.0 Framework) или использовать ядро ​​.NET. Сюда входят Windows, Linux и macOS.

Установка <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG для .NET через NuGet</a>:
1. Использование консоли диспетчера пакетов. Откройте Microsoft Visual Studio и консоль диспетчера пакетов из меню, чтобы открыть консоль диспетчера пакетов. Затем введите команду «Install-Package Aspose.SVG» и нажмите Enter для установки.
2. Использование графического интерфейса диспетчера пакетов NuGet. Откройте Microsoft Visual Studio и Управление пакетами NuGet из меню, чтобы открыть диспетчер пакетов. Найдите «Aspose.SVG», выберите и нажмите «Установить». </br>



Дополнительные сведения об установке библиотеки C# см. в [Документация Aspose.SVG.](https://docs.aspose.com/svg/net/getting-started/installation/)

{{<section other-vectorizers>}}
---
h2: Другие поддерживаемые векторизаторы
---

Вы можете конвертировать изображение в вектор — поддерживаются форматы JPG, PNG, BMP, GIF, TIFF и ICO: