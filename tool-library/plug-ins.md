# Plug-In-Module

Verwenden Sie den Plugin Manager, um nützliche Plugins vom FormIt-Team zu installieren, oder erfahren Sie, wie Sie [**Ihre eigenen FormIt-Plugins erstellen**](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)**.**

#### FormIt Plugin Manager

Der FormIt Plugin Manager dient als Hub zum Erkennen und Verwalten von FormIt-Plugins.

Der Plugin Manager wird beim Starten von FormIt automatisch geladen, sofern FormIt über Internetzugriff verfügt.

Sie können auf den Plugin Manager zugreifen, indem Sie auf das Registerkartensymbol rechts im Anwendungsfenster klicken:

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerTab.PNG)

#### Der Plugin Manager kategorisiert verschiedene Plugin-Typen:

* **Installierte Plugins**
* **Empfohlene Plugins**
   * Plugins, die das FormIt-Team empfiehlt, um die Kernfunktionalität von FormIt zu erweitern und neue Arbeitsabläufe zu nutzen.
   * Von der Community entwickelte Plugins werden hier angezeigt, nachdem sie vom FormIt-Team genehmigt wurden. Weitere Informationen hierzu werden in Zukunft bereitgestellt.
* **Öffentliche Plugins**
   * Plugins, die von der Community erstellt, aber nicht vom FormIt-Team überprüft oder genehmigt wurden.

#### Der Plugin Manager ist mit einer Reihe erweiterbarer und ausblendbarer Benutzeroberflächen ausgestattet, die die Verwaltung von Plugins und deren Repositorys erleichtern:

* **Verwalten von Plugins:**
   * Klicken Sie auf den Namen eines Plugins, um die zugehörige Beschreibung anzuzeigen.
   * Betätigen Sie den Schalter, um es zu installieren oder zu deinstallieren.
      * Das Plugin wird abhängig vom Plugin-Typ als Werkzeugkasten oben in der Anwendung, als Gruppe auf der rechten Seite oder als Dialogfeld in der Mitte angezeigt.
* Wenn Sie [Ihr eigenes Plugin entwickeln](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html), können Sie die private URL in das Feld unten einfügen und auf \(+\) klicken:

![FormIt Plugin Manager](https://formit3d.github.io/FormItExamplePlugins/docs/images/addNew.png)

#### Funktionsweise von Plugins

* Plugins sind webbasiert und in FormIt for Windows und FormIt for Web verfügbar.
* Plugins bestehen aus einer Reihe von Dateien und Ordnern, die auf GitHub bzw. auf einem lokalen Server gehostet werden, wenn Sie Ihr eigenes Plugin erstellen.
* Externe Plugins \(nicht lokal gehostete Plugins\) erfordern eine Internetverbindung, um erstmalig geladen zu werden, was bedeutet:
   * Externe Plugins werden nicht geladen, wenn beim Starten von FormIt keine Internetverbindung erkannt wird.
   * Nach dem Laden können einige externe Plugins für diese Sitzung im Offline-Modus arbeiten, andere können jedoch unterbrochen werden, bis die Verbindung wiederhergestellt ist.
   * Externe Plugins laden bei jeder Ausführung den neuesten Code auf dem Server, sodass ihre Funktionalität aktualisiert wird, sobald der Autor eine Änderung vornimmt.
* Plugins werden asynchron geladen, was bedeutet, dass sich die Reihenfolge der Plugins in der FormIt-Benutzeroberfläche mit jeder neuen Sitzung ändern kann.
* Der Plugin Manager verwendet Registrierungsschlüssel unter Windows, um die installierten Repositorys und Plugins zu speichern.
   * Wenn Sie den Plugin Manager auf die Vorgaben zurücksetzen müssen, löschen Sie den folgenden Registrierungsschlüssel:
      * Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins
      * Beachten Sie, dass dadurch alle vom Benutzer hinzugefügten Repositorys und Plugins deinstalliert werden, und der Plugin Manager wird zurückgesetzt, sodass nur die integrierten Repositorys und Plugins enthalten sind.

