# 1.9 - Aggiunta di dettagli

_FormIt è un ottimo strumento per le volumetrie, oltre a essere un eccellente strumento di modellazione. Cominceremo ad aggiungere dettagli a Casa Farnsworth sotto forma di porte e montanti per il parallelepipedo in vetro. Successivamente, tratteremo alcuni strumenti aggiuntivi ed eseguiremo la procedura di aggiunta di nuova geometria, layer, materiali e gestione di gruppi._

_Se non è stata completata l'ultima sezione, scaricare e aprire il file_ _**1.9 - Add Details.axm**_ _dai_ _**set di dati della Parte I della Guida introduttiva di FormIt**._

## **Creazione di telai di finestre**

_Creeremo un telaio in metallo da 2" e montanti attorno al parallelepipedo in vetro. Questi montanti si sovrappongono intenzionalmente con il parallelepipedo in vetro._

1 - Creare un nuovo layer denominato **Glass Walls** e spostarvi il gruppo **Glass Wall**.

2 - Per facilitare la visualizzazione, disattivare il layer **Roof** in modo da poter visualizzare l'intero parallelepipedo in vetro.

3 - Per iniziare a creare il primo telaio della finestra:

1. Sul lato occidentale dell'edificio, utilizzare lo **strumento Rettangolo \(R\)** per disegnare una nuova superficie direttamente sulla superficie esterna in vetro. Assicurarsi di creare la superficie all'esterno del gruppo **Glass Walls**.
2. Selezionare e trascinare la superficie appena creata **2"** verso l'interno. Premere **ESC** per annullare la selezione. Il risultato finale dovrebbe essere simile a quello mostrato nell'immagine riportata di seguito.
3. Fare clic una sola volta sulla superficie appena creata. Fare clic con il pulsante destro del mouse per accedere al **menu contestuale** e utilizzare lo **strumento Offset superficie \(OF\).**

_**Nota**_ _In caso di problemi nella selezione della nuova superficie, premere il tasto_ _**BARRA SPAZIATRICE**_ _per alternare oggetti selezionabili diversi o disattivare temporaneamente il layer_ _**Glass Walls**_ _._

![](../../.gitbook/assets/0.jpeg)

4 - Per impostare la quota di offset, spostare il mouse all'interno della superficie e immettere **2"** per creare un nuovo rettangolo più piccolo.

![](../../.gitbook/assets/1%20%289%29.png)

5 - Fare clic una sola volta per selezionare il rettangolo interno appena creato. Fare nuovamente clic e trascinare la superficie all'interno dell'edificio fino a quando non scompare. Fare clic ancora una volta per terminare la rimozione del volume centrale dalla geometria del telaio.

![](../../.gitbook/assets/2%20%2821%29.png)

6 - Fare doppio clic per selezionare la geometria appena creata e scegliere **Gruppo \(G\)**. Denominare il gruppo **Mullion Frame – EW**​.

7 - Creare un layer denominato **Mullion** e inserirvi il nuovo gruppo.

8 - Per impostare il materiale del telaio:

1. Nella **tavolozza Materiali**, duplicare il materiale **Metal – Brushed – Colorized** facendovi clic con il pulsante destro del mouse e selezionando **Duplica materiale**.
2. Fare doppio clic sul riquadro di anteprima del nuovo materiale per modificarlo.
3. Rinominarlo **Metal – Brushed – Gray**.
4. Modificare il colore del materiale facendo clic sul riquadro **Colore** nella sezione **Mappe** e scurire il grigio modificando **Val:** in **150**.

![](../../.gitbook/assets/3%20%284%29.png)

9 - Fare clic su **OK** per salvare le modifiche apportate al nuovo materiale, quindi dipingere il gruppo **Mullion Frame – EW**. Successivamente, la **tavolozza Proprietà** del gruppo dovrebbe corrispondere a quella mostrata nell'immagine riportata di seguito:

![](../../.gitbook/assets/4.jpeg)

10 - Creare una nuova istanza del telaio sul lato orientale utilizzando uno qualsiasi dei seguenti strumenti: **Copia rapida**, **Matrice** o **Copia speculare**.

11 - Ripetere i passaggi precedenti per i lati nord e sud del parallelepipedo in vetro. Demoninare il nuovo gruppo **Mullion Frame – NS**. Non dimenticare di dipingerli e di posizionarli sul layer **Mullion**.

![](../../.gitbook/assets/5%20%2816%29.png)

_**Nota**_ _I telai a montanti si sovrappongono in corrispondenza degli angoli. Questo è intenzionale. Il risultato riportato sopra mostra la geometria risultante del telaio a montanti con i layer_ _**Glass Wall**_ _e_ _**Column**_ _disattivati._

**Creazione di montanti**

1 - In piano con la superficie esterna in vetro sul lato sud o nord dell'edificio, disegnare un **Rettangolo \(R\) da 2" x 10"-10"** che si estende dalla parte inferiore alla parte superiore del telaio a montanti. Non importa la posizione esatta del rettangolo lungo il telaio; lo sposteremo in posizione nei seguenti passaggi.

![](../../.gitbook/assets/6%20%2811%29.png)

2 - Estrudere il rettangolo indietro di **2"**, quindi scegliere **Gruppo \(G\)o** e denominare il gruppo **Mullion – Vertical**. Posizionare il gruppo sul layer **Mullion** e dipingerlo con il materiale **Metal – Brushed – Grey**.

**Individuazione dei montanti**

_Ora imposteremo la posizione per il primo montante in modo che sia centrato sul_ _**punto medio**_ _di un pilastro._

1 - Per visualizzare nuovamente i pilastri, attivare il layer **Column**, se è stato disattivato. Nella **tavolozza Layer**, è inoltre possibile disattivare i layer **Lower Terrace** e **Plan Image** per semplificare i passaggi successivi.

