---
translation: true
template: /templates/_template-encoder-child.md
title: Konvertieren Sie PNG in Base64 - Online-Encoder und C#-Code
description: Konvertieren Sie PNG in Base64 online oder in C# und verwenden Sie eine codierte Zeichenfolge für den Daten-URI. Betten Sie es in HTML, CSS.
url: /net/png-to-base64/
family: svg
platformtag: net
feature: encode
informat: PNG
outformat: Base64
---

{{<section banner>}}
---
h1: Konvertieren Sie PNG in Base64 online oder über C#
h2: Codieren Sie PNG in eine Base64-Zeichenfolge und verwenden Sie es als Beispiel für Daten-URI
---

{{<section overview>}}
---
h2: Über das URI-Schema
---

Daten-URI ist eine Methode zum Einbetten von Bildern und anderen Dateien in Webseiten als Textzeichenfolge basierend auf Base64-Codierung. Mit dem Daten-URI-Schema können Sie beliebige Binärdaten in HTML-, CSS-, JSON- oder SVG-Dokumente einfügen. Sie können beispielsweise Bilder in eine Webseite einbetten, als ob sie von einer externen Ressource geladen würden, aber anstatt die URL der Datei anzugeben, fügen Sie den Base64-codierten Inhalt des Bildes ein. Das Daten-URI-Schema wurde in RFC 2397 definiert und wird ab 2022 von den meisten gängigen Browsern vollständig unterstützt. Der Hauptvorteil der Verwendung von Daten-URIs ist eine Beschleunigung des Seitenladens, da der Browser keine zusätzliche Webanforderung stellen muss, um die Datei abzurufen, da das Bild bereits in das HTML-Dokument eingebettet ist.

Die Syntax des Daten-URI lautet wie folgt: `data:[<mime type>][;charset=<charset>][;base64],<codierte Daten>`.

Da die Größe von Base64-codierten Daten um 33 % zunimmt, wird empfohlen, Daten-URI nur für kleine Bilder zu verwenden. Große Base64-Bilder erzeugen viel Code im HTML, was zu einem Verlust an Leistungsvorteilen führt. Wenn Sie PNG in Base64 konvertieren und eine codierte Zeichenfolge zum Einbetten in eine Textdatei verwenden müssen, lernen Sie bitte zuerst alle Vor- und Nachteile kennen.

{{<section code-text>}}
---
h2: So konvertieren Sie PNG in Base64 in C#
title: C#-Code zum Konvertieren von PNG in eine Base64-Zeichenfolge und zum Einbetten in eine SVG-Datei
---

Um PNG in eine Base64-Zeichenfolge zu konvertieren, verwenden wir die API [Aspose.SVG for .NET,](https://products.aspose.com/svg/net/) eine funktionsreiche, leistungsstarke und einfach zu verwendende API. Verwenden Sie die Dokumentbearbeitungs-API für die C#-Plattform. Wir betrachten das Beispiel der Kodierung von PNG zu Base64 und der Einbettung der Base64-Zeichenfolge als Daten-URI in ein SVG-Dokument. Diese Operationen können mit ein paar Zeilen Code durchgeführt werden:

{{<section "code-snippet" i18n-exclude>}}

```cs
    // Open a binary file - PNG image
    var bytes = File.ReadAllBytes(@"image.png");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert PNG to Base64
    img.Href.BaseVal = "data:image/png;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section steps>}}
---
h2: Schritte zum Konvertieren von PNG in Base64 in C#
---
1. Öffnen Sie das zu konvertierende PNG-Bild. Verwenden Sie die ReadAllBytes(`path`)-Methode, um PNG zu öffnen und den Inhalt der Datei in ein Byte-Array einzulesen.
1. Initialisieren Sie eine neue Instanz der Klasse [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor).
1. Verwenden Sie die Methode [CreateElementNS(`namespaceURI,qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) der SVGDocument-Klasse, um eine zu erstellen Bildinstanz. Der `namespaceURI` setzt den Verweis auf die W3C-SVG-Spezifikation. Der „qualifiedName“ muss den String-Tag-Namen des Bildelements enthalten.
1. Konvertieren Sie PNG in Base64. Rufen Sie die ToBase64String(bytes)-Methode auf, um ein Array von 8-Bit-Ganzzahlen in die entsprechende Zeichenfolgendarstellung zu konvertieren, die in Base64-Ziffern codiert ist.
1. Fügen Sie das Bildelement mit der Methode [AppendChild(`node`)](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/) zum SVG-Dokument hinzu.
1. Rufen Sie die Methode [Save(`path`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/save/) auf, um das SVG-Dokument zu speichern.




{{<section online-encoder>}}
---
h2: Online-Base64-Encoder
---

{{<section examples>}}
---
h2: Anwendungsbeispiele für die Base64-Codierung
svg: SVG-Code zum Einbetten von Base64-PNG-Bildern in ein SVG-Dokument
html: HTML-Code zum Einbetten des Base64-PNG-Bildes
css: CSS-Code zum Einbetten eines Base64-PNG-Bilds als Hintergrundbild
xml: XML-Code zum Einbetten von Base64-PNG-Bildern in ein XML-Dokument
json: JSON-Code zum Einbetten des Base64-PNG-Bildes in das JSON-Dokument
---

{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/png;charset=utf-8;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAg..." alt="Red circle"/>
</svg>
```

{{<section "code-html" i18n-exclude>}}

```cs
<body>
    <div>
        <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAg..." alt="Red circle">
    </div>
</body>
```

{{<section "code-css" i18n-exclude>}}

```cs
.class {
    background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAg...');
}
```

{{<section "code-xml" i18n-exclude>}}

```cs
<?xml version="1.0" encoding="UTF-8"?>
<root>
<image mime = "image/png">iVBORw0KGgoAAAANSUhEUgAAACAAAAAg...</image>
</root>
```

{{<section "code-json" i18n-exclude>}}

```cs
{
  "image": {
    "mime": "image/png",
    "data": "iVBORw0KGgoAAAANSUhEUgAAACAAAAAg..."
  }
}
```

{{<section other-encoders>}}
---
title: Andere unterstützte Base64-Encoder
subTitle: "Sie können das Bild in eine Base64-Zeichenfolge konvertieren. JPG-, PNG-, BMP-, GIF-, TIFF-, ICO- und SVG-Formate werden unterstützt:"
---