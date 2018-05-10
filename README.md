# KlimaMonitorWP
WordPress Plugin for KlimaMonitorRasp

Dieses Plugin ermöglicht die Darstellung einer Wettervorhersage, welche mit dem RaspberryPi berechnet wurde. Die notwendigen Daten werden durch Sensoren am GrovePi+ Shield ermittelt.
Aktuell werden Temperatur, Luftfeuchtigkeit und Luftdruck gemessen. Die gemessenen und berechneten Daten, werden in der WordPress Datenbank gespeichert und sind durch Liniendiagramme darstellbar.

Über eine Mail mit dem Einsatzgebiet des Klimamonitors würde ich mich freuen.

Einstellmöglichkeiten
title – Definition des Titels z.B.: title=“Dies ist ein Titel“

trendline – „yes“ , „no“; default ist „no“

chart – Definition der Anzeige, z.B.: char=“temp“

        temp    - zeigt nur die Temperaturen

        temphum - zeigt Temperatur und Luftfeuchte

        hum     - zeigt nur die Luftfeuchte

        press   - zeigt den Luftdruck

        dew     - zeigt den Taupunkt

        hums    - zeigt die spez. Feuchte und die Sättigungsfeuchte

        forecast - zeigt den Verlauf der Vorhersage
day – Definition des Anzeigebereichs, „Today“, „Yesterday“, „Week“, „Month“, „Year“
z.B.: day=“Week“ Anzeige der Daten der letzten 7 Tage

v_title – Definition der y-Achsen Beschriftung

Im Bereich Einstellungen-Allgemein steuert ein Flag, das mögliche Löschen der Datenbanktabelle beim Deaktivieren

Installiere das Plugin in */wp-content/plugins Verzeichnis
Aktiviere das Plugin im „Plugin“ Menü von WordPress, es wird automatisch eine neue Tabelle xxx_climadata angelegt.
(xxx = WordPress prefix
Durch drücken der Wetter-Buttons, wird ein Shortcode für ein Liniendiagramm erzeugt:
[ws_chart title=“Heute“ chart=“temp“ day=“Today“ v_title=“Temperatur“ width=“800px“ height=“400px“ ]
Ändere den erzeugten Code nach Deinen Wünschen ab
Die Wettervorhersage ist durch den Shortcode [cm_forecast] darstellbar.

Was benötige ich für dieses Plugin?

Du benötigst einen Raspberry Pi, ein GrovePi+ Shield, Temperatur- und Luftdrucksensor.
Ebenso benötigst Du das Coding von KlimaMonitorRasp, mit welchem die Daten in die Datenbank geschrieben werden.
Für mehr Informationen, besuche bitte die Projektseite https://www.tipi-camping.de
