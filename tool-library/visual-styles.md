# Stili di visualizzazione

È possibile personalizzare l'aspetto visivo del modello, inclusi l'illuminazione complessiva, gli stili dei bordi e gli effetti ambientali. Il pannello Stili visualizzazione è disponibile facendo clic sull'icona degli occhiali da sole sulla barra delle tavolozze:

![](../.gitbook/assets/20200307-visual-styles-icon.png)

Gli stili di visualizzazione [possono essere impostati per scena](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/visual-settings), in modo da poter salvare le impostazioni di stile preferite e applicarle ad altre scene.

## Superfici 

Consente di gestire il modo in cui le superfici vengono visualizzate e ombreggiate.

![](../.gitbook/assets/visual_styles%20%281%29.png)

**Luminosità ambiente** controlla la luminosità complessiva di tutti i materiali nella scena. Un valore pari a 100 indica che i materiali esposti alla luce verranno visualizzati con la massima luminosità, come definito nel colore o nella trame del materiale. I valori superiori a 100 sovraesporranno i materiali, ma potrebbero essere utili per i modelli di SketchUp che sembrano ancora scuri in FormIt. Il valore di default è 100.

**Contrasto ambiente** controlla il valore in base a cui risultano più scure le superfici all'ombra, se confrontate con quelle esposte alla luce diretta del sole. Un valore pari a 0 indica che l'illuminazione non ha effetto \(tutti i materiali verranno visualizzati in piena luminosità indipendentemente dall'orientamento\), mentre valori più elevati faranno apparire le superfici all'ombra sempre più scure. Il valore di default è 25.

Attivare/Disattivare **Ombre** per vedere come il progetto verrebbe [ombreggiato all'ora corrente del giorno](https://windows.help.formit.autodesk.com/tool-library/shadows).

**Intensità ombra** controlla il modo in cui le ombre scure vengono disegnate sul piano del terreno e su altre superfici. Un valore pari a 0 rende le ombre effettivamente invisibili e un valore pari a 100 rende nere le ombre. Il valore di default è 20.

**Ombre ambiente** consente di aggiungere un tocco di ombreggiatura agli angoli per aggiungere realismo al modello di FormIt.

**Superfici monocromatiche** disattiva il colore e la trama di tutti i materiali e rende bianco l'ambiente circostante. È utile per studi su ombre o ombreggiatura.

La sezione Colori superficie definisce i colori di default per le superfici quando non viene applicato alcun materiale.

**Superfici** è il colore di default di tutte le superfici di FormIt anteriori \(o entrambi i lati, se l'opzione Superfici posteriori è deselezionata\) quando non viene applicato alcun materiale.

**Superfici posteriori** consente di visualizzare materiali diversi su entrambi i lati di una singola superficie, per i modelli di SketchUp importati in FormIt e che richiedono tale funzionalità. Questa opzione è deselezionata per default, ma viene selezionata quando i modelli di SketchUp vengono aperti o importati. Nella geometria non di SketchUp, il colore di Superfici posteriori specificato viene visualizzato sui lati posteriori delle superfici.

Utilizzare le sezioni Effetti di taglio sezione ed Effetti scuri sezione per gestire i colori di default di superfici, linee e l'effetto scuro quando si utilizza lo strumento [Piano di sezione](section-planes.md).

## Piani del terreno

Quando l'opzione Piano del terreno è disattivata in modalità di modifica del gruppo, anche la griglia di Piano di lavoro blu è disattivata.

Il colore di Piano di lavoro può essere personalizzato anche dal gruppo Stili visualizzazione.

![](../.gitbook/assets/screen-shot-2020-03-30-at-1.30.16-pm.png)

## Bordi

Consente di gestire lo stile di visualizzazione di tutti i bordi del modello.

![](../.gitbook/assets/edges.PNG)

**Contrasto** influisce sulla visibilità di tutti i bordi. Un valore pari a 0 renderebbe i bordi effettivamente invisibili. Il valore di default è 60.

**Colore** influisce sul colore di tutti i bordi del modello. Il valore di default è il nero.

**Bordi spessi** rende tutti i bordi più spessi, inclusi i bordi delle silhouette.

**Bordi di schizzo** aggiunge un effetto di schizzo a tutti i bordi per simulare un effetto di disegno a mano.

**Bordi nascosti** visualizza i bordi altrimenti occlusi dalle superfici.

**Bordi estesi** aggiunge un'estensione ad alcuni bordi per simulare un effetto di disegno a mano.

## Ambiente

Consente di attivare/disattivare la visualizzazione degli effetti ambientali e degli oggetti di supporto.

![](../.gitbook/assets/environment.PNG)

**Griglia** controlla la visualizzazione della griglia sul piano del terreno, nonché la griglia mostrata durante la modifica di un gruppo. L'opzione Snap alla griglia verrà disattivata quando Griglia è disattivata.

**Assi** controlla la visualizzazione degli assi XYZ mostrati in corrispondenza dell'origine globale o dell'origine del gruppo se si modifica un gruppo.

**Livelli** controlla la visualizzazione dei [**livelli**](levels-and-area.md) ****impostati nel pannello Livelli.

**Nebbia** controlla la visualizzazione della nebbia disegnata per rendere fluida la transizione tra il piano del terreno e il cielo. Se si disattiva Nebbia, viene generata una linea orizzontale netta in cui il piano del terreno \(se attivato\) incontra il cielo.

**Freccia nord** controlla la visualizzazione di un piccolo widget grafico che indica la direzione del nord di progetto \(come determinato dalla posizione e dalle immagini satellitari\).

È possibile personalizzare anche i colori ambientali, quali il cielo, lo sfondo e il piano del terreno.

Il cielo è costituito da una sfumatura di colori **Inferiore/Sfondo**, **Centrale** e **Superiore**.

Se l'opzione **Cielo** è deselezionata, sarà visibile solo il colore **Inferiore/Sfondo**.

## Diagnostica modello

Attiva/Disattiva la visualizzazione degli strumenti diagnostici.

![](../.gitbook/assets/diagnostics.PNG)

**Identifica i problemi delle superfici a tenuta ermetica** evidenzia in rosso tutti i bordi che non fanno parte di un oggetto solido a tenuta ermetica.

**Identifica le superfici posteriori** evidenzia in rosso tutte le superfici rivolte in modo errato \(tutti gli oggetti solidi devono avere le superfici posteriori rivolte verso l'interno della forma del solido\).

[Ulteriori informazioni sull'utilizzo della diagnostica per le superfici a tenuta ermetica e posteriori per identificare e risolvere i problemi relativi ai modelli solidi](https://formit.autodesk.com/blog/post/repairing-solid-models).