2 - Per spostare il montante nella nuova posizione:

1. Fare clic una sola volta per selezionare il gruppo di montanti verticali appena creato. Eseguire **Zoom \(Z\)** avanti e fare clic sul **punto medio** del bordo esterno inferiore del montante, simboleggiato da un triangolo rosso**.**
2. Iniziare a spostare la geometria orizzontalmente verso un pilastro. Premere **MAIUSC** per bloccare il movimento nell'asse rosso \(**Asse X**\). Notare che una volta bloccato il movimento, l'asse rosso diventa più spesso.
3. Eseguire lo zoom indietro fino a visualizzare la base del pilastro. Tenendo premuto **MAIUSC**, fare clic sul **punto medio** alla base della superficie esterna del pilastro. Il montante continuerà a spostarsi solo lungo l'asse rosso \(**Asse X**\), ma si allineerà al **Punto medio** su cui si è appena fatto clic.

![](../../.gitbook/assets/7%20%281%29.jpeg)

_**Nota**_ _Il montante ora si trova direttamente dietro il pilastro. Disattivare il layer_ _**Column**_ _o eseguire_ _**Orbita \(O\)**_ _per visualizzare il montante._

3 - Premere **ESC** per deselezionare lo strumento **Sposta**.

4 - Utilizzare lo strumento **Matrice \(AR\)** o **Copia rapida** per creare quattro \(4\) montanti verticali sullo stesso lato, distanziati tra loro di **11'**. Per ulteriori informazioni sull'utilizzo dello **strumento Matrice**, consultare i capitoli precedenti.

5 - Utilizzare il tasto TAB per selezionare tutti i gruppi di montanti **verticali** e copiarli sul lato opposto dell'edificio, in modo che sia i telai a **nord** che quelli a **sud** abbiano gli stessi layout di montanti, come mostrato nell'immagine seguente:

![](../../.gitbook/assets/8%20%286%29.png)

## **Creazione dei montanti delle porte**

1 - Eseguire **Orbita \(O\)** per la vista prospettica fino a quando non si osserva il centro del telaio a montanti ovest.

2 - Analogamente alla creazione di telai a montanti, disegnare un pannello di porta largo **3'-6"** con un telaio di **2"x 2"**. Impostarlo come **Gruppo \(G\)** con le proprietà: nome del gruppo: **Curtain Wall Door**; layer: **Mullion**; materiale: **Metal – Brushed – Grey**.

3 - Copiare questo gruppo per creare il secondo telaio della porta e spostarlo in modo che sia centrato nel gruppo **Mullion Frame – EW**, come mostrato di seguito.

![](../../.gitbook/assets/9.jpeg)

## **Creazione di un cornicione del tetto con estrusione su percorso**

_Ora creeremo il cornicione di Casa Farnsworth con uno degli strumenti di modellazione avanzati di FormIt,_ _**Estrusione su percorso**. Per ulteriori informazioni sulla modellazione avanzata, consultare il capitolo_ **2.2 -** _**Modellazione avanzata**_ _nella_ _**Guida introduttiva di FormIt - Parte II**._

_Il primo passaggio per la creazione di un'_ _**estrusione su percorso**_ _consiste nel disegnare un profilo perpendicolare all'estrusione stessa. A tale scopo, utilizzeremo la geometria del tetto come guida._

1 - Attivare il layer **Roof** ed eseguire lo zoom avanti di uno dei relativi angoli.

2 - Utilizzando come riferimento uno dei lati verticali del tetto, disegnare due rettangoli adiacenti. Il primo sarà **6"** di altezza e per **4 5/8**" di larghezza e il secondo sarà **2"x 2"**. Eliminare la linea che divide i due rettangoli per creare una singola superficie. Il risultato dovrebbe essere simile al seguente.

![](../../.gitbook/assets/10.jpeg)

3 - Per creare l'estrusione su percorso:

1. Senza geometria selezionata, fare clic sul pulsante **Strumenti di modellazione avanzati** sulla **barra degli strumenti Standard** e selezionare **Estrusione su percorso \(SW\)**.
2. Verrà avviata la **procedura guidata di selezione dell'estrusione su percorso** e verrà richiesto di **selezionare una superficie \(o i bordi\) per il profilo di estrusione su percorso**. Selezionare la superficie del profilo appena creata.
3. Una volta selezionato il profilo, verrà richiesto di **selezionare una superficie \(o un bordo\) per la traiettoria di estrusione su percorso, quindi fare clic su Fine**. Selezionare la superficie superiore del tetto. FormIt utilizzerà automaticamente i contorni della superficie selezionata come traiettoria dell'estrusione su percorso e l'estrusione stessa verrà creata attorno all'intero tetto.

_**Nota**_ _Se si verificano problemi nella selezione di una delle due superfici,_ eseguire _**Orbita \(O\)**_ _per visualizzare la superficie in modo leggermente migliore e riprovare. Come opzione alternativa, selezionare tutti i bordi del tetto anziché la superficie superiore del tetto per completare l'estrusione su percorso._

![](../../.gitbook/assets/11%20%282%29.png)

4 - Tenere ordinato il modello creando un gruppo **Roof - Cornice**, aggiungendolo al layer **Roof** e assegnandogli il materiale **Metal – Brushed – Colorized**.

![](../../.gitbook/assets/12%20%281%29.png)

5 - Per completare, attivare il layer **Column** e notare che l'estrusione su percorso appena creata interseca la parte superiore dei pilastri. Per risolvere questo problema, modificare uno qualsiasi dei gruppi **Column Tall** e trascinare la superficie superiore verso il basso fino ad allinearla alla parte inferiore del cornicione.

![](../../.gitbook/assets/13%20%285%29.png)

