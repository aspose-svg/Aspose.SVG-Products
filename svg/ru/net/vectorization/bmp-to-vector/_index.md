---
translation: true
template: /templates/_template-vectorization-child.md
title: Vectorize BMP — код C# и онлайн-векторизатор
description: BMP в вектор на C#. Конвертируйте BMP в SVG и получите все преимущества векторной графики. Попробуйте онлайн векторизатор изображений бесплатно!
url: /net/vectorization/bmp-to-svg/
family: svg
platformtag: net
feature: vectorization
informat: BMP
outformat: SVG
---

{{<section banner>}}
---
h1: BMP to Vector — код C# и онлайн-векторизатор
h2: Конвертируйте векторный формат BMP в SVG онлайн или программно.
---

{{<section overview>}}
---
h2: Векторизовать растровое изображение
---

Под векторизацией мы подразумеваем процесс замены растровых изображений математическими кривыми и геометрическими фигурами, составленными из элементов пути и сохраненными в формате SVG. Вы можете захотеть векторизовать растровые изображения по ряду причин. У векторной графики есть ряд преимуществ: масштабирование, небольшой размер файла, поддержка анимации и т. д., или вы просто хотите поэкспериментировать с изображениями и получить забавные эффекты векторизации. В любом случае векторизация растровых изображений — это хороший опыт, если вы интересуетесь фотографией, живописью, дизайном, искусством и веб-разработкой.<br>
[Aspose.SVG для .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) предлагает высокоскоростную библиотеку C#, которую можно использовать для различных задач анализа SVG. . Пространство имен [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) включает классы и интерфейсы для реализации процесса векторизации изображения. В этой статье мы рассмотрим, как конвертировать BMP в векторную графику на C# с помощью Aspose.SVG API. Более того, мы предоставляем онлайн-векторизатор изображений, чтобы вы могли попробовать преобразовать изображение в вектор в реальном времени.

{{<section input-file>}}
---
title: Что такое формат файла BMP?
---

{{<section output-file>}}
---
title: Что такое формат файла SVG?
---

{{<section plagin-text>}}
---
h2: Онлайн векторизатор изображений
---

Если вам нужно векторизовать изображения, воспользуйтесь нашим бесплатным онлайн-инструментом! Image Vectorizer поддерживает форматы JPG, PNG, BMP, ICO, GIF и TIFF. Он предлагает различные варианты предварительной обработки растровых изображений перед их сохранением в формате SVG. Преобразуйте свои изображения в масштабируемые и четкие векторные изображения прямо сейчас!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="JPG">}}

{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Преобразование BMP в SVG на C#
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
    // Vectorize BMP from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.bmp");
    // Save vectorized BMP image as SVG file 
	document.Save(OutputFolder + "image.svg"));
```

{{<section steps>}}
---
h2: Как векторизовать BMP в C#
title: Шаги по преобразованию BMP в SVG на C#
---

Чтобы векторизовать BMP с помощью Aspose.SVG, вы должны выполнить несколько шагов:
1. Инициализируйте экземпляр класса [ImageVectorizer](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/). Используйте один из конструкторов ImageVectorizer() и укажите свойства конфигурации.
    - Свойство [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) делает трассировку более гладкой. Используется для сглаживания фрагментов контуров.
    - Свойство [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) упрощает трассировку. В результате кривая трассировки будет построена из отрезков с меньшим (или большим) числом точек.
    - Свойство [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) задает построитель сегментов пути SVG и влияет на то, насколько резко кривая изгибается в контрольных точках.
1. Векторизировать BMP из указанного файла. Используйте метод [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/), который возвращает SVGDocument.
1. Сохраните векторизованное изображение BMP как файл SVG.



{{<section documentation>}}
---
h2: Основы векторизации в документации
---

 В главе документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Векторизация — базовый обзор </a> вы найдете информацию о векторизации изображения, описание процесса векторизации изображения и параметры векторизации, узнаете, как векторизовать растровые изображения, такие как PNG, JPG, BMP, TIFF, GIF, ICO, в документ SVG. Вы рассмотрите несколько примеров C#, которые демонстрируют функциональные возможности [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) и влияние свойств конфигурации на результат векторизации.

{{<section online-vectorizer>}}

Aspose.SVG предлагает бесплатный онлайн [векторизатор изображений](https://products.aspose.app/svg/image-vectorization), позволяющий конвертировать растровые изображения JPG, PNG, BMP, TIFF, ICO и GIF в векторную графику. Используя это приложение, вы можете применить набор параметров для получения идеального результата. Сэкономьте свое время и воспользуйтесь этим векторизатором изображений, чтобы получить все преимущества векторной графики!

{{<section other-vectorizers>}}
---
title: Другие поддерживаемые векторизаторы
---