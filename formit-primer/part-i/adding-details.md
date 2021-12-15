# 1.9 – Hinzufügen von Details

_FormIt ist ein hervorragendes Körpermodellwerkzeug und ein exzellentes Modellierungswerkzeug. Beginnen Sie nun, dem Farnsworth House Details in Form von Türen und Pfosten für die Glaszelle hinzuzufügen. Anschließend erfahren Sie mehr über einige zusätzliche Werkzeuge, und Sie werden das Hinzufügen neuer Geometrie, Layer, Materialien und die Gruppenverwaltung üben._

_Wenn Sie den letzten Abschnitt nicht bearbeitet haben, laden Sie die Datei_ _**1.9 – Adding Details.axm**_ _aus_ _**FormIt Primer Part 1 Datasets** herunter, und öffnen Sie sie._

## **Erstellen von Fensterrahmen**

_Sie erstellen einen 2" breiten Metallrahmen und Pfosten um die Glaszelle. Beachten Sie, dass diese Pfosten absichtlich mit der Glaszelle überlappen._

1 – Erstellen Sie einen neuen Layer mit der Bezeichnung **Glass Walls**, und verschieben Sie die Gruppe **Glass Wall** dorthin.

2 – Um die Visualisierung zu erleichtern, deaktivieren Sie den Layer **Roof**, sodass Sie die gesamte Glaszelle sehen können.

3 – So erstellen Sie den ersten Fensterrahmen

1. Zeichnen Sie an der Westseite des Gebäudes mit dem **Werkzeug Rechteck \(R\)** eine neue Fläche direkt über der Glasaußenfläche. Erstellen Sie die Fläche außerhalb der Gruppe **Glass Walls**.
2. Wählen Sie die neu erstellte Fläche aus, und ziehen Sie sie **2"** nach innen. Drücken Sie **ESC**, um die Auswahl aufzuheben. Das endgültige Ergebnis sollte wie die folgende Abbildung aussehen.
3. Klicken Sie auf die Fläche, die Sie gerade erstellt haben. Klicken Sie mit der rechten Maustaste, um das **Kontextmenü** aufzurufen und das **Werkzeug Fläche versetzen \(OF\)**

_**Anmerkung:**_ _Wenn Sie Schwierigkeiten bei der Auswahl der neuen Fläche haben, drücken Sie die_ _**LEERTASTE**_ _, um zwischen verschiedenen auswählbaren Objekten zu wechseln, oder deaktivieren Sie vorübergehend den Layer_ _**Glass Walls**_ _._

![](../../.gitbook/assets/0.jpeg)

4 – Um die Versatzbemaßung festzulegen, bewegen Sie den Mauszeiger zur Innenseite der Fläche, und geben Sie **2"** ein, um ein neues kleineres Rechteck zu erstellen.

![](../../.gitbook/assets/1%20%289%29.png)

5 – Klicken Sie, um das gerade erstellte innere Rechteck auszuwählen. Klicken Sie erneut, und ziehen Sie die Fläche in Richtung Gebäudeinnere, bis sie ausgeblendet wird. Klicken Sie erneut, um den Entfernungsvorgang des mittleren Volumens aus der Rahmengeometrie zu beenden.

![](../../.gitbook/assets/2%20%2821%29.png)

6 – Doppelklicken Sie, um die soeben erstellte Geometrie auszuwählen, und **gruppieren \(G\)** Sie sie. Nennen Sie die Gruppe **Mullion Frame – EW**.

7 – Erstellen Sie einen Layer mit dem Namen **Mullion**, und platzieren Sie die neue Gruppe darauf.

8 – So legen Sie das Material des Rahmens fest

1. Duplizieren Sie in der **Materialpalette** das Material **Metal – Brushed – Colorized**, indem Sie mit der rechten Maustaste darauf klicken und **Material duplizieren** auswählen.
2. Doppelklicken Sie auf die Vorschaukachel des neuen Materials, um es zu bearbeiten.
3. Benennen Sie das Material in **Metal – Brushed – Gray** um.
4. Ändern Sie die Materialfarbe, indem Sie auf die Kachel **Farbe** im Abschnitt **Maps** klicken, und dunkeln Sie das Grau ab, indem Sie **Wert** in **150** ändern.

![](../../.gitbook/assets/3%20%284%29.png)

9 – Klicken Sie auf **OK**, um diese Änderungen am neuen Material zu speichern, und versehen Sie dann die Gruppe **Mullion Frame – EW** mit dem neuen Material. Anschließend sollte die **Eigenschaftenpalette** der Gruppe der folgenden Abbildung entsprechen:

