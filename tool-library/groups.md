# Gruppen

Eine der grundlegendsten und dennoch wichtigsten Techniken bei FormIt-Arbeitsabläufen ist die Gruppierung. Mit Gruppen können Sie verhindern, dass Geometrie zusammenklebt, und Sie können Beziehungen zwischen über- und untergeordneten Elementen für kopierte Elemente erstellen, sodass beim Aktualisieren eines Elements beide Elemente aktualisiert werden. [Hier](../formit-primer/part-i/grouping-objects.md) erfahren Sie mehr über Gruppen.

Gruppen können auf zwei Arten erstellt und bearbeitet werden: Entweder über das Kontextmenü einer ausgewählten Gruppe oder über den Hauptwerkzeugkasten.

## Gruppeninteraktionen

Um eine **Gruppe zu erstellen**, wählen Sie die Elemente aus, die Sie gruppieren möchten – dies kann Kanten, Flächen, Volumenkörper oder andere Gruppen umfassen – und klicken Sie mit der rechten Maustaste. Wählen Sie das Werkzeug **Gruppe \(G\)** aus dem Kontextmenü. Importierte Bilder und Satellitenbilder können nicht gruppiert werden.

Um eine **Gruppe auszuwählen**, klicken Sie auf diese. Beachten Sie die gestrichelten Linien, die angezeigt werden, wenn Sie eine Gruppe auswählen. Diese Linien geben die Gesamtgröße der Gruppe an.

Um eine **Gruppe zu bearbeiten**, doppelklicken Sie auf diese. Dadurch wird ein Bearbeitungsmodus gestartet, in dem Sie nur Elemente außerhalb der aktuellen Gruppe anzeigen und fangen, jedoch keine Elemente auswählen können. Sie können auch die Elemente außerhalb der aktuellen Gruppe mithilfe des Tastaturkurzbefehls **H** ausblenden.

Sie können **Gruppen innerhalb von Gruppen** erstellen. Diese werden als **verschachtelte Gruppen** bezeichnet und können im Gruppenbearbeitungsmodus erstellt werden. Um in verschachtelten Gruppen eine Ebene nach oben zu gelangen, klicken Sie auf eine beliebige Stelle außerhalb der Gruppen.

Um den **Gruppenbearbeitungsmodus zu beenden**, doppelklicken Sie auf eine beliebige Stelle außerhalb der Gruppe.

Sie können eine **Gruppe kopieren**, um eine Beziehung zwischen der ursprünglichen Gruppe und ihrer Kopie zu erstellen: Wenn Sie kopierte Gruppen bearbeiten, wirken sich diese Änderungen auf alle zugehörigen Gruppen aus.

Um **die Beziehung zwischen kopierten Gruppen aufzuheben**, wählen Sie die Gruppe(n) aus, die Sie trennen möchten, klicken mit der rechten Maustaste und wählen **Als eindeutig definieren** aus dem Kontextmenü. Sie können auch im Werkzeugkasten Gruppen die Option Als eindeutig definieren auswählen.

Um **alle zugehörigen Gruppen auszuwählen**, bewegen Sie den Mauszeiger über eine Gruppe und drücken die TABULATORTASTE. Wenn alle zugehörigen Gruppen markiert sind, klicken Sie auf die Gruppen, um sie auszuwählen. Sie können dann eine Aktion für alle Gruppen gleichzeitig durchführen.

Die [**Gruppenstruktur**](groups-tree.md) bietet eine zentrale Stelle zum Anzeigen und Verwalten aller Gruppen in einem Projekt.

## Zugriff auf Kontextmenü und Werkzeugkasten für Gruppen

## ![](../.gitbook/assets/grouptoolbar.png)

**Gruppieren von Elementen**

Um eine Gruppe aus dem Werkzeugkastenelement Gruppen zu erstellen, wählen Sie eines oder mehrere Elemente aus, klicken auf das Symbol **Gruppe erstellen** und dann auf das Symbol **Fertig stellen**. Alternativ können Sie **Gruppe erstellen** aus dem Werkzeugkastenelement Gruppen auswählen, die Elemente auswählen, die Sie gruppieren möchten, und dann auf das Symbol **Fertig stellen** klicken.

Um **eine Gruppe über das Werkzeugkastenelement Gruppen zu bearbeiten**, wählen Sie das Symbol **Gruppe bearbeiten** aus und klicken dann auf die Gruppe, die Sie bearbeiten möchten. Wenn Sie alle Änderungen vorgenommen haben, klicken Sie auf das Symbol **Fertig stellen**. Mit diesem Werkzeug können Sie die spezifische Gruppe auswählen, die Sie bearbeiten möchten, auch wenn sie tief verschachtelt ist.

**Um eine Gruppe über den Werkzeugkasten eindeutig zu definieren**, wählen Sie das Symbol **Als eindeutig definieren** im Werkzeugkastenelement Gruppen aus. Darüber hinaus können Sie im Werkzeugkastenelement Gruppen die Option **Als eindeutig definieren** auswählen, dann die Gruppe auswählen, die Sie eindeutig definieren möchten, und auf das Symbol **Fertig stellen** klicken.

**Um die Gruppierung einer Gruppe im Werkzeugkastenelement Gruppen aufzuheben**, wählen Sie die Gruppe aus, die Sie ändern möchten, und klicken Sie im Werkzeugkastenmenü Gruppen auf das Symbol **Gruppierung aufheben**. Dadurch wird die Gruppierung der aktuellen Auswahl aufgehoben, die Gruppierung verschachtelter Gruppen wird jedoch beibehalten. Alternativ können Sie **Gruppierung aufheben** aus dem Werkzeugkasten auswählen, die zu ändernde Gruppe auswählen und dann das Symbol **Fertig stellen** auswählen.

**Um die Gruppierung aller Gruppen, die unterhalb der aktuell ausgewählten Gruppe verschachtelt sind, aufzuheben**, wählen Sie eine Gruppe mit verschachtelten Gruppen und dann **Gruppierung aller Verschachtelten aufheben** aus dem Werkzeugkasten Gruppen aus.

**Um die Gruppierung aller Gruppen in Ihrem Modell aufzuheben**, wählen Sie das Werkzeug **Gruppierung für alle aufheben** im Werkzeugkasten Gruppen aus.

## Gruppen und Revit

Wenn Sie mit Revit-**Familien** vertraut sind, kennen Sie das Konzept von Gruppen in FormIt. FormIt-Gruppen verfügen über Funktionen, mit denen Sie sie intelligent in Revit übertragen können.

**FormIt-Gruppenkategorien**

Sie können die **Kategorien** für Gruppen in FormIt so festlegen, dass Ihre FormIt-Gruppen beim Importieren in Revit zu Familien derselben Kategorien werden. Sie können Ihren FormIt-Gruppen Kategorien zuweisen, indem Sie eine Gruppe auswählen, den **Gruppenbearbeitungsmodus** aufrufen und im Fenster **Eigenschaften** Kategorien auswählen. Sie können Kategorien auch in der Gruppe **Gruppenstruktur** zuweisen.

**FormIt-Gruppennamen**

Sie können auch die Gruppe **Eigenschaften** verwenden, um einen Namen für Ihre FormIt-Gruppe anzugeben. Dies kann beim Navigieren in Ihrem eigenen Modell hilfreich sein. Wenn Sie Ihr Modell in Revit importieren, können Sie Elemente mithilfe des Namens der Gruppe leicht filtern.

Beachten Sie, dass **verschachtelte Gruppen in FormIt nicht als verschachtelte Gruppen in Revit importiert werden**. Dadurch werden stark verschachtelte Revit-Familien verhindert.

