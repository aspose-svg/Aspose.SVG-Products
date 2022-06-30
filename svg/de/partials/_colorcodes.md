---
translation: true
deploy: false
---

{{<section RGB>}}

Der RGB-Farbraum (Rot, Grün, Blau) besteht aus allen möglichen Farben, die durch Mischen von Rot, Grün und Blau erhalten werden können. Dieses Farbmodell ist in der Fotografie, im Fernsehen und in der Computergrafik beliebt. RGB-Werte werden als Ganzzahl zwischen 0 und 255 angegeben. So wird beispielsweise rgb(255,0,0) als rot angezeigt. Der rote Parameter wird auf seinen höchsten Wert (255) gesetzt, und der Rest wird auf 0 gesetzt.<br>
Die C#-Bibliothek Aspose.SVG unterstützt RGB-Prozentsätze (von 0 % bis 100 %). Beispielsweise wird rgb(100%,0,0) als rot angezeigt.


{{<section HEX>}}

HEX-Codes sind die am häufigsten verwendeten Farbcodes. Dies liegt daran, dass sie einfach und leicht zu verstehen sind. HEX-Codes sind nichts anderes als eine hexadezimale Darstellung von RGB. Die sechsstellige Farbnummer ist in drei Zweiergruppen gegliedert, die den Anteil von Rot, Grün und Blau in der Zusatzfarbe angeben. Jedes zweistellige Hexadezimalpaar kann einen Wert von 00 bis FF haben. Dies ergibt über 16 Millionen mögliche Farben. Wenn jede der drei Gruppen Zeichen wie #RRGGBB enthält, können sie als #RGB geschrieben werden. Hexadezimale Farbwerte werden in allen Browsern unterstützt.

{{<section HSL>}}

HSL (Hue, Saturation, Lightness) ist eine Darstellung des RGB-Farbmodells in Zylinderkoordinaten. Der Farbton ist eine beliebige Farbe auf dem Farbkreis; es ist ein Grad auf dem Farbkreis von 0 bis 360. Also ist 0 rot, 120 ist grün, 240 ist blau. Sättigung ist die Intensität oder Reinheit einer Farbe. Es bestimmt, wie lebendig die Farbe sein wird. Beispielsweise ist null Prozent grau und 100 Prozent eine vollständig gesättigte Farbe. Helligkeit ist die Menge an Helligkeit oder Licht in Farbe. Die Helligkeit bestimmt, wie viel Schwarz- oder Weißstich die Farbe hat. Beispielsweise haben 50 Prozent keinen Farbton, null Prozent sind komplett schwarz und 100 Prozent sind komplett weiß.

{{<section HSV>}}

HSV steht für Hue, Saturation und Value (Helligkeitswert). HSV ähnelt HSL, es handelt sich jedoch um zwei unterschiedliche Farbmodelle. Sie basieren beide auf zylindrischen Geometrien, aber HSV basiert auf dem „Hexcone“-Modell, während HSL auf dem „Bi-Hexcone“-Modell basiert. Die Auswahl einer HSV-Farbe beginnt mit der Auswahl eines der verfügbaren Farbtöne und der anschließenden Anpassung der Farbton- und Helligkeitswerte. Hue legt die Position der Farbe auf dem Farbrad fest (von 0 bis 360). Die Sättigung ist ein Sättigungsprozentwert (von 0 % bis 100 %). Helligkeit ist ein Helligkeitsprozentsatz (von 0 % bis 100 %).

{{<section LAB>}}

Wie geografische Koordinaten – Längengrad, Breitengrad und Höhe – geben uns die Farbwerte L*a*b* eine Möglichkeit, Farben zu erkennen. LAB verwendet drei Achsen: L – Helligkeit, a* – vom Rot- zum Grünwert und b* – vom Blau- zum Gelbwert. Die Helligkeit wird in Prozent ausgedrückt und kann 100 % überschreiten. Werte für die a- und b-Achsen können von positiv bis negativ reichen. Es wird üblicherweise auf den Bereich von –128 bis 127 zur Verwendung mit ganzzahligen Codewerten geklemmt. Der LAB-Farbraum und die LAB-Farbcodes werden empfohlen, wenn Sie möchten, dass die Farbe auf dem Bildschirm genauso aussieht wie auf Papier gedruckt.

{{<section LCH>}}

