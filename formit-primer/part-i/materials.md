# 1.7 - Pittura con i materiali

Come abbiamo visto in un **esercizio precedente**, è possibile creare materiali personalizzati e quindi dipingere superfici con tali materiali in FormIt. In questo esercizio, creeremo e modificheremo più materiali, oltre a importare materiali da Autodesk Material Library.

_Se non è stata completata l'ultima sezione, scaricare e aprire il file_ _**1.7 - Paint with Materials.axm**_ _dai_ _**set di dati della Parte I della Guida introduttiva di FormIt**._

## **Creazione dei muri in vetro**

1 - Per visualizzare la pianta contenente le quote a cui si intende fare riferimento, accedere alla **tavolozza Layer** e attivare il layer **Plan Image**.

2 - Selezionare lo **strumento Rettangolo \(R\)**. Creeremo un rettangolo direttamente sopra il gruppo del pavimento esistente. Assicurarsi di non modificare il gruppo del pavimento, ma di disegnare sopra l'oggetto raggruppato esistente.

![](../../.gitbook/assets/0%20%283%29.png)

3 - Per iniziare il rettangolo per l'area in vetro:

1. Fare clic sull'angolo posteriore del pavimento esistente e spostare il mouse lungo il bordo più corto.
2. Digitare **28'-8"** per definire la prima lunghezza del bordo e fare clic su **OK**. La lunghezza deve corrispondere a quella del bordo corto esistente del pavimento.
3. Per definire il secondo bordo, iniziare a spostare il mouse lungo il bordo più lungo esistente del pavimento. Digitare **55'-5 ½"** per impostare la lunghezza del secondo bordo, quindi fare clic su **OK**.
4. Fare clic su **ESC** per uscire dallo strumento Rettangolo. Fare clic una sola volta all'interno del nuovo rettangolo per selezionare la superficie e iniziare a trascinarla verso l'alto.

![](../../.gitbook/assets/1%20%283%29.png)

4 - Per definire l'altezza, spostare il mouse verso l'alto lungo l'**Asse Z**, premere il tasto **TAB** e immettere **11'-2"**.

![](../../.gitbook/assets/2%20%284%29.png)

_**Nota**_ _Ogni volta che si utilizza uno strumento per il quale è possibile immettere una quota, premere_ _**TAB**_ _o iniziare a digitare i numeri._

5 - Fare doppio clic e selezionare **Gruppo \(G\)** per la nuova geometria.

6 - Fare doppio clic sul gruppo per modificarlo. Nella **tavolozza Proprietà**, denominare il gruppo **Glass Walls.**

![](../../.gitbook/assets/3%20%283%29.png)

7 - Per definire lo spessore del muro in vetro:

1. Fare clic con il pulsante destro del mouse sulla superfice superiore e scegliere lo **strumento Offset superficie \(OF\).**
2. Spostare il cursore del mouse verso l'interno e digitare **4".**
3. Premere due volte **ESC** per deselezionare lo strumento e annullare la selezione.

![](../../.gitbook/assets/4%20%2817%29.png)

