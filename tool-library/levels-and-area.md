# Livelli e area

Dopo la creazione della geometria in FormIt, è possibile applicare i livelli per indicare le quote altimetriche del pavimento e per generare i calcoli dell'area.

Consultare la [Guida introduttiva di FormIt](../formit-primer/part-i/adding-floors-with-levels.md) per vedere i livelli in azione.

## Creazione e configurazione di livelli

Il pannello Livelli si trova sul lato destro di FormIt per Windows:

![](../.gitbook/assets/20191217-levels-panel-1.png)

#### Creazione ed eliminazione di livelli

* Creare un nuovo livello facendo clic sul pulsante "+".
* Creare una serie di livelli facendo clic sul pulsante "++".
   * Ciò consentirà di specificare il numero di livelli da creare e la distanza verticale tra di essi.
* Selezionare uno o più livelli e fare clic su "-" per eliminarli.

#### Ridenominazione, impostazione di quote altimetriche e rinumerazione di livelli

* Rinominare un livello facendo doppio clic sul nome oppure facendo clic con il pulsante destro del mouse e scegliendo Modifica nome.
* Regolare la quota altimetrica di un livello facendo doppio clic sul numero oppure facendo clic con il pulsante destro del mouse e scegliendo Modifica quota altimetrica.
* Fare clic sull'icona Aggiorna nella parte superiore per rinumerare i livelli.
   * Ciò risulta utile se sono stati aggiunti o rimossi livelli e lo schema di denominazione di default non è sincronizzato \(ad esempio, Livello 1, Livello 2, Livello 5\).
   * Questo pulsante ignora eventuali livelli con nomi personalizzati, ma rinumera eventuali livelli con il nome che segue la sintassi "Livello 1".

## Applicazione di livelli

Per applicare livelli ad un oggetto, è necessario selezionare l'oggetto e passare al pannello Proprietà.

Tenere presente che per applicare livelli ad un oggetto, l'oggetto deve essere solido, senza superfici posteriori o problemi delle superfici a tenuta ermetica. [Informazioni su come verificare la presenza di problemi delle superfici a tenuta ermetica e superfici posteriori nel modello](https://formit.autodesk.com/blog/post/repairing-solid-models)

Con un oggetto solido selezionato nell'area di disegno \(in questo esempio, la semplice struttura di un edificio\), nel pannello Proprietà viene mostrata la casella di controllo Usa livelli.

* Se per il disegno di FormIt sono già stati definiti i livelli \(vedere sopra\), selezionando questa casella si utilizzeranno tutti i livelli che intersecano questa forma \(ignorando eventualmente quelli che sarebbero troppo alti o troppo bassi\).
* Se il disegno di FormIt non dispone già di livelli, selezionando questa casella verranno creati livelli di default sufficienti.\(altezza interpiano da 12'\) per intersecare l'intera forma e si applicheranno automaticamente tali livelli a questo oggetto.

![](../.gitbook/assets/20191217-properties-panel.png)

## Livelli + Revit

Quando si applicano livelli alla geometria di FormIt, tali livelli verranno inviati a Revit quando si utilizza il [modulo aggiuntivo FormIt](https://formit.autodesk.com/page/formit-revit).

In Revit, è possibile utilizzare i livelli di FormIt per creare pavimenti di massa, pavimento da superficie e piante del pavimento associate ai livelli di FormIt.



