# Array Along Path (Reihe entlang Pfad)

## Powered by Dynamo

In FormIt 2021 und höher können Sie Objekte entlang eines Pfads anordnen und die Ergebnisse sofort und direkt anpassen. Array Along Path (Reihe entlang Pfad) wird von Dynamo unterstützt, d. h., die Reihe kann einfach konfiguriert werden, um die gewünschten Ergebnisse zu erzielen. Durch erneutes Ausführen der Logik wird die Geometrie direkt aktualisiert.

![](../.gitbook/assets/array-along-path.gif)

## Starten von Array Along Path (Reihe entlang Pfad)

* Wechseln Sie zur Gruppe Dynamo in FormIt for Windows, und stellen Sie sicher, dass Sie sich im Verzeichnis Dynamo Samples (Dynamo-Beispiele) befinden.
* Klicken Sie auf das Beispiel für Array Along Path (Reihe entlang Pfad).
* Auf der linken Seite des Bildschirms wird eine Eingabeaufforderung zum Auswählen der anzuordnenden Objekte angezeigt.
   * Sie können für diesen Schritt eine beliebige Kombination von FormIt-Objekten auswählen.
   * Wenn Sie eine Auswahl getroffen haben, können Sie auf den Weiter-Pfeil links auf dem Bildschirm klicken oder einfach die EINGABETASTE drücken.
* Nun wird eine Eingabeaufforderung zum Auswählen des Pfads für die Reihe angezeigt.
   * Hier sollten Sie nur eine Reihe von fortlaufenden Kanten oder eine Gruppe, die eine Reihe von fortlaufenden Kanten enthält, auswählen.
   * Wenn Sie den Pfad ausgewählt haben, klicken Sie auf die Schaltfläche Finish (Fertig stellen), oder drücken Sie die EINGABETASTE.
* In der Gruppe Dynamo wird angezeigt, dass die Änderungen verarbeitet werden. Wenn Sie fertig sind, wird eine in Dynamo generierte Reihe in einer FormIt-Gruppe angezeigt, die Sie bearbeiten können \(siehe unten\).

## Erstellen von Iterationen an Ort und Stelle

Nach dem Ausführen von Array Along Path (Reihe entlang Pfad) werden die Ergebnisse auf Vorgabewerte eingestellt. Sie sollten sie daher an Ihre Anforderungen anpassen.

Wenn Array Along Path (Reihe entlang Pfad) ausgeführt wird, wird eine neue Gruppe mit den Ergebnissen erstellt. FormIt wählt dann automatisch die Gruppe aus und zeigt die verfügbaren Optionen für dieses Exemplar von Array Along Path (Reihe entlang Pfad) an.

Sie können jederzeit zu den Eigenschaften für Array Along Path (Reihe entlang Pfad) zurückkehren, indem Sie die Gruppe auswählen und zur Gruppe Properties (Eigenschaften) wechseln oder die Gruppe bearbeiten, sodass automatisch Eigenschaften angezeigt werden.

![](../.gitbook/assets/array-along-path-options.png)

### Select Object\(s\) to Array (Objekte für Reihe auswählen) <a id="run"></a>

Klicken Sie auf diese Schaltfläche, um zum Auswahlassistenten zurückzukehren und die anzuordnenden Objekte zu ändern.

### Select Array Path (Pfad für Reihe auswählen)

Klicken Sie auf diese Schaltfläche, um zum Auswahlassistenten zurückzukehren und den Pfad zu ändern, der zum Berechnen der Reihe verwendet wird.

### Array Type (Reihentyp) <a id="run"></a>

Hiermit wird der zu berechnende Reihentyp umgeschaltet: By Distance (Nach Abstand) oder By Number (Nach Nummer).

**Wenn True eingestellt ist**, wird die Berechnung By Distance (Nach Abstand) durchgeführt, sodass sich die Zahl unten auf den Abstand zwischen Kopien bezieht.

**Wenn False eingestellt ist**, wird die Berechnung By Number of Copies (Nach Anzahl der Kopien) durchgeführt, sodass sich die Zahl unter diesem Feld auf die Anzahl der Kopien bezieht, die entlang des Pfads eingepasst werden sollen.

### Include Original Selection In Results (Ursprüngliche Auswahl in Ergebnisse einschließen)

Wenn **True**:

