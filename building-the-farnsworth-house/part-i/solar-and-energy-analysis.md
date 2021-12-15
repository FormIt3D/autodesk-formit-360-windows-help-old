# Analisi solare ed energetica

Ora che il modello è stato creato, possiamo utilizzarlo per studiare l'**impatto solare ed energetico** del nostro progetto. Queste funzionalità sono incorporate in FormIt, in modo che i primi studi possano essere compresi dal punto di vista delle prestazioni degli edifici. Queste funzionalità sono disponibili solo in **FormIt Pro**. Se si utilizza l'app Web, è possibile che non si disponga dell'accesso.

Se non è stata completata l'ultima sezione, fare clic su File &gt; Apri e scegliere **farnsworth08.axm** dalla cartella FormIt Primer.

## Ombre

Prima di poter utilizzare uno qualsiasi di questi strumenti di analisi, è necessario [impostare la posizione](). In questo modo FormIt consente di accedere a dati precisi relativi a sole, ombre e clima.

1. Fare clic sull'icona del sole sulla [**barra degli strumenti delle azioni**](../../formit-introduction/tool-bars.md) e selezionare **Ombre \(DS\)**.

   ![](../../.gitbook/assets/3bdf0e2a-0ad4-4aac-b6fc-5e789643b0d6.png)

2. Regolare i dispositivi di scorrimento **Giorno** e **Ora** per vedere come cambiano le ombre.

   ![](../../.gitbook/assets/upperterracesketch_32.png)

3. Notare come la terrazza coperta sia ombreggiata nelle ore più calde dei mesi estivi, sicuramente non a caso.

**Nota** Le ombre possono causare una riduzione delle prestazioni dell'applicazione. Due suggerimenti per ovviare a questo problema: disattivare le ombre se la navigazione risulta lenta o disattivare layer come **Furniture** se non sono necessari per lo studio delle ombre.

## Analisi solare

Essendo dotati di memoria visiva, i progettisti possono imparare e comunicare un'incredibile quantità di informazioni dai diagrammi delle mappe termiche, come quello che stiamo per creare.

1. Nella parte inferiore del [**menu Sole**](../../formit-introduction/tool-bars.md), fare clic sul pulsante **Analisi solare**.
2. Si è in una modalità speciale in cui le **ombre**, i **tasti di scelta rapida** e altre **barre degli strumenti** sono disattivati.
3. Il funzionamento della selezione viene modificato in modalità **Analisi solare**. È possibile selezionare **scorrendo i gruppi**, non è necessario tenere premuto **CTRL** o **MAIUSC** per aggiungere elementi al gruppo di selezione ed è possibile deselezionare gli elementi facendo nuovamente clic. È possibile **fare un singolo clic** sulla geometria, **farvi doppio clic** o eseguirne la **selezione tramite finestra**.
4. Scegliere le superfici che si desidera studiare. **Fare un singolo clic** sulla parte superiore del **tetto** e sulla parte superiore dei **pavimenti**. Evitare di selezionare elementi piccoli come gli arredi.

   ![](../../.gitbook/assets/upperterracesketch_33.png)

5. Nell'angolo superiore sinistro dell'area di disegno, individuare la barra degli strumenti **Analisi solare**. Fare clic su **Analizza**. FormIt consente di calcolare ed eseguire il rendering delle superfici. Le impostazioni qui possono essere regolate prima **e** dopo la fine dell'analisi.

   ![](../../.gitbook/assets/solaranalysis.png)

6. L'impostazione **Mese Picco** mostra i valori di **picco** \(in Btu/ft²\) per il mese specificato. Questa opzione è destinata agli **studi di ombreggiatura**. È possibile modificare l'impostazione del mese e la grafica si aggiorna all'istante. **Posizionare il cursore** su una superficie analizzata per ottenere un valore **specifico**.

   ![](../../.gitbook/assets/460060a0-ea3b-4095-af45-40045811be22.png)

7. L'impostazione **Anno Cumulativo** mostra l'energia **cumulativa** per l'intero anno \(in KwH/m²\). Questa è destinata agli **studi sul potenziale fotovoltaico**.

   ![](../../.gitbook/assets/a9f61dfb-dfc9-4751-b145-b131a69c53cf.png)

8. Questi studi di **Analisi solare** possono essere esportati facendo clic su **File &gt; Esporta \(CTRL+E\)** e scegliendo **Immagine** dall'elenco a sinistra.

## Analisi energetica con Insight

FormIt ha integrato gli stessi strumenti di analisi delle prestazioni degli edifici utilizzati da Revit. **Insight** fornisce una dashboard di parametri di sistema degli edifici che è possibile regolare per riflettere i potenziali scenari senza richiedere la **rianalisi** della geometria del modello. Insight funziona meglio con la geometria di **volumetrie** di FormIt.

1. Assicurarsi di avere eseguito l'accesso con Autodesk Account. Disattivare **tutti** i layer **ad eccezione** del layer **Massing**. Alla geometria deve essere applicato almeno un **livello**.
2. In FormIt verrà inviata solo la geometria **visibile** ad Insight. Notare che anche una **massa** semplice produrrà una serie di dati da **Insight**.

   ![](../../.gitbook/assets/energymassing.png)

3. Fare clic sul pulsante **Insight &gt; Genera informazioni approfondite**. L'analisi verrà eseguita nel cloud, in modo che sia possibile continuare la modellazione durante il calcolo.

   ![](../../.gitbook/assets/energymenu.png)

4. Una volta completata dell'analisi, fare clic sul pulsante **Visualizza informazioni approfondite** per visualizzare il **modello energetico** e i **fattori delle prestazioni** \(se lo si desidera, è possibile visitare il sito Web direttamente all'indirizzo [**http://insight.autodesk.com**](http://insight.autodesk.com/)\).

   ![](../../.gitbook/assets/energydashboard.png)

5. Nella dashboard di Insight, è possibile impostare un valore \(o un intervallo di valori\) per ogni widget **Performance Factor** facendo clic sul fattore e trascinando i punti blu. L'intervallo è utile se non si conosce ancora il sistema specifico che verrà utilizzato dall'edificio.
6. Ad ogni modifica apportata ad un **fattore**, viene aggiornato l'**intervallo di costi energetici** \ (misurato in USD/m²/anno\). È possibile vedere le prestazioni del progetto rispetto a parametri di riferimento come **Ashrae 90.1** e la sfida di **Architecture 2030**.
7. Se il progetto cambia forma drasticamente, è possibile inviare nuovamente la massa aggiornata alla stessa dashboard. Se si desidera creare una **nuova** dashboard per il progetto aggiornato, sarà necessario prima selezionare **Salva con nome** in FormIt.
8. Se l'analisi energetica non riesce, è possibile che siano presenti **problemi delle superfici a tenuta ermetica \(DW\)** basati sulla geometria; questi possono essere esaminati e corretti in FormIt.
9. Disattivare il layer **Massing** e riattivare tutti gli altri layer.

