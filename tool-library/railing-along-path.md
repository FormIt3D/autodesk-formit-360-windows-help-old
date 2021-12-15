# Railing Along Path (Geländer entlang Pfad)

## Powered by Dynamo

In FormIt 2021 und höher können Sie ein Geländer entlang eines Pfads erstellen und die Ergebnisse sofort und direkt anpassen. Railing Along Path (Geländer entlang Pfad) wird von Dynamo unterstützt, d. h., das resultierende Geländer kann einfach konfiguriert werden, um die gewünschten Ergebnisse zu erzielen. Durch erneutes Ausführen der Logik wird die Geometrie direkt aktualisiert.

![](../.gitbook/assets/railing-along-path.gif)

## Starten von Railing Along Path (Geländer entlang Pfad)

* Wechseln Sie zur Gruppe Dynamo in FormIt for Windows, und stellen Sie sicher, dass Sie sich im Verzeichnis Dynamo Samples (Dynamo-Beispiele) befinden.
* Klicken Sie auf das Beispiel für Railing Along Path (Geländer entlang Pfad).
* Auf der linken Seite des Bildschirms wird eine Eingabeaufforderung zum Auswählen des Pfads für das Geländer angezeigt.
   * Sie sollten nur eine Reihe von fortlaufenden Kanten oder eine Gruppe, die nur eine Reihe von Kanten enthält, auswählen.
   * Wenn Sie den Pfad ausgewählt haben, klicken Sie auf die Schaltfläche Finish (Fertig stellen), oder drücken Sie die EINGABETASTE.
* In der Gruppe Dynamo wird angezeigt, dass die Änderungen verarbeitet werden. Wenn Sie fertig sind, wird ein in Dynamo generiertes Geländer in einer FormIt-Gruppe angezeigt, das Sie bearbeiten können \(siehe unten\).

## Erstellen von Iterationen an Ort und Stelle

Nachdem Sie Railing Along Path (Geländer entlang Pfad) ausgeführt haben, werden Sie feststellen, dass die Ergebnisse auf die Vorgabewerte eingestellt sind. Diese Einstellungen sind möglicherweise für Sie geeignet. Sie können das Geländer aber auch umfassend an Ihre Anforderungen anpassen.

Wenn Railing Along Path (Geländer entlang Pfad) ausgeführt wird, wird eine neue Gruppe mit den Ergebnissen erstellt. FormIt wählt dann automatisch die Gruppe aus und zeigt die verfügbaren Optionen für dieses Exemplar von Railing Along Path (Geländer entlang Pfad) an.

Sie können jederzeit zu den Eigenschaften für Railing Along Path (Geländer entlang Pfad) zurückkehren, indem Sie die Gruppe auswählen und zur Gruppe Properties (Eigenschaften) wechseln oder die Gruppe bearbeiten, sodass automatisch Properties (Eigenschaften) angezeigt werden.

![](../.gitbook/assets/railing-along-path-options.png)

### Railing Height (Geländerhöhe)

Die Gesamthöhe des Geländers. Verwendet die aktuellen FormIt-Einheiten.

### Post Spacing (Pfostenabstand)

Der Abstand zwischen den vertikalen Hauptpfosten. Verwendet die aktuellen FormIt-Einheiten.

### Add Posts at Path Vertices (Hinzufügen von Pfosten an Pfadscheitelpunkten)

Wenn **True**, werden an jedem Scheitelpunkt des ausgewählten Pfads Pfosten hinzugefügt, und die Berechnung für die nächste Pfostenpositionierung wird an diesem Punkt zurückgesetzt.

Wenn Sie beispielsweise eine Reihe von drei Kanten ausgewählt haben, wird an jedem der beiden inneren Punkte ein Pfosten angezeigt. Dies ist nützlich, wenn die Scheitelpunkte eine Richtungsänderung \(z. B. Treppensteigen oder um die Ecke biegen\) an Stellen angeben, an denen natürlicherweise ein Pfosten auftreten würde.

Wenn **False**, werden Pfosten nur entlang des Pfads hinzugefügt. Dabei wird an einem Ende begonnen, und die Entfernung entlang des Pfads wird gemessen. Dabei werden Scheitelpunkte entlang des Pfads ignoriert. Dies ist hilfreich, wenn Sie einen Bogen, Spline oder Kreis ausgewählt haben, bei dem die Scheitelpunkte nicht von Bedeutung sind und vom Pfostenabstand ignoriert werden sollen.

### Reverse Path Direction (Pfadrichtung umkehren)

Bei der Berechnung der Positionierung der Pfosten bestimmt die Richtung des ausgewählten Pfads, an welchem Ende des Pfads die Abstandsmessung für die Pfosten beginnt.

In Fällen, in denen der Abstand der Pfosten zu einem verbleibendem Abstand an einem unerwünschten Ende des Pfads führt, können Sie diesen Wert in **True** ändern, um die Kurve umzukehren, und die Messung des Pfostenabstands am gegenüberliegenden Ende beginnen.

### Post Width + Depth (Pfostenbreite und -tiefe)

Die Größe \(in der Draufsicht\) der rechteckigen vertikalen Pfostenprofile. Verwendet die aktuellen FormIt-Einheiten.

### Handrail Width + Height (Handlaufbreite und -höhe)

Die Größe \(in der Schnittansicht\) des rechteckigen Handlaufprofils. Verwendet die aktuellen FormIt-Einheiten.

### Baluster Orientation (Ausrichtung der vertikalen Holmen)

Wenn für diese Option True eingestellt ist, werden vertikale Holme wie Kabel horizontal ausgerichtet. Wenn False festgelegt wurde, werden die vertikalen Holme vertikal ausgerichtet, um eine traditionellere Ästhetik zu erzielen.

### Baluster width + Depth (Stärke und Tiefe vertikaler Holme)

Die Größe des rechteckigen Profils von vertikalen Holmen. Verwendet die aktuellen FormIt-Einheiten.

### Baluster Spacing (Abstand vertikaler Holme)

Der Abstand zwischen den einzelnen vertikalen Holmen. Verwendet die aktuellen FormIt-Einheiten.

### Bottom Rail Start Height (Anfangshöhe des Türkantriegels)

Der Abstand zwischen der Unterkante des Geländers und dem Türkantriegel, auf dem die vertikalen Holme aufliegen. Verwendet die aktuellen FormIt-Einheiten.

### Run (Ausführen)

Klicken Sie nach dem Bearbeiten der Optionen auf die Schaltfläche Run (Ausführen), um das zugrunde liegende Dynamo-Diagramm auszuführen und neue Ergebnisse zu generieren. Diese Schaltfläche wird blau, wenn Parameter geändert wurden. So erkennen Sie, dass Sie darauf klicken müssen, um die Aktualisierungen in der endgültigen Geometrie zu sehen.‌

### Edit Embedded Graph (Eingebettetes Diagramm bearbeiten)

Wenn Sie auf diese Schaltfläche klicken, wird die Dynamo-Diagramm-Editor-Umgebung geöffnet, in der Sie das zugrunde liegende Dynamo-Diagramm anzeigen und bearbeiten können, um Parameter schneller zu ändern, Live-Aktualisierungen anzuzeigen oder die Logik zu prüfen bzw. anzupassen.

