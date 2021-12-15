# 1.11 – Importieren von Modellen mit Inhaltsbibliothek

_In diesem Kapitel importieren Sie vorhandene SketchUp-Modelle und verwenden die FormIt-Inhaltsbibliothek zum Platzieren von aus Revit konvertierten OOTB-Familien. Beachten Sie, dass SKP-Dateien beim Öffnen mit FormIt intakte Materialien, Gruppen und Komponenten, Layer \(Beschriftungen\) sowie Szenen enthalten. Möglicherweise ist eine Bereinigung erforderlich, um Ihre Projekte übersichtlich und organisiert zu halten._

_In diesem Kapitel verwenden Sie Dateien aus dem Ordner_ **Farnsworth House Data Set &gt; Supporting Files**. Wenn Sie dies nicht bereits getan haben, laden Sie die erforderlichen Ordner oder den gesamten Datensatz aus _**FormIt Primer Part 1 Datasets** herunter._

## **Importieren und Bearbeiten von SKP-Dateien**

_Zunächst fügen Sie Ihrer persönlichen Inhaltsbibliothek einen Teil des heruntergeladenen Inhalts hinzu_. Beachten Sie, dass Sie in dieser Übung nur SKP-Dateien verwenden. Weitere Informationen zum Öffnen/Importieren anderer Dateiformate finden Sie in [**diesem Blog-Post zu den Funktionen von FormIt 2021.2**](https://formit.autodesk.com/blog/post/formit-2021-2-and-new-revit-add-in-now-available) und in **diesem Kapitel über** **Erweiterte Import- und Exportdateiformate**.

1 – Achten Sie darauf, geöffnete Dateien mit **Speichern \(STRG+S\)** zu speichern, und beginnen Sie dann eine neue FormIt-Skizze. Dazu haben Sie folgende Möglichkeiten:

1. Öffnen Sie eine weitere FormIt-Sitzung in einem neuen Fenster, indem Sie mit der rechten Maustaste auf das FormIt-Symbol in der **Windows-Taskleiste** und anschließend auf das **FormIt**-Symbol klicken. Dadurch wird ein neues FormIt-Fenster geöffnet, in dem Sie zwei FormIt-Sitzungen nebeneinander ausführen können.
2. ODER starten Sie nach dem Speichern eine **Neue Skizze \(STRG+N\)** aus der Dropdown-Liste **Datei** in der **Hauptmenüleiste**.

![](../../.gitbook/assets/0%20%2819%29.png)

2 – Erstellen Sie einen neuen Ordner mit dem Namen **Custom FormIt Content** im Ordner **Farnsworth House Data Set &gt; Supporting Files &gt; FormIt** im _**Farnsworth House Data Set**._

3 – **Speichern \(STRG+S\)** Sie die neue Skizze in diesem Ordner. Wir empfehlen, sie wie folgt zu benennen: **Ottoman – Barcelona\_Mies.axm**.

4 – Gehen Sie in der neuen, leeren FormIt-Datei folgendermaßen vor:

1. **Importieren Sie eine lokale Datei \(STRG+I\)**, indem Sie **Importieren &gt; Lokal...** aus der Dropdown-Liste **Datei** in der **Hauptmenüleiste** auswählen.
2. Wählen Sie die Datei **Ottoman – Barcelona\_Mies.skp** unter **Farnsworth House Data Set &gt; Supporting Files &gt; SketchUp** aus, und klicken Sie auf **Öffnen**.

_**Anmerkung:**_ _Wenn die Datei_ _**Ottoman – Barcelona\_Mise.skp** nicht angezeigt wird, stellen Sie sicher, dass die Dropdown-Liste für das Dateiformat unten rechts auf_ _**Alle unterstützten Formate** eingestellt ist._

![](../../.gitbook/assets/1%20%287%29.png)

5 – Benennen Sie die importierte Gruppe in **Ottoman – Barcelona\_Mies** um.

6 – Wenn Sie dieses Modell schließlich in die Farnsworth-House-Datei importieren, wird es mithilfe des **Ursprungspunkts** dieser Datei platziert. Um einen Platzierungspunkt zu kontrollieren, verschieben Sie die Gruppe **Ottoman – Barcelona\_Mies** so, dass sich eine der Ecken am **Ursprung** befindet. Vorgehensweise:

1. Stellen Sie sicher, dass **Rasterfang \(SG\)** aktiviert ist. Zeichnen Sie eine **Referenzlinie \(L\)**, die am **Ursprung** beginnt \(dort schneiden sich die X-, Y- und Z-Achsen\). Klicken Sie an eine beliebige Stelle, um den zweiten Punkt zu platzieren.
2. Wählen Sie die Ottoman-Gruppe aus, und starten Sie den Befehl Verschieben, indem Sie wie dargestellt auf die untere linke Ecke des Beins klicken. _Weitere Informationen zum Verschieben von Objekten finden Sie in den vorherigen Kapiteln._
3. Verschieben Sie die Gruppe zum **Ursprung**, indem Sie den Startpunkt der soeben gezeichneten Referenzlinie fangen.
4. Löschen Sie die Referenzlinie.

![](../../.gitbook/assets/2%20%2817%29.png)

7 – Es wird empfohlen, alle unerwünschten Layer zu löschen, die mit der SKP-Datei importiert wurden, da alle Layer dieses Modells schließlich in das Farnsworth-House-Modell importiert werden. Wechseln Sie dazu zur **Layer-Palette**, wählen Sie **Layer 0** aus, und klicken Sie auf die Schaltfläche **-**. Dadurch wird der Layer gelöscht, während die Geometrie erhalten bleibt.

![](../../.gitbook/assets/3%20%2816%29.png)

_**Anmerkung:**_ _Wenn Sie einen Layer löschen, wird jeder Geometrie bzw. allen Gruppen, die sich auf diesem Layer befanden,_ _**Kein Layer** zugewiesen. Dies ist der Vorgabewert für alle Objekte, die noch keinem Layer zugewiesen wurden._

## **Erstellen von Inhaltsminiaturansichten**

_Im nächsten Schritt wird eine Szene eingerichtet, die als Miniaturansicht für_ _**Inhalte**_ _verwendet und in der_ _**Palette Inhaltsbibliothek** angezeigt wird._

1 – So definieren Sie die Ansichtseinstellungen für die Miniaturansicht-Szene

1. Deaktivieren Sie auf der Registerkarte **Umgebung** der **Palette Visueller Stil** alle Kontrollkästchen, und legen Sie für **Unterer/ Hintergrund** die Farbe Weiß fest.
2. Stellen Sie sicher, dass der Ansichtsmodus auf **Perspektivisch** **\(VP\)** eingestellt ist.
3. Verwenden Sie die **Ansichts- und Navigationswerkzeuge**, um die Ansicht zu vergrößern, und wählen Sie eine Kameraposition aus, die das Objekt genau darstellt, ähnlich wie in der Abbildung unten.

![](../../.gitbook/assets/4%20%2813%29.png)

2 – Erstellen Sie eine Szene, um die soeben festgelegten Einstellungen zu speichern:

1. Wechseln Sie zur **Szenenpalette**.
2. Klicken Sie auf die Schaltfläche **+**. Dadurch wird eine neue Szene basierend auf den aktuellen Einstellungen erstellt.
3. Benennen Sie sie in **Thumbnail** um, und stellen Sie sicher, dass mindestens die ersten vier \(4\) Kontrollkästchen aktiviert sind: **Kamera**, **Layer**, **Sonne und Schatten** sowie **Visuelle Stile**. Die übrigen Szeneneinstellungen sind für die Erstellung der Miniaturansicht nicht relevant.
4. Verwenden Sie die Schaltfläche **Szene aktualisieren**, wenn Sie die **Szene** aktualisieren möchten, um die aktuelle Kameraansicht und die visuellen Einstellungen anzupassen.

![](../../.gitbook/assets/5%20%2811%29.png)

3 – **Speichern \(STRG+S\)** Sie das fertige Ottoman-Modell erneut. Beachten Sie, dass die **Inhaltsminiaturansicht** aus der aktuellen Ansicht erstellt wurde, als das Modell zuletzt gespeichert wurde. Vergewissern Sie sich daher vor dem Speichern, dass Sie sich in der **Miniaturansicht-Szene** befinden.

_Wenn Sie möchten, können Sie Ihre Datei mit unserer Datei vergleichen, indem Sie die Datei_ _**Ottoman – Barcelona\_Mies.axm**_ _öffnen, die unter_ _**Farnsworth House Data Set &gt; Supporting Files &gt; FormIt &gt; Furniture**_ _im_ _**Farnsworth House Data Set** gespeichert ist.‌_

_Führen Sie die oben beschriebenen Schritte auch mit den SKP-Dateien für die Bank und den Stuhl aus, die sich im selben Ordner wie der Polsterhocker befinden._

_**Tipp:**_ _Zur Beschleunigung des Vorgangs empfehlen wir die Verwendung der gerade erstellten Datei_ _**Ottoman – Barcelona\_Mies.axm**_ _als Vorlage. Während des Modellierens können Sie das_ _**Raster**_ _und die_ _**Achsen**_ _erneut über die_ _**Palette Visuelle Stile** aktivieren. Indem Sie nur die Kameraposition der_ _**Miniaturansicht-Szene**_ _für jedes Möbelstück anpassen, stellen Sie sicher, dass die_ _**Inhaltsminiaturansichten**_ _für alle Ihre Inhaltsmodelle konsistent bleiben._

## **Verknüpfen einer Inhaltsbibliothek**

_Nun zurück zu unserem Farnsworth-House-Projekt. Sie werden erfahren, wie Sie den Ordner **FormIt** im Ordner **Farnsworth House Data Set** verknüpfen, um innerhalb des Projekts einfach auf alle zugehörigen Dateien – einschließlich der_ **benutzerdefinierten FormIt-Inhalte**, _die Sie gerade erstellt haben – zuzugreifen._

1 – Gehen Sie nach der Rückkehr zum Farnsworth-House-Modell bzw. nach dem erneuten Öffnen dieses Modells folgendermaßen vor: _Wenn Sie das letzte Kapitel nicht bearbeitet haben, laden Sie die Datei_ _**1.11 – Import Models with Content Library.axm**_ _aus_ _**Farnsworth House Data Set** herunter und öffnen sie._

1. Öffnen Sie die **Palette Inhaltsbibliothek**, und klicken Sie auf das Symbol **Inhaltsbibliothek-Verzeichnis verknüpfen**. Das Fenster **Voreinstellungen** wird mit geöffneter Registerkarte **Inhaltsbibliothek** angezeigt.
2. Klicken Sie auf das **+**-Symbol, um **einen neuen Speicherort für die Inhaltsbibliothek hinzuzufügen**. Ein drittes Fenster wird angezeigt, in dem Sie durch das Verzeichnis Ihres Computers navigieren und einen Ordner auswählen können.
3. Navigieren Sie in _**Farnsworth House Data Set** durch die Ordner:_ _**Supporting Files &gt; FormIt**. Dort finden Sie die_ Ordner mit den **.axm**-Dateien, die Sie zuvor in diesem Kapitel erstellt haben. Doppelklicken Sie auf den Ordner **FormIt**, um ihn auszuwählen.
4. Klicken Sie auf **Ordner auswählen**. Der Pfad dieses Ordners wird in der Gruppe **Bibliotheksspeicherorte – Lokal** angezeigt.
5. Klicken Sie im Fenster **Voreinstellungen** auf **OK**. Der verknüpfte Ordner wird der **Inhaltsbibliothek** hinzugefügt.
6. Um auf diese neue Bibliothek zuzugreifen, öffnen Sie oben das Dropdown-Menü für die **Palette Inhaltsbibliothek** und wählen **FormIt** aus.
7. Beachten Sie, dass die Ordnerstruktur und alle **.axm**-Dateien im verknüpften Ordner in der **Palette Inhaltsbibliothek** angezeigt werden. Doppelklicken Sie auf einen beliebigen Unterordner, um auf die darin enthaltenen Dateien zuzugreifen.

![](../../.gitbook/assets/link-library-content.png)

**Anmerkung:** Wenn Sie Zugriff auf **Autodesk Docs** \(ehemals Autodesk 360\) haben, können Sie auch über das Dropdown-Menü **Inhaltsbibliothek** auf dort gespeicherte Dateien zugreifen.

## **Platzieren von Inhalten aus der Bibliothek**

_‌Nun platzieren Sie die erstellten Inhaltselemente im Farnsworth-Modell._

1 – Damit Sie in das Haus hineinsehen können, um die Möbel zu platzieren, deaktivieren Sie den Layer **Roof**, und **umkreisen \(O\)** Sie die Perspektivansicht, bis das gesamte Geschoss des Hauptgebäudes angezeigt wird.

2 – Stellen Sie sicher, dass in der **Palette Inhaltsbibliothek** das Dropdown-Menü weiterhin auf **FormIt** festgelegt ist. Bevor Sie die Möbel platzieren, die Sie gerade erstellt haben, müssen Sie den Kern des Hauses platzieren:

1. Klicken Sie auf den Ordner **Other**, um ihn zu öffnen, und klicken Sie dann auf die Miniaturansicht von **Farnsworth House – Core**, um diese auszuwählen.
2. Bewegen Sie den Mauszeiger über den Layer **Main Building Floor**, um auf den **Schwerpunkt** des Geschosses zu klicken und den **Kern** zu platzieren.
3. Um zum FormIt-Ordner zurückzukehren, verwenden Sie die Schaltfläche **Nach oben navigieren**.

![](../../.gitbook/assets/7%20%282%29.jpeg)

3 – Legen Sie die Kamera auf **Orthogonal \(VO\)** **Draufsicht \(VT\)** fest, und deaktivieren Sie den Layer **Main Building Floor**, um den Layer **Plan Image** anzuzeigen. In den vorherigen Kapiteln finden Sie weitere Informationen zu den Einstellungen für **Ansichten** und **Layer**.

4 – Wählen Sie den Kern **Farnsworth House – Core** aus, und verschieben Sie diesen, bis er genau am Planbild ausgerichtet ist.

![](../../.gitbook/assets/8%20%281%29.png)

_**Anmerkung:**_ _Achten Sie beim Verschieben des_ _**Kerns** darauf, dass die Höhe nicht geändert wird. Sie können entweder die_ _**UMSCHALTTASTE**_ _verwenden, um die Bewegung so zu beschränken, dass sie immer entlang einer der Achsen verläuft, oder sicherstellen, dass die Start- und Endreferenzpunkte des Befehls_ _**Verschieben \(M\)**_ _auf derselben Höhe liegen, indem Sie nur auf das_ _**Planbild** klicken, nicht auf den_ _**Kern**_ _selbst. In den vorherigen Kapiteln finden Sie weitere Informationen zum Werkzeug_ _**Verschieben \(M\)**__.‌_

## **Platzieren von Möbeln aus der Bibliothek**

1 – Mit einem ähnlichen Verfahren können Sie jetzt die Möbel, die Sie zuvor in diesem Kapitel erstellt haben, aus dem Ordner **Custom FormIt Content** platzieren. Wenn Sie nicht alle drei \(3\) SKP-Dateien konvertiert haben, können Sie stattdessen die vordefinierten Versionen im Ordner **Furniture** verwenden.

_**Anmerkungen:**_

* _Aktivieren Sie den Layer_ _**Main Building Floor**_ _erneut, sodass Sie die Möbel direkt auf der Fläche von_ _**Main Building Floor** platzieren können._
* _Verwenden Sie beim Platzieren eines neuen Objekts die_ _**TABULATORTASTE**_, _um zwischen den Platzierungsebenen zu wechseln._
* _Verwenden Sie beim Platzieren eines neuen Objekts die_ _**LEERTASTE**_, _um dieses vor dem Platzieren in 90°-Intervallen zu drehen._

![](../../.gitbook/assets/9%20%283%29.png)

2 – Sehen Sie sich entsprechend die **Beispiele für Inhaltsbibliotheken** an, um OOTB-Inhalte zu platzieren. Beachten Sie, dass, ähnlich wie Familientypen in Revit, bei vielen von diesen verschiedene Größen zur Auswahl stehen.

![](../../.gitbook/assets/10%20%286%29.png)

## **Verwenden des Werkzeugs Maßstab**

1 – Platzieren Sie mithilfe der gerade erlernten Techniken ein Exemplar der Komponente **tree\_pine** aus dem Ordner **Farnsworth House Data Set &gt; FormIt &gt; Planting**.

1. Wählen Sie nach dem Platzieren die Gruppe aus, und benennen Sie sie in **Tree** um. Klicken Sie mit der rechten Maustaste, um das **Kontextmenü** aufzurufen, und wählen Sie **Ungleichmäßig skalieren \(NU\)**.
2. Klicken Sie auf eine der **Schaltflächen für Ungleichmäßig skalieren**, um die Größe und die Proportionen der Gruppe **Tree** nach Bedarf zu ändern.

![](../../.gitbook/assets/11%20%283%29.png)

![](../../.gitbook/assets/12%20%282%29.png)

_**Anmerkung:**_ _Mit dem Werkzeug_ _**Maßstab \(SC\)**_ _können Sie auf ähnliche Weise auch das gesamte Modell oder die gesamte Gruppe gleichmäßig neu skalieren._

2 – Kopieren Sie diese Gruppe, und platzieren Sie mehrere Bäume um das Haus, indem Sie mithilfe der **Maßstabswerkzeuge** eine Vielzahl von Größen und Proportionen erstellen.

![](../../.gitbook/assets/13%20%286%29.png)

_**Anmerkung:**_ _Obwohl die Bäume alle Exemplare derselben Gruppe darstellen, konnten Sie sie auf unterschiedliche Größen_ _**skalieren**__. Wenn Sie die Optionen_ _**Maßstab \(SC\)**_ _und_ _**Ungleichmäßig skalieren \(NU\)**_ _außerhalb des Gruppenbearbeitungsmodus verwenden, können Sie einzelne Exemplare derselben Gruppe ändern. Wenn Sie eine der_ _**Tree**_-_Gruppen bearbeiten und deren Geometrie oder Material ändern wollten, würden alle Gruppenexemplare dennoch aktualisiert. Jedes Exemplar würde allerdings den aktuellen benutzerdefinierten Maßstab beibehalten. Versuchen Sie es!_

### **Ordnung im Modell halten**

_Denken Sie daran, hinzugefügte Inhalte immer auf Layern einzusortieren. In diesem Beispiel empfehlen wir, den Kern und alle Möbel auf dem Layer_ _**Main Building Floor**_ _und die Bäume auf einem neuen Layer mit dem Namen_ _**Planting** zu platzieren._

