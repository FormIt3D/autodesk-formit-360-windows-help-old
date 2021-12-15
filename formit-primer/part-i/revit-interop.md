# 1.15 – Arbeiten mit Revit

_Eine der wichtigsten Funktionen von FormIt ist die Möglichkeit, Ihr Modell von einer flexiblen Modellierungsumgebung wie FormIt in eine leistungsstarke parametrische Umgebung wie Revit zu übertragen. In diesem Kapitel werden einige Übungen beschrieben, mit denen verschiedene Elemente aus FormIt in Revit und aus Revit in FormIt übertragen werden._

_In diesem Kapitel werden Revit-Beispielfamilien verwendet. Falls Sie dies noch nicht getan haben, können Sie diese aus dem Ordner **Farnsworth House Data Set** herunterladen. Wenn Sie das gesamte Lernprogramm bis zu diesem Zeitpunkt noch nicht durchgearbeitet haben, können Sie auch die Datei **1.15 – Working With Revit.axm** aus dem Ordner **FormIt Primer Part 1 Datasets** herunterladen und öffnen._

_In diesen Übungen wird Revit 2022 verwendet, das über verbesserte Interoperabilität mit FormIt verfügt. Vorherige Versionen von Revit enthalten nicht alle Funktionen, die in diesem Lernprogramm vorgestellt werden, und haben eine andere Benutzeroberfläche._

## Von Revit nach FormIt

### Konvertieren von Revit-Familien zur Verwendung in FormIt

Wenn Sie \(oder Ihr Unternehmen\) einen Satz von Revit-Familien haben, die Sie in FormIt verwenden möchten, dann werden Sie an diesem Abschnitt interessiert sein, in dem beschrieben wird, wie Sie RFA-Dateien per Stapelexport nach FormIt übertragen.

_**Anmerkung:**_ _Die folgenden Schritte zeigen die Benutzeroberfläche und die erforderlichen Schritte bei der Verwendung von Revit 2022. Die Werkzeuge zum_ _**Konvertieren von RFA-Dateien für FormIt**_ _sind jedoch seit Revit 2016 verfügbar._

1 – Öffnen Sie ein neues Revit-Projekt oder eine neue Revit-Familie. Gehen Sie anschließend wie folgt vor:

1. Suchen Sie in der Multifunktionsleiste **Zusatzmodule** die Gruppe **FormIt-Konverter**, und klicken Sie auf die Schaltfläche **RFA in FormIt konvertieren**. Das **Dialogfeld Revit-Familien konvertieren** wird angezeigt.
2. Navigieren Sie im Feld **Pfad zu Revit-Familiendateien** zum Speicherort des folgenden Ordners auf Ihrem Computer: **Farnsworth House Data Set &gt; Supporting Files &gt; Revit**.
3. Navigieren Sie im Feld **Pfad zu FormIt-Inhalten** zu **Farnsworth House Data Set &gt; Supporting Files &gt; FormIt &gt; Custom FormIt Content**. Wenn Sie Kapitel **1.11 Importieren von Modellen mit der Inhaltsbibliothek** noch nicht abgeschlossen haben, müssen Sie möglicherweise den Ordner **Custom FormIt Content** erstellen oder ein anderes Ziel auswählen.
4. Klicken Sie auf **OK**, um die Konvertierung zu starten.

![](../../.gitbook/assets/0%20%2823%29.png)

_**Anmerkungen:**_

* _Dieser Vorgang kann einige Zeit in Anspruch nehmen, da Revit die_ _**RFA**_-_Datei im ersten Pfad öffnet, sie dann konvertiert und im_ _**AXMF**_-_Format für FormIt speichert._
* _In dieser Übung konvertieren Sie nur eine einzelne Datei. Sie können dieses Verfahren jedoch auch verwenden, um alle_ _**RFA**_-_Dateien im ausgewählten Ordner \(einschließlich aller_ _**RFA**_-_Dateien in verschachtelten Ordnern\) im Stapel zu konvertieren._

2 – Wenn der Vorgang abgeschlossen ist, kehren Sie zu FormIt zurück. Dort sehen Sie den neuen Inhalt in der **Palette Inhaltsbibliothek** im Ordner **FormIt &gt;** **Custom FormIt Content**, den Sie zuvor verknüpft haben. Wenn Sie die konvertierten **AXMF**-Dateien an einem anderen Speicherort gespeichert haben oder Kapitel **1.11 Importieren von Modellen mit der Inhaltsbibliothek** nicht abgeschlossen haben, müssen Sie diesen Ordner möglicherweise Ihrer Inhaltsbibliothek hinzufügen, um den Inhalt anzuzeigen. In Kapitel 1.11 finden Sie Anweisungen zum Hinzufügen von Ordnern zu Ihrer Inhaltsbibliothek.

