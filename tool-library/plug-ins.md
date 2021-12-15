# Plug-in

Utilizzare Gestione plugin per installare plug-in utili dal team di FormIt o per apprendere come [**creare i plug-in di FormIt**](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)**.**

#### Gestione plugin di FormIt

Gestione plugin di FormIt funziona come un hub per la ricerca e la gestione dei plug-in di FormIt.

Gestione plugin viene caricato automaticamente all'avvio di FormIt, purché FormIt disponga dell'accesso ad Internet.

È possibile accedere a Gestione plugin facendo clic sull'icona della relativa scheda sul lato destro della finestra dell'applicazione:

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerTab.PNG)

#### Gestione plugin consente di classificare diversi tipi di plug-in:

* **Plug-in installati**
* **Plug-in consigliati**
   * Plug-in consigliati dal team di FormIt per espandere le funzionalità principali di FormIt e sbloccare nuovi workflow.
   * I plug-in sviluppati dalla community verranno visualizzati qui dopo l'approvazione da parte del team di FormIt. Ulteriori dettagli su questo argomento saranno forniti in futuro.
* **Plug-in pubblici**
   * Plug-in creati dalla community, ma che non sono stati rivisti o approvati dal team di FormIt.

#### Gestione plugin è stato progettato utilizzando una serie di interfacce espandibili e comprimibili, che semplificano la gestione dei plug-in e dei relativi repository:

* **Gestione dei plug-in:**
   * Fare clic sul nome di un plug-in per visualizzarne la descrizione.
   * Attivare/Disattivare l'interruttore per installarlo o disinstallarlo.
      * Il plug-in viene visualizzato come barra degli strumenti nella parte superiore dell'applicazione, pannello sul lato destro o finestra di dialogo al centro, a seconda del tipo.
* Se si sta [sviluppando un plug-in](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html), è possibile aggiungere il relativo URL privato nel campo in basso e premere \(+\):

![Gestione plugin di FormIt](https://formit3d.github.io/FormItExamplePlugins/docs/images/addNew.png)

#### Funzionamento dei plug-in

* I plug-in sono basati sul Web e sono disponibili in FormIt per Windows e FormIt per il Web.
* I plug-in sono costituiti da una serie di file e cartelle ospitati su GitHub o su un server locale durante la creazione di file personalizzati.
* I plug-in esterni \(i plugin non ospitati localmente\) richiedono una connessione ad Internet per il caricamento iniziale, il che significa che:
   * I plug-in esterni non vengono caricati se, all'avvio di FormIt, non viene rilevata alcuna connessione ad Internet.
   * Una volta caricati, alcuni plug-in esterni possono continuare a lavorare in modalità offline per tale sessione, ma altri potrebbero interrompersi fino al ripristino della connettività.
   * I plug-in esterni caricano il codice più recente sul server ad ogni esecuzione, in modo che le loro funzionalità vengano aggiornate ogni volta che l'autore esegue il push di una modifica.
* I plug-in vengono caricati in modo asincrono, ovvero l'ordine dei plug-in nell'interfaccia di FormIt può cambiare con ogni nuova sessione.
* Gestione plugin utilizza le chiavi del Registro di sistema in Windows per memorizzare i repository e i plug-in installati.
   * Se è necessario ripristinare le impostazioni di default di Gestione plugin, eliminare la seguente chiave del Registro di sistema:
      * Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins
      * Si noti che questa operazione disinstallerà tutti i repository e i plug-in aggiunti dall'utente, reimpostando Gestione plugin in modo da includere solo quelli incorporati.

