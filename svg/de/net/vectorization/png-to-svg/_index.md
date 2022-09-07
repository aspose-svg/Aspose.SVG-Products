---
translation: true
template: /templates/_template-vectorization-child.md
title: PNG vektorisieren - C#-Code und Online-Vektorisierer
description: Konvertieren Sie PNG in SVG in C#. Vektorisieren Sie PNG und nutzen Sie alle Vorteile von Vektorgrafiken. Probieren Sie Online Image Vectorizer kostenlos aus!
url: /net/vectorization/png-to-svg/
family: svg
platformtag: net
feature: vectorization
informat: PNG
outformat: SVG
---

{{<section banner>}}
---
h1: PNG zu Vektor - C#-Code und Online-Vektorisierer
h2: Konvertieren Sie PNG online oder programmgesteuert in das SVG-Format.
---

{{<section overview>}}
---
h2: Vektorisierung von PNG-Bildern
---

Die Bildvektorisierung ist der Prozess der Umwandlung von Bitmap-Bildern in Vektorgrafiken – Bezier-Kurven, Splines und Linien. Sie können Bitmaps aus verschiedenen Gründen vektorisieren - Skalierung, kleine Dateigröße, Animationsunterstützung usw. - oder Sie möchten einfach nur mit Bildern experimentieren und ein paar lustige Vektorisierungseffekte erzielen. In jedem Fall ist die Bitmap-Vektorisierung eine gute Erfahrung, wenn Sie sich für Fotografie, Malerei, Design, Kunst und Webentwicklung interessieren.<br>
[Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) bietet eine Hochgeschwindigkeits-C#-Bibliothek, die Sie für verschiedene SVG-Parsing-Aufgaben verwenden können . Der Namespace [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) enthält Klassen und Schnittstellen zur Implementierung des Bildvektorisierungsprozesses. In diesem Artikel sehen wir uns an, wie Sie Bilder in C# in Vektorgrafiken konvertieren oder einen Online-Bildvektorisierer verwenden.

{{<section input-file>}}
---
title: Was ist das PNG-Dateiformat?
---

{{<section output-file>}}
---
title: Was ist das SVG-Dateiformat?
---

{{<section plagin-text>}}
---
h2: Online-Bildvektorisierer
---

Wenn Sie Bilder vektorisieren müssen, verwenden Sie unser kostenloses Online-Tool! Image Vectorizer unterstützt JPEG, JPG, PJP, PJPEG, PNG, BMP, ICO, GIF, TIFF, WEBP, XBM und andere Bitmap-Formate. Es bietet verschiedene Optionen zur Vorverarbeitung von Bitmaps, bevor sie im SVG-Format gespeichert werden. Wandeln Sie Ihre Bilder jetzt in skalierbare und klare Vektorgrafiken um!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Konvertieren Sie PNG in SVG in C#
---

Aspose.SVG für die .NET-API bietet Klassen und Methoden, mit denen Sie den Bildvektorisierungsprozess implementieren und mit verschiedenen Vorverarbeitungsoptionen für Bilder arbeiten können, bevor Sie sie im Vektorformat speichern. Die Verarbeitung umfasst die Steuerung der folgenden Vektorisierungsoptionen: TraceSimplifier, TraceSmoother, PathBuilder usw.

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
    // Vectorize PNG from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.png");
    // Save vectorized PNG as SVG file 
	document.Save(OutputFolder + "image.svg"));
```

{{<section steps>}}
---
h2: So vektorisieren Sie PNG in C#
title: Schritte zum Konvertieren von PNG in SVG in C#
---

Um ein PNG-Bild mit Aspose.SVG zu vektorisieren, sollten Sie einige Schritte befolgen:
1. Initialisieren Sie eine Instanz der Klasse [ImageVectorizer.](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/) Verwenden Sie einen der ImageVectorizer()-Konstruktoren und geben Sie Konfigurationseigenschaften an.
    - Die Eigenschaft [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) stellt die Spur glatter ein. Es wird verwendet, um Fragmente von Konturen zu glätten.
    - Die Eigenschaft [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) legt die Ablaufverfolgung vereinfacht fest. Als Ergebnis wird die Spurkurve aus Liniensegmenten mit weniger (oder größeren) Punkten aufgebaut.
    - Die Eigenschaft [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) legt den Builder für SVG-Pfadsegmente fest und beeinflusst, wie stark sich die Kurve an den Kontrollpunkten krümmt.
1. PNG aus der angegebenen Datei vektorisieren. Die Methode [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) nimmt den Pfad zur Bilddatei und gibt ein SVGDocument zurück.
1. Speichern Sie das vektorisierte PNG als SVG. Verwenden Sie die Methode [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) und übergeben Sie ihr den Ausgabepfad.

{{<section documentation>}}

Im Dokumentationskapitel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Vectorization – Basic Overview </a> finden Sie Informationen zur Bildvektorisierung, eine Beschreibung des Bildvektorisierungsprozesses und der Vektorisierungsoptionen und erfahren, wie Sie Rasterbilder wie PNG, JPG, BMP, TIFF, GIF, ICO in ein SVG-Dokument vektorisieren. Sie werden einige C#-Beispiele betrachten, die die Funktionen von [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) und die Auswirkung von Konfigurationseigenschaften auf das Vektorisierungsergebnis demonstrieren.

{{<section other-vectorizers>}}
---
title: Andere unterstützte Vektorisierer
---