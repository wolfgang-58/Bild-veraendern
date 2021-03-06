# Bild verändern 2.24
Dieses Script funktioniert mit den Dateimanagern Nemo, Caja, Nautilus und Thunar.

Damit - Bild verändern - ordentlich arbeiten kann braucht es einige installierte Programme auf dem Rechner:
- **ImageMagick** Softwarepaket zur Erstellung und Bearbeitung von Rastergrafiken.
- **yad** (Yet Another Dialog) ermöglicht das Erzeugen grafischer Dialoge.
- **img2pdf** zum erzeugen von PDF-Dateien
- **libheif-example** um Apple HEIC Fotos zu konvertieren


Die benötigten Scripte und Dateien für - Bild verändern - sind:

- **bildveraendern.sh** Programmscript
- **bildveraendern.nemo_action** zum einbinden und Steuerung des Scriptes in >Nemo<
- **xfce-action.txt** zum einbinden und Steuerung des Scriptes in >xfce<
- **install.sh** zum installieren des Programms
- **inst_cmd.sh** das eigentliche Installationscript
- **Thema** in diesem Ordner sind GTK-Themen für das Programmscript.

Nach dem Download von Github müssen die Scripe noch ausführbar gemacht werden
Im Terminal:

_chmod +x bildveraendern.sh install.sh inst_cmd.sh_

Für die Installation liegt dem gepacktem Paket eine >install.sh< bei, mit dieser ist die Installation schnell erledigt.
Auch eine >Deinstallation< ist damit möglich.
Das Script entweder im Terminal oder mit doppelklick & ausführen starten.
Unter >xfce< muss die >install.sh< im Terminal gestartet werden:

_./install.sh_

Sollte die Installation nicht starten ist eventuell das Terminalprogramm nicht mit dem Desktop kompatibel.
In diesem Fall kann die Installation, unter jedem Desktop, mit folgendem Befehl gestartet werden:

_./install.sh -simple_

Das Script führt durch die Installation und die Schritte sind selbsterklärend.
Eine manuellen Installation ist nicht möglich!

**Folgende Einstellungen können während der Installation festgelegt werden:**

Fehlende externe Programm können während der Installation installiert werden.

**Auswahl des Dateimanagers**
- Nemo
- Caja
- Thunar
- Nautilus

**Auswahl des Style**
- flächig Mintfarben
- Rand Mintfarben
- Desktop Einstellunegn

**Höhe und Breite anpassen**

Bei einigen Themen und einer größeren Schrift kann es zu Problemen mit der Darstellung kommen. Dann müssen Höhe und Breite des Programmfensters angepasst werden
Höhe=300, Breite=300 sind die Standardvorgaben damit wird das Programmfenster im kleinstmöglichen Format dargestellt.

**Festlegen der Position des Programmfensters**

Wird >Bild verändern< über das Kontextmenü aufgerufen kann die Position des Programmfenster festgelegt werden.
Es besteht die Möglichkeit das Programmfenster an der Mausposition oder in der Bildschirmmitte zu platzieren

**Festlegen der Betriebsart**
 
Die Betriebsart >action< oder >script< wird während der Installation festgelegt. 
Folgende Betriebsarten können gewählt werden:

Nemo:		action		script

Caja:				    script

Nautilus:			    script

Thunar:			        script

Nur beim Dateimanager -Nemo- steht -Bild veändern- in zwei Betriebsarten zur Verfügung
Dies ist zum einen die Betriebsart -action- und zum anderen die Betriebsart -script-.
Bei der Betriebsart -action- steht -Bild verändern- direkt im Kontextmenü  zur Verfügung. 
Bei der Betriebsart -script- muss -Bild verändern- über den Kontextmenüpunkt -Scripte- aufgerufen werden.
Für die Dateimanager: Caja, Nautilus und Thunar steht nur die Betriebsart -script-  zur Verfügung .
Aufruf von -Bild veändern- für die folgenden Dateimanager:

Caja - im Kontextmenü über -Scripte-

Nautilus - im Kontextmenü über -Scripte-

Thunar - direkt im Kontextmenü

Die Betriebsarten sind in ihrer Funktionalität völlig gleichwertig.

**Verwendung**

Aufruf des Programms, es können eine oder mehrere Bilddateien unterschiedlicher Formate im Dateimanager markiert werden. Nach betätigen der >rechten Maustaste< ist - Bild verändern - im Kontextmenü direkt oder über Scripte auswählbar.
Neben der Konvertierung der Bilddateien ist es auch möglich aus den Dateien eine PDF-Datei zu erzeugen oder
die Dateien in eine x.tar.gz Datei zu packen. Für die PDF Dateien steht eine verlustbehaftete oder eine verlustfrei Option zur Verfügung. Die verlustbehaftete Version enthält ein Lese- Inhaltsverzeichnis.

Nach dem Aufruf steht das Programmfenster sofort zur Verfügung, es besteht die Möglichkeit über die Einstellungen die Startwerte des Programmes festzulegen.

![Programm - Einstellungsfenster](https://user-images.githubusercontent.com/77605776/148199581-e946ccfd-1f0c-4efd-aec4-0ad16ad25ccb.png)

Von -Bild verändern- werden die folgenden Dateiformate verarbeitet:

- jpg:	Skalierung und Qualität frei wählbar - Konvertierung ->Ja< überschreiben ->Ja< 
- jpeg:	Skalierung und Qualität frei wählbar - Konvertierung ->Ja< überschreiben ->Ja< 
- bmp:	Skalierung und Qualität frei wählbar - Konvertierung ->Ja< überschreiben ->Ja< 
- gif:	Skalierung und Qualität frei wählbar - Konvertierung ->Ja< überschreiben ->Ja< 
- webp:	Skalierung und Qualität frei wählbar - Konvertierung ->Ja< überschreiben ->Ja< 
- png:	Skalierung und Qualität frei wählbar - Konvertierung ->Ja< überschreiben ->Nein< *
- tif:	Skalierung und Qualität frei wählbar - Konvertierung ->Ja< überschreiben ->Nein< *
- tiff:	Skalierung und Qualität frei wählbar - Konvertierung ->Ja< überschreiben ->Nein< *
- HEIC(optional): Wird immer verlustfrei nach *.png konvertiert.

*) Bei *.png *.tif und *.tiff ist beim überschreiben nur die Skalierung wirksam, eine Komprimierung mit der Qualitätseinstellung ist nicht wirksam.


Eine detailierte Beschreibung befindet sich in der Datei:

_Beschreibung -Bild verändern- Version 2.24.pdf_
