---
translation: true
template: /templates/_template-encoder.md
title: Konvertieren Sie das Bild in Base64 - Online-Encoder und C#-Code
url: /net/base64-encoder/
description: Konvertieren Sie das Bild in Base64. Verwenden Sie als Daten-URIs codierte Base64-Bilder, um sie in HTML, CSS oder JSON einzubetten.
---

{{<section banner>}}
---
h1: Bild in Base64 online oder über C# codieren
h2: Konvertieren Sie das Bild in eine Base64-codierte Zeichenfolge. JPG-, PNG-, BMP-, GIF-, TIFF-, ICO- und SVG-Formate werden unterstützt.
---

{{<section text-plugin>}}
---
h2: Konvertieren Sie das Bild online in Base64
---

{{<section "app-plugin" i18n-exclude>}}

{{< app/svg/base64 inputFormat="Image" sourceImage="/svg/images/encoder/tulip.jpg">}}
{{< /app/svg/base64>}} 

{{<section base64>}}
---
h2: So codieren Sie Bilder mit C#
title: Base64-Codierung
---

Base64 ist ein Codierungsschema zum Konvertieren von Binärdaten in ein ASCII-Textformat. Es wird im Allgemeinen verwendet, um Daten über das Internet zu übertragen. Das Ergebnis der Konvertierung eines Bildes in Base64 ist nur eine Reihe von lateinischen Buchstaben, Zahlen und zwei Zeichen – „+“ und „/“. Jeder Browser weiß, was damit zu tun ist. Mit anderen Worten, Base64 ist eine Art Binär-zu-Text-Codierung.

 Base64 ist besonders im Web verbreitet, wo seine Verwendung die Möglichkeit umfasst, Bilddateien oder andere binäre Ressourcen in Textressourcen wie HTML- und CSS-Dateien einzubetten. Das Einfügen der Bilddaten in die HTML-Datei bedeutet, dass der Browser keine zusätzliche Webanfrage stellen muss, um die Datei abzurufen, da das Bild bereits in das HTML-Dokument eingebettet ist. Es wird empfohlen, die base64-Codierung nur für kleine Bilder zu verwenden. Große base64-Bilder führen zu viel Code in HTML, was zu einem Verlust an Leistungsvorteilen führt. Es sollte auch beachtet werden, dass ein base64-Bild niemals von Google indiziert wird, da es bei der Bildsuche nicht auftaucht.

{{<section demos>}}
---
h2: Bild in Base64 in C# codieren
title: C#-Code zum Konvertieren von PNG-Bildern in Base64
---

In diesem Artikel wird erläutert, wie eine Bilddatei mithilfe von Aspose.SVG-.NET-API-Funktionen in eine Base64-Zeichenfolge codiert wird. Das folgende C#-Beispiel zeigt, wie ein PNG-Bild in eine Base64-Zeichenfolge konvertiert und in eine SVG-Datei eingebettet wird. Die ReadAllBytes(string)-Methode wird verwendet, um ein Bild (Binärdatei) zu öffnen und den Inhalt der Datei in ein Byte-Array einzulesen. Die ToBase64String(bytes)-Methode konvertiert ein Array von 8-Bit-Ganzzahlen in die entsprechende Zeichenfolgendarstellung, die in Basis-64-Ziffern codiert ist. Die Methode AppendChild() fügt dann das base64-codierte Bild zum SVG-Dokument hinzu.

{{<section "code" i18n-exclude>}}

```cs
    // Open a binary file - PNG image
    var bytes = File.ReadAllBytes(@"image.png");
    // Initialize an SVGDocument object
    var document = new SVGDocument();
    // Create an image element
    var img = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
    // Convert image to base64
    img.Href.BaseVal = "data:image/png;charset=utf-8;base64," + Convert.ToBase64String(bytes);
    // Add the image element into the SVG document
    document.RootElement.AppendChild(img);
    // Save the SVG document
    document.Save(@"image-base64.svg");
```

{{<section html>}}
---
h2: Betten Sie ein Base64-Bild in HTML ein
title: HTML-Code zum Einbetten des Base64-Bildes als Daten-URI
text: Base64-kodierte Bilder können mit dem `<img>`-Tag in HTML eingebettet werden. Fügen Sie einfach die Bilddaten mithilfe der Daten-URI direkt in die HTML-Datei ein. Die Verwendung von Base64-Codierung und Daten-URI-Schema reduziert die Anzahl der HTTP-Anforderungen, die ein Browser zum Rendern einer Webseite benötigt. Dieses Code-Snippet zeigt, wie Sie Base64-Bilder in HTML einbetten können.
---

