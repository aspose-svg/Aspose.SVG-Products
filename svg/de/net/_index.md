---
translation: true
template: template.md
title: C# .NET SVG-Dateien Analyse-API - Aspose
weight: 20
url: /net/
description: C# .NET SVG-Bibliothek zum Laden von Dateien, Lesen und Durchlaufen der Elemente und Konvertieren von SVG in PDF-, XPS- und Bildformate
---

{{<section banner>}}
---
h1: .NET-APIs zum Analysieren von SVG-Dateien
h2: Erstellen, laden, parsen, rendern und konvertieren Sie SVG-Dateien in gängige Formate ohne Softwareabhängigkeiten
---

{{<section overview>}}
---
item1: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/creating-loading-documents/" target="_blank">Erstellen oder laden Sie SVG Dokumente</a> aus einer Datei, URL, Zeichenfolge, Stream usw.
item2: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">SVG konvertieren</a> in PDF , PNG und andere gängige Formate.
item3: <a href="hhttps://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">Vektorisieren Sie Rasterbilder</a> wie z als PNG, JPG, BMP, TIFF, GIF und ICO in ein SVG-Dokument.
item4: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/navigation-inspection/" target="_blank">In SVG-Dokumenten navigieren</a > Verwendung von XPath-Abfrage, CSS-Selektor, Element- und Dokumentdurchlauffunktionen.
item5: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-edit-svg-documents/" target="_blank"> Bearbeiten Sie SVG-Dateien</a>, indem Sie neue Knoten einfügen, entfernen oder den Inhalt vorhandener Knoten bearbeiten.
item6: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target="_blank"> Rendern Sie SVG-Dokumente</a> in hoher Qualität.
item7: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/text-vectorization/" target="_blank">SVG-Text vektorisieren</a > in kurzer Zeit und in professioneller Qualität und Auflösung und mehr.
---

Aspose.SVG für .NET ist eine flexible Bibliothek für die Verarbeitung von SVG-Dateien und vollständig kompatibel mit ihren Spezifikationen. Die API kann SVG-Dateien einfach laden, speichern und konvertieren sowie die Elemente von Dateien über ihr Document Object Model (DOM) lesen und durchlaufen. Die API ist unabhängig von anderer Software und versetzt Entwickler in die Lage, mit SVG-Dateien zu arbeiten, ohne auf die zugrunde liegenden Details des Formats einzugehen.<br><br>
Mit der Aspose.SVG C#-Bibliothek in Ihrem Projekt können Sie die folgenden Aufgaben ausführen:

{{<section glance>}}
---
h3: Auf einen Blick
description: Eine Übersicht über Aspose.SVG für die .NET-API.
---

{{<section platform>}}
---
h3: Plattformunabhängigkeit
description: Aspose.SVG für .NET unterstützt alle wichtigen Plattformen einschließlich.
---

{{<section formats>}}
---
h3: Unterstützte Dateiformate
description: Aspose.SVG für .NET unterstützt alle gängigen Bilddateiformate und mehr.
---

{{<section feature>}}
---
title: Erweiterte .NET-SVG-Parsing-API-Funktionen
feature1: Erstellen und lesen Sie SVG-Dokumente
feature2: Bearbeiten und speichern Sie SVG-Dateien
feature3: Konvertieren Sie SVG in gängige Formate
feature4: Volle Kontrolle über SVG-Knoten
feature5: Knoten hinzufügen und entfernen
feature6: Ändern Sie die Knoteneigenschaften
feature7: Inhaltsnavigation mit XPath-Abfrage
feature8: Navigieren Sie über CSS-Selektoren, Element- und Dokumentendurchlauf
feature9: DOM Tree-Manipulation von offiziellen SVG-Spezifikationen
---

{{<section convert>}}
---
h2: SVG in C# zusammenführen
h3: SVG in PDF zusammenführen – C#
---	
   
Aspose.SVG für .NET kann SVG lesen und in PDF, XPS und die wichtigsten Bildformate konvertieren. Der Konvertierungsprozess ist einfach und zuverlässig, was die SVG .NET API zur perfekten Wahl macht. Sie können die API in Ihrer C#- oder jeder anderen .NET-Anwendung verwenden, um Konverteranwendungen zu entwickeln, ohne sich mit den Details der zugrunde liegenden Dateiformate befassen zu müssen. Das Abrufen der Konvertierungsfunktion ist einfach und hängt von den jeweiligen Anwendungsanforderungen ab. Hier sind ein paar Codezeilen für die Konvertierung zwischen Formaten.

{{<section "code" i18n-exclude>}}
     
using Aspose.Svg;
using System.IO;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;
...
    
    // Initialize an SVG document from a file
    using (var document = new SVGDocument("input.svg"))
    {
        // Create an instance of the ImageSaveOptions class
    	var pngSaveOptions = new ImageSaveOptions();    
    
        // Convert SVG to PNG
    	Converter.ConvertSVG(document, pngSaveOptions, "output.png");
    }

{{<section online-converters>}}

Sie können den Online-SVG-Konverter <a href="https://products.aspose.app/svg/conversion/svg" target="_blank">hier</a> ausprobieren

{{<section other-converters>}}

Andere unterstützte SVG-Konvertierungen:

{{<section image-vector>}}
---
h2: Konvertieren Sie ein Rasterbild in eine Vektorgrafik
h3: Bild in Vektor umwandeln – C#
---

Das Konvertieren eines Bildes in einen Vektor ist mit der Aspose.SVG-API sehr einfach. Der Namespace <a href="https://apireference.aspose.com/svg/net/aspose.svg.imagevectorization/" target="_blank">ImageVectorization</a> enthält Klassen und Schnittstellen zur Implementierung des Bildvektorisierungsprozesses. Das folgende Code-Snippet demonstriert die Verwendung der ImageVectorizer-Klasse für die Bildvektorisierung:

{{<section "code-image" i18n-exclude>}}
     
using Aspose.Svg.ImageVectorization;
using Aspose.Svg.Saving;
...
    
	// Initialize an instance of the ImageVectorizer class
	var vectorizer = new ImageVectorizer
	{
		Configuration = 
		{
			TraceSmoother =   new ImageTraceSmoother(1),
			TraceSimplifier = new ImageTraceSimplifier(0.5f),
			ColorsLimit = 3
		}
	};
	
	// Vectorize raster image from the specified file
	using var document = vectorizer.Vectorize("input.png");
	
	// Save vectorized image as SVG file 
	document.Save("output.svg");

{{<section merge>}}
---
h2: SVG in C# zusammenführen
h3: SVG in PDF zusammenführen – C#
---	
	
Die Renderer()-Methode gibt Ihnen die Möglichkeit, mehrere Dokumente auf einmal an das Ausgabe-Rendering-Gerät zu senden und sie zusammenzuführen. Das Zusammenführen von Dokumenten kann mit ein paar Zeilen Code durchgeführt werden:

{{<section "code-merge" i18n-exclude>}}
     
using Aspose.Svg;
using Aspose.Svg.Rendering;
using Aspose.Svg.Rendering.Pdf;
...   
	
	// Initialize SVG documents from files to merge later
	using (var document1 = new SVGDocument("input1.svg"))
	using (var document2 = new SVGDocument("input2.svg"))
	using (var document3 = new SVGDocument("input3.svg"))
	{
		// Create an instance of SvgRenderer
		using (var renderer = new SvgRenderer())
		{
			// Create an instance of PdfDevice
			using (var device = new PdfDevice("output.pdf"))
			{
				// Merge all SVG documents to PDF
				renderer.Render(device, document1, document2, document3);
			}
		}
	}

{{<section other-mergers>}}	

Andere unterstützte Fusionen: