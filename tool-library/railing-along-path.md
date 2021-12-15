# Railing Along Path

## Con tecnologia di Dynamo

In FormIt 2021 e versioni successive, è possibile generare una ringhiera lungo un percorso e personalizzare rapidamente i risultati localmente. Railing Along Path è gestito da Dynamo, il che significa che la ringhiera risultante è facilmente configurabile per ottenere i risultati desiderati e la riesecuzione della logica aggiornerà la geometria localmente.

![](../.gitbook/assets/railing-along-path.gif)

## Avvio di Railing Along Path

* Accedere al pannello di Dynamo in FormIt per Windows e verificare di trovarsi nella directory Dynamo Samples.
* Fare clic sull'esempio Railing Along Path.
* Sul lato sinistro della schermata, verrà visualizzato il messaggio di richiesta Select path for railing.
   * È necessario selezionare solo una serie di bordi contigui o un gruppo contenente solo una serie di bordi.
   * Dopo aver selezionato il percorso, fare clic sul pulsante di fine o premere INVIO.
* Il pannello di Dynamo indicherà che è in corso l'elaborazione delle modifiche. Al termine, si disporrà di una ringhiera generata da Dynamo in un gruppo di FormIt, pronta per la modifica \(vedere qui sotto\).

## Iterazione locale

Dopo l'esecuzione di Railing Along Path, si noterà che i risultati sono impostati sui valori di default. Forse queste funzioni sono utili, ma è possibile personalizzare pesantemente la ringhiera in base alle esigenze specifiche.

All'esecuzione di Railing Along Path, viene creato un nuovo gruppo contenente i risultati. In FormIt viene selezionato automaticamente il gruppo e sono mostrate le opzioni disponibili per l'istanza di Railing Along Path.

È sempre possibile tornare alle proprietà di Railing Along Path selezionando il gruppo e passando al pannello Proprietà oppure modificando il gruppo che mostrerà automaticamente le proprietà.

![](../.gitbook/assets/railing-along-path-options.png)

### Railing Height

L'altezza totale della ringhiera. Utilizza le unità di FormIt correnti.

### Post Spacing

La spaziatura tra i montanti verticali principali. Utilizza le unità di FormIt correnti.

### Add Posts at Path Vertices?

Quando è **True**, i montanti verranno aggiunti in corrispondenza di ciascun vertice del percorso selezionato e il calcolo per il posizionamento del montante successivo viene reimpostato in quel punto.

Ad esempio, se è stata selezionata una serie di tre bordi, verrà visualizzato un montante in corrispondenza di ciascuno dei due punti interni. Ciò è utile se i vertici indicano un cambio di direzione \(ad esempio, quando si salgono le scale o si svoltano gli angoli\) in cui si presenterebbe naturalmente un montante.

Quando è **False**, i montanti verranno aggiunti solo lungo il percorso a partire da un'estremità e misurando la distanza lungo il percorso, ignorando i vertici lungo il percorso. Questa opzione è utile se è stato selezionato un arco, una spline o un cerchio, in cui i vertici non sono importanti e si desidera che vengano ignorati nella spaziatura dei montanti.

### Reverse Path Direction?

Quando si calcola il posizionamento dei montanti, la direzione del percorso scelto determinerà quale estremità del percorso inizierà la misurazione della spaziatura dei montanti.

Se la spaziatura dei montanti determina uno spazio residuo su un'estremità indesiderata del percorso, è possibile modificare questo valore in **True** per invertire la curva e avviare la misurazione della spaziatura dei montanti all'estremità opposta.

### Post Width e Post Depth

La dimensione \(in pianta\) dei profili rettangolari dei montanti verticali. Utilizza le unità di FormIt correnti.

### Handrail Width e Handrail Height

La dimensione \(in sezione\) del profilo del corrimano rettangolare. Utilizza le unità di FormIt correnti.

### Baluster Orientation

Se è True, le balaustre verranno orientate orizzontalmente, come i cavi. Se è False, le balaustre verranno orientate verticalmente per un aspetto estetico più tradizionale.

### Baluster Width e Baluster Depth

La dimensione del profilo rettangolare della balaustra. Utilizza le unità di FormIt correnti.

### Baluster Spacing

La quantità di spazio tra ogni balaustra. Utilizza le unità di FormIt correnti.

### Bottom Rail Start Height

La distanza tra la parte inferiore della ringhiera e la guida inferiore che supporta le balaustre. Utilizza le unità di FormIt correnti.

### Esegui

Dopo aver modificato le opzioni, fare clic sul pulsante Esegui per eseguire il grafico di Dynamo sottostante e generare nuovi risultati. Questo pulsante diventa blu quando i parametri sono stati modificati, pertanto è necessario fare clic per visualizzare gli aggiornamenti nella geometria finale.‌

### Edit Embedded Graph

Facendo clic su questa opzione si avvia l'ambiente dell'editor grafico di Dynamo, in modo che sia possibile visualizzare e modificare il grafico di Dynamo sottostante per modificare più rapidamente i parametri e visualizzare gli aggiornamenti dinamici o per esaminare/regolare la logica.

