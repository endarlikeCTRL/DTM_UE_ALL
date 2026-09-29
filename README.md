# DTM Projekte
#### SoSe 26

# EP.01 | Dasymetrische Choroplethenkarte
> Kleines Einmaleins der thematischen Kartographie

Die verschiedenen Methoden stellen die Bevölkerung auf Ebene der LOR dar. Dabei wurde die Art der Darstellung der Kennzahlen angepasst: Es werden sowohl absolute Bevölkerungszahlen als auch die Bevölkerungsdichte pro Quadratkilometer nach LOR sowie die Bevölkerungsdichte pro Quadratkilometer nach Wohngebieten ausgewiesen.

|Einfache Choroplethenkarte  |Dasymetrische Choroplethenkarte |Einfache Choroplethenkarte   |
|----------------------------|--------------------------------|-----------------------------|
|Nack LOR                    |Relativ                         |Nach Wohngebieten            |
|Stellt die absolute Bevölkerungszahl summiert pro Lebensweltlich orientiertem Raum (LOR) dar. Die Gesamtzahl wird dabei gleichmäßig über die gesamte administrative Fläche der jeweiligen Einheiten eingefärbt. | Zeigt die Bevölkerungsdichte bezogen auf die LOR-Flächen. Dadurch werden die Werte flächenbereinigt und ermöglichen einen besseren relativen Vergleich zwischen unterschiedlich großen Gebieten. | Visualisiert die Bevölkerungsdichte ausschließlich auf den tatsächlich bewohnten Flächen (Wohngebieten). Unbewohnte Flächen wie Parks, Industriegebiete oder Gewässer werden herausgefiltert, was eine realistischere räumliche Verteilung zeigt. |

<img width="1297" height="915" alt="DTM1" src="https://github.com/user-attachments/assets/2409805d-1a05-4f1d-9227-9a83027db545" />


Die Abgrenzung der Wohngebiete erfolgt unabhängig von den LOR. Industriegebiete ohne oder mit nur wenigen Einwohnern werden dabei ausgeklammert, um Verzerrungen bei der Darstellung von Bevölkerungsdichten sowie bei der Bewertung von Wohnraumpotenzialen zu vermeiden.

# EP.02/EP.03 | Gitter Choroplethenkarte
> Darstellung von Daten in Gittern, hierbei Rechteckig/Quadratisch oder mit Hexagonen
> Hier Repräsentiert von Sakurablüten, die je nach Anzahl der Sakurabäume pro Gitter ihre größe variieren.

<img src="https://github.com/endarlikeCTRL/DTM_UE_ALL/blob/main/blubraster.png"/>

# EP.04 | Value-By-Alpha Mapping

Die Geometrien der 106 ungarischen Wahlkreise wurden ueber eine eindeutige ID mit den Wahldaten verknuepft und als GeoJSON aufbereitet. Die Hauptkarte nutzt eine Value-By-Alpha-Darstellung, bei der die Farbdeckung je nach der Staerke des Wahlsiegs variiert. Zudem wurden ein Inset fuer Budapest und zwei Choroplethenkarten fuer den Parteienvergleich im A3-Layout zusammengestellt.

<img width="3507" height="2480" alt="ungarnwahlen" src="https://github.com/user-attachments/assets/bd2dba23-381d-4824-b450-78cc90fb9bad" />


# EP.05 | Ursprung-Ziel-Karten

Visualisierung des internationalen Studierendenaustauschs der BHT Berlin auf Basis von Daten des Referats Internationale Angelegenheiten. Die Karte nutzt eine auf Berlin zentrierte orthographische Azimutalprojektion, um die weltweiten Verbindungslinien realistisch darzustellen.

<img width="1080" height="1080" alt="globee" src="https://github.com/user-attachments/assets/fc43fff8-0e9f-43b3-bc6b-849a535124e9" />


# EP.06 Tilemaps | EP06
Das Erzeugen von Tilemaps, und einem Verspielten, Klemmbausteinartigem muster anhand von Deutschland, hierbei wurden SRTM-Rasterdaten eingelesen und mit dem Erzeugtem Gitteer vernetzt. Dabei wurde der Mittelwert der Höhe pro Kachel Analysiert.

Die Darstellung ist Ebenenhaft, um Schatten der Höhenschichten zu Simulieren.

<img width="2480" height="3507" alt="Tilemaps06" src="https://github.com/user-attachments/assets/e05b0620-9b2d-4204-a4dc-1d9c8d98d533" />


# EP.07 | Animation in QGIS

Für die Aufgabe wurden aus der Meteormap-Datenbank geeignete Beobachtungsdaten zu den **Leoniden im November** gefiltert. Dabei wurden die Daten der Station **DE000K** verwendet und in QGIS weiterverarbeitet.
Die Anfangs- und Endkoordinaten der beobachteten Meteore wurden als Linien dargestellt und in das verwendete Koordinatensystem **EPSG:5243** transformiert. Anschließend wurden die Meteorbahnen grafisch als sich verjüngende, zum Ende hin transparente Linien dargestellt.

Durch die zeitliche Aufbereitung der Beobachtungen konnte anschließend eine **Animation der Meteorereignisse** erstellt werden. Die einzelnen QGIS-Ausgaben wurden dafür als PNG-Dateien exportiert und anschließend zu einer GIF-Animation zusammengefügt.


<img width="1920" height="1080" alt="meteors_animation" src="https://github.com/user-attachments/assets/32b397e8-44d9-42f0-b4a3-577942977284" />

# EP.08 | Mesh-Daten

In diesem Projekt werden Windgeschwindigkeiten und Windrichtungen für verschiedene Zeitpunkte in QGIS visualisiert und als zeitliche Animation dargestellt. Die Windvektoren zeigen dabei die räumliche Verteilung und Veränderung des Windes über mehrere Stunden.
Für die farbliche Gestaltung der Windvisualisierung wurde **Vincent van Goghs „Sternennacht“** als visuelle Referenz verwendet. Die Farbtöne des Gemäldes wurden dabei als Farbpalette übernommen, um die Windbewegungen atmosphärisch und anschaulich darzustellen.

> Information: die Bilder sind zu groß, daher wurde ein GIF-Compress genutzt!

<img width="1201" height="807" alt="winds_animated_extended(1)(1)" src="https://github.com/user-attachments/assets/9e058c0d-a18e-4b33-b919-840819cc9ec7" />


> Zu viel Van Gogh? Vielleicht das hier?
> 
<img width="1280" height="860" alt="winds_animateboring" src="https://github.com/user-attachments/assets/b51b3256-46ba-4729-8ea0-f45803652a7f" />

# EP.09 | 3D-Gebäudemodelle

## 2,5D-Gebäudevisualisierung

Für die Visualisierung wurden zwei LoD2-Gebäudekacheln zusammengeführt und als 3D-Geometrien in einem GeoPackage gespeichert. Anschließend wurden die Gebäude in QGIS als 2,5D-Modell dargestellt und anhand ihrer Gebäudehöhe mit einem Farbgradienten visualisiert. Dadurch entsteht eine räumliche Darstellung, bei der sowohl die Gebäudehöhe als auch die Unterschiede zwischen den Gebäuden deutlich erkennbar sind.

<img width="1920" height="1357" alt="tddy" src="https://github.com/user-attachments/assets/70456f89-7915-4644-9634-e732417b51ef" />

## oder doch lieber 3D?

<img width="1567" height="304" alt="image" src="https://github.com/user-attachments/assets/a71f94d3-4888-4f61-a6bf-f6e421581060" />





