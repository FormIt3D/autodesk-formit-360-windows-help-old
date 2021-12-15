# Storefront/Curtainwall Mullion System (Ladenfront-/Fassadenpfosten-System)

![](../.gitbook/assets/dynamo-storefront-system-options.gif)

## Powered by Dynamo

Die Möglichkeit, in FormIt schnell Ladenfront-/Fassadenpfosten-Systeme erstellen zu können, wird von Dynamo unterstützt. Sie finden das Ladenfront-/Fassadensystem im Dynamo-Beispielverzeichnis (Dynamo Samples) in der Gruppe Dynamo:

![](../.gitbook/assets/storefront-curtainwall-button%20%281%29.png)

## Auswählen von Glas für das Pfostensystem

Ab FormIt 2021.2 verwendet das Ladenfront-/Fassadensystem den neuen [SelectFromFormIt-Block](https://formit.autodesk.com/page/formit-dynamo#dynamo-formit-nodes), mit dem Sie einen Glaskörper \(eine einzelne Fläche oder einen extrudierten Volumenkörper\) auswählen können, um den ein Pfostensystem erstellt werden soll.

![Einfache Ebene aus Glas mit einer Öffnung für Türen unten](../.gitbook/assets/storefron-system-1_glass-only.png)

Wenn Sie auf die Miniaturansicht Storefront Curtainwall (Ladenfront/Fassade) klicken \(beachten Sie das Symbol, das angibt, dass eine Auswahl erforderlich ist\), fordert FormIt Sie auf, die Glasgeometrie auszuwählen, um fortzufahren:

![](../.gitbook/assets/storefront-curtainwall-prompt.png)

Einige Hinweise und Warnungen zur Funktionsweise der Glasauswahl:

* Derzeit werden nur planare Flächen unterstützt. Wenn Sie eine Reihe von Flächen auswählen \(z. B. eine gekrümmte Fläche, die aus kleineren planaren Flächen besteht\), sucht das Skript die größte planare Fläche und verwendet diese.
* Wenn die Verglasung ein Volumenkörper ist, d. h., wenn eine einzelne Fläche sehr leicht extrudiert wurde, um eine gewisse Dicke zu erhalten, findet das Skript die größte Fläche, sodass die resultierenden Pfosten auf einer Seite des Glasvolumenkörpers generiert werden.
* Sie können Öffnungen für Türen skizzieren und die resultierende Fläche aus der Glasumgrenzung entfernen. Die resultierenden Pfosten berücksichtigen die Türöffnung, sodass diese leer bleibt, damit die Tür hinzugefügt werden kann.
* Aufgrund von Einschränkungen in Dynamo funktioniert dieses Skript nicht, wenn die Glasgeometrie Öffnungen in der Mitte aufweist.

## Tipps und Tricks

Bei der Auswahl von Geometrie für ein Dynamo-Diagramm in FormIt können bestimmte organisatorische Tricks die Arbeit vereinfachen und eine einfache Instanziierung der Ergebnisse ermöglichen:

* Fügen Sie die Verglasung zu einer Gruppe hinzu, und verwenden Sie die Gruppe als Auswahl für das Skript Storefront/Curtainwall (Ladenfront-/Fassade). Auf diese Weise ist es einfacher, das Glasprofil zu bearbeiten, nachdem die Pfosten generiert wurden. Wenn die Verglasung zwischen den Ausführungen umfassend geändert wird und andere Flächen-IDs gelten, stellt die Gruppe sicher, dass das Skript die Verglasung immer findet, da es die Gruppen-ID und nicht die Flächen-ID verwendet.
* Wenn Sie planen, die Ergebnisse des Pfostensystems zu kopieren und an anderen Stellen im Modell einzufügen, sollten die Verglasung und die resultierenden Pfosten in einer Gruppe enthalten sein. Dadurch wird auch verhindert, dass der Auswahlblock nicht weiß, welches Glasexemplar verwendet werden soll, wenn nur die resultierende Pfostengruppe kopiert und eingefügt wird.
   * Fassen Sie die Verglasung zuerst in einer Group (Gruppe) zusammen. Doppelklicken Sie darauf, um die Verglasung auszuwählen, und drücken Sie G, oder verwenden Sie die Gruppenbefehle im Kontextmenü oder im Werkzeugkasten.
   * Wählen Sie die resultierende Gruppe aus, und fügen Sie sie zu einer anderen Gruppe hinzu.
   * Doppelklicken Sie, um die erste Gruppe aufzurufen. Diese ist der Container für die Verglasung und die resultierenden Pfosten.
   * Klicken Sie auf die Miniaturansicht Storefront Curtainwall (Ladenfront/Fassade), und verwenden Sie die Glasgruppe als Auswahl.
   * Nachdem das Skript ausgeführt wurde, können Sie die Gruppe beenden und den Container nach Bedarf kopieren und einfügen. Sie können jedes der Exemplare problemlos bearbeiten \(Anpassen der Glasform oder der Parameter\).

## Optionen des Pfostensystems

Wenn Sie die Verglasung auswählen und das Skript ausführen, erhalten Sie ein Ergebnis in Form einer FormIt-Gruppe im FormIt-Ansichtsbereich. Diese Gruppe wird automatisch ausgewählt, und die verfügbaren Optionen werden in der Gruppe Properties (Eigenschaften) angezeigt.

![](../.gitbook/assets/storefront-curtainwall-parameters.png)

* **Run (Ausführen)**: Wenn Sie die Form der Verglasung ändern und das Diagramm erneut ausführen möchten, um die Pfostergebnisse zu aktualisieren, klicken Sie auf diese Schaltfläche.
* **Edit Embedded Graph (Eingebettetes Diagramm bearbeiten)**: Bearbeiten Sie das Dynamo-Skript, mit dem die Geometrie erstellt wird. Dieses Skript ist in die FormIt-Datei eingebettet und ist spezifisch für diese Gruppe.
* **Select Glass \(Surface or Solid\) (Glas auswählen \(Fläche oder Volumenkörper\))**: Klicken Sie auf diese Option, um einen anderen Glaskörper auszuwählen, um den Pfosten erstellt werden sollen.

Das Skript verwendet für die erste Ausführung Vorgabewerte. Sie sollten diese daher für Ihren speziellen Anwendungsfall anpassen. Für alle Werte werden die aktuellen FormIt-Einheiten verwendet.

* **Mullion Width + Depth (Pfostenbreite und -tiefe)**: Die Breite und Tiefe aller Pfostenelemente.
* **Vertical Mullion Spacing (Abstand vertikaler Pfosten)**: Der Abstand (in der Mitte) zwischen den einzelnen vertikalen Pfosten.
* **Flip Vertical Mullion Layout (Layout vertikaler Pfosten umkehren)**: Das Skript beginnt den vertikalen Pfostenabstand von einer Seite, die beliebig ausgewählt werden kann. Wenn der Pfostenabstand auf der falschen Seite für Ihren Anwendungsfall beginnt, setzen Sie diesen Wert auf True, um das Layout so umzukehren, dass es auf der gegenüberliegenden Seite beginnt.
* **Center Vertical mullion Layout (Layout vertikaler Pfosten zentrieren)**: Anstatt die Berechnung des vertikalen Pfostenabstands an einem Ende der Verglasung zu starten, wird hier die Berechnung in der Mitte gestartet und ein symmetrisches Layout vertikaler Pfosten erstellt.
* **First Horizontal Mullion Spacing (Abstand erster horizontaler Pfosten)**: Legt den Abstand des ersten horizontalen Pfostens von unten fest. Diese Option ist nützlich, wenn Sie eine Reihe kürzerer Verglasungsmodule unten benötigen, getrennt vom Rest des Abstands horizontaler Pfosten.
* **Horizontal Mullion Spacing (Abstand horizontaler Pfosten)**: Der typische horizontale Pfostenabstand in der Mitte, beginnend nach dem ersten Pfosten, wie oben beschrieben.
* **Flip Horizontal Mullion Layout (Layout horizontaler Pfosten umkehren)**: Wenn das Layout der horizontalen Pfosten nicht unten, sondern oben beginnen soll, setzen Sie diese Option auf True.
* **Center Horizontal Mullion Layout (Layout horizontaler Pfosten zentrieren)**: Anstatt die Berechnung des horizontalen Pfostenabstands an der Unter- oder Oberseite der Verglasung zu starten, wird hier die Berechnung in der Mitte gestartet und ein symmetrisches Layout horizontaler Pfosten erstellt.

## Verdeckte Optionen

Sie möchten weitere Anpassungen vornehmen? Mehrere erweiterte Optionen werden aus der Gruppe der FormIt-Eigenschaften ausgeblendet, können jedoch durch Klicken auf Edit Embedded Graph (Eingebettetes Diagramm bearbeiten) aufgerufen werden, um den vollständigen Inhalt des Diagramms in Dynamo anzuzeigen:

![](../.gitbook/assets/dynamo-edit-embedded-graph.png)

### Zufällige Pfosten

![](../.gitbook/assets/storefront-curtainwall-random-verticals.png)

* **Randomize Vertical and Horizontal Mullion Layout (Layout vertikaler und horizontaler Pfosten zufällig anordnen)**: Setzen Sie diese Option auf True, um die vertikalen oder horizontalen Pfosten zufällig anzuordnen.
* **Min/Max Mullion Spacing \(if random\) (Min./Max. Pfostenabstand \(falls zufällig\))**: Passen Sie diese Werte an, um einen Bereich von minimalen und maximalen zufälligen Abstandswerten festzulegen.

### Randpfosten

![](../.gitbook/assets/storefront-curtainwall-border-mullion-options.png)

* **Flip Offset Direction of Border Mullions (Versatzrichtung von Randpfosten umkehren)**: Vorgabemäßig verwendet das Pfostensystem die Glasumgrenzung und versetzt sie nach innen, um die Randpfosten zu erstellen. Um sie nach außen zu versetzen, setzen Sie diese Option auf True. Dadurch wird die Gesamtgröße des Pfostensystems außerhalb der Glasumgrenzung um den Wert für Pfostenbreite erhöht.
* **Tolerance Between Selection and Border Mullions (Toleranz zwischen Auswahl und Randpfosten)**: Vorgabemäßig generiert das Pfostensystem Elemente genau an der Glasgrenze, was zu Z-Fighting an den Stellen führen kann, an denen die Glaskante und die äußeren Flächen der Randpfosten kollidieren. In den meisten Fällen ist dies nicht sichtbar. Wenn es für Ihren Fall jedoch erforderlich ist, dass die Kanten des Systems sichtbar sind und Sie Z-Fighting vermeiden möchten, aktivieren Sie diese Option und passen den Toleranzwert nach Bedarf an.

