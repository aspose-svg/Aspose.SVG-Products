﻿---
translation: true
template: /templates/_template-conversion-child.md
title: Konvertieren Sie SVG in PNG mit C# Core
description: Laden und konvertieren Sie SVG in PNG mit der .NET Core-API unter Windows, macOS und Linux
url: /net/conversion/svg-to-png/
family: svg
platformtag: net
feature: conversion
informat: SVG
outformat: PNG
otherformats: GIF JPEG PNG TIFF PDF XPS BMP
---

{{<section banner>}}
---
h1: Konvertieren Sie SVG in PNG über C#
h2: Hochgeschwindigkeits-.NET-API zum Konvertieren von SVG in PNG unter Windows, macOS und Linux
---

{{<section overview>}}
---
h2: SVG-zu-PNG-Konvertierung über .NET Core
---

SVG ist eines der am häufigsten verwendeten Formate zum Erstellen von Websites und zum Drucken von Grafiken, um Skalierbarkeit zu erreichen. Aber manchmal müssen Sie SVG konvertieren und in einem gängigen Rasterbildformat speichern. Mit der API [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) können Sie SVG programmgesteuert in PNG umwandeln und dabei die volle Kontrolle über eine Vielzahl von Konvertierungsparametern haben. Mit der leistungsstarken C#-API können Sie SVG mit hoher Geschwindigkeit und hoher Qualität in andere gängige Formate konvertieren.


{{<section demos>}}
---
h2: Kostenlose Online-Konverter-Live-Demos
---

Testen Sie die Qualität der SVG-zu-PNG-Konvertierung direkt in Ihrem Browser! Das folgende C#-Beispiel zeigt, wie ein SVG-Dokument mithilfe der ConvertSVG()-Methode konvertiert wird. Wir beschreiben den Quellcode zum Lesen von SVG aus einer Datei und zum anschließenden Konvertieren von SVG in PNG mit Standardspeicheroptionen. Bitte laden Sie SVG aus dem lokalen Dateisystem, wählen Sie das Ausgabeformat und führen Sie das Beispiel aus. Das Ergebnis erhalten Sie sofort als separate Datei.

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/converter SVG PNG "JPG|JPEG" BMP XPS TIFF PDF GIF >}}
using Aspose.Svg;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;
using Aspose.Svg.Rendering.Image;

    using var document = new SVGDocument("image.svg");
{{#if_output 'PDF'}}
    var options = new PdfSaveOptions();
{{/if_output}}
{{#if_output 'XPS'}}
    var options = new XpsSaveOptions();
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
h2: Schritte zum Konvertieren von SVG in PNG mit der Methode ConvertSVG()
---
1. Laden Sie eine SVG-Datei mit einem der SVGDocument()-Konstruktoren der [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/)-Klasse.
1. Erstellen Sie ein neues [ImageSaveOptions](https://reference.aspose.com/svg/net/aspose.svg.saving/imagesaveoptions/)-Objekt. Standardmäßig ist die Eigenschaft „Format“ PNG.
1. Verwenden Sie die Methode [ConvertSVG()](https://reference.aspose.com/svg/net/aspose.svg.converters/converter/convertsvg/), um SVG als PNG-Bild zu speichern. Sie müssen das SVGDocument, die ImageSaveOptions und den Pfad der Ausgabedatei an die Methode ConvertSVG() übergeben.
1. Die PNG-Datei wird im angegebenen Pfad gespeichert.

{{<section steps2>}}
---
h2: Schritte zum Konvertieren von SVG in PNG mit der RenderTo()-Methode
---
1. Initialisieren Sie [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/) mit Ihrer SVG-Datei.
1. Erstellen Sie ein Objekt der ImageRenderingOptions-Klasse. Verwenden Sie den Konstruktor [ImageRenderingOptions()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/imagerenderingoptions/) und geben Sie die Eigenschaft „Format“ des Dokuments an.
1. Initialisieren Sie die Klasse [ImageDevice](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/) und geben Sie den Namen der zu rendernden Ausgabedatei an.
1. Rufen Sie die Methode [RenderTo()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/) auf und übergeben Sie die Instanz von ImageDevice.

{{<section code-text>}}
---
title: Konvertieren Sie SVG in PNG
---

{{<section "code-snippet" i18n-exclude>}}

```cs
using (var document = new SVGDocument("input.svg"))
{
	var options = new ImageRenderingOptions(ImageFormat.Png);
	using (IDevice device = new ImageDevice(options, "output.png"))
	{
		document.RenderTo(device);                    
	}
}
```

{{<section other-conversions>}}
---
title: Andere unterstützte SVG-Konvertierungen
subTitle: "Sie können SVG auch in viele andere Dateiformate konvertieren:"
---