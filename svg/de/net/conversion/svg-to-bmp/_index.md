---
translation: true
template: Vorlage.md
title: Konvertieren Sie SVG in BMP mit .NET Core
description: Laden und konvertieren Sie SVG in BMP mit der .NET Core-API unter Windows, macOS und Linux
url: /net/conversion/svg-to-bmp/
family: &1617081016 SVG
platformtag: Netz
feature: Wandlung
informat: SVG
outformat: BMP
otherformats: GIF-JPEG-PNG-TIFF
---

{{<section banner>}}
---
h1: Konvertieren Sie SVG in BMP über C#
h2: Hochgeschwindigkeits-.NET-API zum Konvertieren von SVG in BMP unter Windows, macOS und Linux
---

{{<section overview>}}
---
h2: SVG-zu-BMP-Konvertierung über .NET Core
---

SVG ist eines der am häufigsten verwendeten Formate zum Erstellen von Websites und zum Drucken von Grafiken, um Skalierbarkeit zu erreichen. Aber manchmal müssen Sie SVG konvertieren und in einem gängigen Rasterbildformat speichern. Mit der API [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) können Sie SVG programmgesteuert in das BMP-Format umwandeln und dabei die volle Kontrolle über eine Vielzahl von Konvertierungsparametern haben. Mit der leistungsstarken C#-API können Sie SVG mit hoher Geschwindigkeit und hoher Qualität in gängige Formate konvertieren.


{{<section demos>}}
---
h2: Kostenlose Online-Konverter-Live-Demos
---

<p>Test the quality of SVG to BMP conversion right in your browser! The following C# example demonstrates how to convert an SVG document using ConvertSVG() method. We describe the source code for reading SVG from a file and then converting SVG to BMP with default saving options. Please load SVG from the local file system, select the output format and run the example. You will immediately get the result as a separate file.</p>

{{<section app-pluging>}}

{{< app/svg/converter SVG BMP XPS TIFF PNG PDF "JPG|JPEG" GIF >}}
using Aspose.Svg;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;
using Aspose.Svg.Rendering.Image;

    using var document = new SVGDocument("image.svg");
{{#if_output 'PDF'}}
    var Optionen = neue PdfSaveOptions();
{{/if_output}}
{{#if_output 'XPS'}}
    var Optionen = neue XpsSaveOptions();
{{/if_output}}
{{#if_output 'BMP' 'JPG' 'GIF' 'PNG' 'TIFF'}}
    var options = new ImageSaveOptions(ImageFormat.{{output param2 camel}});
{{/if_output}}
    Converter.ConvertSVG(document, options, "output.{{output lower}}");
{{< /app/svg/converter>}} 

{{<section documentation>}}

Bitte besuchen Sie <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">unsere Dokumentation</a> um mehr über die Verwendung von Aspose.SVG-API-Konvertierungsfunktionen zu erfahren und C#-Beispiele für die gängigsten SVG-Konvertierungsszenarien zu betrachten. Im Dokumentationsartikel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/convert-svg-to-image/" target="_blank ">SVG in Bild umwandeln</a> können Sie C#-Beispiele betrachten, wie Sie SVG auf unterschiedliche Weise in Bilder umwandeln können. Betrachten wir einige davon:

{{<section steps1>}}
---
h2: Schritte zum Konvertieren von SVG in BMP mit der ConvertSVG()-Methode
---
1. Laden Sie eine SVG-Datei mit einem der SVGDocument()-Konstruktoren der [SVGDocument](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument)-Klasse.
1. Erstellen Sie ein neues [ImageSaveOptions](https://apireference.aspose.com/svg/net/aspose.svg.saving/imagesaveoptions)-Objekt mit BMP ImageFormat. Standardmäßig ist die Eigenschaft „Format“ PNG.
1. Verwenden Sie die Methode [ConvertSVG()](https://apireference.aspose.com/svg/net/aspose.svg.converters/converter/convertsvg/), um SVG als BMP-Bild zu speichern. Sie müssen das SVGDocument, die ImageSaveOptions und den Pfad der Ausgabedatei an die Methode ConvertSVG() übergeben.
1. Die BMP-Datei wird im angegebenen Pfad gespeichert.



{{<section steps2>}}
---
h2: Schritte zum Konvertieren von SVG in BMP mit der RenderTo()-Methode
---
1. Initialisieren Sie [SVGDocument](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument) mit Ihrer SVG-Datei.
1. Erstellen Sie ein Objekt der ImageRenderingOptions-Klasse. Verwenden Sie den Konstruktor [ImageRenderingOptions()](https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/constructors/1) und geben Sie die Eigenschaft „Format“ des Dokuments an.
1. Initialisieren Sie die Klasse [ImageDevice](https://apireference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice) und geben Sie den zu rendernden Ausgabedateinamen an.
1. Rufen Sie die Methode [RenderTo()](https://apireference.aspose.com/svg/net/aspose.svg/svgdocument/methods/renderto) auf und übergeben Sie die Instanz von ImageDevice.



{{<section code-text>}}
---
title: Konvertieren Sie SVG in BMP
---

{{<section code-snippet>}}

```cs
using (var document = new SVGDocument("input.svg"))
{
	var options = new ImageRenderingOptions(ImageFormat.Bmp);
	using (IDevice device = new ImageDevice(options, "output.bmp"))
	{
		document.RenderTo(device);                    
	}
}
```

{{<section get-started>}}
---
h2: Erste Schritte mit der .NET SVG-API
---

Installieren Sie von der Befehlszeile als ```nuget install Aspose.SVG``` oder über die Package Manager Console von Visual Studio mit ```Install-Package Aspose.SVG```.
Alternativ können Sie das Offline-MSI-Installationsprogramm oder DLLs in einer ZIP-Datei von [downloads](https://downloads.aspose.com/svg/net) herunterladen. Aspose.SVG für .NET API ist eine eigenständige Bibliothek und hängt von keiner Software für die Verarbeitung von SVG-Dokumenten ab.
 Weitere Einzelheiten zur Installation der C#-Bibliothek und zu den Systemanforderungen finden Sie in der [Aspose.SVG-Dokumentation] (https://docs.aspose.com/svg/net/getting-started/).

{{<section other-conversions>}}
---
h2: Andere unterstützte SVG-Konvertierungen
---
Sie können SVG auch in viele andere Dateiformate konvertieren: