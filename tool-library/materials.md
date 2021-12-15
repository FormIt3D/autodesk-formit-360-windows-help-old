# Materiali

Rendere visibili i modelli di FormIt con materiali che supportano mappe di riflessione, lucide e di composizione in rilievo.

## Pannello Materiali

![](<../.gitbook/assets/materials-sample-category (2).png>)

Nel pannello Materiali, è possibile scegliere tra una vasta gamma di Campioni di materiali, spostarsi tra le librerie di materiali collegate e, a partire da FormIt 2021, accedere al contenuto Materiali di altri file di FormIt (.AXM) e utilizzarlo.

### Origini della libreria di materiali

In FormIt 2021 e versioni successive, il pannello Materiali dispone di un'interfaccia a discesa che consente di scegliere tra le origini disponibili della libreria di materiali: Nel disegno, Campioni di materiali e [librerie collegate](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

![](<../.gitbook/assets/materials-directory-picker (1).png>)

#### Nel disegno

Mostra i materiali salvati nel disegno di FormIt corrente.

#### Campioni di materiali

Mostra un elenco dei materiali di esempio disponibili. Queste offerte sono memorizzate in un server basato su cloud, quindi si tenga presente quanto segue:

* È necessaria una connessione ad Internet quando si accede per la prima volta alle categorie di Campioni di materiali.
* Quando si accede per la prima volta ad una categoria, questa verrà scaricata e quindi memorizzata nella cache del computer in uso, in modo che le sessioni future non richiedano un download.
* Il team di FormIt può aggiornare occasionalmente le offerte in Campioni di materiali. In tal caso, FormIt eliminerà automaticamente e scaricherà nuovamente le categorie per ottenere le ultime voci.

![](../.gitbook/assets/materials-samples\_original.png)

**Librerie collegate**

