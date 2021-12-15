# 1.13 – Schnittebenen

_In diesem Kapitel lernen Sie, wie Sie mithilfe von_ _**Schnittebenen**_ _Ihr Modell schneiden, sodass Innenräume und Tragwerkselemente sichtbar werden. FormIt unterstützt mehrere_ _**Schnittebenen**_ _gleichzeitig, um einen Schnittbereich-ähnlichen Effekt zu erzielen._

_Wenn Sie das vorherige Kapitel nicht bearbeitet haben, laden Sie die Datei_ _**1.  13 – Section Planes.axm**_ _aus dem Ordner_ _**FormIt Primer Part 1 Datasets** herunter und öffnen sie._

1 – So erstellen Sie eine neue Schnittebene

1. Klicken Sie auf die Schaltfläche **Schnittebene \(SP\)** im **Standard-Werkzeugkasten**.
2. Bewegen Sie den Cursor über das Modell, um eine Ebene festzulegen, die als Referenz verwendet werden soll. Beachten Sie die Pfeile an den Ecken der **Schnittebene**, die die Schnittrichtung angeben. Drücken Sie die **TABULATORTASTE**, um ggf. zwischen verschiedenen Ebenen zu wechseln.
3. Klicken Sie, um die **Schnittebene** an einer beliebigen Stelle auf der südlichen Glaswand des Hauptgebäudes zu platzieren. Die Ebene wird auf die Größe des Modells skaliert und bleibt ausgewählt.

![Schnittebenenvorschau, wenn Sie den Mauszeiger über die Glaswand bewegen](../../.gitbook/assets/0%20%286%29.png)

![Skalierte Schnittebene nach der Platzierung](../../.gitbook/assets/1%20%2819%29.png)

2 – Klicken Sie bei ausgewählter Schnittebene, um sie nach hinten zu verschieben, bis sie einen Teil des Hauptgebäudes durchschneidet, ähnlich wie in der folgenden Abbildung. Dies funktioniert ähnlich wie das Verschieben eines beliebigen Modellelements, mit der Ausnahme, dass die Schnittebene nur entlang einer Achse verschoben werden kann, die lotrecht zu der Richtung verläuft, in die sie zeigt. Wenn Sie mit der Position zufrieden sind, drücken Sie **ESC**, um die Auswahl aufzuheben.

![](../../.gitbook/assets/2%20%2811%29.png)

_**Anmerkung:**_ _Sie können Ihrem Modell bis zu sechs Schnitte gleichzeitig hinzufügen._

3 – Öffnen Sie die **Layer**-**Palette**. Beachten Sie, dass zwei \(2\) neue Layer erstellt wurden – **Section Indicators** und **Section Cut 1**.

1. Schalten Sie den Layer **Section Cut 1** aus und wieder ein. Damit wird gesteuert, ob der Schnitt das Modell schneidet oder nicht.
2. Deaktivieren Sie nun den Layer **Section Indicators**. Dadurch werden die Schnittebene und die Pfeilindikatoren ausgeblendet. Dies hat jedoch keine Auswirkungen darauf, ob der tatsächliche Schnitt aktiv ist oder nicht.

![](../../.gitbook/assets/3%20%286%29.png)

4 – Gehen Sie auf der **Registerkarte Fläche** der **Palette** **Visuelle Stile** folgendermaßen vor:

1. Aktivieren Sie das Kontrollkästchen neben **Schnittmaterialfarbe**, um die Option zu aktivieren. Bei diesem Effekt werden alle durch die Schnittebene geschnittenen Volumenkörper mit einer bestimmten Farbe eingefärbt. Schwarz ist die Vorgabefarbe. Sie können jedoch einfach auf die Farbvorschau klicken, um die Farbe zu ändern.
2. Deaktivieren Sie **Schatten \(DS\)**.

![](../../.gitbook/assets/poche.png)

5 – Um den Schnitt abzuschließen, wechseln Sie zur **Szenenpalette**, erstellen eine neue Szene mit dem Namen **Section** und speichern die aktuelle **Kameraposition**, die Sichtbarkeit der **Layer** und die Einstellungen für **Visuelle Stile**.

![](../../.gitbook/assets/5%20%287%29.png)

