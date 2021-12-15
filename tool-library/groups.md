# Gruppi

Una delle tecniche essenziali ma più importanti nei workflow di FormIt prevede il raggruppamento. I gruppi consentono di evitare che la geometria aderisca e di impostare relazioni padre/figlio tra gli elementi copiati in modo che, se si aggiorna un elemento, vengano aggiornati entrambi gli elementi. Ulteriori informazioni sui gruppi sono disponibili [qui](../formit-primer/part-i/grouping-objects.md).

I gruppi possono essere creati e modificati in due modi: dal menu contestuale di un gruppo selezionato o dalla barra degli strumenti principale.

## Interazioni tra gruppi

Per **creare un gruppo**, selezionare gli elementi che si desidera raggruppare, che possono includere bordi, superfici, solidi o altri gruppi, e fare clic con il pulsante destro del mouse. Scegliere lo strumento **Gruppo \(G\)** dal menu contestuale. Le immagini importate e le immagini satellitari non possono essere raggruppate.

Per **selezionare un gruppo**, fare un singolo clic sul gruppo. Notare le linee tratteggiate visualizzate quando si seleziona un gruppo. Queste linee indicano la dimensione totale del gruppo.

Per **modificare un gruppo**, fare doppio clic. Viene avviata una modalità di modifica in cui è possibile solo visualizzare ed eseguire lo snap agli elementi esterni al gruppo corrente, ma non selezionarli. È inoltre possibile nascondere gli elementi esterni al gruppo corrente utilizzando il tasto di scelta rapida **H**.

È possibile creare **gruppi all'interno di gruppi:** questi sono denominati **gruppi nidificati** e possono essere creati all'interno della modalità di modifica del gruppo. Per spostarsi verso l'alto di un livello nei gruppi nidificati, fare clic in un punto qualsiasi al di fuori dei gruppi.

Per **uscire dalla modalità di modifica del gruppo**, fare doppio clic in un punto qualsiasi al di fuori del gruppo.

È possibile **copiare un gruppo** per creare una relazione tra il gruppo originale e la relativa copia: se si modificano eventuali gruppi copiati, le stesse modifiche avranno effetto su tutti i gruppi correlati.

Per **interrompere la relazione tra i gruppi copiati**, selezionare il gruppo o i gruppi che si desidera impostare come separati, fare clic con il pulsante destro del mouse e scegliere **Rendi univoco** dal menu contestuale. È inoltre possibile selezionare Rendi univoco dalla barra degli strumenti Gruppi.

Per **selezionare tutti i gruppi correlati**, posizionare il cursore su un gruppo e premere il tasto TAB. Quando tutti i gruppi correlati vengono evidenziati, fare clic sui gruppi per selezionarli. È quindi possibile eseguire un'azione su tutti i gruppi contemporaneamente.

[**Struttura gruppi**](groups-tree.md) fornisce un'unica posizione per visualizzare e gestire tutti i gruppi in un progetto.

## Menu contestuale Gruppi e accesso alla barra degli strumenti

## ![](../.gitbook/assets/grouptoolbar.png)

**Raggruppamento di elementi**

Per creare un gruppo dalla voce della barra degli strumenti Gruppi, selezionare uno o più elementi, l'icona **Crea gruppo**, quindi l'icona **Fine**. In alternativa, è possibile selezionare **Crea gruppo** dalla voce della barra degli strumenti Gruppi, quindi scegliere gli elementi che si desidera raggruppare e infine l'icona **Fine**.

Per **modificare un gruppo dalla voce della barra degli strumenti Gruppi**, selezionare l'icona **Modifica gruppo**, quindi fare clic sul gruppo che si desidera modificare. Al termine delle modifiche, selezionare l'icona **Fine**. Questo strumento consente di scegliere il gruppo specifico che si desidera modificare, anche se è nidificato in profondità.

**Per rendere univoco un gruppo dalla barra degli strumenti,** selezionare l'icona **Rendi univoco** nella voce della barra degli strumenti Gruppi. Inoltre, è possibile selezionare **Rendi univoco** dalla voce della barra degli strumenti Gruppi, quindi scegliere il gruppo che si desidera rendere univoco e fare clic sull'icona **Fine**.

**Per scomporre un gruppo dalla voce della barra degli strumenti Gruppi,** selezionare il gruppo che si desidera modificare e scegliere l'icona **Scomponi** dal menu della barra degli strumenti Gruppi. In questo modo si scompone la selezione corrente, ma non si scompongono eventuali gruppi nidificati. In alternativa, è possibile selezionare **Scomponi** dalla barra degli strumenti, selezionare il gruppo che si desidera modificare, quindi scegliere l'icona **Fine**.

**Per scomporre tutti i gruppi nidificati sotto il gruppo attualmente selezionato,** selezionare un gruppo con gruppi nidificati e scegliere **Scomponi tutto** dalla barra degli strumenti Gruppi.

**Per scomporre tutti i gruppi nel modello,** selezionare lo strumento **Scomponi tutto** dalla barra degli strumenti Gruppi.

## Gruppi e Revit

Se si conoscono bene le **famiglie** di Revit, si avrà familiarità con il concetto di gruppi in FormIt. I gruppi di FormIt dispongono di funzionalità che è possibile utilizzare per trasferirli in modo intelligente in Revit.

**Categorie di gruppi di FormIt**

È possibile specificare le **categorie** per i gruppi in FormIt in modo che i gruppi di FormIt diventino famiglie delle stesse categorie durante l'importazione in Revit. È possibile assegnare categorie ai gruppi di FormIt selezionando un gruppo, attivando la modalità di **modifica del gruppo** e utilizzando il pannello **Proprietà** per scegliere le categorie. È inoltre possibile assegnare categorie nel gruppo **Struttura gruppi**.

**Nomi dei gruppi di FormIt**

È inoltre possibile utilizzare il pannello **Proprietà** per specificare un nome per il gruppo di FormIt. Ciò può essere utile per navigare nel modello e, quando si importa il modello in Revit, è possibile filtrare facilmente gli elementi utilizzando il nome del gruppo.

Notare che **i gruppi nidificati in FormIt non vengono importati in Revit come gruppi nidificati**. In questo modo si evitano le famiglie di Revit nidificate in profondità.

