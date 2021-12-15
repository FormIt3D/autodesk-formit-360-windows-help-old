# 3D Text

## Con tecnologia di Dynamo

In FormIt 2021 e versioni successive, è possibile generare e modificare oggetti di 3D Text con tecnologia di Dynamo. Dynamo consente di modificare localmente il font, la dimensione e altre proprietà del testo, senza dover rigenerare e riposizionare il testo quando sono necessarie modifiche.

![](../.gitbook/assets/3d-text.gif)

## Posizionamento di testo 3D

![](../.gitbook/assets/3d-text-placement.gif)

* Accedere al pannello di Dynamo in FormIt per Windows e verificare di trovarsi nella directory Dynamo Samples.
* Fare clic sull'esempio 3D Text.
* Spostare il cursore nell'area di disegno. 3D Text verrà visualizzato sul cursore.
   * Prima del posizionamento, è possibile posizionare il cursore sulla geometria per orientare 3D Text in modo diverso, ad esempio su una superficie verticale per allineare il testo verticalmente. È anche possibile premere TAB per passare da un orientamento all'altro.
* Fare clic per posizionare 3D Text, che verrà generato all'interno di un gruppo di FormIt.
* Dopo il posizionamento, verrà mostrato il pannello Proprietà per visualizzare le opzioni disponibili per 3D Text.

## Iterazione locale

Il vantaggio dell'utilizzo di Dynamo per generare 3D Text è che la modifica è semplice e mantiene il testo nella posizione corrente, per un'iterazione rapida.

Le opzioni di 3D Text sono disponibili nel pannello Proprietà quando è selezionato il gruppo 3D Text o quando si modifica il gruppo.

Dopo aver posizionato inizialmente 3D Text, il pannello Proprietà verrà visualizzato automaticamente. È inoltre possibile selezionare il gruppo e passare direttamente a Proprietà oppure fare doppio clic sul gruppo per passare automaticamente al pannello Proprietà.

![](../.gitbook/assets/3d-text-options.png)

### Text

Immettere il testo che si desidera visualizzare nella geometria di 3D Text. Questo campo visualizza anche l'anteprima del font e della giustificazione selezionati. Premere INVIO per più linee.

### Font

Selezionare il font per 3D Text. Questo elenco visualizza i font disponibili nel computer e la selezione di un nuovo font aggiornerà il campo Text.

Tenere presente che alcuni font presentano una geometria più complessa e potrebbero richiedere più tempo per la generazione utilizzando Dynamo.

### Justification

In questo modo, il testo verrà spostato in modo da allinearlo rispetto all'origine del sistema di coordinate locali del gruppo.

* Con Left il testo inizia in corrispondenza dell'origine del gruppo e si espande verso destra.
* Con Center il testo è sempre centrato rispetto all'origine del gruppo.
* Con Right il testo termina in corrispondenza dell'origine del gruppo.

![](../.gitbook/assets/3d-text-justification-combined.png)

### Text Size

![](../.gitbook/assets/3d-text-text-size.png)

L'altezza del testo, nelle unità di FormIt correnti.

### Extrusion Depth

La quantità di estrusione 3D del testo, nelle unità di FormIt correnti. 3D Text è progettato per essere solido, quindi questo valore non può essere pari a zero. Tuttavia, si può avvicinare molto a zero per renderne meno evidente l'estrusione.

### Tracking

![](../.gitbook/assets/3d-text-tracking.png)

Il tracciamento è utile per regolare la spaziatura di default tra le lettere in un particolare font. Utilizza le unità di FormIt correnti e il valore può essere positivo o negativo. Ad esempio, in piedi, 0.25 aggiungerà 3" di spaziatura tra le lettere. Al contrario, -0,25 avvicinerà di 3" tutte le lettere.

### Multi-Line Spacing

![](../.gitbook/assets/3d-text-multi-line.png)

Se nel campo Text sono presenti più righe, questo valore controlla lo spazio tra le righe di testo. Utilizza le unità di FormIt correnti.

### Invert Text

![](../.gitbook/assets/3d-text-inverted.png)

Quando è True, questa opzione crea un solido attorno al testo e ne rimuove il testo, dando come risultato testo "invertito", come se il testo fosse stato ritagliato da un materiale.

### Inverted Text Border

![](../.gitbook/assets/3d-text-inverted-border.png)

Si applica solo quando Invert Text è True. Specifica la quantità di bordo attorno al testo da utilizzare per il solido da cui viene rimosso il testo. Utilizza le unità di FormIt correnti.

### Curve Faceting Quality

Le curve dei font vengono convertite in segmenti di linea utilizzando 3D Text, pertanto questo valore controlla la precisione con cui le curve sono sfaccettate.

Numeri più bassi genereranno una sfaccettatura più grossolana \(segmenti più lunghi\) e numeri più alti daranno come risultato una sfaccettatura più fine \(segmenti più brevi\). Questo valore sostituisce le impostazioni di sfaccettatura di curve e superfici di FormIt in Preferenze.

### Esegui

Dopo aver modificato le opzioni, fare clic sul pulsante Esegui per eseguire il grafico di Dynamo sottostante e generare nuovi risultati. Questo pulsante diventa blu quando i parametri sono stati modificati, pertanto è necessario fare clic su Esegui per visualizzare gli aggiornamenti nella geometria finale.‌

### Edit Embedded Graph

Facendo clic su questa opzione si avvia l'ambiente dell'editor grafico di Dynamo, in modo che sia possibile visualizzare e modificare il grafico di Dynamo sottostante per modificare rapidamente i parametri e visualizzare gli aggiornamenti dinamici o per esaminare/regolare la logica. Questa operazione non è necessaria, ma può essere utile per la risoluzione dei problemi o per una modifica più rapida. Per ulteriori informazioni, vedere di seguito.

## Iterazione più rapida in Dynamo

Se si esegue l'iterazione sulle opzioni di 3D Text, potrebbe essere più veloce avviare l'editor grafico di Dynamo, che consente di regolare i parametri e visualizzare le modifiche in tempo reale. Ciò consente inoltre di esaminare la logica che si trova dietro il grafico, nel caso di eventuali problemi.

![](../.gitbook/assets/3d-text-edit-embedded.png)

È possibile fare clic sul pulsante Edit Embedded Graph nel pannello Proprietà per avviare l'editor grafico di Dynamo.

![](../.gitbook/assets/3d-text-edit-embedded-windows.png)

## Risoluzione dei problemi

3D Text utilizza Dynamo in background e Dynamo utilizza un kernel di modellazione denominato ASM per generare la geometria, che viene trasferita a FormIt.

Alcuni font possono creare "curve autointersecanti", o altra geometria problematica, che causano errori in ASM.

Se viene visualizzato un messaggio di errore quando si tenta di eseguire 3D Text, o se le lettere scompaiono, è utile fare clic su Edit Embedded Graph per vedere quello che non funziona nel grafico e dove potrebbe verificarsi il problema.

Alcuni font presentano anche problemi noti che ne impediscono la conversione nella geometria corretta. Bahnschrift ne è un esempio. Se si incontra un altro font problematico, [comunicarcelo nei forum](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=en). Faremo tutto il possibile per risolvere eventuali problemi con font specifici.





