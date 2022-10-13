---
translation: true
template: /templates/_template-vectorization-child.md
title: Трафаретирование изображений — код C# и онлайн-конструктор трафаретов
description: Преобразуйте изображение в SVG и примените преобразование трафарета в C#. Векторизация и трафаретная обработка изображений и использование всех преимуществ векторной графики. Попробуйте онлайн-конструктор трафаретов бесплатно!
url: /net/vectorization/stencil/
family: svg
platformtag: net
feature: vectorization, stencil
informat: Image
outformat: SVG
---

{{<section banner>}}
---
h1: Рисунок на станке — код C# и Stencil Maker
h2: Создавайте стандартные изображения онлайн или программно.
---

{{<section overview>}}
---
h2: Что такое трафарет изображения?
---

Трафаретное изображение — это процесс, который превращает обычную фотографию в контурное изображение, которое можно использовать в качестве трафарета для создания эффектов, подобных граффити.

Есть несколько основных шагов для превращения фотографии или изображения в трафарет:
* Преобразование фотографии или изображения в оттенки серого. Этот шаг не является обязательным, так как вместо этого вы можете уменьшить количество цветов для квантизации.
* Квантизируйте изображение, чтобы получить шаблон, после чего вы можете загрузить результат или векторизовать его и получить линии формы шаблона.
* Есть три варианта рисования трафаретов. Первое — «Нет», когда все векторизованные фигуры залиты, второе — «Авто», когда фигуры не залиты и границы имеют «исходный» цвет, и последнее — «Моноцвет», когда фигуры тоже не залиты , но границы имеют предопределенный цвет.


<br>
[Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) offers a high-speed C# library that you can use for different SVG parsing tasks. The [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) Namespace includes classes and interfaces for implementing the image vectorization process with stenciling options.

{{<section input-file>}}
---
title: Что такое формат файла изображения?
---

{{<section output-file>}}
---
title: Что такое формат файла SVG?
---

{{<section plagin-text>}}
---
h2: Онлайн-конструктор трафаретов
---

Если вам нужно превратить ваши фотографии или изображения в трафареты, воспользуйтесь нашим бесплатным онлайн-инструментом! Он позволяет не только получать растровые трафареты, но и векторизовать их и работать с масштабируемыми и четкими векторами. Stencil Maker поддерживает JPEG, JPG, PJP, PJPEG, PNG, BMP, ICO, GIF, TIFF, WEBP, XBM и другие форматы растровых изображений!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image" sourceImage="/svg/images/vectorization/fish.png" colors="3" scale="1" grayscale="true" stencil="monocolor" extent="1" stencilColor="#00ff00">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Преобразование PNG в SVG на C#
---

Aspose.SVG для .NET API предоставляет классы и методы, которые позволяют реализовать процесс векторизации изображения и работать с параметрами трафарета.

{{<section "code" i18n-exclude>}}

```cs       
	// Initialize an instance of the ImageVectorizer class
	var vectorizer = new ImageVectorizer
    {
		//optionally set configuration
        Configuration =
        {
			//optionally set path builder
            PathBuilder = new BezierPathBuilder {
			//optionally set trace smoother
            TraceSmoother = new ImageTraceSmoother(1),
                ErrorThreshold =  30,
                MaxIterations = 30
            },
            ColorsLimit = 10,
            LineWidth = 1,
            Stencil = new StencilConfiguration { Type = StencilType.MonoColor, Color = Aspose.Svg.Drawing.Color.FromRgb(0,0,255) }
        }
    };
    // Vectorize PNG from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.png");
    // Save vectorized PNG as SVG file 
	document.Save(OutputFolder + "image.svg");
```

{{<section steps>}}
---
h2: Как векторизовать PNG в C#
title: Шаги по преобразованию PNG в SVG на C#
---

Чтобы векторизовать PNG-изображение с помощью Aspose.SVG, выполните несколько шагов:
1. Инициализируйте экземпляр класса [ImageVectorizer](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/). Используйте один из конструкторов ImageVectorizer() и укажите свойства конфигурации.
    - Свойство [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) получает или задает построитель сегментов пути SVG.
    - Свойство [ColorsLimit](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/colorslimit/) получает или устанавливает максимальное количество цветов, используемых для квантования изображения.
    - Свойство [Трафарет](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/stencil/) получает или устанавливает конфигурацию эффекта трафарета. По умолчанию эффект трафарета не применяется.
1. Оцифровать изображение из указанного файла. Метод [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) берет путь к файлу изображения и возвращает SVGDocument.
1. Сохраните векторизованный PNG в SVG. Используйте метод [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) и передайте ему выходной путь.



{{<section documentation>}}

В главе документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Векторизация — базовый обзор </a> вы найдете информацию о векторизации изображения, описание процесса векторизации изображения и параметры векторизации, узнаете, как векторизовать растровые изображения, такие как PNG, JPG, BMP, TIFF, GIF, ICO, в документ SVG. Вы рассмотрите несколько примеров C#, которые демонстрируют функциональные возможности [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) и влияние свойств конфигурации на результат векторизации.

{{<section other-vectorizers>}}
---
title: Другие поддерживаемые векторизаторы
---