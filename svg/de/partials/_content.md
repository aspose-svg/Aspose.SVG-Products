---
translation: true
deploy: false
---

{{<section encode-plugin>}}
---
h2: Bilder online kodieren
---

Codieren Sie Bilder mit [Aspose.SVG for .NET](https://products.aspose.com/svg/{{lang.url-fragment}}net/)-API in Echtzeit! Bitte laden Sie ein Bild aus dem lokalen Dateisystem und Sie erhalten sofort das Ergebnis als Daten-URI, Base64-Bildquelle und Base64-CSS-Hintergrundquelle. JPG, JPEG, PJP, PJPEG, PNG, BMP, XBM, GIF, TIFF, ICO, IFIF, WEBP und andere Bildformate werden unterstützt.

{{<section "app-plugin" i18n-exclude>}}

{{< app/svg/base64 sourceImage="/svg/images/encoder/tulip.jpg">}}
{{< /app/svg/base64>}} 

{{<section encode-online>}}

 - [Base64-Encoder](https://products.aspose.app/svg/encoding) sind eine Reihe von Tools, mit denen Sie Binärdaten in verschiedenen Ausgabeformaten codieren können: Plain Base64, JSON, XML, URI oder CSS.
 - [Image Base64 Decoder](https://products.aspose.app/svg/image-base64-decoder) konvertiert einen Daten-URI, der eine Base64-Zeichenfolge enthält, in ein Bild, indem eine URI-Zeichenfolge in das Eingabesteuerelement eingefügt wird.

Aspose.SVG bietet kostenlose Online-Anwendungen zum Kodieren und Dekodieren von Binärdaten:
 
Unsere browserbasierten Anwendungen funktionieren auf allen Plattformen, einschließlich Windows, Linux, Mac OS, Android und iOS. Für Sie ist keine Registrierung, Plugin- oder Softwareinstallation erforderlich. Beginnen Sie mit der sicheren, sicheren und einfachen Nutzung unserer Online-Base64-Codierungs-/Decodierungstools!

{{<section encode-uri>}}
---
h2: Vor- und Nachteile von Daten-URI
---

Der Daten-URI bietet uns eine clevere Möglichkeit, Bilder auf einer Webseite einzubetten. URI-Schemata können auf viele Arten verwendet werden. Aber in jedem Fall gibt es Vor- und Nachteile.

- Beschleunigung des Ladens von Seiten. Der Browser muss keine zusätzliche Webanforderung stellen, um die Datei abzurufen, da das Bild bereits in das HTML-Dokument eingebettet ist.
- Leistungsverbesserung. Der Browser benötigt weniger CPU-Zeit.
- Webseiten werden unabhängig von externen Dateien, sodass sie auch offline einfach geteilt werden können.

<b>Vorteile:</b>

- Die Größe der Base64-codierten Daten ist 1/3 größer als das Binärbild.
- Die verschlüsselten Bilder werden nicht vom Browser zwischengespeichert und bei jedem Besuch einer solchen Seite heruntergeladen.
- Codierte Bilder sind schwer zu bearbeiten, da die Base64-Zeichenfolge zuerst decodiert werden muss.
- Ein Base64-Bild wird niemals von Google indiziert, da es nicht in den Ergebnissen der Bildersuche erscheint.

<b>Nachteile:</b>

{{<section vectorization-use>}}
---
h2: Wie verwende ich den Bildvektorisierer?
---

1. Laden Sie zunächst das Rasterbild aus einem lokalen Dateisystem im JPEG-, JPG-, PJP-, PJPEG-, WEBP-, PNG-, BMP-, ICO-, GIF-, TIFF-, XBM- oder anderen Bitmap-Format. Sie sehen drei Fenster – Source Image, Quantized Image und Vectorized Image – mit der Vorschau der ursprünglichen, farbquantisierten und vektorisierten Bilder.
1. Image Vectorizer konvertiert {{i18n.informat}} in Vektor mit Standardeinstellungen und Sie können vektorisiertes {{i18n.informat}} als SVG-Datei herunterladen. Aber um ein besseres Ergebnis zu erzielen, können Sie die Quantisierungs- und Vektorisierungsprozesse mit zwei Einstellungsseitenleisten handhaben. Klicken Sie auf die Schaltfläche „Quantize“, um die Quantisierungseinstellungen anzuwenden, klicken Sie auf die Schaltfläche „Vectorize“, um die Vektorisierungseinstellungen anzuwenden und {{i18n.informat}} in SVG umzuwandeln.
1. Klicken Sie auf die Schaltfläche „Download Result“, um das Ergebnis zu erhalten. 

Image Vectorizer wandelt Raster-Bitmap-Bilder in Vektorgrafiken um, die aus Umrissen aufgebaut sind. Der Vektorisierungsalgorithmus umfasst die nächsten Schritte: Farbquantisierung, Konturverfolgung, Spurglättung, Spurvereinfachung und Erstellen von SVG-Pfadelementen aus den Spuren. Wende benutzerdefinierte Einstellungen an, um das beste {{i18n.informat}}-Vektorisierungsergebnis zu erhalten.

<b> Seitenleiste Quantization Options</b>

Die Farbquantisierung ist ein Prozess zur Auswahl einer begrenzten Anzahl von Farben, die in einem Bild verwendet werden sollen. Es wird angewendet, wenn die Farbinformationen eines Bildes reduziert werden sollen. Die Farbquantisierung ist ein sehr komplexer Prozess, an dem eine Reihe von Faktoren beteiligt sind. Dies kann unter Verwendung verschiedener Algorithmen implementiert werden. Jeder der Algorithmen bestimmt, welche Farben aus dem größeren Farbsatz im neuen Bild verbleiben und wie die verworfenen Farben den verbleibenden zugeordnet werden.

 - <b>colors</b> - gewünschte Palettengröße;
 - <b>method</b> - Histogrammmethoden, die verschiedene Farbquantisierungsalgorithmen implementieren;
 - <b>minHueCols</b> - ist ein Parameter, der mit Farbverläufen arbeitet;
 - <b>scale</b> - oder Skalierungsfaktor wird für eine feinere oder gröbere Abtastung der Farben in der Ebene eingestellt.

<b>Seitenleiste Vectorization Options</b>

- <b>tolerance</b> - ist verantwortlich für die Verringerung der Anzahl von Punkten in einer Kurve, die durch eine Reihe von Trace-Punkten angenähert wird, und bestimmt die maximal zulässige Fehlertoleranz, damit ein Punkt aus dem Trace eliminiert werden kann. Der Standardwert ist 0,3;
- <b>tension</b> - ist verantwortlich für das Erstellen von Pfadsegmenten aus der Liste der Verfolgungspunkte. Der Spannungswert bestimmt, wie stark sich die Kurve an den Kontrollpunkten krümmt;
- <b>severity</b> - wirkt sich auf die Glättung von Konturen aus und bestimmt die Ausdehnung der Region, die vom Abfragepunkt des Nearest-Neighbor-Ansatzes betrachtet wird.

Vektorgrafiken eignen sich am besten zum Erstellen von Logos, Symbolen, Seitenlayouts, Karten, Grafiken, Strichzeichnungen, Illustrationen, technischen Zeichnungen und mehr. Es ist nicht das am besten geeignete Format für Halbtonbilder mit Farbübergängen oder die Bearbeitung von Fotos. Das Vektorisieren von Fotos kann jedoch zu beeindruckenden künstlerischen Effekten führen, die interessant und nützlich sein können.