# 1.10 – Durch Computational Design erstellte Gruppen aus Dynamo

_In diesem Kapitel nutzen Sie die Rechenleistung von_ [_**Dynamo**_](http://dynamobim.org/), _um flexible Gruppen zu platzieren und zu ändern, die mit OOTB-Dynamo-Diagrammbeispielen verknüpft sind._

_Wenn Sie den letzten Abschnitt nicht bearbeitet haben, laden Sie die Datei_ _**1.10 – Computational Groups with Dynamo.axm**_ _aus dem Ordner_ _**FormIt Primer Part 1 Datasets** herunter und öffnen sie._

[_**Hier**_](http://formit.autodesk.com/page/formit-dynamo) _erfahren Sie mehr darüber, wie FormIt und Dynamo bei Computational Design-Arbeitsabläufen zusammenwirken._

## **Erstellen von Treppen für die untere Terrasse**

1 – Stellen Sie sicher, dass die Layer **Lower Terrace, Main Building Floor** und **Plan Image** aktiviert sind, da Sie an dieser Stelle die Treppen hinzufügen werden.

2 – So platzieren Sie eine Treppengruppe, die mit einem der OOTB-Dynamo-Beispiele verknüpft ist

1. Öffnen Sie die **Dynamo Palette** (Dynamo-Palette) in der Palettenleiste. Im Verzeichnis **Dynamo Samples** (Dynamo-Beispiele) sollten einige integrierte Dynamo-Objekte angezeigt werden.
2. Klicken Sie auf das Dynamo-Beispiel für **Stairs** (Treppen), um es in den Modellbereich zu holen. FormIt führt das Diagramm im Hintergrund aus und generiert die Treppengeometrie aus diesem Diagramm.
3. Bewegen Sie den Cursor über den Ansichtsbereich. Nachdem die Treppe geladen wurde, wird eine Ghost-Vorschau der Treppengeometrie mit der Maus verknüpft. Bewegen Sie den Cursor über den Ansichtsbereich in die Nähe der Terrasse, und klicken Sie, um die Treppe zu platzieren. Drücken Sie **ESC**, um die Auswahl aufzuheben. Beachten Sie, dass nach dem Platzieren der Treppe automatisch die **Properties Palette** (Eigenschaften-Palette) geöffnet wird.

![](../../.gitbook/assets/0%20%2815%29.png)

_**Anmerkung:**_ [_**Sie können auch lokale Verzeichnisse**_](https://formit.autodesk.com/page/formit-dynamo#dynamo-getting-started) _mit Dynamo-Diagrammen verknüpfen und Ihre eigenen lokalen Dynamo-Diagramme wie in diesen Beispielen ausführen._

3 – So aktualisieren Sie die Treppenbemaßungen

1. Ändern Sie bei ausgewählter Treppengruppe die Eingaben im Abschnitt **INPUTS** (Eingaben) von Dynamo unten in der **Properties Palette** (Eigenschaften-Palette) entsprechend, wie im Folgenden dargestellt. Die meisten über Dynamo-Skripte erstellten Gruppen verfügen über einen Dynamo-Abschnitt in den Eigenschaften, wenn sie ausgewählt werden.
   * Add Top Landing (Oberes Podest hinzufügen) = False
   * Add Middle Landing (Mittleres Podest hinzufügen) = False
   * Add Bottom Landing (Unteres Podest hinzufügen) = False
   * Floor-to-Floor Height (Geschosshöhe) = 2.6
   * Stair Width (Treppenbreite) = 12
   * Riser Height (Steigung) = 0.6
   * Tread Length (Auftrittslänge) = 1.25
   * Tread Overlap (Stufe Überstand) = 0.25
   * Tread Thickness (Auftrittshöhe) = 0.25
   * Height Between Middle Landings (Höhe zwischen mittleren Podesten) = \(nicht relevant, da kein mittleres Podest erstellt wird\)
   * Middle Landing Length (Länge des mittleren Podests) = \(nicht relevant, da kein mittleres Podest erstellt wird\)
   * Top/Bottom Landing Length (Länge des oberen/unteren Podests) = \(nicht relevant, da kein Podest erstellt wird\)
2. Klicken Sie auf die Schaltfläche **Run** (Ausführen), um das Dynamo-Skript mit den aktualisierten Eingabewerten erneut auszuführen.
3. Verschieben Sie die Gruppe nach Bedarf, um die Treppe entsprechend dem Layer **Plan Image** an der richtigen Position zu platzieren. Achten Sie darauf, die Höhe der Treppengruppe beim Verschieben nicht zu ändern. In den vorherigen Kapiteln finden Sie weitere Tricks und Techniken zum Verschieben von Modellelementen.

![](../../.gitbook/assets/1%20%2811%29.png)

_**‌Anmerkung:**_ _Die Eingabe für_ _**Floor-to-Floor Height**_ _(Geschosshöhe) ist eine Annäherung an die Gesamthöhe der Treppe._ _**Riser Height**_ _(Steigung) ist der Parameter, der die Höhe der Treppe definiert. In diesem Beispiel wurde_ _**Floor-to-Floor Height**_ _(Geschosshöhe) auf 2.6' festgelegt, die endgültige Treppenhöhe beträgt jedoch 3.0' \(0.6' \(**Riser Height (Steigung)**\) x 5 \(Anzahl Stufen\)\). Da die Spanne zwischen Boden und Oberkante der Terrasse 3'-2" beträgt, sind die verbleibenden 2" in der oberen Steigung enthalten._

## **Erstellen der Hauptgebäudetreppen**

_In den vorherigen Schritten haben Sie eine Treppe ohne Podeste erstellt. Als Nächstes erstellen Sie eine Treppe, bei der ein oberes Podest verwendet wird, das am Layer_ _**Main Building Floor** ausgerichtet ist._

1 – Erstellen Sie zunächst eine Kopie der Treppe, die Sie gerade erstellt haben:

1. Wählen Sie die vorhandene Treppe aus, und klicken Sie dann auf eine beliebige Stelle im Layer **Plan Image**, um den Befehl Move zu starten. Dadurch wird in FormIt die Höhe von **Plan Image** als Startreferenzhöhe für die Platzierung der neuen Kopie verwendet. Drücken Sie die **STRG-Taste**, um eine **schnelle Kopie** zu erstellen.
2. Bewegen Sie den Cursor näher zum Hauptgebäude über der Terrasse. Beachten Sie, dass die obere Fläche der Terrasse jetzt die neue Referenzebene ist. Klicken Sie, um die Gruppe zu platzieren.

![](../../.gitbook/assets/2%20%289%29.png)

_**Anmerkung:**_ _Da sich das_ _**Plan Image**_ _auf der Ebene_ _**Ground Level**_ _(Erdgeschoss) befindet, wird diese Ebene vom_ _**Werkzeug Move**_ _(Verschieben) als Referenz für den Startpunkt verwendet. Beachten Sie die QuickInfo_ _**On Face**_ _(Auf Fläche) in der Abbildung oben, die angibt, dass die Fläche von Plan Image als Startreferenz und die obere Fläche von_ _**Lower Terrace Floor**_ _(Unterer Terrassenboden) als Endreferenz ausgewählt ist._

2 – Verwenden Sie das Werkzeug **Make Unique \(MU\)** (Als eindeutig definieren), damit sich Änderungen an den Dynamo-Eingaben dieser Treppe nicht auf die untere Treppe auswirken. Positionieren Sie die Gruppe nach Bedarf neu, sodass sie sich nahe an der endgültigen Position befindet. Diese wird später genauer festgelegt. Sie können die Sichtbarkeit des Layers **Lower Terrace** umschalten, um den Plan darunter zu Hilfszwecken bei der Positionierung anzuzeigen. Achten Sie jedoch darauf, die Höhe der neuen Treppe beim Verschieben nicht zu ändern.

3 – Aktualisieren Sie in der **Properties Palette** (Eigenschaften-Palette) die **Dynamo Inputs** (Dynamo-Eingaben) wie unten dargestellt, und führen Sie das Skript erneut aus.

* Add Top Landing (Oberes Podest hinzufügen) = True
* Floor-to-Floor Height (Geschosshöhe) = 2.333
* Riser Height (Steigung) = 0.466
* Tread Length (Auftrittslänge) = 1.5
* Top/Bottom Landing Length (Länge des oberen/unteren Podests) = 2.5

![](../../.gitbook/assets/3%20%281%29.jpeg)

_**Anmerkung:**_ _Wenn Sie_ _**Add Bottom Landing**_ _(Unteres Podest hinzufügen) auf_ _**True**_ _einstellen und das Skript erneut ausführen, sollte die obere Fläche des unteren Podests an der oberen Fläche von_ _**Lower Terrace Floor** (Unterer Terrassenboden) ausgerichtet sein. Dies geschieht, weil Sie – anders als bei den vorherigen Treppen–_ _**Riser Height**_ _(Steigung) so angepasst haben, dass sie mit der_ _**Floor-to-Floor Height**_ _(Geschosshöhe) entsprechend der gewünschten echten Höhe \(2'-4" oder 2.333'\)übereinstimmt._

2 – Positionieren Sie die Gruppe erneut an der endgültigen Position. Das obere Podest muss bündig mit dem Layer **Main Building Floor** abschließen.

3 – Um die Treppe fertig zu stellen, fügen Sie das Material **Stone – Travertine** (Stein – Travertin) hinzu, um es an die Geschosse anzupassen. Weitere Informationen zum Anwenden von Materialien finden Sie in den vorherigen Kapiteln.

