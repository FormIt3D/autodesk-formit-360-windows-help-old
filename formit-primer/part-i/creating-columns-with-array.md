# 1.8 – Erstellen von Stützen mit Reihe

_In dieser Übung skizzieren Sie ein detailliertes Element, eine I-Träger-Stütze. Anschließend erstellen Sie mit dem Werkzeug Reihe schnell mehrere Kopien mit gleichem Abstand._

_Wenn Sie den letzten Abschnitt nicht bearbeitet haben, laden Sie die Datei_ _**1.8 – Create Columns with Array.axm**_ _aus_ _**FormIt Primer Part 1 Datasets** herunter und öffnen sie._

## **Skizzieren des Stützenprofils**

1 – So vereinfachen Sie den Entwurfsprozess

1. Wechseln Sie zur **Draufsicht \(VT\)**.
2. Ändern Sie den Ansichtsmodus in **Orthogonal \(VO\)**.
3. Deaktivieren Sie die Layer **Main Building**, **Floor** und **Roof**. Dadurch wird verhindert, dass die neue Geometrie auf den vorhandenen Geometrien dieser Layer gefangen wird.
4. Vergrößern Sie die obere linke Ecke des Bilds des **importierten Grundrisses**, sodass Sie die Stütze im Detail sehen können.
5. Deaktivieren Sie die Funktion **Rasterfang \(SG\)** \(sofern aktiviert\). Dies hilft beim Zeichnen der Detaillinien.

![](../../.gitbook/assets/0%20%2813%29.png)

_Um die Stütze zu zeichnen, zeichnen Sie zunächst eine Hälfte und spiegeln diese dann, um schnell die andere symmetrische Hälfte zu erstellen._

2 – Zum Erstellen der ersten Hälfte des I-Trägers verwenden Sie das **Werkzeug Linie \(L\)**, um die folgende Skizze mit den angegebenen Bemaßungen zu erstellen. Sie müssen sich noch keine Gedanken über die genaue Position der Stütze auf dem Planbild machen.

![](../../.gitbook/assets/1%20%2818%29.png)

3 – So spiegeln Sie die gerade gezeichnete Form

1. Doppelklicken Sie, um alle Flächen und Kanten der gezeichneten Geometrie auszuwählen.
2. Klicken Sie mit der rechten Maustaste, und wählen Sie das **Werkzeug Spiegeln \(MI\)** aus.
3. Klicken Sie auf den orangefarbenen Griff in der Mitte des **Spiegeln-Widgets**, und platzieren Sie es in der unteren linken Ecke der Geometrie.
4. Verwenden Sie den unteren Pfeil der doppelseitigen Pfeil-Schaltfläche im Widget, um die Spiegelachse um -90 Grad \(im Uhrzeigersinn\) zu drehen.
5. Klicken Sie auf eine beliebige Stelle, oder drücken Sie **ESC**, um den Spiegelvorgang abzuschließen. Das Ergebnis sollte wie ein I-Träger-Profil mit einer Linie in der Mitte aussehen. Drücken Sie erneut **ESC**, um die Auswahl aufzuheben.

![](../../.gitbook/assets/2%20%285%29.png)

![](../../.gitbook/assets/3%20%287%29.png)

_**Anmerkung**: Während Sie das Spiegeln-Widget anpassen, wird in der Vorschau die endgültige Position und Ausrichtung der Geometrie mit der blauen Geisterform angezeigt. Sie können diese Vorschau als Referenz verwenden, um die Geometrie an der gewünschten Position zu spiegeln._

4 – Um beide Seiten zu einer einzigen Geometrie zu verbinden, entfernen Sie die sie trennende Linie, indem Sie zum Auswählen darauf klicken und dann **ENTF** drücken. Jetzt sind die beiden Flächen in einer einzigen Fläche verbunden.

5 – So verschieben Sie die Geometrie an ihre endgültige Position

1. Wenn diese Option deaktiviert ist, aktivieren Sie die Layer **Plan Image** und **Roof**, um sie als Hilfsmittel zu verwenden.
2. Doppelklicken Sie auf das Stützenprofil, um seine Fläche und alle Linien auszuwählen. Verschieben Sie die Auswahl entlang der grünen Achse \(**Y-Achse**\). Halten Sie die **UMSCHALTTASTE** gedrückt, und verschieben Sie das Profil, bis es am Dach ausgerichtet ist. Klicken Sie dann, um es zu platzieren.
3. Verschieben Sie die Geometrie ähnlich wie im vorherigen Schritt erneut, und beschränken Sie sie diesmal auf die rote Achse \(**X-Achse**\).
4. Klicken Sie, um sie auf dem I-Träger zu platzieren, der in **Plan Image** gezeichnet wurde. Es reicht, wenn die Platzierung ungefähr stimmt. Wie Sie im folgenden Bild sehen, muss die horizontale Position nicht perfekt sein.

