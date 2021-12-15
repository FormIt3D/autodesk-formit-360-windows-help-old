# Automatisch speichern

Ab Version 17.3 umfasst FormIt for Windows die Funktion Automatisch speichern, wodurch eine Sicherungskopie des FormIt-Modells erstellt wird, während Sie arbeiten. Diese Sicherungsdatei kann verwendet werden, um Daten wiederherzustellen, wenn FormIt mit nicht gespeicherten Änderungen geschlossen wird.

### Aktivieren und Deaktivieren von Automatisch speichern

Suchen Sie die Konfigurationsoptionen für Automatisch speichern unter Bearbeiten &gt; Voreinstellungen &gt; Automatisch speichern.

![](../.gitbook/assets/20190613-autosave.png)

Automatisch speichern ist vorgabemäßig aktiviert, kann jedoch durch Deaktivieren des Kontrollkästchens vollständig deaktiviert werden.

Legen Sie das Intervall \(in Minuten\) fest, in dem mit Automatisch speichern eine Sicherungskopie erstellt wird, indem Sie einen Wert in das Zahlenfeld Intervall für automatisches Speichern (Minuten) eingeben.

Beachten Sie, dass diese Voreinstellungen auf Anwendungsebene festgelegt sind und nicht geändert werden, wenn Sie verschiedene Dateien öffnen.

### Funktionsweise von Automatisch speichern

Wenn die Option Automatisch speichern aktiviert ist, wird abgefragt, ob die aktuelle FormIt-Datei nicht gespeicherte Änderungen enthält. Wenn Änderungen noch nicht gespeichert wurden, wird mit Automatisch speichern im angegebenen Intervall eine Sicherungskopie der Datei erstellt.

Sicherungsdateien werden neben der ursprünglichen Datei gespeichert und haben die Erweiterung `.axmb`.

Wenn Ihre ursprüngliche FormIt-Datei beispielsweise unter `C:/Users/<user>/FormIt/MyProject.axm` gespeichert ist, befindet sich die Sicherungsdatei unter `C:/Users/<user>/FormIt/MyProject.axmb`.

Wenn Sie eine neue FormIt-Sitzung starten, ohne eine vorhandene Datei zu öffnen, können Sie nicht gespeicherte Änderungen unter `C:/Users/<user>/Documents/Untitled.axmb` finden. Wenn Sie das neue Modell an einem anderen Speicherort gespeichert haben, werden bei der Sicherung nicht gespeicherte Änderungen neben dem neuen Speicherort, wie oben beschrieben, hinzugefügt.

Wenn Sie Änderungen an der ursprünglichen Datei speichern, wird die Sicherungsdatei von der Funktion Automatisch speichern automatisch gelöscht, da die Sicherungsdatei nun älter als die ursprüngliche Datei ist. Wenn Sie anschließend Änderungen an der gespeicherten Datei vornehmen, wird Automatisch speichern jedoch erneut aktiviert, und es wird erneut eine Sicherung wird im angegebenen Intervall erstellt.

Wenn Ihre Arbeitsdatei nicht gespeicherte Änderungen enthält und Sie FormIt schließen und die Änderungen verwerfen, wird die automatische Sicherungskopie gelöscht. Wenn FormIt jedoch geschlossen werden muss – entweder durch das Herunterfahren des Computers oder einen Anwendungsabsturz – bleibt die automatische Sicherungskopie erhalten und kann später zur Wiederherstellung von Daten verwendet werden.

### Arbeiten mit aktivierter Funktion Automatisch speichern

FormIt minimiert die potenziellen Auswirkungen von Automatisch speichern auf die Leistung, indem die Sicherung in einem separaten Prozess ausgeführt wird. Bei kleinen bis mittelgroßen Dateien sollten Sie den Vorgang der automatischen Sicherung nicht bemerken. Bei sehr großen Dateien \(~400 MB und mehr\) bemerken Sie möglicherweise nur eine kurze Unterbrechung, während FormIt das gesamte Modell kopiert und in einem separaten Prozess mit der Sicherung beginnt.

Wenn Sie sich fragen, ob die Funktion Automatisch speichern derzeit eine Sicherungskopie erstellt, können Sie in der Statusleiste unten links in der Anwendung nach einer kurzen Meldung zum automatischen Speichern suchen:

![](../.gitbook/assets/20190613-autosave-status-bar.png)

Wenn die Statusleiste deaktiviert ist, können Sie sie unter Fenster &gt; Statusleiste oder über den Kurzbefehl HS aktivieren.

### Wiederherstellen von Daten mit Automatisch speichern

Wenn Sie eine FormIt-Datei mit einer verfügbaren Sicherungskopie öffnen, werden Sie von FormIt darauf hingewiesen, dass die Sicherungsdatei vorhanden ist. Wie bereits erwähnt, kann dies einfach daran liegen, dass Sie FormIt geschlossen haben, ohne die Änderungen an diesem Projekt nach der letzten Bearbeitung zu speichern, oder daran, dass FormIt unerwartet geschlossen wurde.

![](../.gitbook/assets/20190613-autosave-notification.png)

Wenn Sie auf den Hyperlink Öffnen? klicken, wird die `.axmb`-Sicherungsdatei geladen.

Auf ähnliche Weise können Sie auch Datei &gt; Öffnen verwenden und die `.axmb`-Datei manuell im Datei-Explorer auswählen, um eine Sicherungskopie zu öffnen.

Wenn die Sicherungsdatei geöffnet ist, müssen Sie beim nächsten Speichern in FormIt eine andere FormIt-Datei \(`.axm`\) zum Überschreiben auswählen. Sie können keine FormIt-Sicherungsdateien \(`.axmb`\) überschreiben.



