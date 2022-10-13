---
translation: true
template: /templates/_template-vectorization-child.md
title: Bildschablonenerstellung – C#-Code und Online Stencil Maker
description: Konvertieren Sie Bild in SVG und wenden Sie die Schablonentransformation in C# an. Vektorisieren und schablonieren Sie Bilder und nutzen Sie alle Vorteile von Vektorgrafiken. Probieren Sie Online Stencil Maker kostenlos aus!
url: /net/vectorization/stencil/
family: svg
platformtag: net
feature: vectorization, stencil
informat: Image
outformat: SVG
---

{{<section banner>}}
---
h1: Stancil-Zeichnen – C#-Code und Stencil Maker
h2: Erstellen Sie Schablonenbilder online oder programmgesteuert.
---

{{<section overview>}}
---
h2: Was ist eine Bildschablone?
---

Das Bildschablonieren ist ein Prozess, der ein gewöhnliches Foto in ein Umrissbild verwandelt, das als Schablone für Graffiti-ähnliche Effekte verwendet werden kann.

Es gibt mehrere grundlegende Schritte, um ein Foto oder Bild in eine Schablone umzuwandeln:
* Konvertieren Sie ein Foto oder Bild in Graustufen. Dieser Schritt ist optional, da Sie stattdessen die Anzahl der zu quantisierenden Farben reduzieren können.
* Quantisieren Sie das Bild, um die Schablone zu erhalten, danach können Sie das Ergebnis herunterladen oder vektorisieren und die Schablonenformlinien erhalten.
* Es gibt drei Optionen zum Zeichnen von Schablonen. Die erste ist „None“, wenn alle vektorisierten Formen gefüllt sind, die zweite ist „Auto“, wenn die Formen nicht gefüllt sind und die Ränder die „Original“-Farbe haben, und die letzte ist „Monocolor“, wenn die Formen ebenfalls nicht gefüllt sind , aber die Rahmen haben die vordefinierte Farbe.


<br>
[Aspose.SVG for .NET API](https://products.aspose.com/svg/{{lang.url-fragment}}net/) offers a high-speed C# library that you can use for different SVG parsing tasks. The [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) Namespace includes classes and interfaces for implementing the image vectorization process with stenciling options.

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
h2: Online-Schablonenhersteller
---

Wenn Sie Ihre Fotos oder Bilder in Schablonen umwandeln müssen, nutzen Sie unser kostenloses Online-Tool! Es erlaubt nicht nur, Rasterschablonen zu erhalten, sondern sie auch zu vektorisieren und mit skalierbaren und übersichtlichen Vektoren zu arbeiten. Stencil Maker unterstützt JPEG, JPG, PJP, PJPEG, PNG, BMP, ICO, GIF, TIFF, WEBP, XBM und andere Bitmap-Formate!

{{<section "app-plugin" i18n-exclude>}}

{{<app/svg/imagevectorizer id="1" inputFormat="Image" sourceImage="/svg/images/vectorization/fish.png" colors="3" scale="1" grayscale="true" stencil="monocolor" extent="1" stencilColor="#00ff00">}}{{</app/svg/imagevectorizer>}} 

{{<section code-text>}}
---
title: Konvertieren Sie PNG in SVG in C#
---

Aspose.SVG für die .NET-API stellt Klassen und Methoden bereit, mit denen Sie den Bildvektorisierungsprozess implementieren und mit Schablonenoptionen arbeiten können.

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
h2: So vektorisieren Sie PNG in C#
title: Schritte zum Konvertieren von PNG in SVG in C#
---

Um ein PNG-Bild mit Aspose.SVG zu vektorisieren, sollten Sie einige Schritte befolgen:
1. Initialisieren Sie eine Instanz der Klasse [ImageVectorizer](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/). Verwenden Sie einen der ImageVectorizer()-Konstruktoren und geben Sie Konfigurationseigenschaften an.
    - Die Eigenschaft [PathBuilder](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/pathbuilder/) ruft den Builder für SVG-Pfadsegmente ab oder legt ihn fest.
    - Die Eigenschaft [ColorsLimit](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/colorslimit/) ruft die maximale Anzahl von Farben ab oder legt sie fest, die zum Quantisieren eines Bildes verwendet werden.
    - Die Eigenschaft [Stencil](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizerconfiguration/stencil/) ruft die Konfiguration des Schabloneneffekts ab oder legt sie fest. Standardmäßig wird kein Schabloneneffekt angewendet.
1. Vektorisieren Sie ein Bild aus der angegebenen Datei. Die Methode [Vectorize()](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/imagevectorizer/vectorize/) nimmt den Pfad zur Bilddatei und gibt ein SVGDocument zurück.
1. Speichern Sie das vektorisierte PNG als SVG. Verwenden Sie die Methode [Save()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/#save_6) und übergeben Sie ihr den Ausgabepfad.



{{<section documentation>}}

Im Dokumentationskapitel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Vectorization – Basic Overview </a> finden Sie Informationen zur Bildvektorisierung, eine Beschreibung des Bildvektorisierungsprozesses und der Vektorisierungsoptionen und erfahren, wie Sie Rasterbilder wie PNG, JPG, BMP, TIFF, GIF, ICO in ein SVG-Dokument vektorisieren. Sie werden einige C#-Beispiele betrachten, die die Funktionen von [ImageVectorization](https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/) und die Auswirkung von Konfigurationseigenschaften auf das Vektorisierungsergebnis demonstrieren.

{{<section other-vectorizers>}}
---
title: Andere unterstützte Vektorisierer
---