LCH steht für Lightness, Chroma und Hue. Wie bei LAB kann die Helligkeit ein Prozentsatz sein, der 100 % übersteigt. Die Farbkomponenten im LCH-Farbmodell entsprechen ungefähr denen von HSL. Ähnlich wie bei HSL kann der Farbton ein Bereich zwischen 0 und 360 sein. Die LCH-Farbtonwinkel entsprechen jedoch nicht vollständig den Farbtonwerten der gleichen HSL. Chroma stellt die Farbmenge dar, und wir können es uns ähnlich wie die Sättigung in HSL vorstellen. Aber Chroma kann 100 überschreiten - tatsächlich ist es theoretisch unbegrenzt. Der LCH-Farbraum als LAB ist wahrnehmungsmäßig einheitlich, was bedeutet, dass die exakte numerische Änderung der Koordinaten im Farbraum den gleichen Wahrnehmungsunterschied zwischen den Farben ergibt.


{{<section HWB>}}

HWB steht für Hue, Whiteness und Blackness. Das HWB ist den Farbmodellen HSV (Hue, Saturation, Value) und HSL (Hue, Saturation, Lightness) sehr ähnlich, außer dass weder HSV noch HSL eine Weißsättigung liefern. Wie bei HSL und HSV kann der Farbton irgendwo zwischen 0 und 360 liegen. Die anderen beiden Argumente steuern, wie viel Weiß oder Schwarz in diesen Farbton gemischt wird, bis zu 100 % (was zu einer vollständig weißen oder schwarzen Farbe führen würde).  HWB ist besonders nützlich zum Erstellen monochromer Farbpaletten. HWB wird in HTML noch nicht unterstützt, wird aber als neuer Standard in CSS4 vorgeschlagen.


{{<section XYZ>}}

Das XYZ-Farbmodell (CIE 1931 XYZ) ist ein rein mathematischer Raum, der auf den Ergebnissen der CIE-RGB-Version des menschlichen Auges basiert. Im Gegensatz zu RGB, CMYK und anderen Modellen sind die primären Komponenten in XYZ hypothetisch, was bedeutet, dass Sie X, Y und Z keinem Satz von Farben zum Mischen zuordnen können. Diese Farben entsprechen keinen realen Lichtwellenlängen. XYZ ist ein additives Schema von Farbräumen, da es die Mengen von drei Stimuli definiert, die dem Auge zugeführt werden (die drei Primärfarben). XYZ wird häufig in wissenschaftlichen Arbeiten und technischen Bereichen verwendet. Farbbeschreibungen in anderen Farbräumen beziehen sich oft auf ihre Darstellung in diesem Raum.


{{<section RGBA>}}

RGBA-Farbwerte (Rot, Grün, Blau und Alpha) sind eine Erweiterung der RGB-Farbwerte mit einem Alphakanal, der die Deckkraft der Farbe bestimmt. Der Alpha-Parameter ist eine Zahl zwischen 0,0 und 1,0, die die Transparenz angibt. Beispielsweise wird rgba(255, 0, 0) als reines Rot angezeigt, rgba(255, 0, 0, 0,5) wird als Rot mit 50 % Deckkraft angezeigt. Für einen RGBA-Wert gibt es im Gegensatz zu RGB-Werten keine hexadezimale Schreibweise.

{{<section HSLA>}}

Ähnlich wie RGB/RGBA verfügt HSL über einen HSLA-Modus mit Unterstützung für einen Alphakanal zur Angabe der Farbopazität. Der HSLA-Farbwert (Hue, Saturation, Lightness, Alpha) wird mit Farbton, Sättigung, Helligkeit und Alpha angegeben, wobei der Alpha-Parameter die Deckkraft angibt. Der Alpha-Parameter ist eine Zahl zwischen 0,0, was „vollständig transparent“ bedeutet, und 1,0, was „vollständig undurchsichtig“ bedeutet. Beispielsweise wird hsla(0, 100 %, 50 %, 1) als reines Rot angezeigt, hsla (0, 100 %, 50 %, 0,5) wird als rot mit 50 % Deckkraft angezeigt.

{{<section CMYK>}}

CMYK-Farben sind eine Kombination aus Cyan, Magenta, Gelb und Schwarz. Dieses Modell wird als subtraktiv bezeichnet, da Tinten die Farben von Weiß subtrahieren. CMYK ist eines der beliebtesten Farbmodelle. Das CMYK-Farbmodell wird in Druckfarben für Papier verwendet. Dieses Modell enthält viele Farben, aber die Anzahl der Farben ist im Vergleich zu RGB begrenzt. CMYK wird häufig beim Erstellen von Designs für den Druck verwendet, um sicherzustellen, dass die gewünschten Farben genau sind, und niemals für Stylesheets oder HTML. CMYK wird in HTML nicht unterstützt, aber in CSS4 als neuer Standard vorgeschlagen.