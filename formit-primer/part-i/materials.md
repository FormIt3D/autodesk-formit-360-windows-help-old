# 1.7 – Farbe und Materialien

Wie Sie in einer **früheren Übung** gesehen haben, können Sie Ihre eigenen Materialien erstellen und dann in FormIt Flächen mit diesen Materialien versehen. In dieser Übung erstellen und bearbeiten Sie weitere Materialien und importieren Materialien aus der Autodesk-Materialbibliothek.

_Wenn Sie den letzten Abschnitt nicht bearbeitet haben, laden Sie die Datei_ _**1.7 – Paint with Materials.axm**_ _aus_ _**FormIt Primer Part 1 Datasets** herunter und öffnen sie._

## **Erstellen der Glaswände**

1 – Um den Plan mit den Bemaßungen anzuzeigen, die Sie referenzieren möchten, wechseln Sie zur **Layer-Palette** und aktivieren den Layer **Plan Image**.

2 – Wählen Sie das **Werkzeug Rechteck \(R\)** aus. Sie erstellen ein Rechteck direkt über der vorhandenen Geschossdeckengruppe. Vergewissern Sie sich, dass Sie nicht die Geschossdeckengruppe bearbeiten, sondern auf dem vorhandenen gruppierten Objekt zeichnen.

![](../../.gitbook/assets/0%20%283%29.png)

3 – So starten Sie das Rechteck für die Glasfläche

1. Klicken Sie auf die hintere Ecke der vorhandenen Geschossdecke, und bewegen Sie die Maus entlang der kürzeren Kante.
2. Geben Sie **28'-8"** ein, um die erste Kantenlänge zu definieren, und klicken Sie auf **OK**. Diese sollte die gleiche Länge wie die vorhandene kurze Kante der Geschossdecke haben.
3. Um die zweite Kante zu definieren, bewegen Sie den Mauszeiger entlang der längeren Kante der vorhandenen Geschossdecke. Geben Sie **55'-5 ½"** ein, um die Länge der zweiten Kante festzulegen, und klicken Sie dann auf **OK**.
4. Drücken Sie **ESC**, um das Werkzeug Rechteck zu beenden. Klicken Sie in das neue Rechteck, um die Fläche auszuwählen, und ziehen Sie sie nach oben.

![](../../.gitbook/assets/1%20%283%29.png)

4 – Zum Definieren der Höhe bewegen Sie die Maus entlang der **Z-Achse** nach oben, drücken die **TABULATORTASTE** und geben **11'-2"** ein.

![](../../.gitbook/assets/2%20%284%29.png)

_**Anmerkung:**_ _Wenn Sie ein Werkzeug verwenden, für das Sie eine Bemaßung eingeben können, können Sie entweder die_ _**TABULATORTASTE**_ _drücken oder einfach mit der Eingabe von Zahlen beginnen._

5 – Doppelklicken Sie auf die neue Geometrie, und **gruppieren \(G\)** Sie sie.

6 – Doppelklicken Sie auf die Gruppe, um sie zu bearbeiten. Geben Sie der Gruppe in der **Eigenschaftenpalette** den Namen **Glass Walls**

![](../../.gitbook/assets/3%20%283%29.png)

7 – So definieren Sie die Glaswandstärke

1. Klicken Sie mit der rechten Maustaste auf die obere Fläche, und wählen Sie das **Werkzeug Fläche versetzen \(OF\)**
2. Bewegen Sie den Mauszeiger nach innen, und geben Sie **4"**
3. Drücken Sie zweimal **ESC**, um das Werkzeug und die Auswahl zu löschen.

![](../../.gitbook/assets/4%20%2817%29.png)

