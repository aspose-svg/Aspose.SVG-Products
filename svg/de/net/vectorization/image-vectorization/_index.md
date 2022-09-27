---
translation: true
template: /templates/_template-image-vectorization.md
title: Bildvektorisierung – C#-Code und Online-Vektorisierer
description: Bild online oder in C# vektorisieren! Die Bildvektorisierung bietet Ihnen alle Vorteile von Vektorgrafiken. Probieren Sie Online Image Vectorizer kostenlos aus!
url: /net/image-vectorization/
family: svg
platformtag: net
feature: vectorization
informat: Image
outformat: SVG
---

{{<section banner>}}
---
h1: Bildvektorisierung – C#-Code und Online-Vektorisierer
h2: Sind Sie bereit, zum Vektorzeichnen überzugehen?
---

{{<section overview>}}
---
h2: Was ist Bildvektorisierung?
---

Die Bildvektorisierung ist der Prozess der Umwandlung von Bitmap-Bildern in Vektorgrafiken – Bezier-Kurven, Splines und Linien. Die Vektorisierung ist hilfreich, da das Bild beim Vergrößern nicht verpixelt. Skalierung ohne Qualitätsverlust, geringe Dateigröße und Animationsunterstützung – das sind nur einige Vorteile von vektorisierten Bildern. Egal, ob Sie sich für Malerei, Design, Kunst, Druck, Architektur oder Webentwicklung interessieren, Vektorgrafiken sind ein wesentlicher Bestandteil des Berufs. Auf der anderen Seite können Sie einfach mit Bildern experimentieren und lustige Vektorisierungseffekte erzielen. In diesem Artikel sehen wir uns an, wie Sie Bilder in C# in Vektorgrafiken konvertieren oder einen Online-Bildvektorisierer verwenden.


{{<section plugin-text>}}
---
h2: Online-Bildvektorisierer
---

Sind Sie bereit, vom Malen mit Pixeln zum Zeichnen mit Vektoren überzugehen? Image Vectorizer wurde entwickelt, um Rasterbilder in Vektorgrafiken umzuwandeln, die auf geometrischen Formen basieren, die aus Bezier-Kurven und -Linien bestehen. Alle Vektorgrafikelemente werden nach der Vektorisierung in SVG-Dateien gespeichert. Image Vectorizer unterstützt JPEG, JPG, PJP, PJPEG, PNG, BMP, ICO, GIF, TIFF, WEBP, XBM und andere Bitmap-Formate. Sie können die vektorisierte SVG-Datei interaktiv verwalten, indem Sie Steuerelemente verwenden, die mit den richtigen Vektorisierungsoptionen verknüpft sind. Wandeln Sie Ihre Bilder jetzt in skalierbare und klare Vektorgrafiken um!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image" sourceImage="/svg/images/vectorization/flower.png">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Bildvektorisierung in C#
---

 [Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) bietet eine Hochgeschwindigkeits-C#-Bibliothek, die Sie für verschiedene SVG-Parsing-Aufgaben verwenden können . Der Namespace [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) enthält Klassen und Schnittstellen zur Implementierung des Bildvektorisierungsprozesses und arbeitet mit verschiedenen Vorverarbeitungsoptionen für Bilder, bevor sie gespeichert werden im Vektorformat. Die Verarbeitung umfasst die Steuerung der folgenden Vektorisierungsoptionen: TraceSimplifier, TraceSmoother, PathBuilder usw.

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
h2: So vektorisieren Sie Bilder in C#
title: Schritte zum Vektorisieren von Bildern in C#
---

1. Initialisieren Sie eine Instanz der Klasse [ImageVectorizer](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/). Verwenden Sie einen der ImageVectorizer()-Konstruktoren und geben Sie Konfigurationseigenschaften an.
    - Die Eigenschaft [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) stellt die Spur weicher ein. Es wird verwendet, um Fragmente von Konturen zu glätten.
    - Die Eigenschaft [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) legt die Ablaufverfolgung vereinfacht fest. Als Ergebnis wird die Spurkurve aus Liniensegmenten mit weniger (oder größeren) Punkten aufgebaut.
    - Die Eigenschaft [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) legt den Builder für SVG-Pfadsegmente fest und beeinflusst, wie stark sich die Kurve an den Kontrollpunkten krümmt.
1. Bild aus der angegebenen Datei vektorisieren. Die Methode [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) nimmt den Pfad zur Bilddatei und gibt ein SVGDocument zurück.
1. Speichern Sie das vektorisierte Bild als SVG-Datei. Verwenden Sie die Methode [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) und übergeben Sie ihr den Ausgabepfad.  

{{<section documentation>}}
---
h2: Bildvektorisierung in der Dokumentation
---

Skalierbare Vektorgrafiken werden derzeit häufig zum Rendern von Webgrafiken verwendet. Im Vergleich zu Bitmaps können Vektorgrafiken scharfe Bilder erstellen, die auf jede beliebige Größe skaliert werden können, sie sind ideal zum Zeichnen jeder Art von Webillustration, einschließlich Symbolen, Diagrammen, Diagrammen und mehr. Im Dokumentationskapitel [Vectorization - Basic Overview,](https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/) finden Sie eine Beschreibung der Prozess der Bildvektorisierung. <br>
- [Workflow zur Bildvektorisierung](https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/image-vectorization-workflow/) - Hier finden Sie Informationen zur Bildvektorisierung, eine Beschreibung des Bildvektorisierungsprozesses und der Vektorisierungsoptionen, erfahren Sie, wie Sie Rasterbilder wie PNG, JPG, BMP, TIFF, GIF, ICO in ein SVG-Dokument vektorisieren.
- [Bildvektorisierungsbeispiele](https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/image-vectorization-examples/) - Sie werden einige C#-Beispiele betrachten die die ImageVectorization-Funktionalitäten und die Auswirkung von Konfigurationseigenschaften auf das Vektorisierungsergebnis demonstrieren.

{{<section other-vectorizers>}}
---
title: Andere unterstützte Vektorisierer
subTitle: Sparen Sie Zeit und testen Sie diese Bildvektorisierer, um alle Vorteile von Vektorgrafiken zu nutzen!
---