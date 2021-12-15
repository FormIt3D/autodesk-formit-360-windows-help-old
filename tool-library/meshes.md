# Mesh

A partire dalla versione v17.0, FormIt offre un nuovo tipo di geometria: mesh.

Le mesh sono rappresentazioni leggere degli oggetti di FormIt standard e sono ideali per migliorare le prestazioni della geometria con elevato numero di poligoni, come arredo o contesto 3D, ad esempio persone, alberi, automobili e segnaletica. Le mesh sono particolarmente utili anche per la geometria DWG complessa che altrimenti potrebbe influire sulle prestazioni di FormIt.

Gli oggetti possono essere convertiti in mesh e le mesh possono essere riconvertite in oggetti senza perdere eventuali dati. Alcuni tipi di file vengono importati automaticamente come mesh, ad esempio OBJ, STL e DWG. Sono fornite di seguito ulteriori informazioni sulla conversione tra i vari tipi, nonché su altri vantaggi e limitazioni delle mesh.

### Conversione di oggetti in mesh

Qualsiasi combinazione di vertici, bordi, superfici o corpi solidi può essere convertita in mesh.

È sufficiente selezionare Oggetti e utilizzare il collegamento OM \(Oggetti in mesh\) o fare clic con il pulsante destro del mouse e selezionare Oggetti in mesh nel menu contestuale:

![](../.gitbook/assets/context-menu_object-to-mesh.PNG)

Una volta convertiti gli oggetti in mesh, nella parte superiore della schermata viene visualizzato un messaggio di conferma:

![](../.gitbook/assets/success_object-to-mesh.PNG)

**Durante la conversione di oggetti in mesh:**

* I bordi che sono stati levigati negli oggetti rimarranno tali nelle mesh risultanti.
* Gli orientamenti dei materiali negli oggetti rimarranno invariati nelle mesh risultanti.
* Viene creata una mesh per ogni materiale applicato. Ad esempio, se si converte un singolo cubo dipinto con 6 colori diversi, si otterranno 6 mesh diverse.
   * Con la riconversione in un oggetto si riaggiungeranno le singole mesh in un corpo solido.
* La selezione di un corpo solido convertirà e sostituirà l'intero corpo con una mesh, ma la selezione di singoli bordi o vertici appartenenti ad un solido creerà una nuova mesh sulla geometria esistente, senza influire sul corpo originale.
* La conversione di un gruppo di bordi o vertici creerà una singola mesh di linee \(una mesh composta da bordi\) o una singola mesh di punti \(una mesh composta da punti\), il che significa che non sarà possibile selezionare singoli bordi o vertici una volta che sono stati combinati in una singola mesh. Riconvertire le mesh in oggetti se si desidera regolare la posizione di un singolo elemento.

**Conversione della geometria raggruppata in mesh:**

* Le mesh diventano ancora più potenti quando è possibile convertire un intero gruppo e tutti i relativi gruppi nidificati in mesh.
* I gruppi e i relativi contenuti nidificati possono essere convertiti in gruppi utilizzando un plug-in:
   * Cercare l'icona Gestione plugin sul lato destro dell'applicazione:
      * ![](../.gitbook/assets/plugin-manager_icon.PNG)
   * Individuare il plug-in Mesh + Unmesh All e fare clic sulla casella di controllo per installarlo:
      * ![](../.gitbook/assets/plugin-manager_mesh-unmesh-all.PNG)
   * Verrà caricato il plug-in Mesh + Unmesh All. È sufficiente selezionare un gruppo contenente oggetti da convertire in mesh e fare clic su Mesh All.
      * ![](../.gitbook/assets/mesh-unmesh-all-plugin.PNG)
   * Quando si convertono mesh o oggetti nidificati con questo plug-in, verrà visualizzato un messaggio di aggiornamento nella parte superiore della schermata che indica il numero di gruppi e istanze di gruppi interessati dall'operazione:

![](../.gitbook/assets/success_mesh-all.PNG)

### Interazione con le mesh

**A causa della loro natura leggera, le mesh presentano alcune limitazioni e comportamenti:**

* Non sarà possibile modificare le singole superfici, i singoli bordi o vertici di una mesh.
   * Tuttavia, è possibile ridipingere le mesh e spostare le singole mesh create in seguito all'applicazione di materiali diversi alle superfici \(vedere sopra\).
* Lo snap alle mesh è limitato alle superfici e ai vertici delle mesh. Per motivi di prestazioni, le operazioni di snap e deduzione non funzioneranno con i bordi delle mesh.
   * Tuttavia, i file DWG convertiti in mesh \(un tipo diverso di mesh noto come mesh di linee\) manterranno la possibilità di eseguire lo snap e la deduzione ai bordi delle mesh.
* Non è possibile applicare livelli alle mesh.
* Le mesh non riportano problemi delle superfici a tenuta ermetica o delle superfici posteriori. Riconvertirle in oggetti per verificare se sono a tenuta ermetica o meno.
   * Gli oggetti che erano a tenuta ermetica prima della conversione in mesh rimarranno tali quando vengono riconvertiti in un oggetto.
* Le mesh non possono essere utilizzate nelle operazioni di modellazione avanzata, quali unione/taglio di solidi, involucro 3D, offset 3D, raccordo, loft, estrusione su percorso o copertura.

In caso contrario, le mesh verranno visualizzate e si comporteranno come qualsiasi altro oggetto di FormIt: possono essere posizionate in gruppi, assegnate ai layer, visualizzate nelle scene, utilizzate per l'analisi e così via.

**L'eventuale interazione con una mesh è indicata dalla descrizione comando che mostra Sulla mesh o dal pannello Proprietà che riporta una mesh:**

![](../.gitbook/assets/snap_on-mesh.PNG)

![](../.gitbook/assets/properties-panel_mesh.PNG)

**Alcuni tipi di file vengono importati automaticamente come mesh per migliorare le prestazioni:**

* I file STL e OBJ, che possono contenere geometria densa, ad esempio nuvole di punti di altre applicazioni, vengono importati automaticamente come mesh.
* I file DWG, che possono contenere milioni di piccoli segmenti di bordi su curve di alta qualità, vengono importati automaticamente come mesh.

### Riconversione di mesh in oggetti

È sufficiente selezionare Mesh e utilizzare il tasto di scelta rapida MO \(Mesh in oggetti\) oppure fare clic con il pulsante destro del mouse e selezionare Mesh in oggetti nel menu contestuale:

![](../.gitbook/assets/context-menu_mesh-to-object.PNG)

Una volta convertiti gli oggetti in mesh, nella parte superiore della schermata viene visualizzato un messaggio di conferma:

![](../.gitbook/assets/success_mesh-to-object.PNG)

**Durante la riconversione di mesh in oggetti:**

* Eventuali oggetti che erano in precedenza solidi/a tenuta ermetica prima della conversione in mesh verranno riuniti in un solido a tenuta ermetica durante la riconversione in un oggetto.
* La conversione di una serie di bordi \(ad esempio da un file DWG\) o di una serie di vertici \(ad esempio da una nuvola di punti\) in una mesh e viceversa consente di inserire automaticamente gli oggetti senza mesh in un gruppo.
   * In questo modo si evita che i nuovi bordi o vertici si uniscano con altra geometria, il che potrebbe avere effetti negativi e influire sulle prestazioni.
   * È sufficiente scomporre il gruppo risultante per rilasciare i bordi e/o i vertici.

**Riconversione di mesh raggruppate in oggetti:**

* Vedere le istruzioni riportate sopra per utilizzare il plug-in Mesh + Unmesh All per riconvertire i gruppi e le relative mesh nidificate in oggetti.

