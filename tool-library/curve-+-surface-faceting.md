# Sfaccettatura di curve e superfici

FormIt è un sistema di modellazione poliedrica, pertanto oggetti quali cerchi, archi e spline sono rappresentati da una serie di bordi diritti. Analogamente, una superficie curva come il muro di un cilindro, o una cupola, è costituita da una serie di superfici piane con bordi nascosti.

Per default, FormIt utilizza 40 bordi, o sfaccettature, per rappresentare un cerchio e 24 sfaccettature per rappresentare un oggetto curvo 3D, come un cilindro. Per superfici più complesse, ad esempio una cupola, un valore pari a 24 imposta il conteggio delle sfaccettature del perimetro e influisce anche sulla densità di sfaccettatura del resto della forma.

In FormIt per Windows v18 e versioni successive, i valori di sfaccettatura della curva e della superficie sono personalizzabili:

![](../.gitbook/assets/faceting\_planter.gif)

![](<../.gitbook/assets/faceting (1).png>)

**Curve Faceting Quality**

La modifica di Curve Faceting Quality influirà sul numero di sfaccettature utilizzate per il disegno di nuovi cerchi e archi in FormIt, nonché sul posizionamento di forme primitive. Ad esempio, se si imposta questa opzione su 64, si creerebbe un cerchio completo a 64 lati o un arco a quarto di cerchio con 16 sfaccettature.

Questo valore influirà anche sulla qualità dei cerchi e degli archi importati dai file SAT e quando si esegue il baking della geometria da Dynamo. È possibile impostare questo valore per i nuovi disegni o solo per il disegno corrente.

Per le curve esistenti, è anche possibile utilizzare il plug-in Rebuild Curve per ricreare in modo retroattivo un arco o un cerchio **esistente** con un nuovo numero di sfaccettature:

![](../.gitbook/assets/screen-shot-2020-01-10-at-1.20.53-pm.png)

![](../.gitbook/assets/faceting\_rebuild-curve.gif)

**Surface Faceting Quality**

La modifica di questa impostazione globale influirà sulla qualità delle superfici curve 3D importate da file SAT e quando si esegue il baking da Dynamo.

Ad esempio, impostando questa opzione su 64, quindi eseguendo il baking di una sfera da Dynamo verranno utilizzate 64 superfici attorno all'equatore della sfera, più 64 sfaccettature in ciascuno degli anelli che vanno ai poli della sfera, che si aggiungono rapidamente. Utilizzare valori più elevati con cautela, poiché in alcuni casi possono influire sulle prestazioni di FormIt. Una volta ottenuto un risultato di alta qualità, è possibile [convertirlo in una mesh](meshes.md) per migliorare le prestazioni.

Quando si utilizza Dynamo, è possibile modificare la qualità delle sfaccettature e fare clic su Run Graph nel pannello Proprietà senza modificare i parametri, per sfruttare i nuovi conteggi di sfaccettature:

![](../.gitbook/assets/faceting\_column.gif)

Come per le curve, è possibile impostare la qualità delle sfaccettature delle superfici per i nuovi disegni o solo per il disegno corrente.

Tenere presente che i valori di sfaccettatura sono attualmente limitati a multipli di 4, pertanto quando si immettono numeri manualmente, in FormIt vengono arrotondati al multiplo più vicino. È possibile utilizzare i dispositivi di scorrimento e le frecce per scorrere i valori accettati.

![](../.gitbook/assets/units-+-precision.png)
