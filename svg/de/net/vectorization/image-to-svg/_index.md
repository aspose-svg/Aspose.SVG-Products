---
translation: true
template: /templates/_template-vectorization-child.md
title: Bild in SVG konvertieren – C#-Code und Online-Vektorisierer
description: Bild zu Vektor in C#. Konvertieren Sie Bilder in SVG und nutzen Sie alle Vorteile von Vektorgrafiken. Probieren Sie Online Image Vectorizer kostenlos aus!
url: /net/vectorization/image-to-svg/
family: svg
platformtag: net
feature: vectorization
informat: Image
outformat: SVG
---

{{<section banner>}}
---
h1: Bilder vektorisieren - C#-Code und Online-Vektorisierer
h2: Konvertieren Sie Bilder online oder programmgesteuert in das SVG-Format.
---

{{<section overview>}}
---
h2: Bildvektorisierung
---

Die Bildvektorisierung ist der Prozess der Umwandlung von Bitmap-Bildern in Vektorgrafiken – Bezier-Kurven, Splines und Linien. Die Vektorisierung ist hilfreich, da das Bild beim Vergrößern nicht verpixelt. Skalierung ohne Qualitätsverlust, geringe Dateigröße und Animationsunterstützung – das sind nur einige Vorteile von vektorisierten Bildern. Egal, ob Sie sich für Malerei, Design, Kunst, Druck, Architektur oder Webentwicklung interessieren, Vektorgrafiken sind ein wesentlicher Bestandteil des Berufs. Auf der anderen Seite können Sie einfach mit Bildern experimentieren und lustige Vektorisierungseffekte erzielen. [Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) bietet eine Hochgeschwindigkeits-C#-Bibliothek, die Sie für verschiedene SVG-Parsing-Aufgaben verwenden können . Der Namespace [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) enthält Klassen und Schnittstellen zur Implementierung des Bildvektorisierungsprozesses. In diesem Artikel sehen wir uns an, wie Sie Bilder in C# in Vektorgrafiken konvertieren oder einen Online-Bildvektorisierer verwenden.

{{<section input-file>}}
---
title: Was ist ein Bilddateiformat?
---

{{<section output-file>}}
---
title: Was ist das SVG-Dateiformat?
---

{{<section plagin-text>}}
---
h2: Online-Bildvektorisierer
---

Wenn Sie Bilder vektorisieren müssen, verwenden Sie unser kostenloses Online-Tool! Image Vectorizer unterstützt JPEG, JPG, PJP, PJPEG, PNG, BMP, ICO, GIF, TIFF, WEBP, XBM und andere Bitmap-Formate. Es bietet verschiedene Optionen zur Vorverarbeitung von Bitmaps, bevor sie im SVG-Format gespeichert werden. Sie können die vektorisierte SVG-Datei interaktiv verwalten, indem Sie Steuerelemente verwenden, die mit den richtigen Vektorisierungsoptionen verknüpft sind. Wandeln Sie Ihre Bilder jetzt in skalierbare und klare Vektorgrafiken um!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Bild in SVG in C# konvertieren
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
    // Vectorize image from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.png");
    // Save vectorized Image as SVG file 
	document.Save(OutputFolder + "image.svg"));
```

{{<section steps>}}
---
h2: So vektorisieren Sie Bilder in C#
title: Schritte zum Konvertieren von Bildern in SVG in C#
---

Um ein Bild mit Aspose.SVG zu vektorisieren, sollten Sie einige Schritte befolgen:
1. Initialisieren Sie eine Instanz der Klasse [ImageVectorizer.](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/) Verwenden Sie einen der ImageVectorizer()-Konstruktoren und geben Sie Konfigurationseigenschaften an.
    - Die Eigenschaft [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) stellt die Spur glatter ein. Es wird verwendet, um Fragmente von Konturen zu glätten.
    - Die Eigenschaft [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) legt die Ablaufverfolgung vereinfacht fest. Als Ergebnis wird die Spurkurve aus Liniensegmenten mit weniger (oder größeren) Punkten aufgebaut.
    - Die Eigenschaft [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) legt den Builder für SVG-Pfadsegmente fest und beeinflusst, wie stark sich die Kurve an den Kontrollpunkten krümmt.
1. Bild aus der angegebenen Datei vektorisieren. Die Methode [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) nimmt den Pfad zur Bilddatei und gibt ein SVGDocument zurück.
1. Speichern Sie das vektorisierte Bild als SVG-Datei. Verwenden Sie die Methode [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) und übergeben Sie ihr den Ausgabepfad.

{{<section documentation>}}

Im Dokumentationskapitel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Vectorization – Basic Overview </a> finden Sie Informationen zur Bildvektorisierung, eine Beschreibung des Bildvektorisierungsprozesses und der Vektorisierungsoptionen und erfahren, wie Sie Rasterbilder wie PNG, JPG, BMP, TIFF, GIF, ICO in ein SVG-Dokument vektorisieren. Sie werden einige C#-Beispiele betrachten, die die Funktionen von [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) und die Auswirkung von Konfigurationseigenschaften auf das Vektorisierungsergebnis demonstrieren.<br>
Aspose.SVG bietet einen kostenlosen Online-[Image Vectorizer](https://products.aspose.app/svg/image-vectorization) an, mit dem Sie JPG-, PNG-, BMP-, TIFF-, ICO- und GIF-Bitmap-Bilder in Vektorgrafiken konvertieren können. Mit dieser App können Sie eine Reihe von Optionen anwenden, um das perfekte Ergebnis zu erzielen. Sparen Sie Zeit und testen Sie diesen Image Vectorizer, um alle Vorteile von Vektorgrafiken zu nutzen!

{{<section other-vectorizers>}}
---
title: Andere unterstützte Vektorisierer
---