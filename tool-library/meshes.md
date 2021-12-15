# Netze

Ab Version 17.0 bietet FormIt einen neuen Geometrietyp: Netze.

Netze sind vereinfachte Darstellungen von FormIt-Standardobjekten und eignen sich hervorragend zur Verbesserung der Leistung von Geometrie mit vielen Polygonen wie Möbeln oder 3D-Umgebungsobjekten wie Menschen, Bäumen, Autos und Beschilderung. Netze eignen sich auch hervorragend für komplexe DWG-Geometrie, die sich andernfalls auf die Leistung von FormIt auswirken könnte.

Objekte können in Netze konvertiert werden, und Netze können ohne Datenverlust in Objekte zurückkonvertiert werden. Einige Dateitypen werden automatisch als Netze importiert, z. B. OBJ, STL und DWG. Weitere Informationen zum Konvertieren von Typen und anderen Vorteilen und Einschränkungen von Netzen finden Sie weiter unten.

### Konvertieren von Objekten in Netze

Jede Kombination von Scheitelpunkten, Kanten, Flächen oder Volumenkörpern kann in Netze konvertiert werden.

Wählen Sie einfach Objekte aus, und verwenden Sie entweder den Kurzbefehl OM \(Objekte in Netze\) (Objects to Meshes), oder klicken Sie mit der rechten Maustaste, und wählen Sie im Kontextmenü die Option Objects to Meshes (Objekte in Netze) aus:

![](../.gitbook/assets/context-menu_object-to-mesh.PNG)

Nachdem die Objekte in Netze konvertiert wurden, wird oben im Bildschirm eine Bestätigungsmeldung angezeigt:

![](../.gitbook/assets/success_object-to-mesh.PNG)

**Beim Konvertieren von Objekten in Netze geschieht Folgendes:**

* Kanten, die auf den Objekten geglättet wurden, bleiben in den resultierenden Netzen geglättet.
* Die Materialausrichtungen auf den Objekten bleiben in den resultierenden Netzen unverändert.
* Für jedes angewendete Material wird ein Netz erstellt. Wenn Sie beispielsweise einen einzelnen Würfel mit 6 verschiedenen Farben konvertieren, erhalten Sie 6 verschiedene Netze.
   * Durch die Rückkonvertierung in ein Objekt werden die einzelnen Netze wieder zu einem Volumenkörper vereinigt.
* Durch Auswahl eines Volumenkörpers wird der gesamte Körper konvertiert und durch ein Netz ersetzt. Durch Auswahl einzelner Kanten oder Scheitelpunkte, die zu einem Volumenkörper gehören, wird jedoch ein neues Netz über der vorhandenen Geometrie erstellt, ohne dass sich dies auf den ursprünglichen Körper auswirkt.
* Durch die Konvertierung eines Kanten- oder Scheitelpunktsatzes wird ein einzelnes LineMesh \(ein Netz aus Kanten\) oder ein einzelnes Punktnetz \(ein Netz aus Punkten\) erstellt. Dies bedeutet, dass Sie einzelne Kanten oder Scheitelpunkte nicht auswählen können, sobald sie zu einem einzelnen Netz kombiniert wurden. Konvertieren Sie sie wieder in Objekte, wenn Sie die Position eines einzelnen Elements anpassen möchten.

**Konvertieren von gruppierter Geometrie in Netze:**

* Netze werden noch leistungsfähiger, wenn Sie eine komplette Gruppe und alle darin verschachtelten Gruppen in Netze konvertieren können.
* Gruppen und deren verschachtelte Inhalte können mithilfe eines Plugins in Gruppen konvertiert werden:
   * Suchen Sie nach dem Plugin Manager-Symbol auf der rechten Seite der Anwendung:
      * ![](../.gitbook/assets/plugin-manager_icon.PNG)
   * Suchen Sie das Plugin Mesh + Unmesh All, und klicken Sie auf das Kontrollkästchen, um es zu installieren:
      * ![](../.gitbook/assets/plugin-manager_mesh-unmesh-all.PNG)
   * Das Plugin Mesh + Unmesh All wird geladen. Wählen Sie einfach eine Gruppe mit Objekten aus, die Sie in Netze konvertieren möchten, und klicken Sie auf Mesh All (Alle vernetzen).
      * ![](../.gitbook/assets/mesh-unmesh-all-plugin.PNG)
   * Beim Konvertieren verschachtelter Objekte oder Netze mit diesem Plugin wird oben im Bildschirm eine Aktualisierungsmeldung angezeigt, die Ihnen mitteilt, wie viele Gruppen und Exemplare von Gruppen von dem Vorgang betroffen sind:

