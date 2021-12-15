# Ebenen und Fläche

Nachdem Sie in FormIt Geometrie erstellt haben, können Sie Ebenen anwenden, um anzugeben, wo sich Geschossansichten befinden, und um Flächenberechnungen zu erstellen.

Sehen Sie sich die [FormIt-Einführung](../formit-primer/part-i/adding-floors-with-levels.md) an, um zu erfahren, wie Ebenen in der Praxis funktionieren.

## Erstellen und Konfigurieren von Ebenen

Die Gruppe Ebenen befindet sich rechts in FormIt for Windows:

![](../.gitbook/assets/20191217-levels-panel-1.png)

#### Erstellen und Löschen von Ebenen

* Erstellen Sie eine neue Ebene, indem Sie auf die Schaltfläche + klicken.
* Erstellen Sie eine Reihe von Ebenen, indem Sie auf die Schaltfläche ++ klicken.
   * Auf diese Weise können Sie festlegen, wie viele Ebenen erstellt werden sollen, und den vertikalen Abstand zwischen ihnen festlegen.
* Wählen Sie eine oder mehrere Ebenen aus, und klicken Sie auf -, um sie zu löschen.

#### Umbenennen, Festlegen von Höhen und Neunummerieren von Ebenen

* Benennen Sie eine Ebene um, indem Sie auf den Namen doppelklicken oder indem Sie mit der rechten Maustaste klicken und Namen bearbeiten wählen.
* Passen Sie die Höhe einer Ebene an, indem Sie auf die Zahl doppelklicken oder indem Sie mit der rechten Maustaste klicken und Höhe bearbeiten wählen.
* Klicken Sie oben auf das Symbol Aktualisieren, um die Ebenen neu zu nummerieren.
   * Dies ist hilfreich, wenn Sie Ebenen hinzugefügt oder entfernt haben und das vorgegebene Benennungsschema nicht synchron ist \(z. B. Ebene 1, Ebene 2, Ebene 5\).
   * Mit dieser Schaltfläche werden alle Ebenen mit benutzerdefinierten Namen ignoriert, alle Ebenen mit einem Namen entsprechend der Syntax Ebene 1 werden jedoch neu nummeriert.

## Anwenden von Ebenen

Um Ebenen auf ein Objekt anzuwenden, müssen Sie das Objekt auswählen und direkt zur Gruppe Eigenschaften wechseln.

Beachten Sie, dass zum Anwenden von Ebenen auf ein Objekt das Objekt ein Volumenkörper ohne Rückseite oder Dichtheitsprobleme sein muss. [Erfahren Sie, wie Sie Ihr Modell auf Dichtheit und Probleme mit der Rückseite überprüfen](https://formit.autodesk.com/blog/post/repairing-solid-models).

Wenn im Ansichtsbereich ein Volumenkörperobjekt ausgewählt ist \(in diesem Beispiel eine einfache Gebäudehülle\), wird in der Gruppe Eigenschaften das Kontrollkästchen Ebenen verwenden angezeigt.

* Wenn in der FormIt-Skizze bereits Ebenen definiert sind \(siehe oben\), werden durch Aktivieren dieses Kontrollkästchens alle Ebenen verwendet, die diese Form schneiden würden \(wobei alle Ebenen ignoriert werden, die zu hoch oder zu niedrig wären\).
* Wenn die FormIt-Skizze noch keine Ebenen enthält, werden durch Aktivieren dieses Kontrollkästchens genügend Vorgabeebenen erstellt\(Geschosshöhe 12'\), um die gesamte Form zu schneiden, und diese Ebenen werden automatisch auf dieses Objekt angewendet.

![](../.gitbook/assets/20191217-properties-panel.png)

## Ebenen und Revit

Wenn Ebenen auf FormIt-Geometrie angewendet werden, werden diese Ebenen mithilfe des [FormIt-Zusatzmoduls](https://formit.autodesk.com/page/formit-revit) an Revit gesendet.

In Revit können Sie mithilfe der FormIt-Ebenen mit diesen verknüpfte Körpergeschosse, Geschossdecken über Fläche und Grundrisse erstellen.