_**Anmerkung:**_ _Die_ _**UMSCHALTTASTE**_ _beschränkt die Bewegung der Geometrie auf nur eine Achse, in diesem Fall die grüne \(**Y-Achse**\). Dadurch wird sichergestellt, dass das Stützenprofil nicht versehentlich nach oben verschoben und an der Oberseite der Dachebene ausgerichtet wird._

![](../../.gitbook/assets/4%20%289%29.png)

## **Extrudieren und Anordnen der Stütze**

1 – Um den nächsten Zeichenprozess zu erleichtern, ändern Sie den Ansichtsmodus wieder in **Perspektivisch \(VP\)** und **umkreisen \(O\)** die Ansicht, um die Kamera so zu positionieren, dass das I-Träger-Profil aus Nordwest visualisiert wird. Verwenden Sie den Nordpfeil unten links, um die Ansicht zu positionieren.

![](../../.gitbook/assets/5%20%281%29.jpeg)

_**Anmerkung:**_ _Um zu erfahren, wie Sie in der Skizze navigieren, empfehlen wir, das Kapitel_ _**Navigieren in der Szene**_ _zu lesen._

2 – Wählen Sie die Fläche des Stützenprofils aus, und extrudieren Sie die Fläche auf **17'-8"**.

_**Anmerkung:**_ _Wenn das Stützenprofil beim Verschieben am Dach ausgerichtet wird, extrudieren Sie die Fläche um_ _**17'-8"**   nach unten anstatt nach oben._

3 – Verkleinern Sie die Ansicht, und aktivieren Sie den Layer **Roof** \(falls deaktiviert\). Die Oberkante der Stütze sollte an der Oberkante des Dachs ausgerichtet sein.

![](../../.gitbook/assets/6%20%289%29.png)

4 – Um das Modell übersichtlich und ordentlich zu halten, wählen Sie die Stützengeometrie erneut aus und führen die folgenden Schritte durch:

1. **Gruppieren \(G\)** Sie die Geometrie, und nennen Sie sie **Column Tall**.
2. Erstellen Sie einen neuen **Layer** mit der Bezeichnung **Column**, und fügen Sie die Gruppe hinzu.
3. Importieren Sie das Material **Metal – Brushed – Colorized**, und versehen Sie die Gruppe damit.

![](../../.gitbook/assets/7%20%284%29.png)

_**Anmerkung:**_ _Weitere Informationen zu_ _**Gruppen**,_ _**Layern** und_ _**Materialien** finden Sie in den vorherigen Kapiteln._

4 – Klicken Sie auf **ESC**, um das Pinselwerkzeug zu löschen.

## **Stützen in Reihe anordnen**

1 – Wechseln Sie in die **Draufsicht \(VT\)**, und ändern Sie den Kameramodus wieder in **Orthogonal \(VO\)**.

2 – Deaktivieren Sie den Layer **Roof**.

3 – So starten Sie den Reihenprozess

1. Klicken Sie, um die Stützengruppe auszuwählen. Klicken Sie mit der rechten Maustaste, um das **Kontextmenü** aufzurufen, und wählen Sie **Reihe \(AR\)**.
2. Verwenden Sie im Dialogfeld **Reiheneigenschaften**￼ die folgenden Einstellungen:
   * **Länge zwischen Kopien**
   * **Linear** \(Vorgabe\)
   * **Gruppieren: jeder Volumenkörper, dann Reihe** \(Vorgabe\)
   * **Anzahl der Kopien: 3**
   * Klicken Sie auf **OK**, um das Dialogfeld zu schließen.

![](../../.gitbook/assets/8%20%283%29.png)

4 – So platzieren Sie die neuen Elemente

1. Klicken Sie auf die Stütze, um die **Reihe** zu starten. Bewegen Sie den Cursor entlang der roten Achse \(**X-Achse**\).
2. Legen Sie die Bemaßung auf **22'** fest. Sie haben nun **vier** Stützen mit einem Abstand von **22'**.
3. Drücken Sie **ESC**, um die Auswahl aufzuheben.

![](../../.gitbook/assets/9%20%286%29.png)

5 – Um alle Gruppen unter **Tall Column** gleichzeitig auszuwählen, bewegen Sie den Mauszeiger über eine von ihnen und drücken einmal die **TABULATORTASTE**. Beachten Sie, dass alle Begrenzungsrahmen der vier Stützen markiert wurden. Klicken Sie auf die Stütze, über die Sie den Mauszeiger halten. Alle Stützen werden ausgewählt. Dies ist eine schnelle Methode, um alle Exemplare derselben Gruppe gleichzeitig auszuwählen.

