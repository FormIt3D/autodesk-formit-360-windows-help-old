# 1.4 – Hinzufügen von Geschossen mit Ebenen

_Mithilfe von Ebenen können Sie Körper mit einzelnen Geschossbezügen segmentieren und die Bruttofläche nach Gebäudekörper berechnen. FormIt-Ebenen und deren benutzerdefinierte Namen werden in Revit-Ebenen umgewandelt, wenn die Datei in Revit konvertiert wird._

_Wenn Sie den letzten Abschnitt nicht bearbeitet haben, laden Sie die Datei **1.4 – Add Floors with Levels.axm** aus **FormIt Primer Part 1 Datasets** herunter und öffnen sie._

## **Erstellen und Anpassen von Ebenen**

1 – So erstellen Sie Ebenen

1. Wechseln Sie zur **Palette Ebene** in der **Palettenleiste**.
2. Klicken Sie viermal auf **+** \(**Ebene hinzufügen**\), um vier Ebenen zu erstellen.
3. Doppelklicken Sie auf die aktuelle Höhe der einzelnen Ebenen, um sie in **0'-0", 2'-2", 4'-6"** und **17'-8"** zu ändern.
4. Doppelklicken Sie auf den aktuellen Namen der einzelnen Ebenen, und benennen Sie sie um: **Ground, Terrace, Main Building** und **Top of Roof**

![](../../.gitbook/assets/0%20%2816%29.png)

_**Anmerkung**: Sie können auf das Symbol_ _**++**_ _klicken, um mehrere Ebenen mit einem bestimmten und einheitlichen Abstand zu erstellen. Dies ist für mehrstöckige Gebäude praktisch_.

## **Anwenden von Ebenen auf Geometrie**

_In den vorherigen Schritten haben wir nur Ebenen erstellt. Jetzt können wir diese Ebenen auf die erstellte Geometrie anwenden._

1 – So wenden Sie Ebenen auf die vorhandene Geometrie an

1. Wählen Sie den gesamten oberen Terrassenkörper durch Doppelklicken aus.
2. Klicken Sie in der **Eigenschaftenpalette** auf **Ebenen verwenden**. In diesem Schritt werden alle Ebenen, die die ausgewählte Geometrie aktuell schneiden, vorausgewählt.
3. Auf die derzeit ausgewählte Geometrie sind drei Ebenen angewendet \(**Main Building, Terrace,** und **Ground**\). In dieser Übung soll jedoch nur **Ground** angewendet werden. Deaktivieren Sie **Main Building** und **Terrace**.
4. Dadurch wird sichergestellt, dass nur die Fläche, die von **Ground** geschnitten wird, für die Berechnung der Bruttofläche berücksichtigt wird, die im Feld **Fläche nach Ebene** angezeigt wird.

![](../../.gitbook/assets/1%20%284%29.png)

_**Anmerkung**: Wenn am Körper keine blauen Ebenenlinien angezeigt werden, geben Sie_ _**DL**_ _für_ _**Ebenen anzeigen** ein._

![](../../.gitbook/assets/2%20%283%29.png)

