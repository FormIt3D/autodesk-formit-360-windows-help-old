# 1.4 - Aggiunta di pavimenti con livelli

_I livelli consentono di tagliare le masse con singoli riferimenti del pavimento e calcolare l'area lorda per massa dell'edificio. I livelli di FormIt e i relativi nomi personalizzati verranno convertiti in livelli di Revit quando il file viene convertito in Revit._

_Se non è stata completata l'ultima sezione, scaricare e aprire il file **1.4 - Add Floors with Levels.axm** dai **set di dati della Parte I della Guida introduttiva di FormIt**._

## **Creazione e personalizzazione di livelli**

1 - Per creare livelli:

1. Accedere alla **tavolozza Livelli** sulla **barra delle tavolozze**.
2. Fare clic su **+** \(**Aggiungi livello**\) quattro volte per creare quattro livelli.
3. Fare doppio clic sulla quota altimetrica corrente di ciascun livello per modificarla in **0'-0", 2'-2", 4'-6"** e **17'-8"**.
4. Fare doppio clic sul nome corrente di ciascun livello e rinominarlo **Ground, Terrace, Main Building,** e **Top of Roof.**

![](../../.gitbook/assets/0%20%2816%29.png)

_**Nota** È possibile fare clic sull'icona_ _**++**_ _per creare più livelli, con una distanza specificata e uniforme tra loro. Questa opzione è utile per gli edifici a più piani_.

## **Applicazione di livelli alla geometria**

_Nei passaggi precedenti, abbiamo creato solo i livelli. Ora possiamo applicare tali livelli alla geometria che abbiamo creato._

1 - Per applicare i livelli alla geometria esistente:

1. Selezionare l'intera massa della terrazza superiore facendovi doppio clic.
2. Nella **tavolozza Proprietà**, fare clic su **Usa livelli**. Con questo passaggio si preselezionano tutti i livelli che attualmente intersecano la geometria selezionata.
3. Ora alla geometria attualmente selezionata sono applicati tre livelli \(**Main Building, Terrace** e **Ground**\), ma per questo esercizio desideriamo applicare solo **Ground**. Deselezionare **Main Building** e **Terrace**.
4. Questa procedura garantisce che solo l'area intersecata da **Ground** venga considerata per il calcolo dell'area lorda, che può essere visualizzato nel campo **Area per livello**.

![](../../.gitbook/assets/1%20%284%29.png)

_**Nota** Se non sono visualizzate linee di livello blu nella massa, digitare_ _**DL**_ _per_ _**Visualizza livelli**._

![](../../.gitbook/assets/2%20%283%29.png)

