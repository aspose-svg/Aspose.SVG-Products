---
translation: true
template: /templates/_template-merger-child.md
title: Zusammenführen von SVG zu PDF über C# - Aspose.SVG
description: Zusammenführen von SVG in PDF mit C# unter Windows, macOS und Linux
url: /net/merger/svg-to-pdf/
family: svg
platformtag: net
feature: merge
informat: SVG
outformat: PDF
otherformats: XPS PDF GIF JPEG PNG TIFF BMP
---

{{<section banner>}}
---
h1: SVG in PDF über C# zusammenführen
h2: Hochgeschwindigkeits-.NET-API zum Kombinieren von SVG-Dateien unter Windows, macOS und Linux
---

{{<section overview>}}
---
h2: SVG zu PDF in C# zusammenführen
---

SVG ist eines der am häufigsten verwendeten Formate zum Erstellen von Websites und zum Drucken von Grafiken, um Skalierbarkeit zu erreichen. Aber manchmal müssen Sie SVG-Dateien zusammenführen und sie als ein Dokument in einem anderen Dateiformat speichern. PDF ist ein Dateiformat, das von allen Betriebssystemen unterstützt und zur Präsentation von Bildern, Dokumenten und Büchern verwendet wird. Dateien im PDF-Format können einfach angezeigt, gedruckt und online geteilt werden. Mit der API [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) können Sie SVG programmgesteuert mit PDF zusammenführen. Die leistungsstarke C#-API hilft Ihnen, SVG-Dateien schnell und in hoher Qualität zu kombinieren!

{{<section code-text>}}
---
h2: C#-Codebeispiel zum Zusammenführen von SVG zu PDF
title: SVG in PDF zusammenführen – C#
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
    // Create an instance of PdfDevice
    using var device = new Aspose.Svg.Rendering.Pdf.PdfDevice("result.pdf");
    // Merge SVG to PDF
    renderer.Render(device, document1, document2, document3);                
}
```

{{<section steps>}}
---
h2: Schritte zum Zusammenführen von SVG in PDF mit C#
---
1. Laden Sie ein SVG-Dokument mit einem der [SVGDocument()](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/)-Konstruktoren.
1. Erstellen Sie eine neue Instanz der Klasse [SvgRenderer](https://reference.aspose.com/svg/net/aspose.svg.rendering/svgrenderer/).
1. Verwenden Sie den Konstruktor [PdfDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.pdf/pdfdevice/pdfdevice/#constructor_5), um eine neue Instanz der PdfDevice-Klasse zu initialisieren.
1. Rufen Sie die Methode [Render()](https://reference.aspose.com/svg/net/aspose.svg.rendering/renderer-1/) auf, um SVG mit einer PDF-Datei zusammenzuführen.
1. Mehrere SVG-Dateien werden unter dem angegebenen Pfad in einer PDF-Datei gespeichert.



{{<section documentation>}}

Der Namespace [Aspose.Svg.Rendering](https://reference.aspose.com/svg/net/aspose.svg.rendering/) implementiert einfachen Zugriff auf Render()-Methoden. Sie können SVG-Zusammenführungen schnell durchführen und das Kombinationsergebnis in gängige Formate wie PDF, XPS, JPEG, PNG, BMP, TIFF und GIF exportieren. Bitte besuchen Sie <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">unsere Dokumentation</a>, um mehr zu erfahren mehr über die Verwendung von Aspose.SVG-API-Funktionen. Im Dokumentationsartikel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target= "_blank">So führen Sie SVG-Dateien zusammen</a>, können Sie sich C#-Beispiele zum Zusammenführen von SVG ansehen.

{{<section online-merger>}}
---
h2: Online-SVG-Fusion
---

Aspose.SVG bietet eine kostenlose Online-App zum <a href="https://products.aspose.app/svg/merger/svg" target="_blank">SVG zusammenführen</a>, die mehrere SVGs in einer einzigen Datei kombiniert. Sie können eine Art SVG-Merger für verschiedene Ausgabedateien wie SVG, JPG oder PNG auswählen. Unsere Anwendung ist multifunktional. Sie können Bildcollagen erstellen, SVG-Bilder bearbeiten und manipulieren, bevor Sie sie zusammenführen. Mit SVG Merger können Sie Bilder frei hinzufügen, drehen, skalieren, Hintergründe hinzufügen, filtern und jedes Bild verschieben, bis Sie mit dem Endergebnis Ihres Designs zufrieden sind.

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
subTitle: "Sie können SVG und Bilder in andere Dateiformate zusammenführen:"
---