![](../../.gitbook/assets/4.jpeg)

10 – Erstellen Sie mithilfe eines der folgenden Werkzeuge ein neues Exemplar des Rahmens auf der Ostseite: **Schnelles Kopieren**, **Reihe** oder **Spiegeln**.

11 – Wiederholen Sie die obigen Schritte für die Nord- und Südseite der Glaszelle. Nennen Sie die neue Gruppe **Mullion Frame – NS**. Vergessen Sie nicht, die Seiten mit einem Material zu versehen und auf dem Layer **Mullion** zu platzieren.

![](../../.gitbook/assets/5%20%2816%29.png)

_**Anmerkung:**_ _Die Pfostenrahmen überlappen sich an den Ecken. Das ist Absicht. Das obige Ergebnis zeigt die resultierende Pfostenrahmengeometrie mit deaktivierten Layern_ _**Glass Wall**_ _und_ _**Column**_ _._

**Pfosten erstellen**

1 – Zeichnen Sie in der Ebene mit der Glasaußenfläche auf der Süd- oder Nordseite des Gebäudes ein **Rechteck \(R\) mit den Maßen 2" x 10'-10"**, das sich zwischen der Unter- und Oberkante des Pfostenrahmens erstreckt. Sie müssen sich nicht um die genaue Position des Rechtecks entlang des Rahmens kümmern. Es wird in den folgenden Schritten an die gewünschte Position verschoben.

![](../../.gitbook/assets/6%20%2811%29.png)

2 – Extrudieren Sie das Rechteck zurück zum Wert **2"**, **gruppieren \(G\)** Sie es, und geben Sie der Gruppe den Namen **Mullion – Vertical**. Platzieren Sie die Gruppe auf dem Layer **Mullion**, und versehen Sie sie mit dem Material **Metal – Brushed – Grey**.

**Positionieren der Pfosten**

_Jetzt legen Sie die Position für den ersten Pfosten fest, sodass er am_ _**Mittelpunkt**_ _einer Stütze zentriert ist._

1 – Um die Stützen wieder anzuzeigen, aktivieren Sie den Layer **Column**, falls er deaktiviert war. In der **Layer-Palette** können Sie auch die Layer **Lower Terrace** und **Plan Image** deaktivieren, um die nächsten Schritte zu erleichtern.

2 – So verschieben Sie den Pfosten an die neue Position

1. Klicken Sie, um die soeben erstellte vertikale Pfostengruppe auszuwählen. Verwenden Sie **Zoom \(Z\)** zum Vergrößern, und klicken Sie auf den **Mittelpunkt** der unteren Außenkante des Pfostens, der durch ein rotes Dreieck symbolisiert wird**.**
2. Verschieben Sie die Geometrie horizontal in Richtung einer Stütze. Drücken Sie die **UMSCHALTTASTE**, um die Bewegung in der roten Achse \(**X-Achse**\) zu sperren. Beachten Sie, dass die rote Achse dicker wird, sobald die Bewegung gesperrt ist.
3. Verkleinern Sie die Ansicht, bis Sie die Basis der Stütze sehen können. Halten Sie die **UMSCHALTTASTE** gedrückt, und klicken Sie auf den **Mittelpunkt** an der Basis der Außenfläche der Stütze. Der Pfosten wird nur entlang der roten Achse \(**X-Achse**\) verschoben, aber am **Mittelpunkt** ausgerichtet, auf den Sie gerade geklickt haben.

![](../../.gitbook/assets/7%20%281%29.jpeg)

_**Anmerkung:**_ _Der Pfosten befindet sich jetzt direkt hinter der Stütze. Deaktivieren Sie den Layer_ _**Column**_, _oder_ _**umkreisen \(O\)**_ _ Sie die Ansicht, um den Pfosten zu visualisieren._

3 – Drücken Sie **ESC**, um das Werkzeug **Verschieben** zu deaktivieren.

4 – Verwenden Sie das Werkzeug **Reihe \(AR\)** oder **Schnelles Kopieren**, um vier \(4\) weitere vertikale Pfosten mit einem Abstand von **11'** auf derselben Seite zu erstellen. Informationen zur Verwendung des **Werkzeugs Reihe** finden Sie in den vorherigen Kapiteln.

5 – Wählen Sie mit der TABULATORTASTE alle **vertikalen** Pfostengruppen aus, und kopieren Sie sie auf die gegenüberliegende Seite des Gebäudes, sodass sowohl der **Nord**- als auch der **Südrahmen** identische Pfostenlayouts aufweisen, wie in der folgenden Abbildung gezeigt:

