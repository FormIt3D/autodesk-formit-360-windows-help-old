# Snap e deduzioni

Per semplificare il disegno e la modellazione, utilizzare gli snap e i punti di deduzione per creare, posizionare e modificare la geometria in modo preciso. È possibile utilizzare qualsiasi asse scelto come l'asse su cui disegnare o eseguire un'altra azione, ad esempio l'estrusione di una superficie.

**Nota** _Per informazioni su come velocizzare l'utilizzo degli strumenti del software, vedere_ [_Tasti di scelta rapida_](../appendix/keyboard-shortcuts.md)_._

## Snap

Esistono diversi snap che possono essere utili durante il disegno e la modellazione. Lo snap ad oggetti viene attivato automaticamente ed è possibile eseguire lo snap a:

|                                                                                                                                                                            |                                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| Vertici | ![](<../.gitbook/assets/inf3 (3) (2).png>) |
| Bordi. Quando si posiziona il cursore sul bordo, verranno disegnati piccoli punti rossi in corrispondenza delle        estremità e del punto medio. | ![](../.gitbook/assets/inf4.png) |
| Punti medi del bordo | ![](../.gitbook/assets/inf5.png) |
| Il piano di una superficie. Quando si posiziona il cursore sulla superficie, verrà disegnato un piccolo punto rosso
        in corrispondenza del centroide della superficie. In questo modo sarà più semplice trovare il punto,
        se si desidera eseguire lo snap. | ![](../.gitbook/assets/inf6.png) |
| Centroidi della superficie | ![](../.gitbook/assets/inf7.png) |
| Il piano di lavoro, se non si esegue lo snap ad altri elementi. | ![](../.gitbook/assets/inf8.png) |
| Centri del cerchio o dell'arco | ![](../.gitbook/assets/inf9.png) |
| Vertici della mesh | ![](../.gitbook/assets/inf2.png) |
| Il piano di una sfaccettatura della mesh. | ![](../.gitbook/assets/inf1.png) |

Per eseguire lo snap alla griglia, è necessario attivare il pulsante di commutazione **Snap alla griglia (SG)** dal menu Impostazioni.

## Assi e punti di deduzione

La selezione automatica dei punti di deduzione è sempre attivata e consentirà di vincolare il movimento della geometria. Gli assi di deduzione vengono generati automaticamente dagli strumenti o quando si posiziona il cursore del mouse su bordi o punti. Gli assi di deduzione vengono sempre disegnati sulla schermata con trattini in modo da sapere dove si trovano e sia facile eseguire lo snap.

**Asse:** è possibile spostare la geometria lungo l'asse X, Y o Z. L'asse X è rosso, l'asse Y è verde e l'asse Z è blu.

![](../.gitbook/assets/inf10.png)

**Blocco dell'asse:** è possibile bloccare il movimento lungo l'asse X, Y o Z. Tenere premuto il tasto MAIUSC mentre si lavora sulla deduzione di un asse, quindi spostare il mouse per eseguire lo snap e la deduzione ad altri elementi.

![](../.gitbook/assets/inf13.png)

**Parallelo:** è possibile disegnare o spostare la geometria parallelamente agli elementi esistenti. Le deduzioni perpendicolari sono viola. È necessario posizionare il cursore su una linea che si desidera utilizzare come riferimento parallelo.

![](../.gitbook/assets/inf14.png)

**Perpendicolare:** è inoltre possibile disegnare o spostare la geometria perpendicolarmente agli elementi esistenti. Le deduzioni perpendicolari sono viola. È necessario posizionare il cursore su una linea che si desidera utilizzare come riferimento perpendicolare.

![](../.gitbook/assets/inf15.png)

**Estensione da un punto:** è anche possibile utilizzare le deduzioni per l'estensione dal riferimento di un punto. Posizionare il cursore del mouse su un punto che si desidera utilizzare come riferimento fino a quando non viene visualizzata la descrizione comando, quindi utilizzare l'asse di deduzione che si estende dal punto.

![](../.gitbook/assets/inf16.png)

**Centro del cerchio**: se si desidera eseguire lo snap al centro di un arco o di un cerchio, posizionare il cursore sull'arco o sul cerchio. Verrà mostrato un piccolo punto rosso al centro. Rimarrà visibile per circa 5 secondi dopo che si allontana il cursore dall'arco o dal cerchio. Ora spostare il cursore sul punto rosso per eseguire lo snap al centro.

![](../.gitbook/assets/inf17.png)

**Punti medi di archi e spline reali**: quando si posiziona il cursore su un cerchio, un arco o una spline, sarà possibile eseguire lo snap al punto medio reale. Il punto medio e i punti finali verranno mostrati da un piccolo punto rosso. In caso di deduzione su un arco, si eseguirà anche lo snap ai vertici dei bordi diritti che rappresentano l'arco.

![](../.gitbook/assets/inf18.png)

**Cancellazione delle deduzioni**: è possibile che il disegno generi un numero maggiore di deduzioni, che potrebbero posizionare punti che non dovrebbero eseguire lo snap a tali deduzioni. Se si premono i tasti **MAIUSC + BARRA SPAZIATRICE**, tutte le deduzioni verranno cancellate, ad eccezione di quelle dell'ultimo punto posizionato.

![Prima di cancellare le deduzioni](../.gitbook/assets/inf19.png)

![Dopo aver cancellato le deduzioni](../.gitbook/assets/inf20.png)