6 – Führen Sie eine weitere **Reihe \(AR\)** aus, um die Stützen auf der anderen Seite des Gebäudes zu erstellen. Erstellen Sie dieses Mal eine Kopie entlang der grünen Achse im gesamten Gebäude. Legen Sie die Bemaßung auf **29'-4 5/8" fest.**

_**Anmerkung:**_ _29' 4 5/8" = 8 5/8" \(Stützentiefe\) + 28'-8" \(Hauptgebäudebreite\)_

7 – Um das gesamte Gebäude zu visualisieren, wechseln Sie zur **3D-Ansicht \(V3\)** und legen **Perspektivisch \(VP\)** fest. Wenn diese Option deaktiviert ist, aktivieren Sie die Layer **Main Building Floor**, **Roof**, **Lower Terrace** und **Column**.

![](../../.gitbook/assets/10%20%287%29.png)

## **Erstellen der Terrassenstützen**

_Jetzt duplizieren Sie die Hauptgebäudestützen, um ähnliche, aber kürzere Versionen für die Terrasse zu erstellen._

1 – Um das Zeichnen zu erleichtern, empfehlen wir, zu den Einstellungen **Orthogonal \(OV\)** und **Draufsicht \(VT\)** zurückzukehren.

2 – So erstellen Sie die neuen Stützen

1. Halten Sie die **STRG**- oder **UMSCHALTTASTE** gedrückt, und klicken Sie auf die drei Stützen, die sich am nächsten zum **unteren Terrassenboden** befinden, um sie auszuwählen.
2. Klicken Sie auf eine der Stützen, um alle drei ausgewählten Stützen gleichzeitig zu verschieben. Drücken Sie die **STRG-Taste**, um eine **schnelle Kopie** zu erstellen. Eine Geistervorschau der Kopie wird angezeigt.
3. Verschieben Sie die Kopien entlang der grünen Achse \(**Y-Achse**\) um **23'-4 3/8"** nach unten. Drücken Sie die **ESC**-Taste.
4. Verschieben Sie die kopierten Stützen ohne Abwahl um **22'** entlang der roten Achse \(**X-Achse**\), um sie an ihrer endgültigen Position zu platzieren.
5. Klicken Sie mit der rechten Maustaste auf eine der kopierten Stützen, während die drei neuen Stützen weiterhin ausgewählt sind, und wählen Sie **Als eindeutig definieren \(MU\)** aus. Diese Stützen sind jetzt miteinander verknüpft, unterscheiden sich jedoch eindeutig von den Originalen.

_**Anmerkung:**_ _Halten Sie die_ _**UMSCHALTTASTE**_ _oder_ _**STRG-Taste**_ _gedrückt, wenn Sie mehrere Elemente gleichzeitig auswählen oder Elemente aus der aktuellen Auswahl entfernen möchten._

![](../../.gitbook/assets/11%20%287%29.png)

3 – Ändern Sie die neue Stützengruppe:

1. Doppelklicken Sie, um eine der neuen Gruppen zu bearbeiten, und benennen Sie sie in **Column Short**
2. Passen Sie die Höhe der neuen Stütze so an, dass sie an der Oberseite des **unteren** **Terrassenbodens** ausgerichtet ist \(3'-2"\). Dazu wählen Sie die Stützenfläche aus, ziehen sie entlang der blauen Achse \(**Z-Achse**\) nach unten und halten die **UMSCHALTTASTE** gedrückt. Wenn Sie den Mauszeiger an eine beliebige Stelle auf der oberen Fläche des **unteren Terrassenbodens** setzen, wird die Höhe der Stütze automatisch an der unteren Terrasse ausgerichtet. Klicken Sie nach dem Festlegen der Höhe, um den Vorgang abzuschließen.

![](../../.gitbook/assets/12%20%284%29.png)

_**Anmerkung:**_ _Sie können die Höhe der kurzen Stützen mit dem Werkzeug_ _**Messen \(ME\)**_ _überprüfen. Alternativ können Sie eine der vertikalen Kanten der Stütze auswählen und ihre Länge in der_ _**Eigenschaftenpalette** anzeigen._

4 – Kopieren Sie mithilfe der gerade erlernten Techniken die am weitesten entfernte kurze Stütze auf die gegenüberliegende Seite des **unteren Terrassenbodens**, um die letzte verbleibende Stütze zu erstellen.

![](../../.gitbook/assets/13%20%284%29.png)

