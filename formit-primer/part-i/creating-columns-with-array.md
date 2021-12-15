# 1.8 - Creazione di pilastri con matrice

_In questo esercizio, disegneremo un elemento dettagliato, una colonna con trave a I. Quindi utilizzeremo lo strumento Matrice per creare rapidamente più copie con spaziatura uniforme._

_Se non è stata completata l'ultima sezione, scaricare e aprire il file_ _**1.8 - Create Columns with Array.axm**_ _dai_ _**set di dati della Parte I della Guida introduttiva di FormIt**._

## **Disegno del profilo del pilastro**

1 - Per facilitare la procedura di disegno:

1. Accedere a **Vista dall'alto \(VT\)**.
2. Passare alla modalità della vista **Ortogonale \(VO\)**.
3. Disattivare i layer **Main Building** **Floor** e **Roof**. Con questo passaggio si impedirà che la nuova geometria esegua lo snap alla geometria esistente su tali layer.
4. Eseguire lo zoom avanti nell'angolo superiore sinistro dell'immagine della **pianta del pavimento importata** in modo da poter visualizzare il pilastro in dettaglio.
5. Disattivare la funzionalità **Snap a griglia \(SG\)** \(se è stata attivata\). In questo modo, sarà possibile disegnare le linee di dettaglio.

![](../../.gitbook/assets/0%20%2813%29.png)

_Per disegnare il pilastro, disegneremo prima una metà, quindi eseguiremo una copia speculare per creare rapidamente l'altra metà simmetrica._

2 - Per creare la prima metà della trave a I, utilizzare lo **strumento Linea \(L\)** per creare il seguente disegno utilizzando le quote specificate. Non importa per il momento la posizione esatta del pilastro sull'immagine di pianta.

![](../../.gitbook/assets/1%20%2818%29.png)

3 - Per creare una copia speculare della forma appena disegnata:

1. Fare doppio clic per selezionare tutte le superfici e i bordi della geometria disegnata.
2. Fare clic con il pulsante destro del mouse e selezionare lo **strumento Copia speculare \(MI\)**.
3. Fare clic sul grip arancione centrale del **widget Copia speculare** e posizionarlo nell'angolo inferiore sinistro della geometria.
4. Utilizzare la freccia inferiore del pulsante a doppia freccia nel widget per ruotare l'asse della copia speculare di -90 gradi \(senso orario\).
5. Fare clic una sola volta nello spazio o premere **ESC** per completare la procedura di copia speculare. Il risultato dovrebbe essere simile ad un profilo con trave a I con una linea fino al centro. Premere nuovamente **ESC** per annullare la selezione.

![](../../.gitbook/assets/2%20%285%29.png)

![](../../.gitbook/assets/3%20%287%29.png)

_**Nota** La posizione e l'orientamento della geometria finali vengono visualizzati in anteprima con la forma semitrasparente blu durante la regolazione del widget Copia speculare. È possibile utilizzare questa anteprima come riferimento per creare la copia speculare della geometria nella posizione desiderata._

4 - Per unire entrambi i lati in un'unica geometria, rimuovere la linea che li divide facendovi clic per selezionarla e quindi premendo **Elimina**. Ora le due superfici sono unite in una singola superficie.

5 - Per spostare la geometria nella posizione finale:

1. Se disattivati, attivare i layer **Plan Image** e **Roof** per utilizzarli come guida.
2. Fare doppio clic sul profilo del pilastro per selezionarne la superficie e tutte le linee. Iniziare a spostare la selezione lungo l'asse verde \(**Asse Y**\). Tenere premuto **MAIUSC** e spostare il profilo fino a quando non si allinea con il tetto, quindi fare clic per posizionarlo.
3. Analogamente al passaggio precedente, spostare nuovamente la geometria, questa volta bloccandola sull'asse rosso \(**Asse X**\).
4. Fare clic per posizionarlo sopra la trave ad I disegnata in **Plan Image**. Guardando meglio da vicino, come nell'immagine seguente, la posizione orizzontale non deve essere perfetta. 

