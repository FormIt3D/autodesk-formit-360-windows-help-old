# Gestione operazioni annullate

FormIt include un sistema Annulla/Ripeti univoco che può essere utilizzato in due modi diversi per annullare l'operazione per gruppo o in modo cronologico e globale:

* L'opzione Annulla/Ripeti durante la modifica di un gruppo nidificato avrà effetto solo sulle modifiche all'interno di tale gruppo.
   * Ciò significa che è possibile apportare una modifica a questo gruppo, quindi apportare molte modifiche in altri gruppi, tornare al gruppo originale e avere la possibilità di annullare l'ultima modifica apportata a questo gruppo senza influenzare le modifiche eseguite più recentemente, in altre posizioni.
* Annulla/Ripeti nel disegno principale \(non durante la modifica di un gruppo\) funziona come i tradizionali sistemi Annulla/Ripeti: l'ultima modifica apportata in **qualsiasi** gruppo verrà annullata in base all'ordine cronologico.

Gestione operazioni annullate registra ogni modifica all'interno di ogni gruppo nel modello di FormIt, incluse le modifiche apportate nel disegno principale. Questa opzione è utile per comprendere visivamente quali operazioni sono state annullate in qualsiasi gruppo nel modello.

![](../.gitbook/assets/undo-manager.png)

Gestione operazioni annullate indicherà in **grassetto** lo stato corrente, nonché eventuali operazioni precedenti a questo stato ed eventuali operazioni una volta esistenti ma che sono state annullate.

È possibile fare clic con il pulsante destro del mouse su uno stato e selezionare Riporta a per annullare o ripetere correttamente le operazioni necessarie per tornare a tale stato del modello.

I gruppi eliminati esplicitamente o che non sono più presenti a causa di un comando Annulla o Ripeti vengono mostrati come \*Non attivo\*. È possibile ripristinarli annullando o ripetendo le operazioni all'interno del gruppo principale fino a quando non sono recuperati.

