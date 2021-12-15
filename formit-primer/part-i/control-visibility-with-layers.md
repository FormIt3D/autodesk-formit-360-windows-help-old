# 1.6 – Steuern der Sichtbarkeit mit Layern

_Layer in FormIt ermöglichen ähnlich wie in AutoCAD und Photoshop die Verwaltung der Sichtbarkeit von Objekten im Modell. In diesem Kapitel erstellen Sie einen Layer, der das Speichern und Ausblenden des Gebäudekörpers für die spätere Analyse ermöglicht._

_Wenn Sie den letzten Abschnitt nicht bearbeitet haben, laden Sie die Datei_ _**1.6 – Control Visibility with Layers.axm**_ _aus dem Ordner_ _**FormIt Primer Part 1 Datasets** herunter und öffnen sie._

## **Layer erstellen**

1 – So erstellen Sie die neuen Layer

1. Wechseln Sie zur **Layer-Palette**, und klicken Sie dreimal auf das **+**-Zeichen, um drei Layer zu erstellen.
2. Doppelklicken Sie auf die Layernamen, um sie in **Massing**, **Main Building Floor** und **Plan Image**

![](../../.gitbook/assets/0%20%2820%29.png)

_**Anmerkung:**_ _Sie können auf einen Layernamen klicken und ihn nach oben oder unten ziehen, um die Reihenfolge der Layer zu ändern._

2 – So weisen Sie die Gruppe **Massing – Main Building** dem Layer **Massing** zu

1. Wählen Sie im Ansichtsbereich die Gruppe **Massing – Main Building** aus.
2. Wählen Sie in der **Layer-Palette** den Layer **Massing** aus dem Dropdown-Menü **Auswahl für:** aus. Weisen Sie entsprechend die Gruppe **Plan Image** dem Layer **Plan Image** zu.

![](../../.gitbook/assets/1%20%2813%29.png)

## **Gruppe duplizieren**

_Jetzt beginnen Sie mit der detaillierten Modellierung des Gebäudes. Der erste Schritt besteht darin, die Geschossgeometrie basierend auf dem bereits vorhandenen Gebäudekörper zu erstellen._

1 – Wählen Sie erneut die Gruppe **Massing – Main Building** aus. Drücken Sie zum Kopieren die Tastenkombination **STRG+C \(Kopieren\)** und anschließend **STRG+UMSCHALT+V \(An Position einfügen\)**, um den Körper an derselben Stelle einzufügen.

2 – So trennen Sie die neue Gruppengeometrie von der ursprünglichen Gruppe: Klicken Sie mit der rechten Maustaste, um das **Kontextmenü** aufzurufen, und wählen Sie die Option **Als eindeutig definieren \(MU\)**.

![](../../.gitbook/assets/2%20%2818%29.png)

_**Anmerkung**: Die neue Gruppe ist nicht mehr mit dem Original verknüpft. Änderungen an der neuen Gruppe wirken sich nicht auf die ursprüngliche Gruppe aus._

## **Erstellen der Geschossgeometrie**

1 – Neuzuweisen des Layers der Gruppe

1. Klicken Sie einmal, um eine der Gruppen **Massing – Main Building** auszuwählen.
2. Platzieren Sie die Gruppe mithilfe der Dropdown-Liste **Auswahl für:** in der **Layer-Palette** auf dem Layer **Main Building Floor**.
3. Deaktivieren Sie den Layer **Massing**, um die Geometrie auszublenden und den Layer vor versehentlichen Änderungen zu schützen.

![](../../.gitbook/assets/3%20%2818%29.png)

2 – Doppelklicken Sie auf die sichtbare Gruppe **Massing – Main Building**, um sie zu bearbeiten. Benennen Sie die Gruppe **Floor** in der **Eigenschaftenpalette** um.

![](../../.gitbook/assets/4%20%2812%29.png)

3 – **Klicken Sie einmal** auf die **obere Fläche** der Geometrie, um sie auszuwählen. Klicken Sie erneut, und ziehen Sie die Fläche nach unten. Wenn Sie die Fläche nach unten ziehen, geben Sie **11'-2"** ein, und das **Dialogfeld Bemaßung** wird angezeigt. Klicken Sie nach Eingabe des Werts auf **OK**. Die resultierende Geschossdecke muss 1' dick sein. Doppelklicken Sie auf eine Stelle im Raum, um die Gruppe zu verlassen.

![](../../.gitbook/assets/5%20%2810%29.png)

