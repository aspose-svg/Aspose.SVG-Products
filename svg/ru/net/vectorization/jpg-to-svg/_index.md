﻿---
translation: true
template: /templates/_template-vectorization-child.md
title: Преобразование JPG в SVG — C# код и онлайн Векторизатор
description: Конвертация JPG в векторный формат на C#. Векторизуйте JPG и получите все преимущества векторной графики. Попробуйте онлайн Векторизатор!
url: /net/vectorization/jpg-to-svg/
family: svg
platformtag: net
feature: vectorization
informat: JPG
outformat: SVG
---

{{<section banner>}}
---
h1: Преобразование JPG в SVG — C# код и онлайн Векторизатор
h2: Векторизуйте изображение JPG онлайн или программно.
---

{{<section overview>}}
---
h2: Векторизация изображения JPG
---

Векторизация изображения — это процесс преобразования растровых изображений в векторную графику — кривые Безье, сплайны и линии. Векторизация полезна, потому что изображение не будет пикселизироваться, когда вы его увеличите. Масштабирование без потери качества, небольшой размер файла и поддержка анимации — это лишь некоторые преимущества векторных изображений. Занимаетесь ли вы живописью, дизайном, искусством, полиграфией, архитектурой или веб-разработкой, векторные изображения являются неотъемлемой частью вашей профессии. С другой стороны, вы просто можете поэкспериментировать с изображениями и получить забавные эффекты векторизации. [Aspose.SVG для .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) предлагает высокоскоростную библиотеку C#, которую можно использовать для различных задач анализа SVG. Пространство имен [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) включает классы и интерфейсы для реализации процесса векторизации изображения. В этой статье мы рассмотрим, как преобразовать изображение в векторную графику на C# или с помощью онлайн Векторизатора Изображений.

{{<section input-file>}}
---
title: Что такое формат файла JPG?
---

{{<section output-file>}}
---
title: Что такое формат файла SVG?
---

{{<section plagin-text>}}
---
h2: Онлайн Векторизатор Изображений
---

Если вам нужно векторизовать изображения, воспользуйтесь нашим бесплатным онлайн-инструментом! Image Vectorizer поддерживает JPEG, JPG, PJP, PJPEG, WEBP, PNG, BMP, ICO, GIF, TIFF, XBM и другие форматы растровых изображений. Выходное изображение представляет собой векторный файл формата SVG. Вы можете интерактивно управлять векторизованным файлом SVG, используя элементы управления, связанные с соответствующими параметрами векторизации. Преобразуйте свои изображения в масштабируемые и четкие векторные картинки прямо сейчас!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Преобразование JPG в SVG на C#
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
    // Vectorize JPG from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.jpg");
    // Save vectorized JPG image as SVG file 
	document.Save(OutputFolder + "image.svg");
```

{{<section steps>}}
---
h2: Как векторизовать JPG в C#
title: Шаги по преобразованию JPG в SVG на C#
---

Чтобы векторизовать JPG-изображение с помощью Aspose.SVG, выполните несколько шагов:
1. Инициализируйте экземпляр класса [ImageVectorizer.](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/) Используйте один из конструкторов ImageVectorizer() и укажите свойства конфигурации.
    - Свойство [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) делает трассировку более гладкой. Используется для сглаживания фрагментов контуров.
    - Свойство [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) упрощает трассировку. В результате кривая трассировки будет построена из отрезков с меньшим (или большим) числом точек.
    - Свойство [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) задает построитель сегментов пути SVG и влияет на то, насколько резко кривая изгибается в контрольных точках.
1. Векторизировать JPG из указанного файла. Метод [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) берет в качестве параметра путь к файлу изображения и возвращает SVGDocument.
1. Сохраните векторизованный JPG в SVG. Используйте метод [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) и передайте ему выходной путь.



{{<section documentation>}}

В главе документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Векторизация — базовый обзор </a> вы найдете информацию о векторизации изображения, описание процесса векторизации изображения и параметры векторизации, узнаете, как векторизовать растровые изображения, такие как PNG, JPG, BMP, TIFF, GIF, ICO, в документ SVG. Вы рассмотрите несколько примеров C#, которые демонстрируют функциональные возможности [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) и влияние свойств конфигурации на результат векторизации.

Aspose.SVG предлагает бесплатный онлайн [векторизатор изображений](https://products.aspose.app/svg/image-vectorization), позволяющий конвертировать растровые изображения JPG, PNG, BMP, TIFF, ICO и GIF в векторную графику. Используя это приложение, вы можете применить набор параметров для получения идеального результата. Сэкономьте свое время и воспользуйтесь этим векторизатором изображений, чтобы получить все преимущества векторной графики!

{{<section other-vectorizers>}}
---
title: Другие поддерживаемые векторизаторы
---