---
translation: true
template: /templates/_template-merger-child.md
title: Zusammenführen von SVG zu BMP über C# - Aspose.SVG
description: Führen Sie SVG zu BMP über die C#-API unter Windows, macOS und Linux zusammen
url: /net/merger/svg-to-bmp/
family: svg
platformtag: net
feature: merge
informat: SVG
outformat: BMP
otherformats: XPS PDF GIF JPEG PNG TIFF BMP
---

{{<section banner>}}
---
h1: SVG zu BMP über C# zusammenführen
h2: Hochgeschwindigkeits-.NET-API zum Kombinieren von SVG-Dateien unter Windows, macOS und Linux
---

{{<section overview>}}
---
h2: Zusammenführen von SVG zu BMP mit C#
---

SVG ist eines der am häufigsten verwendeten Formate zum Erstellen von Websites und zum Drucken von Grafiken, um Skalierbarkeit zu erreichen. Aber manchmal müssen Sie SVG-Dateien zusammenführen und sie als ein Dokument in einem anderen Dateiformat speichern. BMP-Dateien stellen Bitmap-Bilddateien dar, die zum Speichern hochwertiger digitaler Bitmap-Bilder verwendet werden. Das BMP-Format kann Daten als zweidimensionale digitale Bilder sowohl in Monochrom- als auch in Farbformaten mit verschiedenen Farbtiefen speichern. Mit der API [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) können Sie SVG programmgesteuert mit BMP zusammenführen. Die leistungsstarke C#-API hilft Ihnen, SVG-Dateien schnell und in hoher Qualität zu kombinieren!

{{<section code-text>}}
---
h2: C#-Codebeispiel zum Zusammenführen von SVG zu BMP
title: SVG zu BMP zusammenführen - C#
---

Eine Hochgeschwindigkeits-C#-Bibliothek ermöglicht es .NET-Entwicklern, SVG-Dateien zusammenzuführen und das kombinierte Ergebnis schnell und effizient in andere gängige Formate wie PDF, XPS, JPEG, PNG, BMP, GIF und TIFF zu konvertieren. Das Zusammenführen von Dokumenten kann mit ein paar Zeilen Code durchgeführt werden:

{{<section "code-snippet" i18n-exclude>}}

```cs
// Initialize SVG documents from files to merge 
using (var document1 = new SVGDocument("document1.svg"))
using (var document2 = new SVGDocument("document2.svg"))
using (var document3 = new SVGDocument("document3.svg"))
{
    // Create an instance of SvgRenderer
    using var renderer = new Aspose.Svg.Rendering.SvgRenderer();	
    // Create an instance of ImageDevice
    using var device = new Aspose.Svg.Rendering.Image.ImageDevice("result.bmp");
    // Merge SVG to BMP
    renderer.Render(device, document1, document2, document3);                
}
```

{{<section steps>}}
---
h2: Schritte zum Zusammenführen von SVG zu BMP mit C#
---
1. Laden Sie ein SVG-Dokument mit einem der [SVGDocument()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/)-Konstruktoren.
1. Erstellen Sie eine neue Instanz der Klasse [SvgRenderer](https://reference.aspose.com/svg/net/aspose.svg.rendering/svgrenderer/).
1. Verwenden Sie den Konstruktor [ImageDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/imagedevice/#constructor_5), um eine neue Instanz der ImageDevice-Klasse zu initialisieren.
1. Rufen Sie die Methode [Render()](https://reference.aspose.com/svg/net/aspose.svg.rendering/renderer-1/) auf, um SVG zu BMP-Bild zusammenzuführen.
1. Mehrere SVG-Dateien werden im BMP-Bild im angegebenen Pfad gespeichert.



{{<section documentation>}}

Der Namespace [Aspose.Svg.Rendering](https://reference.aspose.com/svg/net/aspose.svg.rendering/) implementiert einfachen Zugriff auf Render()-Methoden. Sie können SVG-Zusammenführungen schnell durchführen und das Kombinationsergebnis in gängige Formate wie PDF, XPS, JPEG, PNG, BMP, TIFF und GIF exportieren. Bitte besuchen Sie <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">unsere Dokumentation</a>, um mehr zu erfahren mehr über die Verwendung von Aspose.SVG-API-Funktionen. Im Dokumentationsartikel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target= "_blank">So führen Sie SVG-Dateien zusammen</a>, können Sie sich C#-Beispiele zum Zusammenführen von SVG ansehen.

{{<section online-merger>}}
---
h2: Online-Bildzusammenführung
---

Aspose.SVG bietet eine kostenlose Online-<a href="https://products.aspose.app/svg/merger" target="_blank">Image Merger</a>-App, die mehrere Bilder in einer einzigen Datei kombiniert. Sie können eine Art Bildzusammenführung für verschiedene Quelldateien wie SVG, JPG, PNG, BMP, ICO, GIF oder TIFF auswählen und das Ergebnis in einem der folgenden Ausgabeformate speichern: JPG, PNG oder SVG. Unsere Anwendung ist multifunktional. Sie können Bildcollagen erstellen, Bilder vor dem Zusammenführen bearbeiten und manipulieren. Mit Image Merger können Sie Bilder frei hinzufügen, drehen, skalieren, Hintergründe hinzufügen, filtern und jedes Bild verschieben, bis Sie mit dem Endergebnis Ihres Designs zufrieden sind.

{{<section get-started>}}
---
h2: Erste Schritte mit der .NET SVG-API
---

Installieren Sie von der Befehlszeile als ```nuget install Aspose.SVG``` oder über die Package Manager Console von Visual Studio mit ```Install-Package Aspose.SVG```.
Alternativ können Sie das Offline-MSI-Installationsprogramm oder DLLs in einer ZIP-Datei von [downloads](https://releases.aspose.com/svg/net/) herunterladen. Aspose.SVG für .NET API ist eine eigenständige Bibliothek und hängt von keiner Software für die Verarbeitung von SVG-Dokumenten ab.
 Weitere Einzelheiten zur Installation der C#-Bibliothek und zu den Systemanforderungen finden Sie in der [Aspose.SVG-Dokumentation](https://docs.aspose.com/svg/net/getting-started/).

{{<section other-mergers>}}
---
title: Andere unterstützte Fusionen
subTitle: "Sie können SVG und Bilder mit anderen Dateiformaten zusammenführen:"
---