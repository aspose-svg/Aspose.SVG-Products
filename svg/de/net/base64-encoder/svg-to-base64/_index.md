---
translation: true
template: /templates/_template-encoder-child.md
title: Konvertieren Sie SVG in C# in Base64
description: Konvertieren Sie SVG in C# in Base64 und verwenden Sie eine codierte Zeichenfolge für den Daten-URI. Betten Sie es in HTML, CSS, XML, JSON und andere ein.
url: /net/svg-to-base64/
family: svg
platformtag: net
feature: encode
informat: SVG
outformat: Base64
---

{{<section banner>}}
---
h1: Konvertieren Sie SVG in C# in Base64
h2: Codieren Sie das SVG-Bild in C# in eine Base64-Zeichenfolge und verwenden Sie es als Beispiel für Daten-URI
---

{{<section overview>}}
---
h2: Über das URI-Schema
---

Daten-URI ist eine Methode zum Einbetten von Bildern und anderen Dateien in Webseiten als Textzeichenfolge basierend auf Base64-Codierung. Mit dem Daten-URI-Schema können Sie beliebige Binärdaten in HTML-, CSS-, JSON- oder SVG-Dokumente einfügen. Sie können beispielsweise Bilder in eine Webseite einbetten, als ob sie von einer externen Ressource geladen würden, aber anstatt die URL der Datei anzugeben, fügen Sie den Base64-codierten Inhalt des Bildes ein. Der Hauptvorteil der Verwendung von Daten-URIs ist eine Beschleunigung des Seitenladens, da der Browser keine zusätzliche Webanforderung stellen muss, um die Datei abzurufen, da das Bild bereits in das HTML-Dokument eingebettet ist.

Die Syntax des Daten-URI lautet wie folgt: `data:[<mime type>][;charset=<charset>][;base64],<codierte Daten>`.

SVG-Dateien können „unsichere“ Zeichen enthalten. Vektorgrafiken können Raster als eingebetteten Inhalt oder Attribute haben, deren Werte in einfachen oder doppelten Anführungszeichen stehen. Daher ist eine Vorverarbeitung (Normalisierung) dieses Formats erforderlich. Sie können SVG in HTML oder CSS über Daten-URI verwenden. Wenn SVG mit Daten-URI codiert ist, funktioniert es in jedem Browser.

{{<section code-text>}}
---
h2: So konvertieren Sie SVG in Base64 in C#
title: C#-Code zum Konvertieren von SVG in eine Base64-Zeichenfolge und zum Einbetten in eine SVG-Datei
---

Um das SVG-Bild in eine Base64-Zeichenfolge zu konvertieren, verwenden wir die API [Aspose.SVG for .NET](https://products.aspose.com/svg/net/), die eine funktionsreiche, leistungsstarke und einfach zu bedienende API ist - Verwenden Sie die Dokumentbearbeitungs-API für die C#-Plattform. Wir betrachten das Beispiel eines SVG-Bildes für die Base64-Codierung und das Einbetten einer Base64-Zeichenfolge als Daten-URI in ein SVG-Dokument. Diese Operationen können mit ein paar Zeilen Code durchgeführt werden:

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open an SVG image
    var bytes = File.ReadAllBytes(@"flower.svg");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert SVG image to Base64
    img.Href.BaseVal = "data:image/svg+xml;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: Schritte zum Konvertieren von SVG in Base64 in C#
---
1. Öffnen Sie ein zu konvertierendes SVG-Bild. Verwenden Sie die ReadAllBytes(`path`)-Methode, um das SVG-Bild zu öffnen und den Inhalt der Datei in ein Byte-Array einzulesen.
1. Initialisieren Sie eine neue Instanz der Klasse [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor).
1. Verwenden Sie die Methode [CreateElementNS(`namespaceURI,qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) der SVGDocument-Klasse, um eine zu erstellen Bildinstanz. Der `namespaceURI` setzt den Verweis auf die W3C-SVG-Spezifikation. Der „qualifiedName“ muss den String-Tag-Namen des Bildelements enthalten.
1. Konvertieren Sie SVG in Base64. Rufen Sie die ToBase64String(bytes)-Methode auf, um ein Array von 8-Bit-Ganzzahlen in die entsprechende Zeichenfolgendarstellung zu konvertieren, die in Base64-Ziffern codiert ist.
1. Fügen Sie das Bildelement mit der Methode [AppendChild(`node`)](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/) zum SVG-Dokument hinzu.
1. Verwenden Sie die Methode [Save(`path`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/), um das SVG-Dokument zu speichern.




{{<section online-encoder>}}
---
h2: Online-Base64-Encoder
---

{{<section examples>}}
---
h2: Anwendungsbeispiele für die Base64-Codierung
svg: SVG-Code zum Einbetten eines Base64-SVG-Bilds in ein SVG-Dokument
html: HTML-Code zum Einbetten des Base64-SVG-Bilds
css: CSS-Code zum Einbetten eines Base64-SVG-Bilds als Hintergrundbild
xml: XML-Code zum Einbetten eines Base64-SVG-Bilds in ein XML-Dokument
json: JSON-Code zum Einbetten des Base64-SVG-Bilds in das JSON-Dokument
---

{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/svg+xml;charset=utf-8;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..." alt="Blue flower"/>
</svg>
```

{{<section code-html>}}

```cs
<body>
    <div>
        <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..." alt="Blue flower">
    </div>
</body>
```

{{<section code-css>}}

```cs
.class {
    background-image: url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDUwIiBoZWlna...');
}
```

{{<section code-xml>}}

```cs
<?xml version="1.0" encoding="UTF-8"?>
<root>
<image mime = "image/svg+xml">PHN2ZyB3aWR0aD0iNDUwIiBoZWlna...</image>
</root>
```

{{<section code-json>}}

```cs
{
  "image": {
    "mime": "image/svg+xml",
    "data": "PHN2ZyB3aWR0aD0iNDUwIiBoZWlna..."
  }
}
```

{{<section other-encoders>}}
---
title: Andere unterstützte Base64-Encoder
subTitle: "Sie können ein Bild in eine Base64-Zeichenfolge konvertieren – die Formate JPG, PNG, BMP, GIF, TIFF, ICO und SVG werden unterstützt:"
---