---
translation: true
template: /templates/_template-encoder-child.md
title: Konvertieren Sie TIFF in Base64 - Online-Encoder und C#-Code
description: Konvertieren Sie TIFF in Base64 und verwenden Sie eine codierte Zeichenfolge für den Daten-URI. Betten Sie es in HTML, CSS, XML, JSON.
url: /net/tiff-to-base64/
family: svg
platformtag: net
feature: encode
informat: TIFF
outformat: Base64
---

{{<section banner>}}
---
h1: Konvertieren Sie TIFF in Base64 online oder über C#
h2: Codieren Sie TIFF in eine Base64-Zeichenfolge in C# und verwenden Sie sie als Beispiele für Daten-URI
---

{{<section overview>}}
---
h2: Über das URI-Schema
---

Daten-URI ist eine Methode zum Einbetten von Bildern und anderen Dateien in Webseiten als Textzeichenfolge basierend auf Base64-Codierung. Mit dem Daten-URI-Schema können Sie beliebige Binärdaten in HTML-, CSS-, JSON- oder SVG-Dokumente einfügen. Sie können beispielsweise Bilder in eine Webseite einbetten, als ob sie von einer externen Ressource geladen würden, aber anstatt die URL der Datei anzugeben, fügen Sie den Base64-codierten Inhalt des Bildes ein. Das Daten-URI-Schema wurde in RFC 2397 definiert und wird ab 2022 von den meisten gängigen Browsern vollständig unterstützt. Der Hauptvorteil der Verwendung von Daten-URIs ist eine Beschleunigung des Seitenladens, da der Browser keine zusätzliche Webanforderung stellen muss, um die Datei abzurufen, da das Bild bereits in das HTML-Dokument eingebettet ist.

Die Syntax des Daten-URI lautet wie folgt: `data:[<mime type>][;charset=<charset>][;base64],<codierte Daten>`.

Da die Größe von Base64-codierten Daten um 33 % zunimmt, wird empfohlen, Daten-URI nur für kleine Bilder zu verwenden. Große Base64-Bilder erzeugen viel Code im HTML, was zu einem Verlust an Leistungsvorteilen führt. Wenn Sie TIFF in Base64 konvertieren und codierte Zeichenfolgen zum Einbetten in eine HTML-, CSS-, JSON- oder SVG-Datei verwenden müssen, lernen Sie bitte zuerst alle Vor- und Nachteile kennen.

{{<section code-text>}}
---
h2: So konvertieren Sie TIFF in Base64 in C#
title: C#-Code zum Konvertieren von TIFF in eine Base64-Zeichenfolge und zum Einbetten in eine SVG-Datei
---

Um TIFF in Base64-Strings zu konvertieren, verwenden wir die API [Aspose.SVG for .NET](https://products.aspose.com/svg/net/), eine funktionsreiche, leistungsstarke und einfach zu bedienende API. Verwenden Sie die Dokumentmanipulations-API für die C#-Plattform. Wir betrachten das Beispiel der TIFF-zu-Base64-Codierung und Einbettung der Base64-Zeichenfolge als Daten-URI in ein SVG-Dokument. Diese Operationen können mit ein paar Zeilen Code durchgeführt werden:

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open a binary file - TIFF image
    var bytes = File.ReadAllBytes(@"image.tiff");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert TIFF to Base64
    img.Href.BaseVal = "data:image/tiff;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: Schritte zum Konvertieren von TIFF in Base64 in C#
---
1. Öffnen Sie ein zu konvertierendes TIFF-Bild. Verwenden Sie die ReadAllBytes(`path`)-Methode, um das TIFF-Bild zu öffnen und den Inhalt der Datei in ein Byte-Array einzulesen.
1. Initialisieren Sie eine neue Instanz der Klasse [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor).
1. Verwenden Sie die Methode [CreateElementNS(`namespaceURI,qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) der SVGDocument-Klasse, um eine zu erstellen Bildinstanz. Der `namespaceURI` setzt den Verweis auf die W3C-SVG-Spezifikation. Der „qualifiedName“ muss den String-Tag-Namen des Bildelements enthalten.
1. Konvertieren Sie TIFF in Base64. Rufen Sie die ToBase64String(bytes)-Methode auf, um ein Array von 8-Bit-Ganzzahlen in die entsprechende Zeichenfolgendarstellung zu konvertieren, die in Base64-Ziffern codiert ist.
1. Fügen Sie das Bildelement mit der Methode [AppendChild(`node`)](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/) zum SVG-Dokument hinzu.
1. Verwenden Sie die Methode [Save(`path`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/), um das SVG-Dokument zu speichern.




{{<section online-encoder>}}
---
h2: Online-Base64-Encoder
---

{{<section examples>}}
---
h2: Anwendungsbeispiele für die Base64-Codierung
svg: SVG-Code zum Einbetten eines Base64-TIFF-Bildes in ein SVG-Dokument
html: HTML-Code zum Einbetten des Base64-TIFF-Bildes
css: CSS-Code zum Einbetten eines Base64-TIFF-Bildes als Hintergrundbild
xml: XML-Code zum Einbetten eines Base64-TIFF-Bildes in ein XML-Dokument
json: JSON-Code zum Einbetten des Base64-TIFF-Bildes in das JSON-Dokument
---

{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/tiff;charset=utf-8;base64,SUkqAAgAAAAUAP4ABAABAAAAAAAAAAABAw..." alt="Blue circle"/>
</svg>
```

{{<section code-html>}}

```cs
<body>
    <div>
        <img src="data:image/tiff;base64,SUkqAAgAAAAUAP4ABAABAAAAAAAAAAABAw..." alt="Blue circle">
    </div>
</body>
```

{{<section code-css>}}

```cs
.class {
    background-image: url('data:image/tiff;base64,SUkqAAgAAAAUAP4ABAABAAAAAAAAAAABAw...');
}
```

{{<section code-xml>}}

```cs
<?xml version="1.0" encoding="UTF-8"?>
<root>
<image mime = "image/tiff">SUkqAAgAAAAUAP4ABAABAAAAAAAAAAABAw...</image>
</root>
```

{{<section code-json>}}

```cs
{
  "image": {
    "mime": "image/tiff",
    "data": "SUkqAAgAAAAUAP4ABAABAAAAAAAAAAABAw..."
  }
}
```

{{<section other-encoders>}}
---
title: Andere unterstützte Base64-Encoder
subTitle: "Sie können ein Bild in eine Base64-Zeichenfolge konvertieren – die Formate JPG, PNG, BMP, GIF, TIFF, ICO und SVG werden unterstützt:"
---