​_**Anmerkung:**_ _Die Vorgabeeinheit für Projekte mit britischen Einheiten sind Fuß, ähnlich wie in Revit. Wenn Sie eine einzelne Zahl ohne eine bestimmte Einheit eingeben, wie z. B._ _**4**, erhalten Sie_ _**4 Fuß \(4'\)**_ _und nicht_ _**4 Zoll \(4"\)**._

8 – Um den Innenbereich zu gestalten, klicken Sie auf die obere Innenfläche, um sie auszuwählen, und klicken Sie dann erneut, um den Vorgang **Fläche ziehen** zu starten. Drücken Sie die Fläche ganz nach unten, bis sie ausgeblendet wird, und klicken Sie in den Raum, um den Vorgang abzuschließen.

![](../../.gitbook/assets/5%20%2812%29.png)

_**Anmerkung:**_ _Im Gegensatz zu anderer Software können Sie in FormIt die Fläche, die Sie löschen möchten, nicht versehentlich zu weit verschieben, sodass eine neue negative Extrusion erstellt wird._

9 – Beenden Sie den Modus **Gruppe bearbeiten**, indem Sie im Raum doppelklicken oder **ESC**

10 – Wählen Sie die Gruppe **Glass Walls** mit einem einzigen Klick aus, und legen Sie sie auf dem Layer **Main Building Floor** ab.

![](../../.gitbook/assets/6%20%2813%29.png)

## **Importieren eines Materials aus der Autodesk-Materialbibliothek**

1 – Bearbeiten Sie die Gruppe **Glass Walls** erneut, indem Sie darauf doppelklicken.

2 – So importieren Sie ein neues Material in das Modell

1. Wechseln Sie zur **Materialpalette**.
2. Wählen Sie **Materialmuster** im Dropdown-Menü oben in der Palette aus, um durch die **Autodesk-Materialbibliothek** zu navigieren. 
3. Klicken Sie auf den Ordner **Glas/Verglasung**, um ihn zu öffnen.
4. Suchen Sie das Material **Glass – Blue Tint**, und klicken Sie darauf, um das Material der Materialbibliothek **In Skizze** hinzuzufügen.
5. Beachten Sie, dass Sie sich wieder in der Bibliothek **In Skizze** befinden sollten, die jetzt das neu ausgewählte Material enthält.

![](../../.gitbook/assets/7%20%288%29.png)

![](../../.gitbook/assets/8%20%288%29.png)

3 – Nach dem Hinzufügen des Materials sollte automatisch das **Pinselwerkzeug** aktiviert sein. Wenn nicht, klicken Sie einfach erneut auf das Material **Glass – Blue Tint**. Um alle Wände mit einem Material zu versehen, doppelklicken Sie mit dem **Pinselwerkzeug** auf die Geometrie. Dadurch wird das ausgewählte Material auf das gesamte Objekt angewendet. ![](../../.gitbook/assets/9%20%281%29.png)​

4 – Klicken Sie auf **ESC**, um das **Pinselwerkzeug** zu beenden. Drücken Sie erneut auf **ESC**, oder doppelklicken Sie in den Raum, um die Gruppe zu verlassen.

## **Schnelles Kopieren des Geschosses zum Erstellen des Dachs**

1 – So erstellen Sie schnell das Dach basierend auf der Geschossgeometrie

1. Wählen Sie die Gruppe **Floor** mit einem Mausklick aus.
2. Klicken Sie auf eine der unteren Ecken, um das Werkzeug **Verschieben** zu starten.
3. Verschieben Sie das Geschoss entlang der blauen Achse \(**Z-Achse**\) nach oben. Erstellen Sie eine **schnelle Kopie**, indem Sie auf die **STRG-Taste** tippen. Eine Geistervorschau der Kopie sollte angezeigt werden. ​
4. Geben Sie beim Verschieben entlang der blauen Achse \(**Z-Achse**\) zunächst **12' 2"** ein. Daraufhin wird das **Dialogfeld Bemaßung** angezeigt. Klicken Sie auf **OK**, oder drücken Sie die **EINGABETASTE**, um die Position abzuschließen.

![](../../.gitbook/assets/10%20%281%29.png)

![](../../.gitbook/assets/11%20%281%29.png)

## **Bearbeiten des Dachs**

1 – Verwenden Sie bei ausgewählter kopierter Gruppe den Befehl **Als eindeutig definieren \(MU\)**, um die Verknüpfung dieser Gruppe mit der Geschossgruppe zu trennen.

2 – Doppelklicken Sie auf die Gruppe, um sie zu bearbeiten. Benennen Sie die Gruppe in der **Eigenschaftenpalette** in **Roof** um. Verlassen Sie die Gruppe, indem Sie im Raum doppelklicken.

3 – Erstellen Sie in der **Layer-Palette** einen neuen **Layer** mit der Bezeichnung **Roof**, und fügen Sie die Gruppe **Roof** hinzu. Sie können den Layer aktivieren und deaktivieren, um zu überprüfen, ob die richtigen Elemente auf dem Dach vorhanden sind. Weitere Informationen zum Arbeiten mit **Layern** finden Sie in **Kapitel 6**.

4 – Navigieren Sie zurück zur **Materialpalette**, und importieren Sie das Material **Concrete – Broom Finish – Colorized 1** aus dem Ordner **Beton und Asphalt** in der Bibliothek **Materialmuster** **\(Produktion\)**. Beachten Sie, dass durch Klicken auf das Material die ausgewählte Geometrie automatisch mit dem Material versehen und das neue Material der Materialbibliothek **In Skizze** hinzugefügt wird.

![](../../.gitbook/assets/12.jpeg)

_**Anmerkung:**_ _Das Auftragen eines Materials für eine Gruppe außerhalb des_ _**Gruppenbearbeitungsmodus**_ _ist eine nützliche Methode, mit der Sie verschiedene Exemplare derselben Gruppe mit unterschiedlichen Materialien versehen können._

## **Erstellen der unteren Terrasse**

1 – Erstellen Sie basierend auf dem Layer **Plan Image** die untere Terrasse als **Rechteck \(R\)** mit einer Länge von **55' 3"** und einer Breite von **22'-7 3/4"**, und extrudieren Sie sie um 1'. Positionieren Sie das neue Rechteck so, dass es 8 5/8" von der Südkante des Hauptgebäudes entfernt ist \(die Tiefe der Stützen wird später erstellt\).

_**Anmerkungen**:_

* _In den vorherigen Kapiteln erfahren Sie, wie Sie Rechtecke zeichnen und extrudieren._
* _Möglicherweise müssen Sie_ _**Raster fangen \(SG\)**_ _aktivieren oder deaktivieren, um auf die_ Ecke der Terrasse zu klicken.

2 – So schließen Sie die untere Terrasse ab

1. **Gruppieren \(G\)** Sie die Geometrie, und nennen Sie sie **Lower Terrace Floor**.
2. **Verschieben** Sie die Gruppe um **2'-2"** von der Grundebene nach oben.
3. Erstellen Sie einen neuen **Layer** mit der Bezeichnung **Lower Terrace**, und fügen Sie die Gruppe hinzu.
4. Fügen Sie **Terrace Level Floor** der Gruppe hinzu.

![](../../.gitbook/assets/13%20%281%29.png)

_**Anmerkung:**_ _Diese Abbildung stellt nicht den Schritt-für-Schritt-Prozess zum Erstellen und Zuweisen der Geometrie zu Gruppen, Ebenen und Layern dar. Weitere Informationen zu diesen Prozessen finden Sie in den vorherigen Kapiteln in dieser Einführung._

3 – Importieren Sie das Material **Stone &gt; Stone – Travertine**.

4 – Suchen Sie in der **Materialpalette** das importierte **Travertin**-Material, und ändern Sie es:

1. Doppelklicken Sie auf die Vorschaukachel, um das Popup-Fenster **Material-Editor** zu öffnen.
2. Klicken Sie auf die Vorschaukachel **Farbe**, um das Popup-Fenster **Farbeditor** zu öffnen.
3. Ändern Sie den Wert im Feld **Wert** in **190**, um die Tönung des Materials abzudunkeln.

![](../../.gitbook/assets/14%20%282%29.png)

5 – **Versehen** Sie die Gruppen **Floor** und **Lower Terrace Floor** mit dem geänderten **Travertin**-Material.

![](../../.gitbook/assets/15.jpeg)

