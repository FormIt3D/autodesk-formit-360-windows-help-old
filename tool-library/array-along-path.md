# Array Along Path

## Con tecnologia di Dynamo

In FormIt 2021 e versioni successive, è possibile disporre gli oggetti lungo un percorso e personalizzare rapidamente i risultati localmente. Array Along Path è con tecnologia di Dynamo, il che significa che la matrice è facilmente configurabile per ottenere i risultati desiderati e la riesecuzione della logica aggiornerà la geometria localmente.

![](../.gitbook/assets/array-along-path.gif)

## Avvio di Array Along Path

* Accedere al pannello di Dynamo in FormIt per Windows e verificare di trovarsi nella directory Dynamo Samples.
* Fare clic sull'esempio Array Along Path.
* Sul lato sinistro della schermata, viene visualizzato il messaggio di richiesta Select object\(s\) to array.
   * È possibile selezionare qualsiasi combinazione di oggetti di FormIt per questo passaggio.
   * Dopo aver selezionato un elemento, è possibile fare clic sulla freccia avanti sul lato sinistro della schermata o premere INVIO.
* Verrà visualizzato il messaggio di richiesta Select path for array.
   * Qui è necessario selezionare solo una serie di bordi contigui o un gruppo contenente una serie di bordi contigui.
   * Dopo aver selezionato il percorso, fare clic sul pulsante di fine o premere INVIO.
* Il pannello di Dynamo indicherà che è in corso l'elaborazione delle modifiche. Al termine, si disporrà di una matrice generata da Dynamo in un gruppo di FormIt, pronta per la modifica \(vedere qui sotto\).

## Iterazione locale

Dopo l'esecuzione di Array Long Path, i risultati verranno impostati sui valori di default, pertanto sarà necessario modificarli in base alle esigenze specifiche.

All'esecuzione di Array Along Path, viene creato un nuovo gruppo contenente i risultati. In FormIt viene selezionato automaticamente il gruppo e sono mostrate le opzioni disponibili per l'istanza di Array Along Path.

È sempre possibile tornare alle proprietà di Array Along Path selezionando il gruppo e passando al pannello Proprietà oppure modificando il gruppo che mostrerà automaticamente le proprietà.

![](../.gitbook/assets/array-along-path-options.png)

### Select Object\(s\) to Array <a id="run"></a>

Fare clic su questa opzione per tornare alla procedura guidata di selezione per modificare gli oggetti di cui è in corso la creazione della matrice.

### Select Array Path

Fare clic su questa opzione per tornare alla procedura guidata di selezione per modificare il percorso utilizzato per calcolare la matrice.

### Array Type <a id="run"></a>

Questa opzione attiva o disattiva il tipo di matrice da calcolare: By Distance o By Number.

**Se è True**, il calcolo sarà By Distance, quindi il numero seguente si riferisce alla distanza tra le copie.

**Se è False**, il calcolo sarà By Number of Copies, pertanto il numero sotto questo campo si riferisce al numero di copie da adattare lungo il percorso.

### Include Original Selection In Results?

Quando è **True**:

* Gli oggetti selezionati verranno conteggiati come una delle nuove copie.
* Il gruppo di Dynamo risultante includerà la selezione originale nei risultati, in modo che si verifichi lo Z-fighting delle nuove copie con la selezione originale. È possibile inserire la selezione originale in un [layer](layers.md) e disattivarlo per nasconderlo.

Quando è **False**:

* La matrice risultante **non** includerà la selezione originale, pertanto si otterrà il numero di copie specificato **oltre alla** selezione originale e non si verificherà lo Z-fighting dei risultati.

### Rotate Copies Along Path?

Quando è **True**, le copie vengono ruotate per mantenere l'orientamento dell'oggetto originale rispetto al percorso.

Quando è **False**, le copie non vengono ruotate, ma solo spostate.

### Use Relative Positioning Along Path?

Quando è **True**:

* Ogni copia mantiene la distanza tra il percorso e l'oggetto originale.
* Se l'oggetto originale **non** è posizionato in corrispondenza di uno dei punti finali del percorso, per il calcolo della matrice verrà utilizzato il segmento rimanente più grande del percorso.

Quando è **False**:

* L'intera lunghezza del percorso verrà utilizzata per calcolare la matrice, indipendentemente dal punto in cui si trova l'oggetto originale rispetto al percorso.
* In questo modo si disgiunge la posizione del percorso rispetto all'oggetto e si utilizza semplicemente l'intero percorso. È utile se il percorso e l'oggetto non sono vicini l'uno all'altro.

### Reverse Path Direction?

Solo per percorsi chiusi. Quando si utilizza Array Along Path con un percorso chiuso, la direzione della curva potrebbe invertire inaspettatamente i risultati previsti della matrice. Impostare questa opzione su **True** per invertire la direzione della matrice se i risultati vengono invertiti.

### Esegui <a id="run"></a>

Dopo aver modificato le opzioni, fare clic sul pulsante Esegui per eseguire il grafico di Dynamo sottostante e generare nuovi risultati. Questo pulsante diventa blu quando i parametri sono stati modificati, pertanto è necessario fare clic per visualizzare gli aggiornamenti nella geometria finale.‌

### Edit Embedded Graph <a id="edit-embedded-graph"></a>

Facendo clic su questa opzione si avvia l'ambiente dell'editor grafico di Dynamo, in modo che sia possibile visualizzare e modificare il grafico di Dynamo sottostante per modificare più rapidamente i parametri e visualizzare gli aggiornamenti dinamici o per esaminare/regolare la logica.



## Selezione della geometria

Quando si selezionano gli oggetti per Array Along Path e altri grafici di Dynamo basati sulla selezione:

* È possibile selezionare qualsiasi combinazione di oggetti di FormIt, ovvero vertici, bordi, superfici, solidi, gruppi e mesh.
   * Tenere presente che, a seconda del passaggio, alcuni di questi oggetti non devono essere selezionati.
   * Ad esempio, quando si seleziona il percorso, è necessario selezionare solo una serie contigua di bordi o un gruppo contenente una serie contigua di bordi. Qualsiasi altra operazione causerà un errore del grafico.
* È possibile fare doppio clic su un oggetto per selezionare tutti gli elementi associati.
* È possibile utilizzare la finestra di selezione dell'area per acquisire una serie di oggetti.
* È possibile selezionare gli oggetti già selezionati per deselezionarli.
* Per procedere con un passaggio basato sulla selezione, è necessario almeno un oggetto.



