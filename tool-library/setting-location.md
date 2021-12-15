# Festlegen des Standorts

Die Angabe des geografischen Standorts Ihres Projekts ist wichtig für die Genauigkeit Ihres Modells und für Analysen im weiteren Verlauf des Projekts. Dazu zählt Folgendes:

* Der Standort wird verwendet, um ein Satellitenbild zu importieren, das zum Nachzeichnen eines vorhandenen Grundstücks oder Gebäudes verwendet werden kann.
* Der Standort wird verwendet, um 3D-Gelände zu importieren, das zum Referenzieren topologischer Daten für ein Grundstück verwendet werden kann.
* Der Standort wird für die genaue Positionierung der Sonne am Himmel verwendet, was sich auf die Berechnung von Schatten auswirkt.
* Der Standort wird für die Solar- und Energieanalyse verwendet, um genaue analytische Berechnungen zu ermöglichen.

Sie müssen sich mit Ihrem Konto bei Autodesk Account anmelden, um auf das Dialogfeld Standort festlegen und die zugehörigen Dienste zuzugreifen.

### Erste Schritte mit Standort

* Öffnen Sie das Dialogfeld **Standort festlegen** über das Werkzeug **Standort** im Werkzeugkasten oder über den Tastaturbefehl SL.

![](../.gitbook/assets/location-toolbar.png)

* Beginnen Sie, indem Sie den Standort des Projekts in das Suchfeld in der oberen linken Ecke des Fensters _Standort festlegen_ eingeben.

![](../.gitbook/assets/location-step-1%20%281%29.png)

* Wählen Sie eine der Optionen für die automatische Angabe der Standortdaten, oder drücken Sie die EINGABETASTE, um die erste Option zu wählen.
* Der gesuchte Standort wird automatisch vergrößert.

### Nur Standort festlegen im Vergleich mit Satellitenbilder und Gelände importieren

Nachdem Sie nach einem Standort gesucht haben, können Sie eine von zwei Optionen wählen:

* **Nur Standort festlegen** legt den Standort in der Datei fest, ohne Satellitenbilder zu importieren.
* **Satellitenbilder und Gelände importieren** legt den Standort fest und importiert außerdem Satellitenbilder und Geländedaten mit einem Zoomfaktor und Grenzen, die Sie konfigurieren können.

### Importieren von Satellitenbildern

* Klicken Sie auf **Satellitenbilder und Gelände importieren** oben rechts im Fenster **Standort festlegen**.
* Eine Vorschau der Satellitenbilder wird in der Mitte des Fensters angezeigt, zusammen mit einem Hinweis darauf, wo der FormIt-Ursprung relativ zu den Bildern angezeigt wird.

![](../.gitbook/assets/location-step-2.png)

* Ziehen Sie die Satellitenbilder innerhalb des Quadrats, um ihre Position anzupassen.
* Wenn sich die gewünschten Bilder innerhalb der quadratischen Fläche befinden, klicken Sie auf **Import beenden**.
* Das Bild wird maßstabsgetreu mit dem geografischen Norden nach oben und zentriert am Ursprung des FormIt-Ansichtsbereichs importiert. Sie können die Transparenz und Z-Reihenfolge des importierten Bildes ändern, indem Sie darauf doppelklicken und die [**Eigenschaftenpalette**](../formit-introduction/tool-bars.md) verwenden.

![](../.gitbook/assets/location-step-3.png)

### Aktualisieren von Satellitenbildern

Nachdem Sie Satellitenbilder erstmalig importiert haben, können Sie im Fenster Standort festlegen den Zoomfaktor oder die Grenzen der Satellitenbilder anpassen.

* Starten Sie das Fenster **Standort festlegen** erneut, indem Sie es wie oben beschrieben über den Werkzeugkasten aufrufen.
* Klicken Sie auf **Satellitenbilder und Gelände importieren**
* Sie sehen den aktuellen Zoomfaktor und die Grenzen des Satellitenbilds, wie im FormIt-Ansichtsbereich dargestellt.
* Passen Sie einfach die Position an, oder zoomen Sie, und klicken Sie wie zuvor auf **Import beenden**.
* Wenn das Bild wieder in den Ansichtsbereich importiert wird, wird es an die richtige Position relativ zur ursprünglichen Bildposition verschoben \(und ist möglicherweise nicht mehr am Ursprung zentriert\):

![](../.gitbook/assets/location-step-4.png)

### Importieren von Gelände

Neu in FormIt 2021.3 ist, dass Sie auch Geländedaten erhalten, wenn Sie das Dialogfeld **Standort festlegen** verwenden, um Satellitenbilder zu importieren.

![](../.gitbook/assets/terrain-button_original.png)

Wenn Geländedaten importiert werden, werden diese auf einem Layer platziert, der vorgabemäßig deaktiviert ist \(falls Sie schon mit dem Modellieren begonnen haben, wird Ihr Modell möglicherweise vom Gelände überdeckt\).

Wenn Sie bereit sind, das Gelände anzuzeigen, aktivieren Sie das Kontrollkästchen, um den Gelände-Layer anzuzeigen:

![](../.gitbook/assets/terrain-layer%20%281%29.png)

![](../.gitbook/assets/terrain_solid.png)

### Arbeiten mit Geländedaten

Geländedaten werden in eine FormIt-Gruppe eingefügt. Doppelklicken Sie auf die Gruppe, um sie zu bearbeiten.

Darin finden Sie zwei Netze: eines für die Seiten und die Unterseite und eines für die Oberseite.

Wenn Sie das Gelände ändern möchten, müssen Sie die Netze in ein einzelnes Volumenkörperobjekt umwandeln:

* Wählen Sie beide Netze aus.
* Klicken Sie mit der rechten Maustaste, und wählen Sie die Option Netze in Objekte, oder verwenden Sie den Kurzbefehl MO.

![](../.gitbook/assets/terrain-mesh-context.png)

Wenn beide Netze gleichzeitig in ein Objekt konvertiert werden, kann FormIt sie zu einem bündigen Volumenkörperobjekt kombinieren, das für Volumenkörperoperationen wie die Boolesche Operation Ausschneiden verwendet werden kann.

Hier können Sie eine Kombination aus [Draufsicht](orthographic-views.md) und [orthogonaler Kamera](orthographic-camera.md) verwenden, um die Grundstücksgrenze auf einer horizontalen Ebene nachzuzeichnen, und dann diese Ebene in ein Volumen extrudieren, das das Gelände schneidet. Die Verwendung eines transparenten [Materials](materials.md) hilft Ihnen dabei, das Gelände durch den Schnittvolumenkörper zu sehen:

![](../.gitbook/assets/terrain-cutter-before.png)

Verwenden Sie das Werkzeug Geometrie ausschneiden, und wählen Sie unter Zu schneidenden Volumenkörper auswählen das Gelände und als Volumenkörper, der entfernt werden soll, das Schnittvolumen aus.

![](../.gitbook/assets/terrain-cut-menu.png)

Das Ergebnis ist das Gelände, aus dem der Schnittvolumenkörper entfernt wurde, sodass ein Abzugskörper entsteht, in dem Sie das neue Grundstück und das neue Fundament zeichnen können.

![](../.gitbook/assets/terrain-cutter-after.png)

Sie können [Layer](layers.md) verwenden, um den Schnittvolumenkörper auszublenden oder sogar Kopien des Geländes mit und ohne Schnitt zu erstellen, falls Sie das ursprüngliche Gelände referenzieren müssen, oder Sie können die Schnittform ändern, bevor Sie den Volumenkörperschnitt ausführen.

