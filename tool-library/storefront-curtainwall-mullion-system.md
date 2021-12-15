# Sistemi di montanti di facciata continua/facciata del negozio

![](../.gitbook/assets/dynamo-storefront-system-options.gif)

## Con tecnologia di Dynamo

La capacità di creare rapidamente sistemi di montanti di facciata continua/facciata del negozio in FormIt è con tecnologia di Dynamo. È possibile trovare il sistema Storefront Curtainwall nella directory Dynamo Samples nel pannello di Dynamo:

![](../.gitbook/assets/storefront-curtainwall-button%20%281%29.png)

## Selezione di "vetro" per il sistema di montanti

A partire da FormIt 2021.2, il sistema Storefront Curtainwall utilizza il nuovo [nodo SelectFromFormIt](https://formit.autodesk.com/page/formit-dynamo#dynamo-formit-nodes), che consente di selezionare un pezzo di "vetro" \(una superficie singola o un solido estruso\) attorno al quale generare un sistema di montanti.

![Un semplice piano di &quot;vetro&quot; con un'apertura per le porte nella parte inferiore.](../.gitbook/assets/storefron-system-1_glass-only.png)

Quando si fa clic sulla miniatura Storefront Curtainwall \(notare l'icona che indica che è necessaria una selezione\), in FormIt verrà richiesto di selezionare la geometria del vetro per continuare:

![](../.gitbook/assets/storefront-curtainwall-prompt.png)

Ecco alcune note e avvertenze sul funzionamento della selezione del vetro:

* Attualmente, sono supportate solo le superfici piane. Se si seleziona una serie di superfici \(ad esempio, una superficie "curva" composta da superfici piane più piccole\), lo script troverà la superficie piana più grande e la utilizzerà.
* Se il vetro è solido, ovvero una singola superficie estrusa molto leggermente per fornire un po' di spessore, lo script troverà la superficie più grande, in modo che i montanti risultanti vengano generati su un lato del solido in vetro.
* È possibile disegnare aperture per le porte e rimuovere la superficie risultante dal contorno del vetro. I montanti risultanti rispetteranno l'apertura della porta, lasciandola vuota per l'aggiunta di porte.
* A causa delle limitazioni di Dynamo, questo script non funziona se la geometria del vetro presenta aperture al centro.

## Suggerimenti

Quando si seleziona la geometria per un grafico di Dynamo in FormIt, alcuni trucchi organizzativi possono semplificare l'esperienza e consentire una facile creazione di istanze dei risultati:

* Inserire il vetro in un gruppo e utilizzare il gruppo come selezione per lo script di Storefront Curtainwall. In questo modo, è più semplice modificare il profilo del vetro dopo la generazione dei montanti e, se il vetro viene notevolmente modificato tra le esecuzione e gli ID superficie sono stati modificati, il gruppo garantisce che lo script troverà sempre il vetro, poiché utilizza l'ID gruppo e non l'ID superficie.
* Se si prevede di copiare e incollare i risultati del sistema di montanti in altre posizioni del modello, è preferibile disporre del vetro e dei montanti risultanti contenuti in un gruppo. In questo modo si evitano inoltre problemi con il nodo di selezione nel caso in cui non si conosca l'istanza del vetro da utilizzare quando viene copiato e incollato solo il gruppo di montanti risultante.
   * Inserire prima il vetro in un gruppo. Fare doppio clic per selezionare il vetro e premere G o utilizzare i comandi Gruppo nel menu contestuale o sulla barra degli strumenti.
   * Selezionare il gruppo risultante e inserirlo in un altro gruppo.
   * Fare doppio clic per accedere al primo gruppo. Questo è il "contenitore" sia per il vetro che per i montanti risultanti.
   * Fare clic sulla miniatura Storefront Curtainwall e utilizzare il gruppo del vetro come selezione.
   * Dopo l'esecuzione dello script, è possibile uscire dal gruppo e copiare/incollare il contenitore in base alle esigenze. È possibile modificare una qualsiasi delle istanze \(regolando la forma o i parametri del vetro\) senza problemi.

## Opzioni del sistema di montanti

Dopo aver selezionato il vetro ed eseguito lo script, si otterrà un risultato nell'area di disegno di FormIt, sotto forma di un gruppo di FormIt. Questo gruppo verrà selezionato automaticamente e nel pannello Proprietà verranno mostrate le opzioni disponibili.

![](../.gitbook/assets/storefront-curtainwall-parameters.png)

* **Esegui**: se si modifica la forma del vetro e si desidera eseguire nuovamente il grafico per aggiornare i risultati dei montanti, fare clic su questo pulsante.
* **Edit Embedded Graph**: consente di modificare lo script di Dynamo che sta generando la geometria. Questo script è incorporato nel file di FormIt ed è specifico per questo gruppo.
* **Select Glass \(Surface or Solid\)**: fare clic su questa opzione per aggiornare la selezione ad un altro pezzo di vetro attorno al quale generare i montanti.

Lo script utilizzerà i valori di default per la prima esecuzione, pertanto sarà possibile regolarli in base al caso di utilizzo univoco. Tutti i valori utilizzeranno le unità di FormIt correnti.

* **Mullion Width e Mullion Depth**: la larghezza e la profondità di tutti gli elementi del montante.
* **Vertical Mullion Spacing**: la distanza, al centro, tra i montanti verticali.
* **Flip Vertical Mullion Layout?**: lo script avvia la spaziatura dei montanti verticali da un lato, scelta arbitrariamente. Se il risultato avvia la spaziatura dei montanti sul lato errato per il caso di utilizzo, impostare questa opzione su True per invertire il layout in modo che inizi sul lato opposto.
* **Center Vertical mullion Layout?**: anziché avviare il calcolo della spaziatura dei montanti verticali in corrispondenza di un'estremità del vetro, avviare il calcolo al centro, creando un layout simmetrico di montanti verticali.
* **First Horizontal Mullion Spacing**: imposta la spaziatura dei primi montanti orizzontali dalla parte inferiore. È utile se è necessaria una fila di moduli di vetrate più corti nella parte inferiore, separati dal resto della spaziatura dei montanti orizzontali.
* **Horizontal Mullion Spacing**: la spaziatura tipica dei montanti orizzontali al centro, a partire dal primo montante come descritto in precedenza.
* **Flip Horizontal Mullion Layout?**: se si desidera che il layout dei montanti orizzontali inizi nella parte superiore anziché in quella inferiore, impostare questa opzione su True.
* **Center Horizontal Mullion Layout?**: anziché avviare il calcolo della spaziatura dei montanti orizzontali nella parte inferiore o superiore del vetro, avviare il calcolo al centro, creando un layout simmetrico di montanti orizzontali.

## Opzioni nascoste

Se si desidera una maggiore personalizzazione, diverse opzioni avanzate sono nascoste dal pannello Proprietà di FormIt, ma sono accessibili facendo clic su Edit Embedded Graph per visualizzare l'intero contenuto del grafico in Dynamo:

![](../.gitbook/assets/dynamo-edit-embedded-graph.png)

### Montanti casuali

![](../.gitbook/assets/storefront-curtainwall-random-verticals.png)

* **Randomize Vertical and Horizontal Mullion Layout?**: impostare questa opzione su True per spaziare i montanti verticali o orizzontali in modo casuale.
* **Min./Max. Vert. Spacing \(if random\)**: regolare questi valori per impostare un intervallo di valori di spaziatura minimi e massimi casuali.

### Montanti sul bordo

![](../.gitbook/assets/storefront-curtainwall-border-mullion-options.png)

* **Flip Offset Direction of Border Mullions?**: per default, il sistema di montanti utilizzerà il contorno del vetro e ne eseguirà l'offset verso l'interno per creare i montanti sul bordo. Per eseguire l'offset verso l'esterno, impostare questa opzione su True. In questo modo, la dimensione complessiva del sistema di montanti all'esterno del contorno del vetro verrà aumentata mediante l'impostazione Mullion Width.
* **Add Tolerance Between Selection and Border Mullions?**: per default, il sistema di montanti viene generato esattamente sul bordo del vetro, il che potrebbe causare lo Z-fighting nel punto in cui il bordo del vetro e le superfici esterne dei montanti sul bordo collidono. Nella maggior parte dei casi, questa opzione non sarà visibile, ma se il caso di utilizzo richiede che i bordi del sistema siano visibili e si desidera evitare lo Z-fighting, attivare questa opzione e regolare il valore di tolleranza in base alle esigenze.