​_**Nota**_ _L'unità di default per i progetti con unità di misura imperiali è piedi, analogamente a Revit. Se si immette un numero singolo senza un'unità specificata, ad esempio_ _**4**, si otterrà_ _**4 piedi \(4'\)**_ _e non_ _**4 pollici \(4"\)**._

8 - Per ritagliare l'area interna, fare clic una sola volta sulla superficie superiore interna per selezionarla, quindi fare di nuovo clic per avviare l'operazione di **trascinamento della superficie**. Spingere completamente la superficie verso il basso fino a quando non scompare e fare clic nello spazio per completare la procedura.

![](../../.gitbook/assets/5%20%2812%29.png)

_**Nota**_ _In FormIt, a differenza di altro software, non è possibile spingere accidentalmente "troppo" la superficie che si sta tentando di eliminare in modo da formare una nuova estrusione negativa._

9 - Terminare la modalità **Modifica gruppo** facendo doppio clic nello spazio o premendo **ESC.**

10 - Selezionare il gruppo **Glass Walls** con un solo clic e inserirlo nel layer **Main Building Floor**.

![](../../.gitbook/assets/6%20%2813%29.png)

## **Importazione di un materiale da Autodesk Material Library**

1 - Modificare nuovamente il gruppo **Glass Walls** facendovi doppio clic.

2 - Per importare un nuovo materiale nel modello:

1. Accedere alla **tavolozza Materiali**.
2. Scegliere **Campioni di materiali** nel menu a discesa nella parte superiore della tavolozza per spostarsi all'interno di **Autodesk Material Library.** ​
3. Fare clic sulla cartella **Glass+Glazing** per aprirla.
4. Individuare il materiale **Glass – Blue Tint** e fare clic una sola volta per aggiungere tale materiale alla libreria di materiali **Nel disegno**.
5. Si noti che è necessario tornare alla libreria **Nel disegno**, che ora include il materiale appena selezionato.

![](../../.gitbook/assets/7%20%288%29.png)

![](../../.gitbook/assets/8%20%288%29.png)

3 - Dopo aver aggiunto il materiale, dovrebbe attivarsi automaticamente lo strumento del **pennello**. In caso contrario, è sufficiente fare clic una sola volta di nuovo sul materiale **Glass – Blue Tint**. Per dipingere tutti i muri, fare doppio clic sulla geometria con lo strumento del **pennello**. In questo modo il materiale selezionato verrà applicato all'intero oggetto. ![](../../.gitbook/assets/9%20%281%29.png)​

4 - Fare clic su **ESC** per uscire dallo strumento del **pennello**. Fare nuovamente clic su **ESC** oppure fare doppio clic nello spazio per uscire dal gruppo.

## **Copia rapida del pavimento per creare il tetto**

1 - Per creare rapidamente il tetto in base alla geometria del pavimento:

1. Selezionare il gruppo **Floor** con un solo clic.
2. Fare clic su uno degli angoli inferiori per avviare lo strumento **Sposta**.
3. Iniziare a spostare il pavimento verso l'alto lungo l'asse blu \(**Asse Z**\). Creare una **copia rapida** toccando il tasto **CTRL**. Dovrebbe essere visualizzata un'anteprima "semitrasparente" della copia. ​
4. Durante lo spostamento lungo l'asse blu \(**Asse Z**\), iniziare a digitare **12' 2"** e verrà visualizzata la **finestra di dialogo Quota**. Fare clic su **OK** o premere **INVIO** per finalizzare la posizione.

![](../../.gitbook/assets/10%20%281%29.png)

![](../../.gitbook/assets/11%20%281%29.png)

## **Modifica del tetto**

1 - Mentre il gruppo copiato è ancora selezionato, utilizzare il comando **Rendi univoco \(MU\)** per dissociare questo gruppo dal gruppo Floor.

2 - Fare doppio clic sul gruppo per modificarlo. Rinominare il gruppo **Roof** nella **tavolozza Proprietà**. Uscire dal gruppo facendo doppio clic nello spazio.

3 - Nella **tavolozza Layer**, creare un nuovo **layer** denominato **Roof** e aggiungervi il gruppo **Roof**. È possibile attivare e disattivare il layer per verificare che gli elementi corretti si trovino sul tetto. Fare riferimento al **capitolo 6** per ulteriori informazioni su come utilizzare i **layer**.

4 - Tornare alla **tavolozza Materiali** e importare il materiale **Concrete - Broom Finish - Colorized 1** dalla cartella **Concrete+Asphalt** nella libreria **Campioni di materiali** **\(Produzione\)**. Notare che facendo clic sul materiale, la geometria selezionata verrà automaticamente dipinta e il nuovo materiale verrà aggiunto alla libreria di materiali **Nel disegno**.

![](../../.gitbook/assets/12.jpeg)

_**Nota**_ _La pittura di un gruppo al di fuori della_ _**modalità di modifica del gruppo**_ _è una tecnica utile che consente di dipingere diverse istanze dello stesso gruppo con materiali diversi._

## **Creazione della terrazza inferiore**

1 - In base a **Plan Image**, creare la terrazza inferiore come **Rettangolo \(R\)** lungo **55' 3"** e largo **22'-7 3/4"** ed estruderla di 1'. Posizionare il nuovo rettangolo in modo che si trovi a 8 5/8" dal bordo sud dell'edificio principale \(la profondità dei pilastri che verranno creati in seguito\).

_**Note:**_

* _Consultare i capitoli precedenti per informazioni su come disegnare ed estrudere i rettangoli._
* _Potrebbe essere necessario attivare o disattivare_ _**Snap alla griglia \(SG\)**_ _per fare clic_ sull'angolo della terrazza.

2 - Per finalizzare la terrazza inferiore:

1. Selezionare **Gruppo \(G\)** per la geometria e denominarlo **Lower Terrace Floor**.
2. **Spostare** il gruppo verso l'alto di **2'-2"** dal piano di base.
3. Creare un nuovo **layer** denominato **Lower Terrace** e aggiungervi il gruppo.
4. Aggiungere **Terrace Level Floor** al gruppo.

![](../../.gitbook/assets/13%20%281%29.png)

_**Nota**_ _Questa immagine non rappresenta la procedura passo passo per creare e assegnare la geometria a gruppi, livelli e layer. Per ulteriori informazioni su queste procedure, consultare i capitoli precedenti di questa Guida introduttiva._

3 - Importare il materiale **Stone &gt; Stone - Travertine**.

4 - Nella **tavolozza Materiali**, individuare il materiale **Travertine** importato e modificarlo:

1. Fare doppio clic sul riquadro di anteprima per aprire la finestra popup **Editor materiali**.
2. Fare clic sul riquadro di anteprima **Colore** per aprire la finestra popup **Scegli colore per questo materiale**.
3. Modificare il campo **Val** in **190** per scurire la tinta del materiale.

![](../../.gitbook/assets/14%20%282%29.png)

5 - **Disegnare** i gruppi **Floor** e **Lower Terrace Floor** con il materiale **Travertine** modificato.

![](../../.gitbook/assets/15.jpeg)