![](../../.gitbook/assets/1%20%2824%29.png)‌

**Anmerkung**: _Nicht alle Kategorien aus Revit werden für den Export unterstützt. Die freistehenden oder ebenenbasierten Familien werden unterstützt, die basisbauteilbasierten Familien wie Türen und Fenster jedoch nicht. Körper, Schreinerarbeiten, Umgebung, Möbel, Möbelsystem, Allgemeines Modell, Parkplatz, Grundstück und Sonderausstattung werden alle unterstützt. Alle nicht unterstützten Familien im ausgewählten Ordner werden einfach übersprungen._

## Aus FormIt nach Revit

_Es gibt zwei verschiedene Möglichkeiten, Geometrie aus FormIt nach Revit zu übertragen. Sie können eine vorhandene_ _**.axm**-Datei in ein Revit-Projekt oder eine Revit-Familiendatei importieren, die sich ähnlich wie ein importiertes Modell oder eine importierte CAD-Datei verhält. Alternativ können Sie FormIt in Revit starten und jede FormIt-Gruppe als einzelnes Element des Typs Allgemeines Modell in Revit importieren. Die zweite Methode wird in **Teil II** im Kapitel_ _**2.8**_ _**Erweiterte Revit-Arbeitsabläufe** behandelt._

### Importieren des Farnsworth-Hauses in Revit

1 – Um eine FormIt-Datei \(**.axm**\) in Revit zu importieren, starten Sie ein neues Revit-Projekt und öffnen die vorgegebene 3D-Ansicht. Gehen Sie anschließend wie folgt vor:

1. Wechseln Sie zur **Registerkarte Einfügen**, und klicken Sie auf die Schaltfläche **CAD importieren**. Das Fenster **CAD-Formate importieren** wird geöffnet.
2. Stellen Sie sicher, dass die Dropdown-Liste **Dateityp** auf **FormIt-Dateien \(\*.axm\)** festgelegt ist.
3. Navigieren Sie zu der Farnsworth-Datei (**.axm**), an der Sie gearbeitet haben, und wählen Sie sie aus. Wenn Sie den ersten Teil der Einführung nicht durchgearbeitet haben, können Sie auch die Datei **1.15 – Working With Revit.axm** im Ordner **Farnsworth House Data Set &gt; Chapter Files** öffnen.
4. Stellen Sie sicher, dass **FormIt-Ebenen importieren** aktiviert ist.
5. Nachdem Sie die Einstellungen definiert haben, klicken Sie auf **Öffnen**. Die FormIt-Geometrie wird als einzelnes Element in Revit importiert.

![](../../.gitbook/assets/2%20%2824%29.png)

Importieren einer FormIt-Datei mithilfe der Schaltfläche CAD importieren

![](../../.gitbook/assets/3%20%2821%29.png)  
Importiertes AXM-Element. Beachten Sie, dass die Ebenen aus dem FormIt-Modell ebenfalls in Revit importiert werden.

_Ähnlich wie bei anderen CAD-Formaten werden die Layer in der ursprünglichen Datei in Revit importiert. Mit dieser Funktion können Sie verschiedene Sichtbarkeitseinstellungen für die einzelnen Layer definieren, um die grafische Darstellung Ihrer FormIt-Datei in jeder Revit-Ansicht einfach zu ändern._

2 – So passen Sie die Layer-Sichtbarkeit der importierten AXM-Datei an

1. Wechseln Sie im Fenster **Überschreibungen Sichtbarkeit/Grafiken \(VG oder VV\)** zur Registerkarte **Importierte Kategorien**, erweitern Sie die importierte FormIt-Datei, deaktivieren Sie den Layer **Planting**, um den Layer in der aktuellen Ansicht auszuschalten, und klicken Sie auf **OK**.
2. Ändern Sie den **visuellen Stil** in **Realistisch**. Sie werden sehen, dass alle FormIt-Materialien in Revit importiert wurden.

![](../../.gitbook/assets/4%20%2820%29.png)

3 – Die importierten FormIt-Materialien sind jetzt in diesem Revit-Projekt verfügbar, das mit der Klasse **FormIt** gekennzeichnet ist. Öffnen Sie einfach den **Material-Browser**, suchen Sie nach FormIt, und Sie sehen alle Materialien. Diese können nun wie alle anderen Materialien in Ihrem Revit-Projekt verwendet werden.

![](../../.gitbook/assets/5%20%2819%29.png)

