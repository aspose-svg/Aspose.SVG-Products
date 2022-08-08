---
translation: true
template: /templates/_template-color-child.md
title: RGB-zu-LCH-Konvertierung - C#
description: Arbeiten Sie mit Farbcodes und konvertieren Sie RGB in LCH in C#
url: /net/color-converter/rgb-to-lch/
family: svg
platformtag: net
feature: color converter
informat: RGB
outformat: LCH
otherformats: HEX HSV HSL HWB CMYK LAB XYZ OKLAB OKLCH NCOL
---

{{<section banner>}}
---
h1: Konvertieren Sie RGB in LCH über C#
h2: Verwenden Sie die Hochgeschwindigkeits-.NET-API, um RGB in LCH-Farben unter Windows, macOS und Linux zu konvertieren
---

{{<section overview>}}
---
h2: Konvertieren Sie RGB in LCH mit C#
---

[Aspose.SVG for .NET API](https://products.aspose.com/svg/net/) bietet eine Hochgeschwindigkeits-C#-Bibliothek, die Sie für verschiedene SVG-Parsing-Aufgaben verwenden können. Eine der API-Funktionen ist der einfache Zugriff auf die Arbeit mit mehreren Farbräumen. Der Namensraum Aspose.Svg.Converters implementiert einfachen Zugriff auf die Klasse [ColorConverter,](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/) die Farben analysiert (RGB, HEX, HSL, HWB , CMYK, NCOL, LCH, OKLCH, LAB, OKLAB) aus einem String und gibt die IConvertibleColor-Schnittstelle zur Konvertierung in verschiedene Farbräume zurück.<br>
Farbcodes oder Farbformate sind eng mit den Methoden zur Beschreibung und Definition von Farben verbunden und werden häufig im Web, Design, Polygrafie, Fotografie, Kunst usw. verwendet. Und für unterschiedliche Aufgaben werden unterschiedliche Farbformate bevorzugt. Daher müssen Sie manchmal Farbcodes konvertieren.

{{<section input-color>}}
---
title: Was ist RGB-Farbe?
---

{{<section output-color>}}
---
title: Was ist LCH-Farbe?
---

{{<section code-text>}}
---
h2: Online-Farbkonverter
title: RGB in LCH umwandeln - C#
---

Wenn Sie Farben von einem Farbmodell in ein anderes konvertieren müssen, verwenden Sie unser kostenloses Online-Tool! Es unterstützt verschiedene Farbräume, darunter HEX, RGB, CMYK, HSL, LAB, XYZ usw. Sie müssen nur den Farbwert für die Konvertierung eingeben! Klicken Sie in den Farbbereich, um eine Farbe auszuwählen, oder geben Sie einen Farbcode in das Textfeld Eingabe ein. Sie sehen sofort andere Farbcodes für die ausgewählte Farbe im Abschnitt Ausgabe.

{{<section "app-pluging" i18n-exclude>}}

{{< app/svg/color id=1 input="RGB" output="LCH">}}
// Parse RGB color from a string
var color = ColorConverter.ConvertFrom("rgb(222, 180, 135)");

// Convert RGB to LCH 
string lchColor = color.ToLchString();

// Print the result into console
Console.WriteLine(lchColor);
//result should be: lch(76.339%, 20.768%, 68.746%)
{{< /app/svg/color>}}

{{<section steps>}}
---
h2: Schritte zum Konvertieren von RGB in LCH mit C#
---

Wenn Sie die Konvertierungsfeatures in Ihrem Produkt verwenden oder Farbcodes programmgesteuert konvertieren möchten, sehen Sie sich das obige C#-Codebeispiel an. Die Farbkonvertierung kann mit ein paar Zeilen Code durchgeführt werden:

1. Rufen Sie die Methode [ConvertFrom()](https://reference.aspose.com/svg/net/aspose.svg.converters/colorconverter/convertfrom/) der Klasse ColorConverter auf und übergeben Sie den RGB-Code als String.
1. Die ConvertFrom()-Methode analysiert die Farbe aus der Zeichenfolgendarstellung und gibt die Schnittstelle [IConvertibleColor](https://reference.aspose.com/svg/net/aspose.svg.drawing/iconvertiblecolor/) zurück, um sie in die erforderliche Farbe zu konvertieren Räume.
1. Die Methode IConvertibleColor.ToLchString() konvertiert RGB in LCH-Farbe im Format: lch(0%,0%,0%).

{{<section documentation>}}

Bitte besuchen Sie unsere Dokumentation, um mehr über die Verwendung von Aspose.SVG-API-Funktionen zu erfahren und C#-Beispiele für die gängigsten SVG-Verarbeitungsszenarien zu betrachten. Im Dokumentationsartikel <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-change-svg-color/" target= "_blank">So ändern Sie die SVG-Farbe</a>, Sie können sehen, wie Sie die Farbe von Elementen und Hintergrund in SVG-Bildern mit der Aspose.SVG .NET-Bibliothek ändern. Der Artikel <a href="https://docs.aspose.com/svg/net/drawing-basics/svg-color/" target="_blank">SVG-Farbe</a> befasst sich ausführlich damit SVG-Text und -Formen können eingefärbt werden.

{{<section online-color-converter>}}
---
h2: Online-Farbkonverter
---

[Farbkonverter](https://products.aspose.app/svg/color-converter) sind kostenlose Online-Webanwendungen, mit denen Sie Farben zwischen verschiedenen Farbcodes wie RGB, HEX, HSL, HSV, HWB, LAB, CMYK konvertieren können, LCH, XYZ, OKLAB, OKLCH, RGBA, HSLA usw. im Handumdrehen. Farbkonverter sind einfach zu bedienen und funktionieren auf jedem Browser und Betriebssystem. Das Ergebnis erhalten Sie sofort nach Eingabe des zu konvertierenden Farbcodes.

{{<section other-color-converters>}}
---
title: Andere unterstützte Farbkonverter
---