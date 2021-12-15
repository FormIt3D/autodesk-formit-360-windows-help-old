# Bildstile

Passen Sie die visuelle Darstellung Ihres Modells an, einschließlich der allgemeinen Beleuchtung, Kantenstile und Umgebungseffekte. Die Gruppe Visuelle Stile können Sie aufrufen, indem Sie auf das Sonnenbrillensymbol in der Palettenleiste klicken:

![](../.gitbook/assets/20200307-visual-styles-icon.png)

Visuelle Stile [können pro Szene festgelegt werden](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/visual-settings), sodass Sie Ihre bevorzugten Stileinstellungen speichern und auf andere Szenen anwenden können.

## Flächen

Verwalten Sie, wie Flächen angezeigt und schattiert werden.

![](../.gitbook/assets/visual_styles%20%281%29.png)

Die Option **Umgebungshelligkeit** steuert die Gesamthelligkeit aller Materialien in der Szene. Ein Wert von 100 bedeutet, dass den Lichtstrahlen ausgesetzte Materialien mit ihrer vollen Helligkeit angezeigt werden, wie in der Farbe oder Textur des Materials definiert. Bei Werten über 100 würden die Materialien überbelichtet, könnten aber für SketchUp-Modelle nützlich sein, die in FormIt immer noch dunkel aussehen. Der Vorgabewert ist 100.

Die Option **Umgebungskontrast** steuert, wie viel dunkler Flächen im Schatten im Vergleich zu Flächen, die direktem Sonnenlicht ausgesetzt sind, angezeigt werden. Der Wert 0 bedeutet, dass die Beleuchtung keine Auswirkung hat \(alle Materialien werden unabhängig von der Ausrichtung mit voller Helligkeit angezeigt\), während bei höheren Werten Flächen im Schatten immer dunkler erscheinen. Der Standardwert ist 25.

Aktivieren Sie die Option **Schatten**, um zu sehen, wie Ihr Entwurf [zur aktuellen Tageszeit beschattet wird](https://windows.help.formit.autodesk.com/tool-library/shadows).

Die Option **Schattenintensität** steuert, wie dunkel Schatten auf der Grundplatte und anderen Flächen gezeichnet werden. Bei einem Wert von 0 werden Schatten effektiv unsichtbar, und bei einem Wert von 100 werden Schatten schwarz. Der Vorgabewert ist 20.

Mit **Umgebungsschatten** werden Ecken Schattierungen hinzugefügt, um das FormIt-Modell realistischer zu gestalten.

Die Option **Monotone Oberflächen** deaktiviert die Farbe und Textur aller Materialien und macht die Umgebung weiß. Dies ist für Schatten- oder Schattierungsstudien hilfreich.

Im Abschnitt Oberflächenfarben werden Vorgabefarben für Flächen definiert, wenn kein Material angewendet wird.

**Flächen** ist die Vorgabefarbe aller nach vorne weisenden FormIt-Flächen \(oder beider Seiten, wenn Rückseiten deaktiviert ist\), wenn kein Material angewendet wird.

**Rückseiten** wird verwendet, um verschiedene Materialien auf beiden Seiten einer einzelnen Fläche für SketchUp-Modelle anzuzeigen, die in FormIt importiert werden und dies erfordern. Diese Option ist vorgabemäßig deaktiviert, wird aber aktiviert, wenn SketchUp-Modelle geöffnet oder importiert werden. In Nicht-SketchUp-Geometrie wird die angegebene Farbe für die Rückseite an den Rückseiten von Flächen angezeigt.

Verwenden Sie die Optionen Schnitt – Schnitteffekte und Schnitt – Schnittmaterialeffekte, um die Vorgabefarben von Flächen, Linien und den Schnittmaterialeffekt zu verwalten, wenn das Werkzeug [Schnittebene](section-planes.md) verwendet wird.

## Grundplatten

Wenn die Grundplatte im Gruppenbearbeitungsmodus deaktiviert ist, ist das blaue Arbeitsebenenraster jetzt ebenfalls deaktiviert.

Die Farbe der Arbeitsebene kann auch über die Gruppe Visuelle Stile angepasst werden.

![](../.gitbook/assets/screen-shot-2020-03-30-at-1.30.16-pm.png)

## Kanten

Verwalten Sie den Anzeigestil aller Kanten im Modell.

![](../.gitbook/assets/edges.PNG)

Der **Kontrast** wirkt sich auf die Sichtbarkeit aller Kanten aus. Bei einem Wert von 0 werden die Kanten praktisch unsichtbar. Der Vorgabewert lautet 60.

**Farbe** wirkt sich auf die Farbe aller Kanten im Modell aus. Die Vorgabe ist Schwarz.

**Dicke Kanten** macht alle Kanten dicker, einschließlich Silhouettenkanten.

Mit **Skizzenartige Kanten** wird allen Kanten ein skizzenartiger Effekt hinzugefügt, um den Effekt einer Handzeichnung zu simulieren.

**Verdeckte Kanten** zeigt Kanten an, die ansonsten von Flächen verdeckt sind.

**Erweiterte Kanten** fügt einigen Kanten eine Verlängerung hinzu, um den Effekt einer Handzeichnung zu simulieren.

## Umgebung

Blenden Sie Umgebungseffekte und Hilfsobjekte ein und aus.

![](../.gitbook/assets/environment.PNG)

**Raster** steuert die Anzeige des Rasters auf der Grundplatte sowie das Raster, das beim Bearbeiten einer Gruppe angezeigt wird. Die Option Rasterfang wird deaktiviert, wenn das Raster deaktiviert ist.

Die Option **Achsen** steuert die Anzeige der XYZ-Achsen, die beim Weltursprung oder beim Gruppenursprung angezeigt werden, wenn eine Gruppe bearbeitet wird.

Die Option **Ebenen** steuert die Anzeige der [**Ebenen**](levels-and-area.md)****, die in der Gruppe Ebenen festgelegt wurden.

**Nebel** steuert die Anzeige von Nebel, der gezeichnet wird, damit der Übergang zwischen der Grundplatte und dem Himmel nahtlos aussieht. Wenn Sie Nebel deaktivieren, erhalten Sie eine scharfe Horizontlinie, an der die Grundplatte \(falls aktiviert\) an den Himmel grenzt.

**Nordpfeil** steuert die Anzeige eines kleinen grafischen Widgets, das die Richtung des Projektnordens angibt \(wie durch Standort und Satellitenbilder festgelegt\).

Umgebungsfarben wie Himmel, Hintergrund und Grundplatte können ebenfalls angepasst werden.

Der Himmel besteht aus einem Verlauf der Farben für **Unten/Hintergrund**, **Mitte** und **Oben**.

Wenn die Option **Himmel** deaktiviert ist, ist nur die Farbe **Unten/Hintergrund** sichtbar.

## Diagnose

Blenden Sie Diagnosewerkzeuge ein und aus.

![](../.gitbook/assets/diagnostics.PNG)

Die Option **Dichtheitsprobleme** hebt alle Kanten, die nicht Teil eines wasserdichten Volumenkörperobjekts sind, rot hervor.

Die Option **Rückseiten** hebt alle Flächen, die in die falsche Richtung zeigen, rot hervor \(die Rückseiten aller Volumenkörperobjekte sollten zur Innenseite der Volumenkörperform weisen\).

[Erfahren Sie mehr über die Verwendung der Dichtheits- und Rückseitendiagnose zum Identifizieren und Beheben von Problemen mit Volumenkörpermodellen](https://formit.autodesk.com/blog/post/repairing-solid-models).