![](../.gitbook/assets/success_mesh-all.PNG)

### Interaktion mit Netzen

**Aufgrund ihrer Einfachheit weisen Netze bestimmte Einschränkungen und Verhaltensweisen auf:**

* Sie können die einzelnen Flächen, Kanten oder Scheitelpunkte eines Netzes nicht bearbeiten.
   * Sie können jedoch Netze neu mit Material versehen und einzelne Netze verschieben, die als Ergebnis der Anwendung verschiedener Materialien auf Flächen erstellt wurden \(siehe oben\).
* Der Objektfang an Netzen ist auf die Flächen und Scheitelpunkte von Netzen beschränkt. Um die Leistung zu verbessern, funktionieren Objektfang und Ableitung bei Kanten von Netzen nicht.
   * Bei in Netze konvertierten DWG-Dateien \(ein anderer Netztyp, der als LineMesh bezeichnet wird\) können jedoch weiterhin Netzkanten gefangen und abgeleitet werden.
* Auf Netze können keine Ebenen angewendet werden.
* Bei Netzen werden keine Probleme mit der Dichtheit oder Rückseiten gemeldet. Konvertieren Sie sie wieder in Objekte, um zu sehen, ob sie wasserdicht sind oder nicht.
   * Objekte, die vor der Konvertierung in ein Netz wasserdicht waren, bleiben bei der Rückkonvertierung in ein Objekt weiterhin wasserdicht.
* Netze können nicht in erweiterten Modellierungsoperationen wie Volumenkörperverbindung/-schnitt, 3D-Hülle, 3D-Versatz, Abrundung, Erhebung, Sweep oder Abdeckung verwendet werden.

Andernfalls werden Netze angezeigt und verhalten sich wie alle anderen FormIt-Objekte: in Gruppen platziert, Layern zugewiesen, in Szenen visualisiert, für die Analyse verwendet usw.

**Dass Sie mit einem Netz interagieren, können Sie daran erkennen, dass in der QuickInfo On Mesh (Auf Netz angezeigt) oder in der Gruppe Properties (Eigenschaften) von Netzen gesprochen wird:**

![](../.gitbook/assets/snap_on-mesh.PNG)

![](../.gitbook/assets/properties-panel_mesh.PNG)

**Einige Dateitypen werden zur Verbesserung der Leistung automatisch als Netze importiert:**

* STL- und OBJ-Dateien, die dichte Geometrie wie Punktwolken aus anderen Anwendungen enthalten können, werden automatisch als Netze importiert.
* DWG-Dateien, die Millionen von kleinen Kantensegmenten auf hochwertigen Kurven enthalten können, werden automatisch als Netze importiert.

### Zurückkonvertieren von Netzen in Objekte

Wählen Sie einfach Meshes (Netze) aus, und verwenden Sie entweder den Kurzbefehl MO \(Netze in Objekte\) )Meshes to Objects), oder klicken Sie mit der rechten Maustaste, und wählen Sie im Kontextmenü die Option Meshed to Objects (Netze in Objekte) aus:

![](../.gitbook/assets/context-menu_mesh-to-object.PNG)

Nachdem die Objekte in Netze konvertiert wurden, wird oben im Bildschirm eine Bestätigungsmeldung angezeigt:

![](../.gitbook/assets/success_mesh-to-object.PNG)

**Beim Zurückkonvertieren von Netzen in Objekte:**

* Alle Objekte, die vor der Konvertierung in ein Netz ein wasserdichter Volumenkörper waren, werden beim Konvertieren in ein Objekt wieder zu einem wasserdichten Volumenkörper verbunden.
* Beim Konvertieren einer Reihe von Kanten \(z. B. aus einer DWG-Datei\) oder einer Reihe von Scheitelpunkten \(z. B. aus einer Punktwolke\) in ein Netz und umgekehrt werden die nicht vernetzten Objekte automatisch in einer Gruppe platziert.
   * Dadurch wird verhindert, dass die neuen Kanten oder Scheitelpunkte mit anderer Geometrie zusammengeführt werden, was sich nachteilig auf die Leistung auswirken könnte.
   * Sie können die Gruppierung der resultierenden Gruppe einfach aufheben, um die Kanten und/oder Scheitelpunkte freizugeben.

**Zurückkonvertieren von gruppierten Netzen in Objekte:**

* Befolgen Sie die oben stehenden Anweisungen, um das Plugin Mesh + Unmesh All zu verwenden und so Gruppen und deren verschachtelte Netze wieder in Objekte zu konvertieren.

