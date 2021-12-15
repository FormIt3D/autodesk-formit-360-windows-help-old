# 1.15 - Utilizzo di Revit

_Una delle funzionalità più interessanti di FormIt è la possibilità di spostare il modello da un ambiente di modellazione flessibile come FormIt ad un ambiente parametrico potente come Revit. In questo capitolo, esamineremo alcuni esercizi che consentono di spostare vari elementi da FormIt a Revit e da Revit a FormIt._

_In questo capitolo verranno utilizzate le famiglie di Revit di esempio. Se non è già stato fatto, è possibile scaricarle dal **set di dati di Casa Farnsworth.**Se non è stata seguita l'intera esercitazione fino a questo momento, è anche possibile scaricare e aprire il file **1.15 – Working With Revit.axm** dai **set di dati della Parte I della Guida introduttiva di FormIt**._

_In questi esercizi, utilizzeremo Revit 2022, che offre funzionalità di interoperabilità migliorate con FormIt. Nelle versioni precedenti di Revit non sono presenti alcune o nessuna delle funzionalità mostrate in questa esercitazione e l'interfaccia utente sarà diversa._

## Da Revit a FormIt

### Conversione di famiglie di Revit per l'utilizzo in FormIt

Se si dispone di una serie di famiglie di Revit che si desidera utilizzare in FormIt, sarà interessante consultare questa sezione, che illustra come esportare in batch i file RFA in FormIt.

_**Nota**_ _Nella procedura riportata di seguito vengono mostrati l'interfaccia e i passaggi necessari quando si utilizza Revit 2022, ma gli strumenti_ _**Converti RFA in FormIt**_ _sono disponibili a partire da Revit 2016._

1 - Aprire un nuovo progetto o una nuova famiglia di Revit. Quindi:

1. Sulla barra multifunzione **Moduli aggiuntivi**, individuare il gruppo **Convertitore FormIt** e fare clic sul pulsante **Converti RFA in FormIt**. Viene visualizzata la **finestra di dialogo Converti famiglie di Revit**.
2. Nel campo **Percorso dei file di famiglia di Revit**, individuare la posizione in cui è stata salvata la seguente cartella nel computer: **Farnsworth House Data Set &gt; Supporting Files &gt; Revit**.
3. Nel campo **Percorso del contenuto di FormIt**, individuare **Farnsworth House Data Set &gt; Supporting Files &gt; FormIt &gt; Custom FormIt Content**. Se il capitolo **1.11 Importazione di modelli con Libreria del contenuto** non è stato completato, potrebbe essere necessario creare la cartella **Custom FormIt Content** o scegliere un'altra destinazione.
4. Fare clic su **OK** per avviare il processo di conversione.

![](../../.gitbook/assets/0%20%2823%29.png)

_**Note **_

* _Questo processo richiede tempo poiché in Revit viene aperto il file_ _**RFA**_ _nel primo percorso, quindi viene convertito e salvato in formato_ _**AXMF**_ _per FormIt._
* _In questo esercizio, stiamo convertendo un solo file, ma è possibile utilizzare questo processo per convertire in batch tutti i file_ _**RFA**_ _nella cartella selezionata \(inclusi eventuali file_ _**RFA**_ _nelle cartelle nidificate\)._

2 - Una volta completato il processo, tornare a FormIt. In questa posizione, il nuovo contenuto verrà visualizzato nella **tavolozza Libreria del contenuto**, all'interno della cartella **FormIt &gt;** **Custom FormIt Content** precedentemente collegata. Se i file **AXMF** convertiti sono stati salvati in un percorso diverso o il capitolo **1.11 Importazione di modelli con Libreria del contenuto** non è stato completato, potrebbe essere necessario aggiungere tale cartella alla libreria di contenuti per visualizzarne il contenuto. Consultare il capitolo 1.11 per istruzioni su come aggiungere cartelle alla libreria di contenuti.

![](../../.gitbook/assets/1%20%2824%29.png)‌

**Nota** _Non tutte le categorie di Revit sono supportate per l'esportazione. Le famiglie "indipendenti" o "basate sul livello" sono supportate, ma le famiglie "basate sull'host" come porte e finestre non lo sono. Le opzioni Massa, Arredi fissi, Contesto, Arredo, Sistemi di arredo, Modelli generici, Parcheggio, Planimetria e Attrezzature speciali sono tutte supportate. Eventuali famiglie non supportate nella cartella selezionata verranno semplicemente ignorate._

## Da FormIt a Revit

_Esistono due modi diversi per importare la geometria da FormIt a Revit. È possibile importare un file_ _**.axm** esistente in un progetto di Revit o in un file di famiglia Revit, che funzionerà in modo simile ad un modello importato o ad un file CAD. In alternativa, è possibile avviare FormIt da Revit e importare ogni gruppo di FormIt in Revit come singolo elemento modello generico. Il secondo metodo è descritto nella **Parte II**, capitolo_ _**2.8**_ _**Workflow di Revit avanzati**._

### Importazione di Casa Farnsworth in Revit

1 - Per importare un file di FormIt \(**.axm**\) in Revit, avviare un nuovo progetto di Revit e aprire la vista 3D di default. Quindi:

1. Passare alla **scheda Inserisci** e fare clic sul pulsante **Importa CAD**. Viene visualizzata la finestra **Importa formati CAD**.
2. Verificare che l'elenco a discesa **Tipo file** sia impostato su **File FormIt \(\*.axm\)**.
3. Individuare e selezionare il file **.axm** di Casa Farnsworth su cui si sta lavorando. Se non è stata seguita la Parte I della Guida introduttiva, è anche possibile aprire il file **1.15 - Working With Revit.axm** nella cartella **Farnsworth House Data Set &gt; Chapter Files**.
4. Assicurarsi che l'opzione **Importa livelli di FormIt** sia selezionata.
5. Una volta definite le impostazioni, fare clic su **Apri** per importare la geometria di FormIt in Revit come singolo elemento.

![](../../.gitbook/assets/2%20%2824%29.png)

Importazione di un file di FormIt utilizzando il pulsante Importa CAD.

![](../../.gitbook/assets/3%20%2821%29.png)  
Elemento .axm importato. Notare che anche i livelli del modello di FormIt vengono importati in Revit.

_Analogamente ad altri formati CAD, i layer del file originale vengono importati in Revit. Questa funzionalità consente di definire diverse impostazioni di visibilità per ciascun layer per manipolare facilmente l'aspetto grafico del file di FormIt in qualsiasi vista di Revit._

2 - Per regolare la visibilità dei layer del file .axm importato:

1. Accedere alla finestra **Sostituzioni visibilità/grafica \(VG o VV\)**, scheda **Categorie importate**, espandere il file di FormIt importato e deselezionare il layer **Verde** per disattivare il layer nella vista corrente, quindi fare clic su **OK**.
2. Impostare **Stile visualizzazione** su **Realistico** e si noterà che tutti i materiali di FormIt sono stati importati in Revit.

![](../../.gitbook/assets/4%20%2820%29.png)

3 - Infatti, i materiali di FormIt importati saranno ora disponibili in questo progetto di Revit, etichettati con la classe **FormIt**. È sufficiente aprire il **Browser dei materiali** e cercare "FormIt" per visualizzarli tutti. Ora possono essere utilizzati nel progetto di Revit come qualsiasi altro materiale.

![](../../.gitbook/assets/5%20%2819%29.png)