Altre directory e posizioni verranno visualizzate dopo il [collegamento delle librerie di materiali](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

### Creazione, eliminazione e contagocce

![](../.gitbook/assets/materials\_add.PNG) **Crea un nuovo materiale** definendone le impostazioni di colore, trama, mappa di composizione in rilievo, mappa di ritaglio, trasparenza e riflessione/lucidità.

![](<../.gitbook/assets/materials\_delete (1) (1).PNG>) **Eliminare** i materiali selezionati.

![](../.gitbook/assets/materials\_eyedropper.PNG) Utilizza il **contagocce** per un materiale dipinto nella scena e inizia immediatamente a dipingerlo.

* Fare clic sullo strumento del contagocce, quindi fare clic su una superficie dipinta con un materiale.
* Il materiale che si trova sulla superficie verrà evidenziato nel pannello e lo strumento del pennello diventerà attivo con il materiale caricato.

### Aggiornamento, collegamento di librerie ed eliminazione di materiali inutilizzati

\*\*\*\*![](../.gitbook/assets/materials-link.png) **Collega le librerie di materiali** da directory locali. Nelle directory contenenti file JPG, PNG o AXM (FormIt) verrà visualizzato il contenuto. Per ulteriori informazioni, vedere [Collegamento delle librerie di materiali](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

![](../.gitbook/assets/materials-refresh.png)**Aggiorna** la directory corrente. Il pulsante viene attivato solo quando si visualizza una directory collegata localmente (non Nel disegno o Campioni di materiali).

![](../.gitbook/assets/materials-purge.png) **Elimina materiali inutilizzati** dal disegno di FormIt corrente.

I materiali inutilizzati possono accumularsi naturalmente durante la procedura di iterazione, ma possono essere aggiunti in modo significativo alle dimensioni del file se utilizzano trame di alta qualità.

I materiali inutilizzati compaiono con un nome di colore grigio nell'elenco Nel disegno.

Fare clic sullo strumento Elimina inutilizzati per eliminare tutti i materiali inutilizzati. Prima verrà visualizzato un messaggio di richiesta, in modo da poter annullare l'operazione in caso di eventuali dubbi. Questo pulsante è attivato solo nell'elenco Nel disegno.

### Collegamento delle librerie di materiali

FormIt 2021 e versioni successive offre la possibilità di collegare il pannello Materiali alle directory locali (librerie) contenenti il contenuto Materiali, incluse le cartelle di file JPG, PNG e/o FormIt:

![](../.gitbook/assets/materials-axms.png)

![Vista di singoli materiali da un file di FormIt o file JPG/PNG in una directory.](../.gitbook/assets/materials-axm-content.png)

* **file JPG/PNG** verranno visualizzati come Materiali, che possono essere disegnati direttamente nel disegno di FormIt corrente.
   * Facendo clic su una miniatura, il file di immagine viene convertito in un materiale di FormIt al volo e copiato nel disegno corrente.
   * In FormIt si tornerà alla directory Nel disegno per visualizzare il materiale appena copiato nel disegno.
* **file di FormIt (\*.axm)** verranno visualizzati come cartelle con un'icona di FormIt.
   * Facendo clic sulle cartelle dei file di FormIt verranno visualizzati tutti i materiali di FormIt salvati in tale file.
   * Si noti che in FormIt, per ottenere il contenuto Materiali, si deve caricare parte del file, pertanto la visualizzazione di Materiali nel pannello potrebbe richiedere più tempo per i file di grandi dimensioni.

### Interazioni di materiali

**Dipingere un materiale** facendo clic una sola volta sulla miniatura. Verrà attivato lo strumento del pennello, grazie al quale è ora possibile posizionare il cursore sulla geometria nell'area di disegno di FormIt e fare clic su superfici o gruppi per dipingerli.

Una volta attivato lo strumento del pennello:

* Dipingere superfici e gruppi facendo clic una sola volta.
   * Quando si dipingono i gruppi, il materiale verrà sovrapposto in serie nella geometria nidificata e coprirà qualsiasi superficie o gruppo dipinto con il materiale di default.
* Dipingere interi solidi facendo doppio clic su una superficie per selezionare ogni elemento associato.

È inoltre possibile selezionare prima le superfici e i gruppi, quindi fare clic una sola volta su una miniatura del materiale per dipingere la selezione con tale materiale.

**Modificare un materiale** facendo doppio clic sulla miniatura, il che consentirà di visualizzare l'Editor materiali (vedere di seguito).

**Rinominare un materiale** facendo doppio clic sul nome.

**Identificare un materiale** dipinto sulla geometria selezionandolo e cercando l'evidenziazione e l'icona che indicano quali materiali sono dipinti sulla geometria selezionata.

![](../.gitbook/assets/material\_selected.png)

**Il materiale di default** può essere utilizzato per "cancellare" in modo efficace una superficie o un gruppo di eventuali materiali. Qualsiasi geometria non dipinta con un materiale viene dipinta implicitamente con il materiale di default.

### Gestione di elenchi

Regolare la dimensione delle miniature regolando la larghezza della colonna (fare clic e trascinare la linea verticale a destra del "materiale").

Filtrare la visualizzazione per materiali specifici digitando sulla barra "Filtro...".

I materiali con nomi visualizzati in un font grigio indicano che tali materiali non sono utilizzati nel disegno corrente.

## Creazione e modifica di materiali

![](<../.gitbook/assets/materials-editor (1).png>)

Quando si crea o si modifica un materiale, verrà visualizzata la finestra di dialogo Editor materiali, in cui è possibile personalizzare:

* **Colore**
* **Mappe immagine**
   * Fare clic sulla miniatura per scegliere una nuova mappa.
   * Fare clic sull'icona Salva per salvare la mappa per la modifica in un'altra applicazione.
   * Fare clic sull'icona Elimina per eliminare la mappa da questo materiale.
      * **Trama di un file di immagine**
         * File JPG o PNG
      * **Mappa di composizione in rilievo di un file di immagine**
         * File JPG consigliato
         * Ideale per aggiungere effetti di profondità ai materiali
         * È possibile utilizzare freeware come ShaderMap per generare mappe di composizione in rilievo a partire da una trama.
      * **Mappa di ritaglio di un file di immagine**
         * PNG
         * Ideale per i materiali con trasparenza selettiva, ad esempio le recinzioni o i pannelli perforati.
* **Nome**
* **Scala orizzontale e verticale**
   * Quando è attivato, il pulsante di blocco delle proporzioni assicura che la scala orizzontale e verticale rispetti le proporzioni della trama.
   * Stirare un materiale regolando la scala orizzontale indipendentemente dalla scala verticale.
   * È possibile sostituire la scala orizzontale e verticale per ogni superficie utilizzando lo strumento Regola posizionamento materiale (vedere di seguito).
* **Trasparenza**, **Riflesso: Diretto o Riflesso: Obliquo** e **Lucentezza**

## Regolazione del posizionamento dei materiali

Quando si dipinge un materiale su una superficie, FormIt ipotizza l'orientamento migliore:

* Le superfici verticali verranno orientate con la parte superiore della trama orientata lungo l'asse Z.
* Le superfici orizzontali orienteranno la trama in senso longitudinale lungo il lato più lungo della superficie.

Utilizzare lo strumento **Regola posizionamento materiale** per sostituire il posizionamento di default del materiale, nonché la scala del materiale in superfici specifiche:

* Selezionare una o più superfici dipinte con un materiale.
   * Se la superficie eredita il materiale dal gruppo principale, sarà necessario prima dipingere la superficie direttamente.
* Accedere allo strumento Regola posizionamento materiale tramite il tasto di scelta rapida MP o dal menu di scelta rapida:

![](../.gitbook/assets/adjust-material-placement.PNG)

Utilizzare i controlli su schermo per spostare, ruotare e mettere in scala interattivamente le trame dei materiali direttamente sulla superficie:

![](../.gitbook/assets/materialplacement.gif)

![](../.gitbook/assets/adjust-material-placement.gif)

Per ripristinare una qualsiasi delle modifiche apportate al posizionamento del materiale, è sufficiente dipingere nuovamente la superficie con il materiale originale, dal pannello Materiali.

## Conversione di materiali in Revit

I materiali verranno trasferiti in Revit quando si utilizza il [modulo aggiuntivo FormIt](https://formit.autodesk.com/page/formit-revit) per Revit 2018 o versione successiva.
