# Sonnenstudie und Energieanalyse

Da das Modell nun erstellt wurde, können Sie es zur Untersuchung der **Sonnen- und Energieauswirkungen** im Entwurf verwenden. Diese Funktionen sind in FormIt integriert, damit die ersten Studien von der Perspektive der Gebäudeleistung aus nachvollzogen werden können. Diese Funktionen sind nur in **FormIt Pro** verfügbar. Wenn Sie die Web-App verwenden, haben Sie möglicherweise keinen Zugriff darauf.

Wenn Sie den letzten Abschnitt nicht bearbeitet haben, wählen Sie Datei &gt; Öffnen und anschließend **farnsworth08.axm** aus dem Ordner FormIt Primer.

## Schatten

Bevor Sie eines dieser Analysewerkzeuge verwenden können, müssen Sie den [Standort festlegen](). Damit erhält FormIt Zugriff auf präzise Sonnen-, Schatten- und Klimadaten.

1. Klicken Sie auf das Sonnensymbol in der [**Aktionsleiste**](../../formit-introduction/tool-bars.md), und aktivieren Sie **Schatten \(DS\)**.

   ![](../../.gitbook/assets/3bdf0e2a-0ad4-4aac-b6fc-5e789643b0d6.png)

2. Passen Sie die Schieberegler **Tag** und **Zeit** an, um zu sehen, wie sich die Schatten ändern.

   ![](../../.gitbook/assets/upperterracesketch_32.png)

3. Beachten Sie, wie hier die überdachte Terrasse während der heißesten Tageszeit in den Sommermonaten beschattet wird. Dies ist kein Zufall, sondern bewusst in dieser Form entworfen.

**Anmerkung**: Schatten können zu einer Verringerung der Anwendungsleistung führen. Zwei Vorschläge zur Abmilderung dieses Problems: Deaktivieren Sie Schatten, wenn die Navigation langsam wird, oder deaktivieren Sie Layer wie **Möbel**, wenn sie nicht zur Untersuchung von Schatten benötigt werden.

## Sonnenstudie

Als visuelle Menschen können Designer eine unglaubliche Menge an Informationen aus Heatmap-Diagrammen wie dem, das Sie erstellen werden, herauslesen und vermitteln.

1. Klicken Sie unten im [**Menü Sonne**](../../formit-introduction/tool-bars.md) auf die Schaltfläche **Solaranalyse**.
2. Sie befinden sich in einem speziellen Modus, in dem **Schatten**, **Tastaturbefehle** und andere **Werkzeugkästen** deaktiviert sind.
3. Das Auswahlverhalten wird im Modus **Solaranalyse** geändert. Sie können **gruppenübergreifende** Auswahlen treffen, Sie müssen nicht die **STRG**- oder **UMSCHALTTASTE** gedrückt halten, um Elemente zum Auswahlsatz hinzuzufügen, und Sie können die Auswahl von Elementen aufheben, indem Sie erneut darauf klicken. Sie können Geometrie per **einfachem Klick**, **Doppelklick** oder **Fensterauswahl** auswählen.
4. Wählen Sie die Flächen, die Sie untersuchen möchten. **Klicken Sie einmal** auf die Oberseite des **Dachs** und die Oberseite der **Geschosse**. Vermeiden Sie die Auswahl kleiner Elemente wie Möbel.

   ![](../../.gitbook/assets/upperterracesketch_33.png)

5. Suchen Sie in der oberen linken Ecke des Ansichtsbereichs den Werkzeugkasten **Solaranalyse**. Klicken Sie auf **Analysieren**. FormIt berechnet und rendert die Flächen. Die Einstellungen hier können vor **und** nach Abschluss der Analyse angepasst werden.

   ![](../../.gitbook/assets/solaranalysis.png)

6. Die Einstellung **Monatsspitze** zeigt die **Spitzenwerte** \(in BTU/sq ft\) für den angegebenen Monat. Dies ist für **Schattierungsstudien** vorgesehen. Sie können die Monatseinstellung ändern, und die Grafiken werden sofort aktualisiert. Indem Sie den **Cursor auf eine der analysierten Flächen setzen**, erhalten Sie deren **spezifischen** Wert.

   ![](../../.gitbook/assets/460060a0-ea3b-4095-af45-40045811be22.png)

7. Die Einstellung **Jahr kumulativ** zeigt den **Gesamtwert** der Energie für das ganze Jahr \(in kWh/qm\). Dies ist für **PV-Potenzialstudien** vorgesehen.

   ![](../../.gitbook/assets/a9f61dfb-dfc9-4751-b145-b131a69c53cf.png)

8. Diese Studien zur **Solaranalyse** können exportiert werden, indem Sie auf **Datei &gt; Exportieren \(STRG+E\)** klicken und **Bild** aus der Liste auf der linken Seite auswählen.

## Energieanalyse mit Insight

FormIt verfügt über dieselben integrierten Werkzeuge zur Gebäudeleistungsanalyse, die auch Revit verwendet. **Insight** bietet ein Dashboard mit Gebäudesystemparametern, die angepasst werden können, um mögliche Szenarien zu berücksichtigen, ohne dass Sie die Modellgeometrie **erneut analysieren** müssen. Insight funktioniert am besten mit FormIt**-Körpergeometrie**.

1. Vergewissern Sie sich, dass Sie bei Ihrem Konto bei Autodesk Account angemeldet sind. Deaktivieren Sie **alle** Layer **außer** dem Layer **Massing**. Auf Ihre Geometrie muss mindestens eine **Ebene** angewendet sein.
2. FormIt sendet nur **sichtbare** Geometrie an Insight. Beachten Sie, dass auch bei einem einfachen **Körper** eine Vielzahl von Daten in **Insight** generiert werden.

   ![](../../.gitbook/assets/energymassing.png)

3. Klicken Sie auf die Schaltfläche **Insight &gt; Insight generieren**. Die Analyse wird in der Cloud ausgeführt, sodass Sie während der Berechnung mit dem Modellieren fortfahren können.

   ![](../../.gitbook/assets/energymenu.png)

4. Wenn die Analyse abgeschlossen ist, klicken Sie auf die Schaltfläche **Insight anzeigen**, um das **Energiemodell** und die **Leistungsfaktoren** anzuzeigen. \(Optional können Sie die Website direkt unter [**http://insight.autodesk.com**](http://insight.autodesk.com/) aufrufen.\)

   ![](../../.gitbook/assets/energydashboard.png)

5. Im Insight-Dashboard können Sie einen Wert \(oder einen Wertebereich\) für jedes **Leistungsfaktor**-Widget festlegen, indem Sie auf den Faktor klicken und die blauen Punkte ziehen. Der Bereich ist hilfreich, wenn Sie das spezifische System, das Ihr Gebäude verwenden wird, noch nicht kennen.
6. Mit jeder Änderung an einem **Faktor** wird der gesamte **Energiekostenbereich** \(gemessen in USD/qm/Jahr\) aktualisiert. Sie können die Leistung Ihres Entwurfs anhand von Benchmarks wie **Ashrae 90.1** und der Herausforderung von **Architecture 2030** ermitteln.
7. Wenn sich Ihr Entwurf drastisch ändert, können Sie den aktualisierten Körper erneut an dasselbe Dashboard senden. Wenn Sie für den aktualisierten Entwurf ein **neues** Dashboard erstellen möchten, müssen Sie den Entwurf zunächst in FormIt mit **Speichern unter** speichern.
8. Wenn die Energieanalyse fehlschlägt, liegen möglicherweise geometriebasierte **Dichtheitsprobleme \(DW\)** vor. Diese können in FormIt geprüft und behoben werden.
9. Deaktivieren Sie den Layer **Massing**, und aktivieren Sie alle anderen Layer wieder.

