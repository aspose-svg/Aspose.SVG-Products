---
translation: true
template: /templates/_template-vectorization.md
title: Bild oder Text vektorisieren – C#-Code und Online-Vektorisierer
url: /net/vectorization/
description: Konvertieren Sie Bilder oder SVG-Text in Vektorgrafiken und speichern Sie die Ausgabe im SVG-Format. Online oder in C# vektorisieren!
---

{{<section banner>}}
---
h1: Bild oder Text in C# vektorisieren
h2: Bild in C# in Vektor umwandeln. JPG, JPEG, PNG, BMP, GIF, TIFF, ICO, IFIF, WEBP und andere Bitmap-Formate werden unterstützt.
---

{{<section overview>}}
---
title: Bildvektorisierung
---

Ein Rasterbild ist eine Abbildung von Pixeln – Punkten oder Körnern – auf Film, Papier oder Bildschirm. Jedes Pixel hat seine eigene Farbe. Das Skalieren eines Rasterbildes führt zu Rauschen und Unschärfen, die darauf erscheinen. Um solche Artefakte zu vermeiden, können Sie ein Bitmap-Bild in ein Vektorformat umwandeln, beispielsweise in eine SVG-Grafik. Die Bildvektorisierung ist eine Möglichkeit, ein Bild in Vektorform darzustellen. Ein Vektorbild basiert auf einer Formel – es basiert nicht auf Pixeln, sondern auf Grundelementen wie Punkten, Linien, Kurven, die durch mathematische Ausdrücke dargestellt werden. Linien und gefüllte farbige Bereiche in solchen Bildern werden als mathematische Kurven dargestellt, die durch kartesische Punkte definiert sind, die durch Pfade verbunden sind, um sie zu bilden. Ein Vektorbild hat alle Vorteile von Vektorgrafiken und wird beim Skalieren nicht verpixelt.
 
Sie können Bilder mit Aspose.SVG für die .NET-API in Echtzeit vektorisieren. Probieren Sie unseren kostenlosen Image Vectorizer aus und konvertieren Sie Pixelfarbinformationen in einfache geometrische Objekte! Bitte wählen Sie ein Bild zum Vektorisieren aus. JPG, JPEG, PJP, PJPEG, PNG, BMP, XBM, GIF, TIFF, ICO, IFIF, WEBP und andere Bitmap-Formate werden unterstützt.

{{<section "app-pluging" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}}

{{<section plugin-use>}}
---
h2: Wie verwende ich den Bildvektorisierer?
---

Der Image Vectorizer hat drei Bereiche: Source, Quantized und Vectorized.

<b>Source</b> - dieser Bereich enthält das Quell-Rasterbild für die Vektorisierung.

<b>Quantized</b> - dieser Bereich enthält ein Rasterbild nach Anwendung der Farbquantisierung. Die Farbquantisierung ist ein Prozess zur Auswahl einer begrenzten Anzahl von Farben, die in einem Bild verwendet werden sollen. Es wird angewendet, wenn die Farbinformationen eines Bildes reduziert werden sollen. Die Farbquantisierung ist ein sehr komplexer Prozess, an dem eine Reihe von Faktoren beteiligt sind. Dies kann unter Verwendung verschiedener Algorithmen implementiert werden. Jeder der Algorithmen bestimmt, welche Farben aus dem größeren Farbsatz im neuen Bild verbleiben und wie die verworfenen Farben den verbleibenden zugeordnet werden. <br>Sie können die Anzahl der <b>Farben</b> und andere Farbquantisierungseinstellungen in der Seitenleiste manuell auswählen.

<b>Vectorized</b> - dieser Bereich enthält das vektorisierte Bild und eine Seitenleiste mit Einstellungen. Sie können Werte für Toleranz, Schweregrad, Spannung und Linienbreite festlegen. Weitere Einzelheiten zu Bildvektorisierungsoptionen finden Sie im Dokumentationsartikel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/image-vectorization-examples/" target="_blank">Beispiele für die Vektorisierung von Bildern.</a>

{{<section image-vectorization>}}
---
h2: So vektorisieren Sie Bilder mit C#
title: C#-Code zum Konvertieren von JPG-Bildern in Vektoren
---

Das Konvertieren eines Bildes in einen Vektor ist mit <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/" target="_blank">Aspose.SVG for .NET API</a> sehr einfach. Der ImageVectorization-Namespace enthält Klassen und Schnittstellen zum Implementieren eines Bildvektorisierungsprozesses. Das folgende Code-Snippet demonstriert die Verwendung der <a href="https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/" target="_blank">ImageVectorizer</a>-Klasse ein Bild vektorisieren:

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
	document.Save(OutputFolder + "example.svg");
