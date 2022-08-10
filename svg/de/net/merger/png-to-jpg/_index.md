---
translation: true
template: /templates/_template-merger-child.md
title: Zusammenführen von PNG zu JPG über C# - Aspose.SVG
description: Zusammenführen von PNG in JPG mit C# unter Windows, macOS und Linux
url: /net/merger/png-to-jpg/
family: svg
platformtag: net
feature: merge
informat: PNG
outformat: JPG
otherformats: GIF JPEG PNG TIFF BMP
---

{{<section banner>}}
---
h1: PNG zu JPG über C# zusammenführen
h2: Hochgeschwindigkeits-.NET-API zum Kombinieren von PNG-Dateien unter Windows, macOS und Linux
---

{{<section overview>}}
---
h2: PNG zu JPG mit C# zusammenführen
---

PNG bezieht sich auf eine Art von Rasterbilddateiformat, das verlustfreie Komprimierung verwendet, was es bei Benutzern beliebt macht. Manchmal werden Sie mit der alles entscheidenden Frage konfrontiert, ob Sie Ihre digitalen Bilder als JPG- oder PNG-Dateien speichern sollen. Dies sind zwei der beliebtesten Rasterbilddateitypen, die online verwendet werden, und beide Dateiformate haben ihre eigenen Vor- und Nachteile. In vielen Fällen müssen Sie möglicherweise PNG-Bilder kombinieren und als eine JPG-Datei speichern. Mit der API [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) können Sie PNG programmgesteuert mit JPG zusammenführen. Die leistungsstarke C#-API hilft Ihnen, PNG-Dateien schnell und in hoher Qualität zu kombinieren!

{{<section code-text>}}
---
h2: C#-Codebeispiel zum Zusammenführen von PNG zu JPG
title: PNG zu JPG zusammenführen - C#
---

Kombinieren Sie mehrere PNG-Dateien und speichern Sie das Ergebnis ganz einfach als einzelnes JPG! Das Zusammenführen von Bildern kann mit ein paar Zeilen Code erfolgen:

{{<section "code-snippet" i18n-exclude>}}

```cs
// Images to merge 
var images = new string[] { @"image1.png", "image2.png" };
// Initialize a new instance of SVGDocument
using (var document = new SVGDocument())
{
    // Declare an image function
    SVGImageElement CreateThumbnail(string imagePath, int width, int height)
    {
        var image = (SVGImageElement)document.CreateElementNS("http://www.w3.org/2000/svg", "image");
        image.Href.BaseVal = imagePath;
        image.Width.BaseVal.Value = width;
        image.Height.BaseVal.Value = height;
        return image;
    }
    // Set a thumbnail size
    const int thumbnailWidth = 200;
    const int thumbnailHeight = 200;
    const int thumbnailMargin = 10;
    // Create thumbnails merging loop
    for (var i = 0; i < images.Length; i++)
    {
        // Create a thumbnail
        var thumbnail = CreateThumbnail(images[i], thumbnailWidth, thumbnailHeight);
        // Define coordinates 
        thumbnail.X.BaseVal.Value = 0;
        thumbnail.Y.BaseVal.Value = (thumbnailHeight + thumbnailMargin) * i;
        // Append the thumbnail to the document
        document.DocumentElement.AppendChild(thumbnail);
    }
    // Define saving options
    var options = new ImageRenderingOptions
    {
        Format = ImageFormat.Jpeg,
        PageSetup =
        {
            Sizing = SizingType.FitContent
        }
    };    
    // Render document 
    document.RenderTo(new ImageDevice(options, "merged.jpg"));
}
```

{{<section steps>}}
---
h2: Schritte zum Zusammenführen von PNG zu JPG mit C#
---
1. Definieren Sie zusammenzuführende PNG-Bilder.
1. Initialisieren Sie eine neue Instanz der Klasse [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor).
1. Deklarieren Sie eine Bildfunktion. Sie sollten die Methode [CreateElementNS(`namespaceURI,qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) der SVGDocument-Klasse verwenden, um eine Bildinstanz. Der `namespaceURI` setzt den Verweis auf die W3C-SVG-Spezifikation. Der „qualifiedName“ muss den String-Tag-Namen des Bildelements enthalten.
1. Rufen Sie die Bildfunktion auf, um ein Thumbnail-Objekt zu erstellen.
1. Verwenden Sie zum Hinzufügen von Miniaturansichten zum Dokument die Methode [AppendChild()](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/#appendchild).
1. Verwenden Sie einen der [ImageRenderingOptions()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/)-Konstruktoren, um eine neue Instanz der ImageRenderingOptions-Klasse zu initialisieren. Sie können den Rendering-Prozess anpassen, indem Sie die Seitengröße, das Bildformat usw. angeben. PNG wird als Standardbildformat verwendet.
1. Erstellen Sie eine Instanz von ImageDevice mit dem Konstruktor [ImageDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/imagedevice/#constructor_3).
1. Rufen Sie die Methode [RenderTo(`device`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/#renderto) auf, um das aktuelle Dokument an das Ausgaberenderinggerät zu senden.
1. Mehrere PNG-Bilder werden in einer JPG-Datei im angegebenen Pfad gespeichert.



{{<section documentation>}}

Eine Hochgeschwindigkeits-C#-Bibliothek ermöglicht es .NET-Entwicklern, PNG-Dateien schnell und effizient zu einem JPG-Bild zusammenzuführen. Der Namensraum [Aspose.Svg.Rendering.Image](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/) stellt spezifische Geräteklassen sowie einige für das Rendern zuständige Rendering-Optionsklassen bereit in Rasterformate: JPEG, PNG, BMP, GIF und TIFF. Bitte besuchen Sie <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">unsere Dokumentation</a>, um mehr zu erfahren mehr über die Verwendung von Aspose.SVG-API-Funktionen.

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
subTitle: "Sie können Bilder mit anderen Dateiformaten zusammenführen:"
---