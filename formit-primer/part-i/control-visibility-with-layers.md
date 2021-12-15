# 1.6 - Controllo della visibilità con i layer

_Analogamente ad AutoCAD e Photoshop, i layer in FormIt consentono di gestire la visibilità degli oggetti nel modello. In questo capitolo, creeremo un layer per salvare e nascondere la massa dell'edificio per un'analisi futura._

_Se non è stata completata l'ultima sezione, scaricare e aprire il file_ _**1.6 - Control Visibility with Layers.axm**_ _dai_ _set di dati della Parte I della Guida introduttiva di FormIt**.**_

## **Creazione di layer**

1 - Per creare i nuovi layer:

1. Accedere alla **tavolozza Layer** e fare clic sul segno **+** tre volte per creare tre layer.
2. Fare doppio clic sui nomi dei layer per rinominarli **Massing**, **Main Building Floor** e **Plan Image.**

![](../../.gitbook/assets/0%20%2820%29.png)

_**Nota**_ _È possibile fare clic sul nome di un layer e trascinarlo verso l'alto o verso il basso per riordinare i layer._

2 - Per assegnare il gruppo **Massing - Main Building** al layer **Massing**:

1. Nell'area di disegno, selezionare il gruppo **Massing - Main Building**.
2. Nella **tavolozza Layer**, scegliere il layer **Massing** dal menu a discesa **Selezione su:**. Analogamente, assegnare il gruppo **Plan Image** al layer **Plan Image**.

![](../../.gitbook/assets/1%20%2813%29.png)

## **Duplicazione del gruppo**

_Ora inizieremo il processo di modellazione dell'edificio in modo più dettagliato. Il primo passaggio consiste nel creare la geometria del pavimento in base alla volumetria dell'edificio già presente._

1 - Selezionare nuovamente il gruppo **Massing - Main Building**. Premere **CTRL+C \(Copia\)** per copiare, quindi **CTRL+MAIUSC+V \(Incolla nella stessa posizione\)** per incollare la massa nella stessa posizione.

2 - Per dissociare la geometria del nuovo gruppo dal gruppo originale: fare clic con il pulsante destro del mouse per accedere al **menu contestuale** e scegliere l'opzione **Rendi univoco \(MU\)**.

![](../../.gitbook/assets/2%20%2818%29.png)

_**Nota** Il nuovo gruppo non è più associato all'originale. Le modifiche apportate al nuovo gruppo non altereranno il gruppo originale._

## **Creazione della geometria del pavimento**

1 - Riassegnare il layer del gruppo:

1. Fare un singolo clic per selezionare uno dei gruppi **Massing – Main Building**.
2. Posizionare il gruppo sul layer **Main Building Floor** utilizzando l'elenco a discesa **Selezione su:** nella **tavolozza Layer**.
3. Deselezionare il layer **Massing** per nasconderne la geometria e proteggerla da eventuali modifiche accidentali.

![](../../.gitbook/assets/3%20%2818%29.png)

2 - Fare doppio clic sul gruppo **Massing – Main Building** visibile per modificarlo. Rinominare il gruppo **Floor** nella **tavolozza Proprietà**.

![](../../.gitbook/assets/4%20%2812%29.png)

3 - **Fare un singolo clic** sulla **superficie superiore** della geometria per selezionarla. Fare nuovamente clic e iniziare a trascinare la superficie verso il basso. Mentre si trascina la superficie verso il basso, digitare **11'-2"**. Verrà visualizzata la **finestra di dialogo Quota**. Fare clic su **OK** dopo aver immesso il valore. Il pavimento risultante dovrebbe essere spesso 1'. Fare doppio clic nello spazio per uscire dal gruppo.

![](../../.gitbook/assets/5%20%2810%29.png)

