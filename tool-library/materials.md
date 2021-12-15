# Materialien

Versehen Sie Ihre FormIt-Modelle mit Materialien, die Reflexions-, Glanz- und Relief-Maps unterstützen.

## Gruppe Materialien

![](<../.gitbook/assets/materials-sample-category (2).png>)

In der Gruppe Materialien können Sie aus einer Vielzahl von Materialmustern wählen, zwischen verknüpften Materialbibliotheken navigieren und ab FormIt 2021 auf die Materialinhalte anderer FormIt-Dateien (.AXM) zugreifen und diese verwenden.

### Materialbibliotheksquellen

In FormIt 2021 und höher verfügt die Gruppe Materialien über eine Dropdown-Benutzeroberfläche, in der Sie aus den verfügbaren Materialbibliotheksquellen wählen können: In Skizze, Materialmuster und [verknüpfte Bibliotheken](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

![](<../.gitbook/assets/materials-directory-picker (1).png>)

#### In Skizze

Zeigt die Materialien an, die in der aktuellen FormIt-Skizze gespeichert sind.

#### Materialmuster

Zeigt eine Liste der verfügbaren Mustermaterialien an. Diese Angebote werden auf einem Cloud-basierten Server gespeichert. Beachten Sie daher Folgendes:

* Eine Internetverbindung ist erforderlich, wenn Sie zum ersten Mal auf die Kategorien für Materialmuster zugreifen.
* Wenn Sie eine Kategorie zum ersten Mal aufrufen, wird sie heruntergeladen und dann auf Ihrem Computer zwischengespeichert, sodass für zukünftige Sitzungen kein Herunterladen mehr erforderlich ist.
* Das FormIt-Team kann gelegentlich die Angebote in den Materialmustern aktualisieren. In diesem Fall werden die Kategorien von FormIt automatisch gelöscht und erneut heruntergeladen, um die neueste Version zu erhalten.

![](../.gitbook/assets/materials-samples\_original.png)

**Verknüpfte Bibliotheken**

Nach dem [Verknüpfen von Materialbibliotheken](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries) werden andere Verzeichnisse und Speicherorte angezeigt.

### Erstellen, Löschen und Pipette

![](../.gitbook/assets/materials\_add.PNG) **Erstellen Sie ein neues Material**, indem Sie die Einstellungen für Farbe, Textur, Relief-Map, Ausschnitt-Map, Transparenz und Reflexion/Glanz festlegen.

![](<../.gitbook/assets/materials\_delete (1) (1).PNG>) **Löschen** Sie die ausgewählten Materialien.

Verwenden Sie ![](../.gitbook/assets/materials\_eyedropper.PNG) **Pipette** für ein Material, das in der Szene vorhanden ist, und nutzen Sie es sofort zum Auftragen.

* Klicken Sie auf das Werkzeug Pipette und dann auf eine mit einem Material versehene Fläche.
* Das Material auf der Fläche wird in der Gruppe hervorgehoben, das Pinselwerkzeug wird aktiviert, und das Material wird geladen.

### Aktualisieren, Bibliotheken verknüpfen und Nicht verwendete bereinigen

\*\*\*\*![](../.gitbook/assets/materials-link.png) **Verknüpfen Sie Materialbibliotheken** aus lokalen Verzeichnissen. In Verzeichnissen mit JPG-, PNG- oder AXM-Dateien (FormIt) werden Inhalte angezeigt. Weitere Informationen finden Sie unter [Verknüpfen von Materialbibliotheken](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

![](../.gitbook/assets/materials-refresh.png)**Aktualisieren** Sie das aktuelle Verzeichnis. Nur aktiviert, wenn ein lokal verknüpftes Verzeichnis angezeigt wird (nicht In Skizze oder Materialmuster).

![](../.gitbook/assets/materials-purge.png) **Bereinigen Sie nicht verwendete** Materialien aus der aktuellen FormIt-Skizze.

Nicht verwendete Materialien können sich naturgemäß aufgrund von Iterationen ansammeln. Durch sie wird allerdings unter Umständen die Dateigröße erheblich erhöht, wenn sie qualitativ hochwertige Texturen umfassen.

Nicht verwendete Materialien werden in der Liste In Skizze grau angezeigt.

Klicken Sie auf das Werkzeug Nicht verwendete bereinigen, um alle nicht verwendeten Materialien zu löschen. Sie werden noch einmal zur Bestätigung aufgefordert. Wenn Sie sich umentschieden haben, können Sie den Vorgang also noch abbrechen. Diese Schaltfläche ist nur in der Liste In Skizze aktiviert.

### Verknüpfen von Materialbibliotheken

FormIt 2021 und höher bietet die Möglichkeit, die Gruppe Materialien mit lokalen Verzeichnissen (Bibliotheken) zu verknüpfen, in denen sich Materialinhalte befinden, einschließlich Ordnern mit JPG-, PNG- und/oder FormIt-Dateien:

![](../.gitbook/assets/materials-axms.png)

![Zeigen Sie einzelne Materialien aus einer FormIt-Datei oder JPG-/PNG-Dateien in einem Verzeichnis an.](../.gitbook/assets/materials-axm-content.png)

* **JPG-/PNG-Dateien** werden als Materialien angezeigt, die direkt in die aktuelle FormIt-Skizze integriert werden können.
   * Wenn Sie auf eine Miniaturansicht klicken, wird die Bilddatei sofort in ein FormIt-Material konvertiert und in die aktuelle Skizze kopiert.
   * FormIt wechselt zurück zum Verzeichnis In Skizze, in dem das Material angezeigt wird, das Sie gerade in die Skizze kopiert haben.
* **FormIt-Dateien (\*.axm)** werden als Ordner mit einem FormIt-Symbol angezeigt.
   * Wenn Sie auf die FormIt-Dateiordner klicken, werden alle in dieser Datei gespeicherten FormIt-Materialien angezeigt.
   * Beachten Sie, dass FormIt einen Teil der Datei laden muss, um den Materialinhalt abzurufen. Bei größeren Dateien kann es daher länger dauern, Materialien in der Gruppe anzuzeigen.

### Materialinteraktionen

**Tragen Sie ein Material auf**, indem Sie auf die Miniaturansicht klicken. Das Pinselwerkzeug wird geöffnet, in dem Sie dann den Mauszeiger über die Geometrie im FormIt-Ansichtsbereich bewegen und auf Flächen oder Gruppen klicken können, um sie mit einem Material zu versehen.

Wenn Sie das Pinselwerkzeug aufgerufen haben:

* Versehen Sie Flächen und Gruppen durch einfaches Klicken mit einem Material.
   * Wenn Sie Gruppen mit einem Material versehen, wird das Material auf die verschachtelte Geometrie kaskadiert, und alle Flächen oder Gruppen, die mit dem Vorgabematerial versehen wurden, werden bedeckt.
* Versehen Sie ganze Volumenkörper mit einem Material, indem Sie auf eine Fläche doppelklicken, um alle zugeordneten Objekte auszuwählen.

Sie können auch zuerst Flächen und Gruppen auswählen und dann auf die Miniaturansicht eines Materials klicken, um die Auswahl mit diesem Material zu versehen.

**Bearbeiten Sie ein Material**, indem Sie auf die Miniaturansicht doppelklicken. Dadurch wird der Material-Editor geöffnet (siehe unten).

**Benennen Sie ein Material um**, indem Sie darauf doppelklicken.

**Identifizieren Sie ein Material**, das auf Geometrie aufgetragen wurde, indem Sie es auswählen und nach der Hervorhebung und dem Symbol suchen, die angeben, welche Materialien auf die ausgewählte Geometrie aufgetragen wurden.

![](../.gitbook/assets/material\_selected.png)

Das **Vorgabematerial** kann verwendet werden, um eine Fläche oder eine Gruppe mit beliebigen Materialien effektiv zu löschen. Geometrien, auf die kein Material aufgetragen wird, werden implizit mit dem Vorgabematerial versehen.

### Listenverwaltung

Passen Sie die Größe der Miniaturansichten an, indem Sie die Breite der Spalte anpassen (klicken Sie auf die vertikale Linie, und ziehen Sie sie nach rechts neben Material).

Filtern Sie nach bestimmten Materialien, indem Sie in der Filterleiste einen Begriff eingeben.

Materialien mit Namen, die in grauer Schrift angezeigt werden, weisen auf Materialien hin, die nicht in der aktuellen Skizze verwendet werden.

## Erstellen und Bearbeiten von Materialien

![](<../.gitbook/assets/materials-editor (1).png>)

Wenn Sie ein Material erstellen oder bearbeiten, wird das Dialogfeld Material-Editor angezeigt, in dem Sie Folgendes anpassen können:

* **Farbe**
* **Bild-Maps**
   * Klicken Sie auf die Miniaturansicht, um eine neue Map auszuwählen.
   * Klicken Sie auf das Symbol Speichern, um die Map zur Bearbeitung in einer anderen Anwendung zu speichern.
   * Klicken Sie auf das Symbol Löschen, um die Map aus diesem Material zu löschen.
      * **Textur aus einer Bilddatei**
         * JPG oder PNG
      * **Relief-Map aus einer Bilddatei**
         * JPG wird empfohlen
         * Diese Option eignet sich hervorragend zum Hinzufügen von Tiefeneffekten zu Materialien.
         * Sie können Freeware wie ShaderMap verwenden, um Relief-Maps für eine bestimmte Textur zu generieren.
      * **Ausschnitt-Map aus einer Bilddatei**
         * PNG
         * Diese Option eignet sich hervorragend für Materialien mit selektiver Transparenz, wie Maschendrahtzäune oder perforierte Elemente.
* **Name**
* **Horizontaler und Vertikaler Maßstab**
   * Wenn diese Option aktiviert ist, stellt die Schaltfläche Seitenverhältnis sperren sicher, dass der horizontale und vertikale Maßstab das Seitenverhältnis der Textur berücksichtigen.
   * Strecken Sie ein Material, indem Sie den horizontalen Maßstab unabhängig vom vertikalen Maßstab anpassen.
   * Sie können den horizontalen und vertikalen Maßstab pro Fläche mit dem Werkzeug Materialplatzierung anpassen überschreiben (siehe unten).
* **Transparenz**, **Reflexion** und **Glanz**

## Anpassen der Materialplatzierung

Beim Auftragen eines Materials auf eine Fläche wird in FormIt eine Einschätzung der optimalen Ausrichtung vorgenommen:

* Vertikale Flächen werden so ausgerichtet, dass die Oberseite der Textur entlang der Z-Achse ausgerichtet ist.
* Bei horizontalen Flächen wird die Textur längs entlang der längsten Seite der Fläche ausgerichtet.

Verwenden Sie das Werkzeug **Materialplatzierung anpassen**, um die vorgegebene Materialplatzierung sowie die Materialskalierung auf bestimmten Flächen zu überschreiben:

* Wählen Sie eine oder mehrere Flächen aus, die mit einem Material versehen sind.
   * Wenn die Fläche das Material aus der übergeordneten Gruppe übernimmt, müssen Sie die Fläche zuerst direkt mit dem Material versehen.
* Sie können das Werkzeug Materialplatzierung anpassen über den Tastaturkurzbefehl MP oder über das Kontextmenü aufrufen:

![](../.gitbook/assets/adjust-material-placement.PNG)

Verwenden Sie die Steuerelemente auf dem Bildschirm, um die Materialtexturen direkt auf der Fläche interaktiv zu verschieben, zu drehen und zu skalieren:

![](../.gitbook/assets/materialplacement.gif)

![](../.gitbook/assets/adjust-material-placement.gif)

Um Änderungen an der Materialplatzierung zurückzusetzen, tragen Sie in der Gruppe Materialien das ursprüngliche Material einfach erneut auf die Fläche auf.

## Materialübertragung nach Revit

Materialien werden nach Revit übertragen, wenn Sie das [FormIt-Zusatzmodul](https://formit.autodesk.com/page/formit-revit) für Revit 2018 oder höher verwenden.