Der Daten-URI besteht aus zwei Teilen, die durch ein Komma getrennt sind. Der erste Teil gibt ein Base64-codiertes Bild an, und der zweite Teil gibt eine Base64-codierte Bildzeichenfolge an:
1. `data:image/jpeg;base64`, ist der Header des Daten-URI-Schemas.
1. `iVBORw0KGgoAAAANSUhEUg...` sind die codierten Base64-Daten.

{{<section css>}}
---
h2: Beispiel für das Einbetten eines Base64-Bildes als CSS-Hintergrundcode
title: CSS-Code zum Einbetten des Base64-Bildes als Daten-URI
---

Eine weitere Möglichkeit, die Anzahl der HTTP-Anfragen für Bilder zu reduzieren, ist die Verwendung der CSS-Eigenschaft `background-image`. Die Eigenschaft `background-image` definiert Bilder als Hintergrund eines Elements. Jedes Bild für die background-image-Eigenschaft kann als URL oder als Bilddaten-URI angegeben werden. Der Unterschied besteht darin, dass im ersten Fall der Browser eine HTTP-Anfrage sendet, um das externe Bild zu erhalten, während im zweiten Fall das base64-Bild direkt in das Dokument eingebettet wird und nicht auf andere Quellen hinweist. Daher muss der Browser keine HTTP-Anforderungen laden, um die Ausgabe zu liefern.

{{<section svg>}}
---
title: SVG-Code zum Einbetten des Base64-Bildes
---

Das Fragment der resultierenden image-base64.svg-Datei ist unten dargestellt. Die Base64-Zeichenfolge wurde abgeschnitten, um das SVG-Codebeispiel nicht zu überladen. Das Format zum Einbetten von Base64-Bildern als URI-Daten ist das folgende, um genau zu sein:

`data:[<mime type>][;charset=<charset>][;base64],<codierte Daten>`


{{<section "code-svg" i18n-exclude>}}

```cs
<svg xmlns="http://www.w3.org/2000/svg">
	<image href="data:image/png;charset=utf-8;base64,iVBORw0KGgoAAAANSUhEUg..." alt="Red border"/>
</svg>
```

{{<section "code-html" i18n-exclude>}}

```cs
<body>
    <div>
        <img src="data:image/jpeg;base64,iVBORw0KGgoAAAANSUhEUg..." alt="Red border">
    </div>
</body>
```

{{<section "code-css" i18n-exclude>}}

```cs
body {
    background-image: url('data:image/jpeg;base64,iVBORw0KGgoAAAANSUhEUg...');
}
```

{{<section encoder-online>}}
---
h2: Online-Base64-Encoder
---

Online-<a href="https://products.aspose.app/svg/{{lang}}/encoding" target="_blank">Base64-Encoder</a> konvertieren den Inhalt von SVG-Dokumenten oder Bilddateien in sein Äquivalent Zeichenfolgendarstellung, die mit Base-64-Ziffern codiert ist. Sie bieten auch Beispiele für Daten-URI, JSON, XML und andere. Codierungstools helfen Ihnen, verschiedene Datencodierungsprobleme zu vermeiden, die Website-Inhalte oder E-Mail-Nachrichten unlesbar machen. Base64-Encoder sind sicher, einfach zu verwenden und völlig kostenlos. Sie funktionieren in jedem Browser und auf jedem Betriebssystem.

{{<section installing>}}
---
h2: Aspose.SVG für die .NET-Bibliothek installieren
---

Aspose.SVG für .NET ist eine plattformübergreifende flexible Bibliothek, die entwickelt wurde, um eine breite Palette von Funktionen zum Verarbeiten und Rendern von SVG-Dokumenten bereitzustellen. Es lässt sich nahtlos in Ihre .NET-Apps integrieren, um mit SVG-Dateien zu arbeiten, ohne Software von Drittanbietern zu installieren. Unsere SVG .NET-API kann mit jeder .NET-Sprache wie C#, VB.NET, ASP.NET usw. verwendet werden. Sie funktioniert gleichermaßen gut auf jedem Betriebssystem, das Mono installieren (.NET 4.0 Framework-Unterstützung) oder .NET verwenden kann Ader. Dazu gehören Windows, Linux und macOS.

Installieren von <a href="https://www.nuget.org/packages/Aspose.SVG" target="_blank">Aspose.SVG für .NET über NuGet</a>:
1. Verwenden der Paket-Manager-Konsole.
1. Verwenden der NuGet Package Manager-GUI.

Weitere Einzelheiten zur Installation der C#-Bibliothek finden Sie in der [Aspose.SVG-Dokumentation.](https://docs.aspose.com/svg/net/getting-started/installation/)

{{<section other-encoders>}}
---
h2: Andere unterstützte Encoder
---

Sie können auch SVG- oder Bilddateien in Base64 codieren: