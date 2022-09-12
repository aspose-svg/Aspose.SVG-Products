---
translation: true
template: /templates/_template-text-vectorization.md
title: Konvertieren Sie Text in Vektorpfade in C# - Aspose.SVG
description: Vektorisieren Sie Text in SVG-Dateien mit C#. Konvertieren Sie Text in Vektorgrafiken und speichern Sie ihn als SVG.
url: /net/vectorization/text-to-vector/
family: svg
platformtag: net
feature: vectorization
informat: SVG
outformat: SVG
---

{{<section banner>}}
---
h1: Text zu Vektor in C#
h2: Vektorisieren Sie Text in SVG-Dokumenten und speichern Sie ihn als Vektorgrafik
---

{{<section overview>}}
---
h2: Konvertieren Sie Text in Vektorpfade
---

Bei der Textvektorisierung wird Text in eine Vielzahl von Vektorpfaden und geometrischen Formen umgewandelt. Sie können verschiedene Schriftarten verwenden und diese dann in Vektorkonturen umwandeln, um Ihre eigenen Vektorschriftarten zu erstellen. Ein solcher Text wird zu einer Vektorzeichnung und kann nicht im Texteditor bearbeitet werden. Sie können die Vektorzeichen jedoch bearbeiten und anpassen, indem Sie die Elemente `<path>`, `<use>`, `<mask>`, `<g>` im SVG-Code manipulieren. Sie können „Filter“, „Maske“, „Deckkraft“ und andere Effekte auf den vektorisierten SVG-Text anwenden, indem Sie seine Eigenschaften wie Deckkraft, Lichteffekte usw. anpassen. Darüber hinaus können Sie Ränder, Striche, Schatten, Glühen und andere SVG-Aspekte, die Ihnen beim Entwerfen von Text helfen können. Sie können mit all diesen SVG-Funktionen spielen, um die besten Ergebnisse zu erzielen. Der vektorisierte Text, der Vektorgrafiken ist, ermöglicht die Verwendung von Schriftarten ohne Installation auf dem Client-Computer und behält seinen Stil bei, wenn er in einer beliebigen Computerumgebung verwendet wird. Daher ist die Konvertierung von Text in Vektorformen sehr hilfreich für die Verwendung in Logos, Symbolen, Bannern, Anzeigen usw.

[Aspose.SVG for .NET](https://products.aspose.com/svg/{{lang.url-fragment}}net/) API bietet die Funktion der Textvektorisierung in SVG-Dokumenten. Schauen Sie sich unsere C#-Bibliothek an, damit Sie SVG-Text ganz einfach in Vektorgrafiken umwandeln können!

{{<section code-text>}}
---
h2: C#-Codebeispiel zum Vektorisieren von Text in einem SVG-Dokument
title: Text in Vektor umwandeln – C#
---

Im vektorisierten SVG-Text werden alle Schriftzeichen durch eine Kombination von Grafikelementen ersetzt. Aspose.SVG for .NET API bietet die Funktion zum Vektorisieren von Textelementen in SVG-Dokumenten. Um Text zu vektorisieren, setzen Sie die Eigenschaft [VectorizeText](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/vectorizetext/) der Klasse SVGSaveOptions auf „true“. Die Textvektorisierung kann mit ein paar Zeilen Code durchgeführt werden:

{{<section "code-snippet" i18n-exclude>}}

```cs
// Load an SVG document from a file
var document = new SVGDocument(InputFolder + "text.svg");
// Create a Save Options object 
var saveOptions = new SVGSaveOptions
{
    VectorizeText = true
};    
// Save the SVG document with specified saveOptions
document.Save((OutputFolder + "text-vectorized.svg"), saveOptions);
```

{{<section steps>}}
---
h2: Schritte zum Vektorisieren von SVG-Text in C#
---
1. Laden Sie ein SVG-Dokument mit einem der [SVGDocument()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/)-Konstruktoren.
1. Erstellen Sie eine neue Instanz der Klasse [SVGSaveOptions.](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/) Verwenden Sie den Konstruktor [SVGSaveOptions()](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/svgsaveoptions/) und legen Sie den [VectorizeText](https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/vectorizetext/) Eigenschaft als `true`. Es weist darauf hin, Textelemente durch Pfade zu ersetzen.
1. Rufen Sie die Methode [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_8) auf und übergeben Sie ihr den Ausgabepfad und das Objekt mit den Speicheroptionen.

{{<section documentation>}}

Im Dokumentationskapitel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Vectorization – Basic Overview </a> finden Sie Informationen zur Textvektorisierung, erfahren, wie Sie Text in einem SVG-Dokument vektorisieren, und betrachten C#-Beispiele. Im Dokumentationsartikel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/text-vectorization/" target="_blank">Textvektorisierung & Textsicherheit</a> kennen Sie die Vorteile der Textvektorisierung.

{{<section online-vectorizer>}}
---
h2: Online-Textvektorisierer
---

Aspose.SVG bietet eine kostenlose Online-App <a href="https://products.aspose.app/svg/text-to-vector" target="_blank">Text in Vektor</a>, die Text in eine SVG-Datei umwandelt in Vektorformen. Text to Vector funktioniert auf jedem Gerät und auf jeder Plattform. Für Sie ist keine Registrierung, Plugin- oder zusätzliche Softwareinstallation erforderlich. Wandeln Sie Ihren SVG-Text in einen Vektor um und nutzen Sie alle Vorteile von Vektorgrafiken!

{{<section other-vectorizers>}}
---
title: Andere unterstützte Vektorisierer
---