---
translation: true
template: /templates/_template-text-vectorization.md
title: Преобразование текста в векторные пути на C# - Aspose.SVG
description: Векторизация текста в файлах SVG с помощью C#. Преобразуйте текст в векторную графику и сохраните его в формате SVG.
url: /net/vectorization/text-to-vector/
family: svg
platformtag: net
feature: vectorization
informat: SVG
outformat: SVG
---

{{<section banner>}}
---
h1: Преобразование текста в векторную графику на C#
h2: Векторизуйте текст в документах SVG и сохраните его как векторные формы
---

{{<section overview>}}
---
h2: Преобразование текста в векторные контуры
---

Векторизация текста — это процесс преобразования текста в различные векторные контуры и геометрические формы. Вы можете использовать разные шрифты, а затем преобразовывать их в векторную графику, создавая свои собственные векторные шрифты. Такой текст становится векторным рисунком и не может быть отредактирован в текстовом редакторе. Но вы можете редактировать и настраивать векторные символы, манипулируя элементами `<path>`, `<use>`, `<mask>`, `<g>` в коде SVG. Вы можете применять «filter», «mask», «opacity» и другие эффекты к векторизованному тексту SVG, настраивая его функции, такие как непрозрачность, световые эффекты и т. д. В дополнение к этому вы можете преобразовывать границы, тени, свечение и другие аспекты SVG, которые могут помочь вам для оформления текста. Вы можете поиграть со всеми этими функциями SVG, чтобы получить наилучшие результаты. Векторизованный текст, являясь векторной графикой, позволяет использовать шрифты без установки на клиентский компьютер и сохраняет свой стиль при использовании в любой компьютерной среде. Преобразование текста в векторные формы очень полезно для использования в логотипах, значках, баннерах, рекламных объявлениях и т. д.

[Aspose.SVG for .NET](https://products.aspose.com/svg/{{lang.url-fragment}}net/) API предоставляет возможность векторизации текста в документах SVG. Воспользуйтесь нашей библиотекой C#, чтобы с легкостью преобразовывать текст SVG в векторную графику!

{{<section code-text>}}
---
h2: Пример кода C# для векторизации текста в документе SVG
title: Преобразование текста в векторную графику — C#
---

В векторизованном тексте SVG все глифы шрифта заменяются комбинацией графических элементов. Aspose.SVG для .NET API предоставляет возможность векторизации текстовых элементов в документах SVG. Чтобы векторизовать текст, установите для свойства [VectorizeText](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/vectorizetext/) класса SVGSaveOptions значение «true». Векторизацию текста можно выполнить с помощью нескольких строк кода:

{{<section "code-snippet" i18n-exclude>}}

```cs
// Load an SVG document from a file
var document = new SVGDocument("text.svg");
// Create a Save Options object 
var saveOptions = new SVGSaveOptions
{
    VectorizeText = true
};    
// Save the SVG document with specified saveOptions
document.Save("text-vectorized.svg", saveOptions);
```

{{<section steps>}}
---
h2: Шаги для векторизации текста SVG на C#
---
1. Загрузите документ SVG с помощью одного из конструкторов [SVGDocument().](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/)
1. Создайте новый экземпляр класса [SVGSaveOptions.](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/) Используйте конструктор [SVGSaveOptions()](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/svgsaveoptions/) и установите [VectorizeText](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/vectorizetext/) как «true». Он указывает на замену текстовых элементов графическими контурами - путями.
1. Вызовите метод [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_8) и передайте ему путь для сохранения результата векторизации и объект опций сохранения.

{{<section documentation>}}

В главе документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Векторизация — базовый обзор </a> вы найдете информацию о векторизации текста, узнаете, как векторизовать текст в документе SVG, и рассмотрите примеры C#. В статье документации <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/text-vectorization/" target="_blank">Векторизация текста & Безопасность текста</a>, вы узнаете о преимуществах векторизации текста.

{{<section online-vectorizer>}}
---
h2: Онлайн приложение для векторизации текста
---

Aspose.SVG предлагает бесплатное онлайн-приложение <a href="https://products.aspose.app/svg/text-to-vector" target="_blank">Текст в Вектор</a>, которое преобразует текст из файла SVG в векторные формы. Приложение Текст в Вектор работает с любого устройства, любой платформы. Для вас не требуется регистрация или установка дополнительного программного обеспечения. Векторизуйте текст SVG и получите все преимущества векторной графики!

{{<section other-vectorizers>}}
---
title: Другие поддерживаемые Векторизаторы
---