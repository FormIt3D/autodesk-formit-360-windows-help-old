# Häufig gestellte Fragen

## Info zu FormIt

**Was sind FormIt und FormIt Pro?**

FormIt ist eine 3D-Modellierungs-, Visualisierungs-, Analyse- und Berechnungsumgebung für Architekturentwürfe.

FormIt-Funktionen:

* Robuste Engine für die Volumenkörpermodellierung mit leistungsstarken Werkzeugen und Arbeitsabläufen, die für Gebäudeentwürfe optimiert sind
* Erweiterte Umweltvisualisierung zur Veranschaulichung von Entwurfsoptionen, einschließlich gespeicherter Modellzustände mithilfe von Szenen
* Standort, Satellitenbilder und 3D-Gelände mit Bing Maps
* Materialien aus der Autodesk-Materialbibliothek
* Modellorganisations- und Sichtbarkeitswerkzeuge wie Gruppen, Layer und Szenen
* Analysewerkzeuge, darunter:
   * Dichtheits- und Rückseitenprüfung für Volumenmodelldiagnose und -reparatur
   * Sonne und Schatten
   * Sonnenstudie
   * Energieanalyse
* Autodesk-Produktintegration:
   * BIM 360 Docs
   * Insight \(Energieanalyse\)
   * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
   * [Revit](https://formit.autodesk.com/page/formit-revit)
* Unterstützung von Dateiformaten:
   * Öffnen/Importieren
      * AXM, DWG, FBX, SAT, STL, OBJ, WSM, SketchUp, Image
   * Exportieren
      * AXM, FBX, OBJ, STL, SAT, DAE, DXF

FormIt ist kostenlos unter [iOS](https://itunes.apple.com/us/app/autodesk-formit-360/id575282599?mt=8) und [in Ihrem Browser](https://app.formit.autodesk.com/) verfügbar. Ein **FormIt Pro**-Abonnement ist erforderlich, um [FormIt for Windows](https://formit.autodesk.com/page/download), die leistungsstärkste und funktionsreichste Version von FormIt, zu verwenden. Das **FormIt Pro**-Abonnement bietet außerdem zusätzliche Funktionen für iOS und das Web, wie z. B. Solar- und Energieanalysen. **FormIt Pro** ist in der [Autodesk AEC Collection](https://www.autodesk.de/collections/architecture-engineering-construction/overview) enthalten.

**Was ist mit FormIt for Android passiert?**

Um das Produktangebot von FormIt zu optimieren, haben wir die schwere Entscheidung getroffen, die Android-App einzustellen. Wenn Sie diese installiert haben, kann sie weiterhin ausgeführt werden, ist jedoch nicht mehr im Play Store verfügbar.

**Wie erhalte ich FormIt?**

Um die Windows-Version auszuführen, müssen Sie Zugriff auf **FormIt Pro** haben, das Teil unseres Abonnements der [AEC Industry Collection](https://www.autodesk.de/collections/architecture-engineering-construction/overview) ist. Wenn Sie in Ihrem Büro mit Revit arbeiten, haben Sie wahrscheinlich bereits Zugriff auf FormIt. Sie können [FormIt for Windows direkt von unserer Website](https://formit.autodesk.com/page/download) oder über die Autodesk Desktop-App herunterladen.

Darüber hinaus kann die Web-Version direkt und kostenlos über unsere Website [http://formit.autodesk.com](http://formit.autodesk.com) ausgeführt werden.

Die iOS-Version kann kostenlos aus dem Apple App Store \(nur iPad\) heruntergeladen werden.

**Erhalte ich als Schüler, Student oder Lehrkraft kostenlosen Zugriff auf FormIt Pro?**

Ja. Sie können über das [Autodesk Education Portal](https://www.autodesk.de/education/edu-software/overview?sorting=featured&page=1) auf das FormIt Pro-Abonnement zugreifen.

**Wie lerne ich den Umgang mit FormIt?**

Am besten beginnen Sie mit dem [FormIt-Einführungslernprogramm](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html).

Es gibt mehrere Abschnitte in der Einführung für Einsteiger \(Erstellen eines kompletten modernen Hauses\) oder Fortgeschrittene \(Erweiterte Verwendung von Revit und Dynamo\).

In unserer FormIt-Webinarserie am Freitag finden Sie außerdem mehr als 20 Videos. Diese finden Sie auf unserem [YouTube-Kanal](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH).

## Arbeiten mit Revit

**Wie funktioniert FormIt mit Revit?**

FormIt ist eine separate 3D-Skizzier- und -Entwurfsanwendung. Die erstellten Daten können jedoch [mithilfe des FormIt-Zusatzmoduls für Revit](https://formit.autodesk.com/page/formit-revit) problemlos in Revit-Daten konvertiert werden.

**Was passiert beim Importieren in Revit?**

Ab Version 2016 ist Revit mit einem Zusatzmodul für die Arbeit mit FormIt-Daten ausgestattet. Wenn Sie eine FormIt-AXM-Datei in Revit importieren, durchsucht dieses Zusatzmodul alle Objekte in der Datei und erstellt sie mithilfe der API in Revit neu. Vorgabemäßig werden alle Elemente in FormIt als Körper kategorisiert.

Der FormIt-Konverter erstellt mithilfe der [API DirectShape](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/DEU/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html) aus jedem Körperobjekt eine Körperfamilie in Revit.

DirectShape ist ein nicht bearbeitbares Objekt, das in IFC-Arbeitsabläufen verwendet wird. Obwohl es nicht bearbeitet werden kann, bietet es den Vorteil, dass die vollständigen Materialtexturen zwischen FormIt und Revit übertragen werden. [In diesem Lernprogramm](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html) wird der Arbeitsablauf für die Übertragung von FormIt in Revit ausführlicher erläutert.

**Können in FormIt Wände, Geschossdecken und andere Revit-Systemfamilien erstellt werden?**

Nicht direkt. Wie oben angegeben, ist für jedes Objekt vorgabemäßig die Kategorie Körper ausgewählt. Um Wände, Geschossdecken usw. zu erstellen, sollten Sie das Modell mithilfe des Konverter-Zusatzmoduls in Revit importieren und mithilfe der nativen Revit-Werkzeuge Systemfamilien aus dem zugrunde liegenden Körpermodell erstellen.

**Kann Revit Daten zurück an FormIt senden?**

Ja. Um Daten wieder in FormIt zu importieren, exportieren Sie die gesamte Revit-Datei oder vorzugsweise einen _Teil_ davon in das SAT-Dateiformat. In der Regel ist es nicht erforderlich, ALLE Revit-Daten an FormIt zu senden. Erstellen Sie stattdessen in Revit eine gefilterte Ansicht, die nur die unbedingt notwendigen Daten \(z. B. Geschossdecken und Wände\) enthält, bevor Sie sie im SAT-Format speichern.

## Arbeiten mit anderen Apps

**Warum lautet das vorgegebene Dateiformat .AXM?**

Der interne Codename von FormIt vor Vergabe des offiziellen Namens lautete XModeler. Das von uns erstellte Dateiformat lautete also Autodesk X Modeler, kurz AXM.

**Welche 3D-Formate kann FormIt importieren?**

* Windows: AXM, DWG, FBX, OBJ, SAT, SKP, STL
* Web: OBJ, STL
* iOS: OBJ, STL, SAT

**Welche Formate kann FormIt exportieren?**

* Windows: FBX, OBJ, SAT, STL, DAE, DXF
* Web: OBJ, SAT, STL
* iOS: OBJ

**Wie funktioniert FormIt mit Dynamo?**

[Erfahren Sie, wie FormIt und Dynamo zusammen verwendet werden können](https://formit.autodesk.com/page/formit-dynamo), um Arbeitsabläufe für Computational Design zu erstellen.

**Wie lässt sich FormIt mit SketchUp vergleichen?**

* Bessere [**Interoperabilität mit Revit**](../tool-library/revit.md) ****
* [**Integration von Dynamo**](../tool-library/dynamo.md) für Computational Design
* Native Werkzeuge für [**Solaranalysen**](../tool-library/solar-analysis.md) und [**Energieanalysen**](../tool-library/energy-analysis.md) mit Autodesk Insight
* Robusterer Kernel für die Volumenkörpermodellierung, der erweiterte Modellierungsoperationen ermöglicht
* Native erweiterte Modellierungswerkzeuge wie [**Sweep, Abdeckung, Erhebung**](../tool-library/cover-sweep-loft.md), Volumenkörper versetzen/einhüllen, 3D-Übergang/-Rundung und [**Flächen abflachen**](../tool-library/flatten-face.md)
* Mehrere sichtbare [**Schnittebenen** ](../tool-library/section-planes.md)
* Diagnosewerkzeuge wie [**Anzeige: Dichtheitsprobleme und Anzeige: Rückseiten**](../tool-library/visual-styles.md)
* [**Exportieren von Teilen des Modells**](../tool-library/export-data.md) basierend auf der Auswahl und/oder Sichtbarkeit
* Nativer OBJ-, SAT- und STL-Export

**Kann ich die SketchUp-Tastaturbefehle verwenden?**

Ja. FormIt for Windows verfügt über eine vollständig bearbeitbare Tastaturzuordnung. Viele häufig verwendete SketchUp-Kurzbefehle sind vorgabemäßig bereits vorhanden, können aber im Menü Bearbeiten &gt; Voreinstellungen bearbeitet werden.

**Kann ich meine DWG-Dateien verwenden?**

Ja. In FormIt können 2D- und 3D-DWG-Dateien importiert werden.

## Allgemeine Support-Fragen

**Wie erhalte ich Support?**

Sie können Ihren Autodesk-Fachhändler fragen oder sich über das [FormIt-Forum](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=de) an uns wenden. Suchen Sie am besten zuerst nach der Frage, die Sie haben, und wenn sie noch nicht beantwortet wurde, posten Sie ein neues Thema. Das FormIt-Team antwortet Ihnen dann.

**Was muss ich tun, wenn ich mich nicht anmelden kann?**

* In diesem [Forums-Post](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572?profile.language=de) werden häufige Probleme bei der Anmeldung behandelt.
* Wenn Sie einen PC mit einem schaltbaren Grafikprozessor \(GPU\) haben, müssen Sie sicherstellen, dass FormIt immer die GPU mit höherer Leistung verwendet. Hier finden Sie Anweisungen für [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) und [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1).

**Was tun, wenn die Insight-Energieanalyse fehlschlägt?**

Wenn bei der Insight-Energieanalyse ein Fehler gemeldet wird oder keine Ergebnisse zurückgegeben werden, [finden Sie auf der Seite für die Insight-Energieanalyse](https://formit.autodesk.com/page/formit-insight) allgemeine Tipps zur Fehlerbehebung.

