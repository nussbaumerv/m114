# Bilder Codieren 

## 1
- RGB(255, 255, 255) entspricht der Farbe: Weiß
- RGB(0, 0, 0) entspricht der Farbe: Schwarz
- RGB(252, 178, 91) entspricht der Farbe: Orange
- #FF0000 entspricht der Farbe: Rot
- #00FF00 entspricht der Farbe: Grün
- #0000FF entspricht der Farbe: Blau
- #FFFF00 entspricht der Farbe: Gelb
- #00FFFF entspricht der Farbe: Türkis
- #FF00FF entspricht der Farbe: Magenta
- #000000 entspricht der Farbe: Schwarz
- #FFFFFF entspricht der Farbe: Weiß
- #00BC00 entspricht der Farbe: Grün

## 2

- C:0%, M:100%, Y:100%, K:0% entspricht der Farbe: Rot
- C:100%, M:0%, Y:100%, K:0% entspricht der Farbe: Grün
- C:100%, M:100%, Y:0%, K:0% entspricht der Farbe: Blau
- C:0%, M:0%, Y:100%, K:0% entspricht der Farbe: Gelb
- C:100%, M:0%, Y:0%, K:0% entspricht der Farbe: Cyan
- C:0%, M:100%, Y:0%, K:0% entspricht der Farbe: Magenta
- C:100%, M:100%, Y:100%, K:0% entspricht der Farbe: Schwarz
- C:0%, M:0%, Y:0%, K:100% entspricht der Farbe: Schwarz
- C:0%, M:0%, Y:0%, K:0% entspricht der Farbe: Weiß
- C:0%, M:46%, Y:38%, K:22% entspricht der Farbe: Rot-Braun

## 3

Ein RGB-Bild hat 3 Farbkanäle (Rot, Grün & Blau). Wenn jeder Kanal 8 Bit hat, benötigt jedes Pixel 3 * 8 = 24 Bits.

Das Bild hat 640 x 480 = 307.200 Pixel.

307.200 * 24 Bit/Pixel = 7.372.800 Bits = 921.600 Bytes

## 4

16:9 -> 1920x1080

## 5

30 * 2,54 cm = 76,2 cm

10x^2 * 16x^2 = 76,2^2 cm
356x^2 = 5.806,44 cm
x^2 = 16,31022471910112 cm
x = 4,038591922824232 cm

16 * 4 = 64

64 / 2,54 = 25,19685039370079 ppi

2,54 cm = 100 ppi

## 6

2.000 Pixel / 600 dpi * 2,54 cm = 8,467 cm

## 7

1080 * 1920 * 3 = 6.220.800 Byte

## 8

180 * 6.220.800 Byte = 1.119.744.000 Byte

## 9 

RAW bietet maximale Bearbeitungsmöglichkeiten und höchste Qualität, eignet sich aber eher für professionelle Fotografen, die bereit sind, Zeit in die Nachbearbeitung zu investieren. JPG ist ideal für schnelle, unkomplizierte Anwendungen und das sofortige Teilen von Bildern, jedoch mit geringeren Möglichkeiten in der Postproduktion aufgrund der verlustbehafteten Komprimierung.

## 10 

Für die Veröffentlichung des Gameplay-Videos auf YouTube sollte man das MP4-Format mit H.264-Video-Codec und AAC-Audio-Codec verwenden. Die Bildrate sollte der Aufnahme entsprechen, und die Farbauflösung sollte standardmäßig 8 Bit betragen. Man sollte auf Urheberrechte und Lizenzvereinbarungen achten, um rechtliche Probleme zu vermeiden.

## 11

Interlaced: Halbbilder (Ungerade Zeilen / Gerade Zeilen)
Progressiv: Ganze Bilder

## 12

a. Der Moiré-Effekt ist ein optischer Effekt, bei dem durch Überlagerung von regelmäßigen Rastern ein wiederum periodisches Raster entsteht, das spezielle Strukturen aufweist, die in keinem der Einzelmuster vorhanden sind und bei Veränderung der Überlagerungsweise variieren.
b. Strukturen im Bild, die z.B. durch eine Komprimierung entstehen (DCT: Blockingartefakte)

## 13

1920 x 1080 x 3 Byte = 6.220.800 B
i50 bedeutet 50 Halbbilder pro Sekunde
6.220.800 B x 25 = 155.520.000 B oder 155,52 MB/s bzw. 1,24416 Gb/s

## 14

4700 MB / 155,52 MB/s = 30 Sekunden oder ½ Minute

## 15

4700 MB / 155,52 MB/s = 30 Sekunden oder ½ Minute

## 16

### a. 
Weil die ALU im Mikroprozessor nur "digital" versteht.

### b. Warum geht eine A/D-Wandlung immer mit einem Datenverlust einher?
Je nach Samplingrate und Auflösung verliert man Informationen zwischen den Samples/Messwerten. Würde man das digitalisierte Signal wieder in ein analoges Signal zurückwandeln, erhielte man einen treppenartigen Verlauf. Die Werte zwischen den Stufen bleiben somit unbekannt.

### c.
Je höher die Samplingrate, desto näher kommt die digitale Abbildung dem Original. Bei Musik wird z.B. wegen des menschlichen Hörbereichs von 20 Hz bis 20 kHz die Samplingrate auf 44 kHz festgelegt. Das fordert das sogenannte Abtast-Theorem, das besagt, dass die Samplingfrequenz der doppelten oberen Grenzfrequenz entsprechen muss.