```

{{<section link-image>}}

Sie können mehr über Bildvektorisierung erfahren, indem Sie auf den Link <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/vectorization/image-to-svg/"> klicken Bild in SVG.</a>

{{<section text-vectorization>}}
---
title: Text zu Vektor
h2: So vektorisieren Sie Text in C#
title-code: C#-Code zum Konvertieren von SVG-Text in Vektor
text: "Wir möchten Ihnen eine Funktion zum Vektorisieren von Textelementen in einem SVG-Dokument vorstellen. Textvektorisierung ist der Prozess der Umwandlung von Text in digitale Grafiken. Im vektorisierten SVG-Text werden alle Font-Glyphen durch die Kombination aus `path`, `use`, `mask`, `g`-Elementen usw. ersetzt. Somit fördert die Vektorisierung den Textschutz vor einfachem Kopieren, unerwünschter Verwendung, Ausleihe und Änderung."
---

Falls Sie an der Entwicklung skalierbarer Vektorgrafiken und deren Anwendung interessiert sind, werfen Sie einen Blick auf unser flexibles, schnelles Aspose.SVG für .NET-API mit einem leistungsstarken Satz von Schnittstellen für C# und andere .NET-Programmiersprachen. Der Namespace <a href="https://reference.aspose.com/svg/net/aspose.svg.saving/" target="_blank">Aspose.Svg.Saving</a> enthält den <a href=" https://reference.aspose.com/svg/net/aspose.svg.saving/svgsaveoptions/" target="_blank">SVGSaveOptions</a>-Klasse, mit der Sie den Textvektorisierungsprozess implementieren können. Um Text zu vektorisieren, setzen Sie die Eigenschaft `VectorizeText` der Klasse SVGSaveOptions auf true:

{{<section "code-text" i18n-exclude>}}

```cs
// Load an SVG document from a file
var document = new SVGDocument("text.svg");
// Set text elements vectorization 
var saveOptions = new SVGSaveOptions
{
    VectorizeText = true
};    
// Save the SVG document with specified saveOptions
document.Save("text_vectorized.svg", saveOptions);
```

{{<section link-text>}}

Sie können mehr über die Textvektorisierung erfahren, indem Sie auf den Link <a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/vectorization/text-to-vector/"> klicken Text zu Vektor.</a>

{{<section installing>}}
---
h2: Aspose.SVG für die .NET-Bibliothek installieren
---

<a href="https://products.aspose.com/svg/{{lang.url-fragment}}net/" target="_blank">Aspose.SVG for .NET</a> ist plattformübergreifend flexible Bibliothek, die entwickelt wurde, um eine Vielzahl von Funktionen zum Verarbeiten und Rendern von SVG-Dokumenten bereitzustellen. Es lässt sich nahtlos in Ihre .NET-Apps integrieren, um die Verarbeitung und das Rendern von SVG-Dateien zu ermöglichen, ohne Modellierungs- oder Rendering-Software von Drittanbietern zu installieren. Aspose.SVG für .NET bietet Entwicklern die Möglichkeit, mit seinem DOM zu arbeiten, das vollständig mit den offiziellen SVG-Spezifikationen kompatibel ist. Unsere API kann mit jeder .NET-Sprache wie C#, VB.NET, ASP.NET usw. verwendet werden. Sie funktioniert gleichermaßen gut auf jedem Betriebssystem, das Mono (.NET 4.0 Framework-Unterstützung) installieren oder .NET Core verwenden kann. Dazu gehören Windows, Linux und macOS.

Installieren von <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG for .NET über NuGet</a>:
1. Verwenden der Paket-Manager-Konsole. Öffnen Sie Microsoft Visual Studio und die Paket-Manager-Konsole über das Menü, um die Paket-Manager-Konsole zu öffnen. Geben Sie dann den Befehl „Install-Package Aspose.SVG“ ein und drücken Sie die Eingabetaste, um zu installieren.
2. Verwenden der NuGet Package Manager-GUI. Öffnen Sie Microsoft Visual Studio und verwalten Sie NuGet-Pakete aus dem Menü, um den Paket-Manager zu öffnen. Suchen Sie nach "Aspose.SVG", wählen Sie es aus und klicken Sie auf "Installieren". </br>



Weitere Einzelheiten zur Installation der C#-Bibliothek finden Sie in der [Aspose.SVG-Dokumentation.](https://docs.aspose.com/svg/net/getting-started/installation/)

{{<section other-vectorizers>}}
---
h2: Andere unterstützte Vektorisierer
---

Sie können Bilder in Vektoren konvertieren – JPG-, PNG-, BMP-, GIF-, TIFF- und ICO-Formate werden unterstützt: