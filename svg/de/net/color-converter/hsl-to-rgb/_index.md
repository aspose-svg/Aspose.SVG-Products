---
translation: true
template: ./../_template-child.md
title: HSL-zu-RGB-Konvertierung in C#
description: Arbeiten Sie mit Farbcodes und konvertieren Sie HSL in RGB in C#
url: /net/color-converter/hsl-to-rgb/
family: svg
platformtag: net
feature: color converter
informat: HSL
outformat: RGB
otherformats: HEX HSL HSV HWB CMYK LAB LCH XYZ OKLAB OKLCH NCOL
---

{{<section banner>}}
---
h1: Konvertieren Sie HSL über C# in RGB
h2: Verwenden Sie die Hochgeschwindigkeits-.NET-API, um HSL in RGB-Farbe unter Windows, macOS und Linux zu konvertieren
---

{{<section overview>}}
---
h2: Konvertieren Sie HSL in RGB mit C#
---

[Aspose.SVG for .NET API](https://products.aspose.com/svg/net/) bietet eine Hochgeschwindigkeits-C#-Bibliothek, die Sie für verschiedene SVG-Parsing-Aufgaben verwenden können. Eine der API-Funktionen ist der einfache Zugriff auf die Arbeit mit mehreren Farbräumen. Der Namensraum Aspose.Svg.Converters implementiert einfachen Zugriff auf die Klasse [ColorConverter](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/), die Farben analysiert (RGB, HEX, HSL, HWB , CMYK, NCOL, LCH, OKLCH, LAB, OKLAB) aus einem String und gibt die IConvertibleColor-Schnittstelle zur Konvertierung in verschiedene Farbräume zurück.<br><br>
Farbcodes oder Farbformate sind eng mit den Methoden zur Beschreibung und Definition von Farben verbunden und werden häufig im Web, Design, Polygrafie, Fotografie, Kunst usw. verwendet. Und für unterschiedliche Aufgaben werden unterschiedliche Farbformate bevorzugt. Daher müssen Sie manchmal Farbcodes konvertieren.

{{<section input-color>}}
---
title: Was ist HSL-Farbe?
---

{{<section output-color>}}
---
title: Was ist RGB-Farbe?
---

{{<section code-text>}}
---
h2: C#-Codebeispiel zum Konvertieren von HSL in RGB
title: Konvertieren Sie HSL in RGB – C#
---

Die Hochgeschwindigkeits-C#-Bibliothek ermöglicht es .NET-Entwicklern, HSL schnell und effizient in RGB-Farben zu konvertieren. Die Farbkonvertierung kann mit ein paar Zeilen Code durchgeführt werden:

{{<section "code-snippet" i18n-exclude>}}

```cs

// Parse HSL color from a string
var color = ColorConverter.ConvertFrom("hsl(31.034, 57%, 70%)");
// Convert HSL to RGB 
string rgbColor = color.ToRgbString();
// Print the result into console
Console.WriteLine(rgbColor);
//result should be: rgb(222, 180, 134)

```

{{<section steps>}}
---
h2: Schritte zum Konvertieren von HSL in RGB mit C#
---
1. Rufen Sie die Methode [ConvertFrom()](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/convertfrom/) der Klasse ColorConverter auf und übergeben Sie den HSL-Code als Zeichenfolge.
1. Die ConvertFrom()-Methode analysiert die Farbe aus der Zeichenfolgendarstellung und gibt die Schnittstelle [IConvertibleColor](https://reference.aspose.com/svg/net/aspose.svg.drawing/iconvertiblecolor/) zurück, um sie in die erforderliche Farbe zu konvertieren Räume.
1. Die Methode IConvertibleColor.ToRgbString() konvertiert HSL in RGB-Farbe im Format: rgb(0, 0, 0).



{{<section documentation>}}

Bitte besuchen Sie unsere Dokumentation, um mehr über die Verwendung von Aspose.SVG-API-Funktionen zu erfahren und C#-Beispiele für die gängigsten SVG-Verarbeitungsszenarien zu betrachten. Im Dokumentationsartikel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-change-svg-color/" target= "_blank">So ändern Sie die SVG-Farbe</a>, Sie können sehen, wie Sie die Farbe von Elementen und Hintergrund in SVG-Bildern mit der Aspose.SVG .NET-Bibliothek ändern. Der Artikel <a href="https://docs.aspose.com/svg/net/drawing-basics/svg-color/" target="_blank">SVG-Farbe</a> befasst sich ausführlich damit SVG-Text und -Formen können eingefärbt werden.

{{<section online-color-converter>}}
---
h2: Online-Farbkonverter
---

[Farbkonverter](https://products.aspose.app/svg/color-converter) sind kostenlose Online-Webanwendungen, mit denen Sie Farben zwischen verschiedenen Farbcodes wie RGB, HEX, HSL, HSV, HWB, LAB, CMYK konvertieren können , LCH, XYZ, OKLAB, OKLCH, RGBA, HSLA usw. im Handumdrehen. Farbkonverter sind einfach zu bedienen und funktionieren auf jedem Browser und Betriebssystem. Das Ergebnis erhalten Sie sofort nach Eingabe des zu konvertierenden Farbcodes.

{{<section get-started>}}
---
h2: Erste Schritte mit der .NET SVG-API
---

Installieren Sie von der Befehlszeile als ```nuget install Aspose.SVG``` oder über die Package Manager Console von Visual Studio mit ```Install-Package Aspose.SVG```.
Alternativ können Sie das Offline-MSI-Installationsprogramm oder DLLs in einer ZIP-Datei von [downloads](https://downloads.aspose.com/svg/net) herunterladen. Die Aspose.SVG-API ist eine eigenständige API und kann für die Bearbeitung und Analyse von SVG-Dokumenten in Anwendungen verwendet werden.
Weitere Einzelheiten zur Installation der C#-Bibliothek und zu den Systemanforderungen finden Sie in der [Aspose.SVG-Dokumentation](https://docs.aspose.com/svg/net/getting-started/).

{{<section other-color-converters>}}
---
title: Andere unterstützte Farbkonverter
---