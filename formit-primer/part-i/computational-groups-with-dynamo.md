# 1.10 - Gruppi di calcolo con Dynamo

_In questo capitolo, utilizzeremo la potenza di elaborazione di_ [_**Dynamo**_](http://dynamobim.org/) _per posizionare e modificare i gruppi flessibili associati agli esempi di grafici di Dynamo predefiniti._

_Se non è stata completata l'ultima sezione, scaricare e aprire il file_ _**1.10 - Computational Groups with Dynamo.axm**_ _dal_ _**set di dati della Parte I della Guida introduttiva di FormIt**._

_È possibile_ [_**ottenere ulteriori informazioni qui**_](http://formit.autodesk.com/page/formit-dynamo) _sul modo in cui FormIt e Dynamo collaborano per i workflow di progettazione computazionale._

## **Creazione di scale della terrazza inferiore**

1 - Assicurarsi che i layer **Lower Terrace, Main Building Floor** e **Plan Image** siano attivati, poiché è qui che aggiungeremo le scale.

2 - Per posizionare un gruppo scale collegato ad uno degli esempi di Dynamo predefiniti:

1. Aprire la **tavolozza di Dynamo** sulla barra delle tavolozze. Dovrebbero essere visualizzati alcuni oggetti di Dynamo incorporati nella directory **Dynamo Samples**.
2. Fare clic sull'esempio di Dynamo **Stairs** per portarlo nello spazio modello. In FormIt si eseguirà in background il grafico, da cui verrà generata la geometria della scala.
3. Spostare il cursore nell'area di disegno e, una volta caricata la scala, un'anteprima semitrasparente della geometria della scala si sposterà ora insieme al mouse. Spostare il cursore nell'area di disegno, vicino alla terrazza, quindi fare clic per posizionare la scala. Premere **ESC** per annullare la selezione. Notare che dopo il posizionamento delle scale, la **tavolozza Proprietà** si aprirà automaticamente.

![](../../.gitbook/assets/0%20%2815%29.png)

_**Nota**_ [_**È inoltre possibile collegare le directory locali**_](https://formit.autodesk.com/page/formit-dynamo#dynamo-getting-started) _contenenti i grafici di Dynamo ed eseguire i grafici di Dynamo locali come questi esempi._

3 - Per aggiornare le quote delle scale:

1. Con il gruppo scale selezionato, modificare gli input disponibili nella sezione **INPUTS** di Dynamo nella parte inferiore della **tavolozza Proprietà** in modo che corrispondano come mostrato di seguito. La maggior parte dei gruppi creati tramite gli script di Dynamo includerà una sezione di Dynamo nelle relative proprietà quando selezionate.
   * Add Top Landing = False
   * Add Middle Landing = False
   * Add Bottom Landing = False
   * Floor-to-Floor Height = 2.6
   * Stair Width = 12
   * Riser Height = 0.6
   * Tread Length = 1.25
   * Tread Overlap = 0.25
   * Tread Thickness = 0.25
   * Height Between Middle Landings = \(non pertinente poiché non viene creato alcun pianerottolo centrale\)
   * Middle Landing Length = \(non pertinente poiché non viene creato alcun pianerottolo centrale\)
   * Top/Bottom Landing Length = \(non pertinente poiché non viene creato alcun pianerottolo\)
2. Fare clic sul pulsante **Esegui** per rieseguire lo script di Dynamo utilizzando i valori di input aggiornati.
3. Spostare il gruppo in base alle esigenze per posizionare la scala nella posizione corretta, in base a **Plan Image**. Prestare attenzione a non modificare il prospetto del gruppo scale mentre lo si sposta. Consultare i capitoli precedenti per ulteriori informazioni sui trucchi e sulle tecniche per lo spostamento degli elementi del modello.

![](../../.gitbook/assets/1%20%2811%29.png)

_**Nota**_ _L'input_ _**Floor-to-Floor Height**_ _è un'approssimazione dell'altezza totale della scala._ _**Riser Height**_ _è il parametro che definisce effettivamente l'altezza delle scale. In questo esempio impostiamo_ _**Floor-to-Floor Height**_ _su 2.6' ma l'altezza finale della scala è 3.0' \(0.6' \(**Riser Height**\) x 5 \(numero di alzate\)\). Poiché lo spazio tra il terreno e la parte superiore della terrazza del pavimento è di 3'-2", il valore rimanente 2" è contenuto nell'alzata superiore._

## **Creazione di scale dell'edificio principale**

_Nei passaggi precedenti abbiamo creato una scala senza pianerottoli. Ora creeremo una scala che utilizza un pianerottolo superiore allineato con_ _**Main Building Floor**._

1 - Iniziare creando una copia delle scale appena create:

1. Selezionare la scala esistente, quindi fare clic in un punto qualsiasi di **Plan Image** per avviare un comando di spostamento. In questo modo in FormIt verrà utilizzato il prospetto di **Plan Image** come altezza di riferimento iniziale per il posizionamento della nuova copia. Premere **CTRL** per eseguire una **copia rapida**.
2. Spostare il cursore più vicino all'edificio principale sopra la terrazza. Notare che ora la superficie superiore della terrazza è il nuovo piano di riferimento. Fare clic per posizionare il gruppo.

![](../../.gitbook/assets/2%20%289%29.png)

_**Nota**_ _Poiché_ _**Plan Image**_ _si trova sul piano_ _**Ground Level**_ _, lo_ _**strumento Sposta**_ _utilizzerà quel piano come riferimento per il punto iniziale. Notare la descrizione comando_ _**Sulla superficie**_ _nell'immagine precedente, ad indicare che la superficie Plan Image è selezionata come riferimento iniziale e la superficie superiore di_ _**Lower Terrace Floor**_ _è selezionata come riferimento finale._

2 - Utilizzare lo strumento **Rendi univoco \(MU\)** in modo che quando modifichiamo gli input di Dynamo di questa scala, la scala inferiore non verrà influenzata. Riposizionare il gruppo in base alle esigenze in modo che si trovi vicino alla posizione finale. Perfezioneremo questo elemento in un secondo momento. È possibile attivare o disattivare la visibilità del layer **Lower Terrace** per visualizzare la pianta sottostante in modo da posizionarla, ma è necessario fare nuovamente attenzione a non modificare il prospetto della nuova scala mentre la si sposta.

3 - Nella **tavolozza Proprietà** aggiornare la sezione **Inputs di Dynamo** come mostrato di seguito ed eseguire nuovamente lo script.

* Add Top Landing = True
* Floor-to-Floor Height = 2.333
* Riser Height = 0.466
* Tread Length = 1.5
* Top/Bottom Landing Length = 2.5

![](../../.gitbook/assets/3%20%281%29.jpeg)

_**Nota**_ _Se si imposta_ _**Add Bottom Landing**_ _su_ _**True**_ _e si riesegue lo script, la superficie superiore del pianerottolo inferiore deve essere allineata alla superficie superiore di_ _**Lower Terrace Floor**. Ciò accade perché, diversamente dalle scale precedenti, è stata regolata l'opzione_ _**Riser Height**_ _in modo che_ _**Floor-to-Floor Height**_ _corrisponda all'altezza reale desiderata \(2'-4" o 2.333"\)._

2 - Riposizionare il gruppo nella posizione finale. Il pianerottolo superiore deve essere allineato con **Main Building Floor**.

3 - Per finalizzare le scale, aggiungere il materiale **Stone - Travertine** per uniformarle ai pavimenti. Per ulteriori informazioni sull'applicazione dei materiali, vedere i capitoli precedenti.

