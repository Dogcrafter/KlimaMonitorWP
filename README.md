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
