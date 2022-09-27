---
translation: true
template: /templates/_template-image-vectorization.md
title: Векторизация изображений — код C# и онлайн-векторизатор
description: Векторизация изображения онлайн или на C#! Преобразуйте изображение в векторный формат и получите все преимущества векторной графики! 
url: /net/image-vectorization/
family: svg
platformtag: net
feature: vectorization
informat: Image
outformat: SVG
---

{{<section banner>}}
---
h1: Векторизация растровых изображений
h2: Вы готовы перейти от пиксельного изображения к векторному?
---

{{<section overview>}}
---
h2: Что такое векторизация изображения?
---

Векторизация изображения — это процесс преобразования растровых изображений в векторную графику — кривые Безье, сплайны и линии. Векторизация полезна, потому что изображение не будет пикселизироваться, когда вы его увеличите. Масштабирование без потери качества, небольшой размер файла и поддержка анимации — это лишь некоторые преимущества векторных изображений. Занимаетесь ли вы живописью, дизайном, искусством, полиграфией, архитектурой или веб-разработкой, векторные изображения являются неотъемлемой частью вашей профессии. С другой стороны, вы просто можете поэкспериментировать с изображениями и получить забавные эффекты векторизации. В этой статье мы рассмотрим, как преобразовать изображение в векторную графику на C# или с помощью онлайн Векторизатора изображений.


{{<section plugin-text>}}
---
h2: Онлайн Векторизатор Изображений
---

Готовы ли вы перейти от рисования пикселями к рисованию векторами? Image Vectorizer предназначен для преобразования растровых изображений в векторную графику на основе геометрических фигур, состоящих из кривых и линий Безье. Все элементы векторной графики после векторизации сохраняются в файлы SVG. Image Vectorizer поддерживает JPEG, JPG, PJP, PJPEG, PNG, BMP, ICO, GIF, TIFF, WEBP, XBM и другие форматы растровых изображений. Вы можете интерактивно управлять векторизованным файлом SVG, используя элементы управления, связанные с соответствующими параметрами векторизации. Преобразуйте свои изображения в масштабируемые и четкие векторные картинки прямо сейчас!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Векторизация изображений на C#
---

 [Aspose.SVG для .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) предлагает высокоскоростную библиотеку C#, которую можно использовать для различных задач анализа SVG. Пространство имен [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) включает классы и интерфейсы для реализации процесса векторизации изображений и работы с различными параметрами их предварительной обработки перед сохранением в векторном формате. Обработка включает в себя управление следующими параметрами векторизации: TraceSimplifier, TraceSmoother, PathBuilder и т.д.

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
    // Vectorize image from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.png");
    // Save vectorized Image as SVG file 
	document.Save(OutputFolder + "image.svg");
```

{{<section steps>}}
---
h2: Как векторизовать изображение на C#
title: Шаги по векторизации изображения на C#
---
1. Инициализируйте экземпляр класса [ImageVectorizer.](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/) Используйте один из конструкторов ImageVectorizer() и укажите свойства конфигурации.
    - Свойство [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) делает трассировку более гладкой. Используется для сглаживания фрагментов контуров.
    - Свойство [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) упрощает трассировку. В результате кривая трассировки будет построена из отрезков с меньшим (или большим) числом точек.
    - Свойство [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) задает построитель сегментов пути SVG и влияет на то, насколько резко кривая изгибается в контрольных точках.
1. Векторизуйте изображение из указанного файла. Метод [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) берет путь к файлу изображения и возвращает SVGDocument.
1. Сохраните векторизованное изображение как файл SVG. Используйте метод [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) и передайте ему выходной путь.  

{{<section documentation>}}
---
h2: Векторизация изображений в документации
---

Масштабируемая векторная графика SVG в настоящее время широко используется для рендеринга веб-графики. По сравнению с растровыми изображениями, векторная графика может создавать четкие изображения, масштабируемые до любого размера, они идеально подходят для рисования любых веб-иллюстраций, включая значки, логотипы, диаграммы, схемы и многое другое. В главе документации [Vectorization - Basic Overview](https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/) вы найдете описание процесс векторизации изображений. <br>
- [Image Vectorization Workflow](https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/image-vectorization-workflow/) - Вы найдете информацию о векторизации изображения, описание процесса векторизации изображения и параметров векторизации, узнать, как векторизовать растровые изображения, такие как PNG, JPG, BMP, TIFF, GIF, ICO, в документ SVG.
- [Image Vectorization Examples](https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/image-vectorization-examples/) - Вы рассмотрите несколько примеров C# которые демонстрируют функциональные возможности пространства имен ImageVectorization и влияние свойств конфигурации на результат векторизации.

{{<section other-vectorizers>}}
---
title: Другие поддерживаемые Векторизаторы
subTitle: Сэкономьте свое время и воспользуйтесь Векторизаторами Изображений, чтобы получить все преимущества векторной графики!
---