---
translation: true
template: /templates/_template-vectorization-child.md
title: BMP zu SVG – C#-Code und Online-Vektorisierer
description: BMP zu Vektor in C#. Konvertieren Sie BMP in SVG und nutzen Sie alle Vorteile von Vektorgrafiken. Probieren Sie den Online-Vektorisierer aus
url: /net/vectorization/bmp-to-svg/
family: svg
platformtag: net
feature: vectorization
informat: BMP
outformat: SVG
---

{{<section banner>}}
---
h1: BMP-Bild vektorisieren – C#-Code und Online-Vektorisierer
h2: Konvertieren Sie BMP online oder programmgesteuert in das SVG-Format.
---

{{<section overview>}}
---
h2: BMP-Bildvektorisierung
---

Unter Vektorisierung verstehen wir das Ersetzen von Bitmaps durch mathematische Kurven und geometrische Formen, die aus Pfadelementen bestehen und als SVG gespeichert werden. Es kann aus verschiedenen Gründen sinnvoll sein, Bitmaps zu vektorisieren. Vektorgrafiken haben eine Reihe von Vorteilen: Skalierung, kleine Dateigröße, Animationsunterstützung usw. Oder Sie möchten einfach nur mit Bildern experimentieren und ein paar lustige Vektorisierungseffekte erzielen. Auf jeden Fall ist die Bitmap-Vektorisierung eine gute Erfahrung, wenn Sie sich für Fotografie, Malerei, Design, Kunst und Webentwicklung interessieren.<br>
[Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) bietet eine Hochgeschwindigkeits-C#-Bibliothek, die Sie für verschiedene SVG-Parsing-Aufgaben verwenden können . Der Namespace [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) enthält Klassen und Schnittstellen zur Implementierung des Bildvektorisierungsprozesses. In diesem Artikel sehen wir uns an, wie Sie BMP in C# mithilfe der Aspose.SVG-API in Vektorgrafiken konvertieren. Darüber hinaus stellen wir Ihnen einen Online-Bildvektorisierer zur Verfügung, mit dem Sie die Bild-zu-Vektor-Konvertierung in Echtzeit ausprobieren können.

{{<section input-file>}}
---
title: Was ist das BMP-Dateiformat?
---

{{<section output-file>}}
---
title: Was ist das SVG-Dateiformat?
---

{{<section plagin-text>}}
---
h2: Online-Bildvektorisierer
---

Wenn Sie Bilder vektorisieren müssen, verwenden Sie unser kostenloses Online-Tool! Image Vectorizer unterstützt die Formate JPG, PNG, BMP, ICO, GIF und TIFF. Es bietet verschiedene Optionen zur Vorverarbeitung von Bitmaps, bevor sie im SVG-Format gespeichert werden. Wandeln Sie Ihre Bilder jetzt in skalierbare und klare Vektorgrafiken um!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Konvertieren Sie BMP in SVG in C#
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
    // Vectorize BMP from the specified file
	using var document = vectorizer.Vectorize(InputFolder + "image.bmp");
    // Save vectorized BMP image as SVG file 
	document.Save(OutputFolder + "image.svg"));
```

{{<section steps>}}
---
h2: So vektorisieren Sie BMP in C#
title: Schritte zum Konvertieren von BMP in SVG in C#
---

Um BMP mit Aspose.SVG zu vektorisieren, sollten Sie einige Schritte befolgen:
1. Initialisieren Sie eine Instanz der Klasse [ImageVectorizer.](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/) Verwenden Sie einen der ImageVectorizer()-Konstruktoren und geben Sie Konfigurationseigenschaften an.
    - Die Eigenschaft [TraceSmoother](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesmoother/) stellt die Spur glatter ein. Es wird verwendet, um Fragmente von Konturen zu glätten.
    - Die Eigenschaft [TraceSimplifier](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/tracesimplifier/) legt die Ablaufverfolgung vereinfacht fest. Als Ergebnis wird die Spurkurve aus Liniensegmenten mit weniger (oder größeren) Punkten aufgebaut.
    - Die Eigenschaft [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) legt den Builder für SVG-Pfadsegmente fest und beeinflusst, wie stark sich die Kurve an den Kontrollpunkten krümmt.
1. BMP aus der angegebenen Datei vektorisieren. Verwenden Sie die Methode [Vectorize(),](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) die ein SVGDocument zurückgibt.
1. Speichern Sie das vektorisierte BMP-Bild als SVG-Datei.

{{<section documentation>}}

Bildvektorisierung ist der Prozess der Umwandlung von Rasterbildern in Vektorgrafiken – die Bezier-Kurven, Splines und Linien. Im Dokumentationskapitel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Vectorization – Basic Overview </a> finden Sie Informationen zur Bildvektorisierung, eine Beschreibung des Bildvektorisierungsprozesses und der Vektorisierungsoptionen und erfahren, wie Sie Rasterbilder wie PNG, JPG, BMP, TIFF, GIF, ICO in ein SVG-Dokument vektorisieren. Sie werden einige C#-Beispiele betrachten, die die Funktionen von [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) und die Auswirkung von Konfigurationseigenschaften auf das Vektorisierungsergebnis demonstrieren.

Aspose.SVG bietet einen kostenlosen Online-[Image Vectorizer](https://products.aspose.app/svg/image-vectorization) an, mit dem Sie JPG-, PNG-, BMP-, TIFF-, ICO- und GIF-Bitmap-Bilder in Vektorgrafiken konvertieren können. Mit dieser App können Sie eine Reihe von Optionen anwenden, um das perfekte Ergebnis zu erzielen. Sparen Sie Zeit und testen Sie diesen Image Vectorizer, um alle Vorteile von Vektorgrafiken zu nutzen!

{{<section other-vectorizers>}}
---
title: Andere unterstützte Vektorisierer
---