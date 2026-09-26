# DTM Projekte
#### SoSe 26

## Dasymetrische Choroplethenkarte | EP01
> Kleines Einmaleins der thematischen Kartographie

Die verschiedenen Methoden stellen die Bevölkerung auf Ebene der LOR dar. Dabei wurde die Art der Darstellung der Kennzahlen angepasst: Es werden sowohl absolute Bevölkerungszahlen als auch die Bevölkerungsdichte pro Quadratkilometer nach LOR sowie die Bevölkerungsdichte pro Quadratkilometer nach Wohngebieten ausgewiesen.

|Einfache Choroplethenkarte  |Dasymetrische Choroplethenkarte |Einfache Choroplethenkarte   |
|----------------------------|--------------------------------|-----------------------------|
|Nack LOR                    |Relativ                         |Nach Wohngebieten            |

<img width="1297" height="915" alt="DTM1" src="https://github.com/user-attachments/assets/2409805d-1a05-4f1d-9227-9a83027db545" />


Die Abgrenzung der Wohngebiete erfolgt unabhängig von den LOR. Industriegebiete ohne oder mit nur wenigen Einwohnern werden dabei ausgeklammert, um Verzerrungen bei der Darstellung von Bevölkerungsdichten sowie bei der Bewertung von Wohnraumpotenzialen zu vermeiden.

## Gitter Choroplethenkarte | EP02/EP03
> Darstellung von Daten in Gittern, hierbei Rechteckig/Quadratisch oder mit Hexagonen
> Hier Repräsentiert von Sakurablüten, die je nach Anzahl der Sakurabäume pro Gitter ihre größe variieren.

<img src="https://github.com/endarlikeCTRL/DTM_UE_ALL/blob/main/blubraster.png"/>

## Tilemaps | EP06
Das Erzeugen von Tilemaps, und einem Verspielten, Klemmbausteinartigem muster anhand von Deutschland, hierbei wurden SRTM-Rasterdaten eingelesen und mit dem Erzeugtem Gitteer vernetzt. Dabei wurde der Mittelwert der Höhe pro Kachel Analysiert.

Die Darstellung ist Ebenenhaft, um Schatten der Höhenschichten zu Simulieren.

<img width="2480" height="3507" alt="Tilemaps06" src="https://github.com/user-attachments/assets/4a1a0f74-8337-4ca7-890e-08ae2fc8f788" />

## EP.07 | Animation in QGIS

Für die Aufgabe wurden aus der Meteormap-Datenbank geeignete Beobachtungsdaten zu den **Leoniden im November** gefiltert. Dabei wurden die Daten der Station **DE000K** verwendet und in QGIS weiterverarbeitet.
Die Anfangs- und Endkoordinaten der beobachteten Meteore wurden als Linien dargestellt und in das verwendete Koordinatensystem **EPSG:5243** transformiert. Anschließend wurden die Meteorbahnen grafisch als sich verjüngende, zum Ende hin transparente Linien dargestellt.

Durch die zeitliche Aufbereitung der Beobachtungen konnte anschließend eine **Animation der Meteorereignisse** erstellt werden. Die einzelnen QGIS-Ausgaben wurden dafür als PNG-Dateien exportiert und anschließend zu einer GIF-Animation mit einer Anzeigedauer von zwei Sekunden pro Bild zusammengefügt.


<img width="1920" height="1080" alt="meteors_animation" src="https://github.com/user-attachments/assets/32b397e8-44d9-42f0-b4a3-577942977284" />
