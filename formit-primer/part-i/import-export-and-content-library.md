# 1.11 - Importazione di modelli con Libreria del contenuto

_In questo capitolo, importeremo i modelli di SketchUp esistenti, nonché utilizzeremo la Libreria del contenuto di FormIt per posizionare le famiglie predefinite convertite da Revit. Notare che quando si aprono i file SKP con FormIt, questi includono materiali, gruppi e componenti, layer \(etichette\) e scene intatti. Potrebbe essere necessario eseguire alcune operazioni di pulizia per tenere ordinati e organizzati i progetti._

_Per questo capitolo utilizzeremo i file della cartella_ **Farnsworth House Data Set &gt; Supporting Files**. Se non è già stato fatto, assicurarsi di scaricare le cartelle richieste, o l'intero set di dati, dai _**set di dati della Parte I della Guida introduttiva di FormIt**._

## **Importazione e modifica di file SKP**

_Innanzitutto, descriveremo la procedura di aggiunta di una parte del contenuto scaricato alla libreria del contenuto personale_. Tenere presente che in questo esercizio utilizzeremo solo file SKP. Per ulteriori informazioni su come aprire/importare altri formati di file, consultare [**questo post del blog sulle funzionalità di Formit 2021.2**](https://formit.autodesk.com/blog/post/formit-2021-2-and-new-revit-add-in-now-available ) e **questo capitolo sui** **formati di file di importazione ed esportazione estesi**.

1 - Assicurarsi di eseguire **Salva \(CTRL+S\)** per qualsiasi lavoro aperto, quindi avviare un nuovo disegno di FormIt. A tale scopo, è possibile:

1. Aprire un'altra sessione di FormIt in una nuova finestra facendo clic con il pulsante destro del mouse sull'icona di FormIt sulla **barra delle applicazioni di Windows** e facendo clic sull'icona di **FormIt**. Verrà aperta una nuova finestra di FormIt, che consente di eseguire due sessioni di FormIt affiancate.
2. OPPURE, dopo il salvataggio, selezionare **Nuovo disegno \(CTRL + N\)** dall'elenco a discesa **File** sulla barra **Menu principale**.

![](../../.gitbook/assets/0%20%2819%29.png)

2 - Creare una nuova cartella denominata **Custom FormIt Content** all'interno della cartella **Farnsworth House Data Set &gt; Supporting Files &gt; FormIt** nel _**set di dati su Casa Farnsworth**._

3 - Eseguire **Salva \(CTRL+S\)** per il nuovo disegno in tale cartella. Consigliamo di denominarlo **Ottoman – Barcelona\_Mies.axm**.

4 - Nel nuovo file di FormIt vuoto:

1. **Importare un file locale \(CTRL+I\)** selezionando **Importa &gt; Localmente...** dall'elenco a discesa **File** sulla barra **Menu principale**.
2. Scegliere **Ottoman – Barcelona\_Mies.skp** da **Farnsworth House Data Set &gt; Supporting Files &gt; SketchUp** e fare clic su **Apri**.

_**Nota**_ _Se il file_ _**Ottoman – Barcelona\_Mise.skp file** non è visibile, verificare che l'elenco a discesa dei formati di file in basso a destra sia impostato su_ _**Tutti i formati supportati**._

![](../../.gitbook/assets/1%20%287%29.png)

5 - Rinominare il gruppo importato **Ottoman - Barcelona\_Mies**.

6 - Quando alla fine importiamo questo modello nel file di Casa Farnsworth, verrà posizionato utilizzando il punto di **origine** di questo file. Per controllare il punto di posizionamento, desideriamo spostare il gruppo **Ottoman - Barcelona\_Mies** in modo che uno dei relativi angoli sia posizionato in corrispondenza dell'**origine**. Procedura:

1. Verificare che l'opzione **Snap alla griglia \(SG\)** sia attivata. Disegnare una **linea \(L\)** di riferimento a partire dall'**origine** \(gli assi X, Y e Z si intersecano\). Fare clic in un punto qualsiasi per posizionare il secondo punto.
2. Selezionare il gruppo dell'ottomana e avviare il comando di spostamento facendo clic una sola volta sull'angolo inferiore sinistro della gamba, come mostrato. _Per ulteriori informazioni su come spostare gli oggetti, consultare i capitoli precedenti._
3. Spostare il gruppo fino all'**origine**, eseguendo lo snap al punto iniziale della linea di riferimento appena disegnata.
4. Eliminare la linea di riferimento.

![](../../.gitbook/assets/2%20%2817%29.png)

7 - Consigliamo di eliminare eventuali layer indesiderati importati con il file SKP, poiché eventuali layer di questo modello verranno infine importati nel nostro modello di Casa Farnsworth. A tale scopo, accedere alla **tavolozza Layer**, selezionare **Layer 0** e fare clic sul pulsante **-**. In questo modo il layer verrà eliminato mantenendone la geometria.

![](../../.gitbook/assets/3%20%2816%29.png)

_**Nota**_ _Ogni volta che si elimina un layer, a qualsiasi geometria o a eventuali gruppi che si trovavano su tale layer viene assegnato_ _**Nessun layer**, che rappresenta il valore di default per qualsiasi oggetto non ancora assegnato ad un layer._

## **Creazione della miniatura del contenuto**

_Questo passaggio successivo consente di impostare una scena da utilizzare come miniatura del_ _**contenuto**_ _, che verrà visualizzata nella_ _**tavolozza Libreria del contenuto**._

1 - Per definire le impostazioni della vista per la scena della miniatura:

1. Nella scheda **Ambiente** della **tavolozza Stili visualizzazione**, deselezionare tutte le caselle di controllo e impostare il colore **Inferiore/Sfondo** su bianco.
2. Verificare che la modalità della vista sia impostata su **Prospettica** **\(VP\)**.
3. Utilizzare gli **strumenti di navigazione nella vista** per eseguire lo zoom avanti e selezionare una posizione della cinepresa che rappresenti bene l'oggetto, analogamente all'immagine riportata di seguito.

![](../../.gitbook/assets/4%20%2813%29.png)

2 - Per salvare le impostazioni appena impostate, creare una scena:

1. Accedere alla **tavolozza Scene**.
2. Fare clic sul pulsante **+**. In questo modo verrà creata una nuova scena in base alle impostazioni correnti.
3. Rinominarla **Thumbnail** e verificare che almeno le prime quattro \(4\) caselle di controllo siano state selezionate: **Cinepresa**, **Layer**, **Sole e ombre** e **Stili visualizzazione**. Le altre impostazioni della scena non sono realmente rilevanti per la creazione dell'immagine di miniatura.
4. Utilizzare il pulsante **Aggiorna scena** ogni volta che si desidera aggiornare la **scena** in modo che corrisponda alle impostazioni correnti di visualizzazione e di vista della cinepresa.

![](../../.gitbook/assets/5%20%2811%29.png)

3 - Eseguire nuovamente **Salva \(CTRL+S\)** per il modello di ottomana completato. Notare che la **miniatura del contenuto** viene creata dalla vista corrente al momento dell'ultimo salvataggio del modello, pertanto assicurarsi di trovarsi nella **scena Thumbnail** prima di eseguire il salvataggio.

_Se lo si desidera, è possibile confrontare il file con il nostro aprendo il file_ _**Ottoman - Barcelona\_Mies.axm**_ _salvato in_ _**Farnsworth House Data Set &gt; Supporting Files &gt; FormIt &gt; Furniture**_ _nel_ _**set di dati di Casa Farnsworth**.‌_

_È possibile eseguire gli stessi passaggi descritti sopra con i file SKP di panchina e sedia che si trovano nella stessa cartella dell'ottomana._

_**Suggerimento**_ _Per accelerare la procedura, consigliamo di utilizzare il file_ _**Ottoman - Barcelona\_Mies.axm**_ _appena creato come modello. Durante la modellazione, è possibile attivare nuovamente_ _**Griglia**_ _e_ _**Assi**_ _dalla_ _**tavolozza Stili visualizzazione**. Regolando solo la posizione della cinepresa della_ _**scena Thumbnail**_ _per ogni elemento di arredo, si garantisce che le_ _**miniature del contenuto**_ _rimangano coerenti per tutti i modelli di contenuto._

## **Collegamento di una libreria del contenuto**

_Torniamo ora al nostro progetto di Casa Farnsworth. Illustreremo come collegare la cartella **FormIt** nel **set di dati di Casa Farnsworth** per accedere facilmente a tutti i file, incluso il_ **contenuto personalizzato di FormIt** _appena creato, all'interno del progetto._

1 - Dopo il ripristino o la riapertura del modello di Casa Farnsworth. _Se non è stato completato l'ultimo capitolo, scaricare e aprire il file_ _**1.11 - Import Models with Content Library.axm**_ _dal_ _**set di dati di Casa Farnsworth**._

1. Aprire la **tavolozza Libreria del contenuto** e fare clic sull'icona **Collega directory della Libreria del contenuto**. Viene visualizzata la finestra **Preferenze** con la scheda **Libreria del contenuto** aperta.
2. Fare clic sull'icona **+** per **aggiungere una nuova posizione alla libreria del contenuto**. Verrà visualizzata una terza finestra che consente di spostarsi nella directory del computer in uso e selezionare una cartella.
3. Nel _**set di dati di Casa Farnsworth**, spostarsi tra le cartelle_ _**Supporting Files > FormIt**. Qui sono disponibili le_ cartelle contenenti i file **.axm** creati in precedenza in questo capitolo. Fare doppio clic sulla cartella **FormIt** per selezionarla.
4. Fare clic su **Seleziona cartella** per visualizzare il percorso della cartella nel pannello **Posizioni libreria – Locale**.
5. Nella finestra **Preferenze**, fare clic su **OK** e la cartella collegata verrà aggiunta alla **Libreria del contenuto**.
6. Per accedere a questa nuova libreria, aprire il menu a discesa nella parte superiore della **tavolozza Libreria del contenuto** e selezionare **FormIt**.
7. Notare che la struttura delle cartelle e tutti i file **.axm** nella cartella collegata verranno mostrati nella **tavolozza Libreria del contenuto**. Fare doppio clic su eventuali sottocartelle per accedere ai file in esse contenuti.

![](../../.gitbook/assets/link-library-content.png)

**Nota** Se si dispone dell'accesso ad **Autodesk Docs** \(precedentemente noto come Autodesk 360\), è possibile accedere anche ai file che potrebbero esservi memorizzati tramite il menu a discesa **Libreria del contenuto**.

## **Posizionamento del contenuto dalla libreria**

_‌Ora posizioneremo gli elementi del contenuto creati all'interno del modello di Farnsworth._

1 - Per poter vedere all'interno della casa e posizionare gli arredi, disattivare il layer **Roof** ed eseguire **Orbita \(O\)** nella vista prospettica fino a visualizzare l'intero piano dell'edificio principale.

2 - Tornando alla **tavolozza Libreria del contenuto**, verificare che l'elenco a discesa sia ancora impostato su **FormIt**. Prima di posizionare uno qualsiasi degli arredi che abbiamo appena realizzato, dobbiamo posizionare il "nucleo" della casa:

1. Fare clic sulla cartella denominata **Other** per aprirla, quindi fare clic sulla miniatura **Farnsworth House – Core** per selezionarla.
2. Posizionare il cursore del mouse su **Main Building Floor** per fare clic sul **centroide** del pavimento per posizionare **Core**.
3. Per tornare su alla cartella di FormIt, utilizzare il pulsante **Naviga su**.

![](../../.gitbook/assets/7%20%282%29.jpeg)

3 - Impostare la cinepresa su **Vista dall'alto \(VT\)**, **Ortogonale \(VO\)** e disattivare **Main Building Floor** per visualizzare **Plan Image**. Consultare i capitoli precedenti per ulteriori informazioni sulle impostazioni relative alle **viste** e ai **layer**.

4 - Selezionare **Farnsworth House - Core** e spostarlo fino a quando non si allinea perfettamente con Plan Image.

![](../../.gitbook/assets/8%20%281%29.png)

_**Nota**_ _Durante lo spostamento di_ _**Core**, prestare attenzione a non modificarne la quota altimetrica. È possibile utilizzare il tasto_ _**MAIUSC**_ _per limitare il movimento in modo che sia sempre lungo uno degli assi o assicurarsi che i punti di riferimento iniziale e finale del comando_ _**Sposta \(M\)**_ _siano entrambi alla stessa altezza facendo clic solo su_ _**Plan Image**, non su_ _**Core**_ _. Per ulteriori informazioni sullo strumento_ _**Sposta \(M\)**_ _, consultare i capitoli precedenti.‌_

## **Posizionamento di arredi dalla libreria**

1 - Utilizzando una procedura simile, è ora possibile posizionare gli arredi creati in precedenza in questo capitolo dalla cartella **Custom FormIt Content**. Se non sono stati convertiti tutti e tre \(3\) i file SKP, è possibile utilizzare le versioni predefinite all'interno della cartella **Furniture**.

_**Note **_

* _Riattivare il layer_ _**Main Building Floor**_ _, in modo da poter posizionare gli arredi direttamente sulla superficie di_ _**Main Building Floor**._
* _Durante il posizionamento di un nuovo oggetto, utilizzare il tasto_ _**TAB**_ _per alternare i piani di posizionamento._
* _Durante il posizionamento di un nuovo oggetto, utilizzare il tasto_ _**BARRA SPAZIATRICE**_ _per ruotarlo di 90 intervalli prima del posizionamento._

![](../../.gitbook/assets/9%20%283%29.png)

2 - Analogamente, esplorare **Esempi della Libreria del contenuto** per posizionare il contenuto predefinito. Si noti che molte di queste famiglie hanno diverse dimensioni tra cui scegliere, simili ai tipi di famiglia in Revit.

![](../../.gitbook/assets/10%20%286%29.png)

## **Utilizzo dello strumento Scala**

1 - Utilizzando le tecniche appena apprese, posizionare un'istanza del componente **tree\_pine** dalla cartella **Farnsworth House Data Set &gt; FormIt &gt; Planting**.

1. Una volta posizionato, selezionare il gruppo e rinominarlo **Tree**. Fare clic con il pulsante destro del mouse per accedere al **menu contestuale** e scegliere **Scala non uniforme \(NU\)**.
2. Fare clic su uno dei **pulsanti di Scala non uniforme** per ridimensionare e modificare le proporzioni del gruppo **Tree** come desiderato.

![](../../.gitbook/assets/11%20%283%29.png)

![](../../.gitbook/assets/12%20%282%29.png)

_**Nota**_ _Analogamente, lo strumento_ _**Scala \(SC\)**_ _può essere utilizzato per rimettere in scala un intero modello o gruppo in modo uniforme._

2 - Copiare questo gruppo e posizionare più alberi attorno alla casa, utilizzando gli **strumenti di Scala** per creare una varietà di dimensioni e proporzioni.

![](../../.gitbook/assets/13%20%286%29.png)

_**Nota**_ _Anche se gli alberi sono tutte istanze dello stesso gruppo, siamo stati in grado di_ _**metterli in scala**_ _in base a dimensioni diverse. L'utilizzo delle opzioni_ _**Scala \(SC\)**_ _e_ _**Scala non uniforme \(NU\)**_ _al di fuori della modalità di modifica del gruppo consente di modificare singole istanze dello stesso gruppo. Se dovessimo modificare uno dei gruppi_ _Tree****_ _e cambiarne la geometria o il materiale, tutte le istanze del gruppo verrebbero comunque aggiornate, ma ognuna manterrebbe la scala personalizzata corrente. Eseguire una prova._

### **Tenere ordinato il modello**

_Ricordarsi di ordinare sempre sui layer il contenuto aggiunto. In questo esempio, consigliamo di posizionare il nucleo e tutti gli arredi sul layer_ _**Main Building Floor**_ _e gli alberi su un nuovo layer denominato_ _**Planting**._