_**Nota**_ _Il tasto_ _**MAIUSC**_ _blocca la geometria per spostarsi lungo un solo asse, in questo caso quello verde \(**Asse Y**\). In questo modo, il profilo del pilastro non si sposta accidentalmente verso l'alto e non si allinea alla parte superiore del piano del tetto._

![](../../.gitbook/assets/4%20%289%29.png)

## **Estrusione e creazione della matrice del pilastro**

1 - Per facilitare la successiva procedura di disegno, ripristinare la modalità della vista **Prospettica \(VP\)** ed eseguire **Orbita \(O\)** per posizionare la cinepresa in modo da visualizzare il profilo con trave a I da nord-ovest. Utilizzare la freccia a nord nell'angolo inferiore sinistro per posizionare la vista.

![](../../.gitbook/assets/5%20%281%29.jpeg)

_**Nota**_ _Per informazioni su come spostarsi all'interno del disegno, è consigliabile consultare il capitolo_ _**Navigazione nella scena**_ _._

2 - Selezionare la superficie del profilo del pilastro ed estrudere la superficie fino a **17'-8"**.

_**Nota**_ _Se durante lo spostamento del profilo del pilastro, la superficie viene allineata al tetto, estruderla verso il basso di_ _**17'-8"**   anziché verso l'alto._

3 - Eseguire lo zoom indietro e attivare il layer **Roof** \(se disattivato\). La parte superiore del pilastro deve essere allineata alla parte superiore del tetto.

![](../../.gitbook/assets/6%20%289%29.png)

4 - Per mantenere organizzato e ordinato il modello, selezionare nuovamente la geometria del pilastro ed effettuare le seguenti operazioni:

1. Selezionare **Gruppo \(G\)** e denominarlo **Column Tall**.
2. Creare un nuovo **Layer** denominato **Column** e aggiungervi il gruppo.
3. Importare il materiale **Metal - Brushed - Colorized** e dipingere il gruppo.

![](../../.gitbook/assets/7%20%284%29.png)

_**Nota**_ _Per ulteriori informazioni su_ _**gruppi**,_ _**layer** e_ _**materiali**, vedere i capitoli precedenti._

4 - Fare clic su **ESC** per deselezionare lo strumento del pennello.

## **Creazione della matrice di pilastri**

1 - Accedere a **Vista dall'alto \(VT\)** e impostare nuovamente la modalità della cinepresa su **Ortogonale \(VO\)**.

2 - Disattivare il layer **Roof**.

3 - Per avviare la procedura di creazione della matrice:

1. Fare clic una sola volta per selezionare il gruppo di pilastri. Fare clic con il pulsante destro del mouse per visualizzare il **menu contestuale** e scegliere **Matrice \(AR\)**.
2. Nella finestra di dialogo **Proprietà matrice**, utilizzare le seguenti impostazioni:
   * **Lunghezza tra le copie**
   * **Lineare** \(default\)
   * **Raggruppa ogni solido, poi crea la matrice** \(default\)
   * **Numero di copie: 3**
   * Premere **OK** per chiudere la finestra di dialogo.

![](../../.gitbook/assets/8%20%283%29.png)

4 - Per posizionare i nuovi elementi:

1. Fare clic una sola volta sul pilastro per avviare **Matrice**. Spostare il cursore lungo l'asse rosso \(**Asse X**\).
2. Impostare la quota su **22'**. Ora sono presenti **quattro** pilastri distanziati a **22'**.
3. Premere **ESC** per annullare la selezione.

![](../../.gitbook/assets/9%20%286%29.png)

5 - Per selezionare tutti i gruppi **Tall Column** contemporaneamente, posizionare il cursore del mouse su uno di essi e premere una volta il tasto **TAB**. Notare che sono stati evidenziati tutti i riquadri di delimitazione dei 4 pilastri. Fare clic una sola volta sul pilastro su cui si trova il cursore del mouse e verranno selezionati tutti. Questo è un modo rapido per selezionare contemporaneamente tutte le istanze dello stesso gruppo.

