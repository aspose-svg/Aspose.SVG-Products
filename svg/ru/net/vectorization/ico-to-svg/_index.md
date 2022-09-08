---
translation: true
template: /templates/_template-vectorization-child.md
title: Преобразование ICO в SVG — C# код и онлайн Векторизатор
description: Векторизация растрового изображения на C# или онлайн. Преобразуйте ICO в SVG и получите все преимущества векторной графики.
url: /net/vectorization/ico-to-svg/
family: svg
platformtag: net
feature: vectorization
informat: ICO
outformat: SVG
---

{{<section banner>}}
---
h1: Преобразование ICO в SVG — C# код и онлайн Векторизатор
h2: Векторизуйте изображения онлайн или программно.
---

{{<section overview>}}
---
h2: Векторизация изображения ICO
---

Векторизация изображения — это процесс преобразования растровых изображений в векторную графику — кривые Безье, сплайны и линии. Вы можете захотеть векторизовать растровые изображения по ряду причин — масштабирование, небольшой размер файла, поддержка анимации и т. д., или вы просто хотите поэкспериментировать с изображениями и получить забавные эффекты векторизации. В любом случае векторизация растровых изображений — это хороший опыт, если вы интересуетесь фотографией, живописью, дизайном, искусством и веб-разработкой.<br>
[Aspose.SVG для .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) предлагает высокоскоростную библиотеку C#, которую можно использовать для различных задач анализа SVG. . Пространство имен [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) включает классы и интерфейсы для реализации процесса векторизации изображения. В этой статье мы рассмотрим, как преобразовать ICO в векторную графику на C# с помощью API Aspose.SVG. Более того, мы предоставляем онлайн Векторизатор Изображений, чтобы вы могли попробовать преобразовать изображение в векторный формат в реальном времени.

{{<section input-file>}}
---
title: Что такое формат файла ICO?
---

{{<section output-file>}}
---
title: Что такое формат файла SVG?
---

{{<section plagin-text>}}
---
h2: Онлайн Векторизатор Изображений
---

Если вам нужно векторизовать изображения, воспользуйтесь нашим бесплатным онлайн-инструментом! Image Vectorizer поддерживает JPEG, JPG, PJP, PJPEG, PNG, BMP, ICO, GIF, TIFF, WEBP, XBM и другие форматы растровых изображений. Он предлагает различные варианты предварительной обработки растровых изображений перед их сохранением в формате SVG. Преобразуйте свои изображения в масштабируемые и четкие векторные изображения прямо сейчас!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Преобразование ICO в SVG на C#
---

Aspose.SVG для .NET API предоставляет классы и методы, позволяющие реализовать процесс векторизации изображения и работать с различными параметрами предварительной обработки изображений перед их сохранением в векторном формате. Обработка включает в себя управление следующими параметрами векторизации: TraceSimplifier, TraceSmoother, PathBuilder и т.д.

{{<section "code" i18n-exclude>}}

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
    // Vectorize ICO image from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.ico");
    // Save vectorized ICO as SVG file 
	document.Save(OutputFolder + "image.svg"));
```

{{<section steps>}}
---
h2: Как векторизовать ICO в C#
title: Шаги по преобразованию ICO в SVG на C#
---

Чтобы векторизовать изображение ICO с помощью Aspose.SVG, вам необходимо выполнить несколько шагов:
1. Инициализируйте экземпляр класса [ImageVectorizer](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/). Используйте один из конструкторов ImageVectorizer() и укажите свойства конфигурации.
    - Свойство [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) делает трассировку более гладкой. Используется для сглаживания фрагментов контуров.
    - Свойство [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) упрощает трассировку. В результате кривая трассировки будет построена из отрезков с меньшим (или большим) числом точек.
    - Свойство [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) задает построитель сегментов пути SVG и влияет на то, насколько резко кривая изгибается в контрольных точках.
1. Векторизировать ICO из указанного файла. Метод [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) берет в качестве параметра путь к файлу изображения и возвращает SVGDocument.
1. Сохраните векторизованное изображение ICO в виде файла SVG. Используйте метод Save() и передайте ему выходной путь.

{{<section documentation>}}

В главе документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Векторизация — базовый обзор </a> вы найдете информацию о векторизации изображения, описание процесса векторизации изображения и параметры векторизации, узнаете, как векторизовать растровые изображения, такие как PNG, JPG, BMP, TIFF, GIF, ICO, в документ SVG. Вы рассмотрите несколько примеров C#, которые демонстрируют функциональные возможности [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) и влияние свойств конфигурации на результат векторизации.

{{<section other-vectorizers>}}
---
title: Другие поддерживаемые векторизаторы
---