* Die ausgewählten Objekte werden als eine der neuen Kopien gezählt.
* Die resultierende Dynamo-Gruppe nimmt die ursprüngliche Auswahl in die Ergebnisse auf, sodass für die neuen Kopien ein Z-Fighting-Effekt mit der ursprünglichen Auswahl auftritt. Sie können die ursprüngliche Auswahl auf einem [Layer](layers.md) platzieren und diesen deaktivieren, um ihn auszublenden.

Wenn **False**:

* Die resultierende Reihe enthält die ursprüngliche Auswahl **nicht**, sodass Sie **zusätzlich** zur ursprünglichen Auswahl die angegebene Anzahl der Kopien erhalten. Bei den Ergebnissen findet kein Z-Fighting statt.

### Rotate Copies Along Path (Kopien entlang Pfad drehen)

Wenn **True** eingestellt ist, werden die Kopien gedreht, um die Ausrichtung des ursprünglichen Objekts relativ zum Pfad beizubehalten.

Wenn **False** eingestellt ist, werden die Kopien nicht gedreht, sondern nur verschoben.

### Use Relative Positioning Along Path (Relative Positionierung entlang Pfad verwenden)

Wenn **True**:

* Bei jeder Kopie wird der Abstand zwischen dem Pfad und dem ursprünglichen Objekt beibehalten.
* Wenn das ursprüngliche Objekt **nicht** an einem der Endpunkte des Pfads positioniert ist, wird das größte verbleibende Segment des Pfads für die Reihenberechnung verwendet.

Wenn **False**:

* Die gesamte Länge des Pfads wird zur Berechnung der Reihe verwendet, unabhängig davon, wo sich das ursprüngliche Objekt relativ zum Pfad befindet.
* Dadurch wird die Position des Pfads relativ zum Objekt entkoppelt, und es wird einfach der gesamte Pfad verwendet. Dies ist nützlich, wenn der Pfad und das Objekt nicht nahe beieinander liegen.

### Reverse Path Direction (Pfadrichtung umkehren)

Nur für geschlossene Pfade. Wenn Sie Array Along Path (Reihe entlang Pfad) mit einem geschlossenen Pfad verwenden, werden die erwarteten Ergebnisse der Reihe möglicherweise durch die Richtung der Kurve unerwartet umgekehrt. Setzen Sie diesen Wert auf **True**, um auch die Reihenrichtung umzukehren, wenn die Ergebnisse umgekehrt werden.

### Run (Ausführen) <a id="run"></a>

Klicken Sie nach dem Bearbeiten der Optionen auf die Schaltfläche Run (Ausführen), um das zugrunde liegende Dynamo-Diagramm auszuführen und neue Ergebnisse zu generieren. Diese Schaltfläche wird blau, wenn Parameter geändert wurden. So erkennen Sie, dass Sie darauf klicken müssen, um die Aktualisierungen in der endgültigen Geometrie zu sehen.‌

### Edit Embedded Graph (Eingebettetes Diagramm bearbeiten) <a id="edit-embedded-graph"></a>

Wenn Sie auf diese Schaltfläche klicken, wird die Dynamo-Diagramm-Editor-Umgebung geöffnet, in der Sie das zugrunde liegende Dynamo-Diagramm anzeigen und bearbeiten können, um Parameter schneller zu ändern, Live-Aktualisierungen anzuzeigen oder die Logik zu prüfen bzw. anzupassen.



## Auswählen von Geometrie

Bei der Auswahl von Objekten für Array Along Path (Reihe entlang Pfad) und andere auswahlbasierte Dynamo-Diagramme gilt Folgendes:

* Sie können eine beliebige Kombination von FormIt-Objekten auswählen: Scheitelpunkte, Kanten, Flächen, Volumenkörper, Gruppen oder Netze.
   * Beachten Sie, dass je nach Schritt einige dieser Objekte nicht ausgewählt werden sollten.
   * Wenn Sie beispielsweise den Pfad auswählen, sollten Sie nur eine fortlaufende Reihe von Kanten oder eine Gruppe mit einer fortlaufenden Reihe von Kanten auswählen. Andernfalls schlägt das Diagramm fehl.
* Sie können auf ein Objekt doppelklicken, um alle zugeordneten Objekte auszuwählen.
* Sie können das Fenster für die Bereichsauswahl verwenden, um eine Reihe von Objekten zu erfassen.
* Sie können bereits ausgewählte Objekte auswählen, um deren Auswahl aufzuheben.
* Mindestens ein Objekt ist erforderlich, um mit einem auswahlbasierten Schritt fortzufahren.