6 - Eseguire un'altra volta **Matrice \(AR\)** per creare i pilastri sull'altro lato dell'edificio. Questa volta creare 1 copia lungo l'asse verde dell'edificio. Impostare la quota su **29'- 4 5/8".**

_**Nota**_ _29' 4 5/8" = 8 5/8" \(profondità del pilastro\) + 28'-8" \(larghezza dell'edificio principale\)._

7 - Per visualizzare l'intero edificio, accedere a **Vista 3D \(V3\)** e impostarla su **Prospettica \(VP\)**. Se disattivati, attivare i layer **Main Building Floor**, **Roof**, **Lower Terrace** e **Column**.

![](../../.gitbook/assets/10%20%287%29.png)

## **Creazione di pilastri della terrazza**

_Ora duplicheremo i pilastri dell'edificio principale per creare versioni simili, ma più corte, per la terrazza._

1 - Per semplificare il disegno, consigliamo di tornare alle impostazioni **Ortogonale \(OV\)** e **Vista dall'alto \(VT\)**.

2 - Per creare i nuovi pilastri:

1. Tenere premuto **CTRL** o **MAIUSC** e fare clic sui 3 pilastri più vicini a **Lower Terrace Floor** per selezionarli.
2. Fare clic una sola volta su uno qualsiasi dei pilastri per iniziare a spostare contemporaneamente tutti e 3 i pilastri selezionati. Premere una volta il tasto **CTRL** per creare una **copia rapida**. Verrà visualizzata un'anteprima semitrasparente della copia.
3. Spostare le copie verso il basso lungo l'asse verde \(**Asse Y**\) di **23'-4 3/8**". Premere **ESC**.
4. Senza deselezionarli, spostare i pilastri copiati lungo l'asse rosso \(**Asse X**\) di **22'** per collocarli nella posizione finale.
5. Nuovamente, con i 3 nuovi pilastri ancora selezionati, fare clic con il pulsante destro del mouse su uno dei pilastri copiati e selezionare **Rendi univoco \(MU\)**. Questi pilastri sono ora associati tra loro, ma univoci rispetto agli originali.

_**Nota**_ _Tenendo premuto_ _**MAIUSC**_ _o_ _**CTRL**_ _è possibile selezionare più elementi contemporaneamente o rimuovere elementi dalla selezione corrente._

![](../../.gitbook/assets/11%20%287%29.png)

3 - Modificare il nuovo gruppo di pilastri:

1. Fare doppio clic per modificare uno dei nuovi gruppi e rinominarlo **Column Short.**
2. Regolare l'altezza del nuovo pilastro per allinearlo alla parte superiore di **Lower Terrace** **Floor** \(3'-2"\). A tale scopo, selezionare e trascinare la superficie del pilastro verso il basso lungo l'asse blu \(**Asse Z**\) e tenere premuto **MAIUSC**. Posizionare il cursore in un punto qualsiasi della superficie superiore di **Lower Terrace Floor** e l'altezza del pilastro verrà allineata automaticamente alla terrazza inferiore. Una volta impostata l'altezza, fare clic per terminare.

![](../../.gitbook/assets/12%20%284%29.png)

_**Nota**_ _È possibile controllare l'altezza dei pilastri corti utilizzando lo strumento_ _**Misura \(ME\)**_ _. In alternativa, è possibile selezionare uno dei bordi verticali del pilastro e visualizzarne la lunghezza nella_ _**tavolozza Proprietà**._

4 - Utilizzando le tecniche appena apprese, copiare il pilastro corto più lontano sul lato opposto di **Lower Terrace Floor** per creare l'ultimo pilastro rimanente.

![](../../.gitbook/assets/13%20%284%29.png)