![](../../.gitbook/assets/8%20%286%29.png)

## **Erstellen der Türpfosten**

1 – **Umkreisen (O\)** Sie die Perspektivansicht, bis Sie auf die Mitte des westlichen Pfostenrahmens blicken.

2 – Zeichnen Sie ähnlich wie beim Erstellen von Pfostenrahmen ein **3'-6"** breites Türelement mit einem Rahmen von **2" x 2"**. Erstellen Sie eine **Gruppe \(G\)** mit den folgenden Eigenschaften: Gruppenname: **Curtain Wall Door**; Layer: **Mullion**; Material: **Metal – Brushed – Grey**.

3 – Kopieren Sie diese Gruppe, um den zweiten Türrahmen zu erstellen, und verschieben Sie Rahmen so, dass sie sich in der Mitte der Gruppe **Mullion Frame – EW** befinden, wie unten gezeigt.

![](../../.gitbook/assets/9.jpeg)

## **Erstellen eines Dachgesims mit Sweep**

_Sie erstellen nun das Gesims des Farnsworth House mithilfe eines der erweiterten Modellierungswerkzeuge von FormIt:_ _**Sweep**. Weitere Informationen über erweiterte Modellierung finden Sie im Kapitel_ **2.2 –** _**Erweiterte Modellierung** in_ _der_ _**FormIt-Einführung, Teil II**._

_Der erste Schritt beim Erstellen eines_ _**Sweep**_ _besteht darin, ein Profil lotrecht zur Sweep-Extrusion zu zeichnen. Dazu verwenden Sie die Dachgeometrie als Orientierung._

1 – Aktivieren Sie den Layer **Roof**, und vergrößern Sie eine der Ecken.

2 – Zeichnen Sie mithilfe einer der vertikalen Seiten des Dachs als Referenz zwei benachbarte Rechtecke. Die erste ist **6"** hoch und **4 5/8"** breit, und die zweite hat die Maße **2" x 2"**. Löschen Sie die Linie, die die beiden Rechtecke teilt, um eine einzige Fläche zu erhalten. Das Ergebnis sollte der folgenden Abbildung entsprechen.

![](../../.gitbook/assets/10.jpeg)

3 – So erstellen Sie das Sweeping

1. Klicken Sie ohne ausgewählte Geometrie auf die Schaltfläche **Erweiterte Modellierungswerkzeuge** im **Standard-Werkzeugkasten **, und wählen Sie **Sweep \(SW\)** aus.
2. Der **Sweep-Auswahlassistent** wird gestartet und fordert Sie auf, eine **Fläche \(oder Kanten\) für das Sweep-Profil auszuwählen**. Wählen Sie die Profilfläche aus, die Sie gerade erstellt haben.
3. Nachdem Sie das Profil ausgewählt haben, werden Sie aufgefordert, eine **Fläche \(oder Kante\) für den Sweep-Pfad auszuwählen und dann auf Fertig stellen zu klicken**. Wählen Sie die obere Dachfläche aus. FormIt verwendet automatisch die Begrenzungen der ausgewählten Fläche als Sweep-Pfad, und das Sweeping wird um das gesamte Dach erstellt.

_**Anmerkung:**_ _Wenn Sie Schwierigkeiten bei der Auswahl einer der Flächen haben,_ _**umkreisen (O\)**_ _Sie die Ansicht, um die Fläche besser sehen zu können, und versuchen Sie es erneut. Alternativ können Sie auch alle Kanten des Dachs statt der oberen Dachfläche auswählen, um das Sweeping abzuschließen._

![](../../.gitbook/assets/11%20%282%29.png)

4 – Halten Sie Ihr Modell übersichtlich, indem Sie eine Gruppe **Roof – Cornice** erstellen, sie dem Layer **Roof** hinzufügen und ihr das Material **Metal – Brushed – Colorized** zuweisen.

![](../../.gitbook/assets/12%20%281%29.png)

5 – Aktivieren Sie zum Abschluss den Layer **Column**. Sie sehen nun, dass das neu erstellte Sweeping die Oberseiten der Stützen schneidet. Dieses Problem können Sie beheben, indem Sie eine der Gruppen unter **Column Tall** bearbeiten und die obere Fläche nach unten ziehen, bis sie am unteren Rand des Gesims ausgerichtet ist.

![](../../.gitbook/assets/13%20%285%29.png)

