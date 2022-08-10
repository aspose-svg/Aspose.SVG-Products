---
translation: true
template: /templates/_template-merger-child.md
title: GIF zu TIFF über C# zusammenführen - Aspose.SVG
description: Zusammenführen von GIF zu TIFF mithilfe der .NET Core-API unter Windows, macOS und Linux
url: /net/merger/gif-to-tiff/
family: svg
platformtag: net
feature: merge
informat: GIF
outformat: TIFF
otherformats: GIF JPG PNG TIFF BMP
---

{{<section banner>}}
---
h1: GIF zu TIFF über C# zusammenführen
h2: Hochgeschwindigkeits-.NET-API zum Kombinieren von GIF-Dateien unter Windows, macOS und Linux
---

{{<section overview>}}
---
h2: GIF zu TIFF mit C# zusammenführen
---

GIF und TIFF sind Dateiformate, die zum Speichern digitaler Bilder verwendet werden. Sie unterscheiden sich jedoch in der Art und Weise, wie sie verwendet werden. GIF-Dateien haben eine kleine Dateigröße, wodurch sie ideal für die Verwendung auf Websites für Logos, Strichzeichnungen und einfache Cartoons sind. Andererseits ist TIFF bei Grafikern, der Verlagsbranche sowie Amateur- und Berufsfotografen beliebt. Beide Dateiformate haben ihre eigenen Vor- und Nachteile, und in einigen Fällen müssen Sie möglicherweise GIF-Bilder kombinieren und als eine TIFF-Datei speichern. Mit der API [Aspose.SVG for .NET](https://products.aspose.com/svg/net/) können Sie GIF programmgesteuert mit TIFF zusammenführen. Die leistungsstarke C#-API hilft Ihnen, GIF-Dateien schnell und in hoher Qualität zu kombinieren!

{{<section code-text>}}
---
h2: C#-Codebeispiel zum Zusammenführen von GIF zu TIFF
title: GIF zu TIFF zusammenführen – C#
---

Kombinieren Sie mehrere GIF-Dateien und speichern Sie das Ergebnis ganz einfach als einzelne TIFF-Datei! Das Zusammenführen von Bildern kann mit ein paar Zeilen Code erfolgen:

{{<section "code-snippet" i18n-exclude>}}

```cs
// Images to merge 
var images = new string[] { @"image1.gif", "image2.gif" };
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
        Format = ImageFormat.Tiff,
        PageSetup =
        {
            Sizing = SizingType.FitContent
        }
    };    
    // Render document 
    document.RenderTo(new ImageDevice(options, "merged.tiff"));
}
```

{{<section steps>}}
---
h2: Schritte zum Zusammenführen von GIF zu TIFF mit C#
---
1. Definieren Sie GIF-Bilder zum Zusammenführen.
1. Initialisieren Sie eine neue Instanz der Klasse [SVGDocument](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/svgdocument/#constructor).
1. Deklarieren Sie eine Bildfunktion. Sie sollten die Methode [CreateElementNS(`namespaceURI,qualifiedName`)](https://reference.aspose.com/svg/net/aspose.svg.dom/document/createelementns/#createelementns) der SVGDocument-Klasse verwenden, um eine Bildinstanz. Der `namespaceURI` setzt den Verweis auf die W3C-SVG-Spezifikation. Der „qualifiedName“ muss den String-Tag-Namen des Bildelements enthalten.
1. Rufen Sie die Bildfunktion auf, um ein Thumbnail-Objekt zu erstellen.
1. Verwenden Sie zum Hinzufügen von Miniaturansichten zum Dokument die Methode [AppendChild()](https://reference.aspose.com/svg/net/aspose.svg.dom/node/appendchild/#appendchild).
1. Verwenden Sie einen der [ImageRenderingOptions()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagerenderingoptions/)-Konstruktoren, um eine neue Instanz der ImageRenderingOptions-Klasse zu initialisieren. Sie können den Rendering-Prozess anpassen, indem Sie die Seitengröße, das Bildformat usw. angeben. PNG wird als Standardbildformat verwendet.
1. Erstellen Sie eine Instanz von ImageDevice mit dem Konstruktor [ImageDevice()](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/imagedevice/imagedevice/#constructor_3).
1. Rufen Sie die Methode [RenderTo(`device`)](https://reference.aspose.com/svg/net/aspose.svg/svgdocument/renderto/#renderto) auf, um das aktuelle Dokument an das Ausgaberenderinggerät zu senden.
1. Mehrere GIF-Bilder werden in einer TIFF-Datei im angegebenen Pfad gespeichert.



{{<section documentation>}}

Eine Hochgeschwindigkeits-C#-Bibliothek ermöglicht es .NET-Entwicklern, GIF-Dateien schnell und effizient zu einem TIFF-Bild zusammenzuführen. Der Namensraum [Aspose.Svg.Rendering.Image](https://reference.aspose.com/svg/net/aspose.svg.rendering.image/) stellt spezifische Geräteklassen sowie einige für das Rendern zuständige Rendering-Optionsklassen bereit in Rasterformate: JPEG, PNG, BMP, GIF und TIFF. Bitte besuchen Sie <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/" target="_blank">unsere Dokumentation</a>, um mehr zu erfahren mehr über die Verwendung von Aspose.SVG-API-Funktionen.

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
subTitle: "Sie können Bilder in andere Dateiformate zusammenführen:"
---