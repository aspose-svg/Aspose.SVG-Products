---
translation: true
template: /templates/_template-net.md
title: C# API синтаксического анализа файлов SVG — Aspose
weight: 20
url: /net/
description: C# библиотека для загрузки файлов SVG, чтения и обхода элементов, преобразования SVG в форматы PDF, XPS и изображения.
---

{{<section banner>}}
---
h1: C# API для анализа файлов SVG
h2: Создавайте, загружайте, анализируйте, визуализируйте и конвертируйте файлы SVG в популярные форматы без каких-либо программных зависимостей.
---

{{<section overview>}}
---
item1: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/creating-loading-documents/" target="_blank">Создание или загрузка SVG документов</a> из файла, URL, строки, потока и т. д.
item2: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">Преобразование SVG</a> в PDF , PNG и другие популярные форматы.
item3: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Векторизация растровых изображений</a>, например PNG, JPG, BMP, TIFF, GIF и ICO в документ SVG.
item4: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/navigation-inspection/" target="_blank">Навигация по документам SVG</a > используя функции XPath Query, CSS Selector, Element и Document Traversal.
item5: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-edit-svg-documents/" target="_blank"> Редактирование файлов SVG</a>, добавляя новые узлы, удаляя или редактируя содержимое существующих узлов.
item6: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target="_blank"> Отрисовка документов SVG</a> с высоким качеством.
item7: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/text-vectorization/" target="_blank">Векторизация текста SVG</a > с профессиональным качеством и разрешением и многое другое.
---

Aspose.SVG для .NET — это гибкая библиотека для обработки файлов SVG, полностью совместимая с ее спецификациями. API может легко загружать, сохранять и преобразовывать файлы SVG, а также читать и просматривать элементы файлов через объектную модель документа (DOM). API не зависит от какого-либо другого программного обеспечения и позволяет разработчикам работать с файлами SVG, не вникая в основные детали формата.<br><br>
Использование библиотеки C# Aspose.SVG в вашем проекте позволяет выполнять следующие задачи:

{{<section glance>}}
---
h3: С одного взгляда
description: Обзор Aspose.SVG для .NET API.
---

{{<section platform>}}
---
h3: Независимость от платформы
description: "Aspose.SVG для .NET поддерживает все основные платформы, в том числе:"
---

{{<section formats>}}
---
h3: Поддерживаемые форматы файлов
description: Aspose.SVG для .NET поддерживает все популярные форматы файлов изображений и многое другое.
---

{{<section feature>}}
---
title: Расширенные функции Aspose.SVG for .NET API
feature1: Создание и чтение документов SVG
feature2: Редактирование и сохранение SVG файлов
feature3: <a href="/svg/{{lang.url-fragment}}net/conversion/">Преобразование SVG в популярные форматы</a>
feature4: Полный контроль над узлами SVG
feature5: <a href="/svg/{{lang.url-fragment}}net/color-converter/">Преобразование цветовых кодов</a>
feature6: Изменение свойств узла
feature7: Навигация по содержимому с использованием XPath Query
feature8: Навигация с помощью селекторов CSS, обхода элементов и документов
feature9: Манипуляции DOM Tree согласно официальным спецификациям SVG
---

{{<section converter>}}
---
h2: Преобразование SVG в другие форматы файлов
h3: Преобразование SVG в PNG — C#
---
   
Aspose.SVG для .NET может читать и преобразовывать SVG в PDF, XPS и основные форматы изображений. Процесс преобразования прост и надежен, что делает SVG .NET API идеальным выбором. Вы можете использовать API в своем C# или любом другом приложении .NET для разработки приложений-конвертеров, не вдаваясь в подробности базовых форматов файлов. Получить функциональность преобразования просто и зависит от требований каждого приложения. Вот несколько строк кода для преобразования между форматами.


{{<section "code" i18n-exclude>}}
     
using Aspose.Svg;
using System.IO;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;
...
    
    // Initialize an SVG document from a file
    using (var document = new SVGDocument("input.svg"))
    {
    	// Create an instance of the ImageSaveOptions class
    	var pngSaveOptions = new ImageSaveOptions();    
    
        // Convert SVG to PNG
    	Converter.ConvertSVG(document, pngSaveOptions, "output.png");
    }

{{<section online-converters>}}

Вы можете попробовать онлайн Конвертер SVG перейдя по <a href="https://products.aspose.app/svg/conversion/svg" target="_blank">ссылке</a>.

{{<section other-converters>}}

Другие поддерживаемые преобразования SVG:

{{<section image-vector>}}
---
h2: Преобразование растрового изображения в векторную графику
h3: Преобразование изображения в вектор — C#
---

Конвертировать растровое изображение в векторную графику очень просто с помощью Aspose.SVG API. Пространство имен <a href="https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/" target="_blank">ImageVectorization</a> включает классы и интерфейсы для реализации процесса векторизации изображения. Следующий фрагмент кода демонстрирует использование класса ImageVectorizer для векторизации изображения:

{{<section "code-image" i18n-exclude>}}
     
using Aspose.Svg.ImageVectorization;
using Aspose.Svg.Saving;
...
    
	// Initialize an instance of the ImageVectorizer class
	var vectorizer = new ImageVectorizer
	{
		Configuration = 
		{
			TraceSmoother =   new ImageTraceSmoother(1),
			TraceSimplifier = new ImageTraceSimplifier(0.5f),
			ColorsLimit = 3
		}
	};
	
	// Vectorize raster image from the specified file
	using var document = vectorizer.Vectorize("input.png");
	
	// Save vectorized image as SVG file 
	document.Save("output.svg");

{{<section merge>}}
---
h2: Объединить несколько SVG файлов используя C#
h3: Объединить SVG в PDF — C#
---	
	
Метод Renderer() дает вам возможность одновременно отправлять несколько документов на выходное устройство рендеринга и объединять их. Слияние документов можно выполнить с помощью нескольких строк кода:

{{<section "code-merge" i18n-exclude>}}
     
using Aspose.Svg;
using Aspose.Svg.Rendering;
using Aspose.Svg.Rendering.Pdf;
...   
	
	// Initialize SVG documents from files to merge later
	using (var document1 = new SVGDocument("input1.svg"))
	using (var document2 = new SVGDocument("input2.svg"))
	using (var document3 = new SVGDocument("input3.svg"))
	{
		// Create an instance of SvgRenderer
		using (var renderer = new SvgRenderer())
		{
			// Create an instance of PdfDevice
			using (var device = new PdfDevice("output.pdf"))
			{
				// Merge all SVG documents to PDF
				renderer.Render(device, document1, document2, document3);
			}
		}
	}

{{<section other-mergers>}}	

Другие поддерживаемые Объединения: