# Versatz-Linie

Zeichnen Sie parallele oder versetzte Linien mit dem Werkzeug Versatzlinie. Dies ist nützlich, um 2D-Formen zu erstellen, die später extrudiert werden können, sodass sie 3D-Wänden ähneln.

![](../.gitbook/assets/image%20%283%29.png)

Das Werkzeug **Versatzlinie** funktioniert wie das Werkzeug [**Linie** ](https://windows.help.formit.autodesk.com/tool-library/line-tool):

* Klicken Sie, um den ersten Punkt festzulegen, und bewegen Sie dann den Cursor, um die nachfolgenden Punkte zu platzieren. Dabei werden vorhandene Geometrie oder Ableitungsachsen gefangen.
* Eine Vorschau der resultierenden Form wird angezeigt. Der zweite und dritte Punkt bestimmen die Ebene, der die restlichen Punkte folgen sollen, sodass das Ergebnis planar ist.
* Fügen Sie weitere Punkte hinzu, und drücken Sie **ESC**, oder doppelklicken Sie, um das Werkzeug zu beenden.
* Alle Selbstüberschneidungen werden bereinigt und zusammengeführt, sodass Sie eine extrudierbare Fläche erhalten.

![Nach dem Platzieren von zwei Punkten und Ziehen des dritten Punkts](../.gitbook/assets/walls1.png)

Die Eingabezeile wird rot angezeigt und vorgabemäßig in der Mitte der Versatzlinien platziert.

Sie können die Ausrichtung der Versatzlinien und deren Stärke ändern, indem Sie die **TABULATORTASTE** drücken. Dadurch wird das Dialogfeld **Werkzeugoptionen** aufgerufen:

![Optionen für das Werkzeug Versatzlinie](../.gitbook/assets/walls2.png)

Ändern Sie die **Ausrichtung** beispielsweise in **Links** und die **Stärke** in 6", und die Versatzlinien werden links neben den Eingabelinien gezeichnet, 6 Zoll voneinander entfernt.

![](../.gitbook/assets/walls3.png)

## Nützliche Tipps

Sie können eine geschlossene Form zeichnen, indem Sie den ersten platzierten Punkt fangen. Die resultierende Ecke wird automatisch bereinigt:

![](../.gitbook/assets/walls4.png)

Sie können die Eingabelinien beliebig übereinander zeichnen. Wenn das Werkzeug fertig ist, werden die resultierenden Schnittpunkte bereinigt.

![](../.gitbook/assets/walls5.png)

![](../.gitbook/assets/walls6.png)

Grundsätzlich muss mit dem Werkzeug Versatzlinie Geometrie auf einer Ebene generiert werden, sodass die ersten Punkte die Ebene bestimmen, der die übrigen Punkte folgen.

Beginnen Sie beispielsweise mit dem Zeichnen auf der Seite eines Würfels, um die Ebene dieser Fläche zu verwenden. Nachdem drei nicht kollineare Punkte platziert wurden, wird die Eingabeebene für den Rest der Eingabe fixiert. Beachten Sie, dass beim Zeichnen auf einer Fläche die resultierende Form in die Fläche eingefügt und in mehrere Flächen aufgeteilt wird. Um das Einfügen zu verhindern, muss die Fläche, auf der Sie zeichnen, Teil einer [Gruppe](https://windows.help.formit.autodesk.com/tool-library/groups) sein.

![Zeichnen auf einer vertikalen Fläche](../.gitbook/assets/walls7.png)

![Nach Beenden des Werkzeugs werden die Linien eingefügt, und die getrennten Flächen können weiter bearbeitet werden.](../.gitbook/assets/walls8.png)

Sie können auch das Werkzeug Versatzlinie verwenden, um eine Draufsicht nachzuzeichnen. Importieren Sie den Plan als Bild.

* Ändern Sie die Größe des Bilds, sodass der Plan den richtigen Maßstab aufweist. Dies wird [hier](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/work-with-images-and-the-ground-plane) genauer beschrieben.
* Sie können die [orthogonale Kamera](orthographic-camera.md) zum Nachzeichnen in orthogonalen [Draufsichten](orthographic-views.md) verwenden.

![](../.gitbook/assets/walls9.png)

![](../.gitbook/assets/walls10.png)



