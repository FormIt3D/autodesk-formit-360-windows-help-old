# Domande frequenti

## Informazioni su FormIt

**Che cosa sono FormIt e FormIt Pro?**

FormIt è un ambiente di calcolo, analisi, visualizzazione e modellazione 3D per la progettazione architettonica.

Funzionalità di FormIt:

* Un efficiente motore di modellazione di solidi, con potenti strumenti e workflow ottimizzati per la progettazione di edifici
* Visualizzazione ambientale migliorata per illustrare le varianti di progetto, inclusi gli stati dei modelli salvati utilizzando le scene
* Posizione, immagini satellitari e terreno 3D utilizzando Bing Maps
* Materiali di Autodesk Material Library
* Strumenti di visibilità e organizzazione dei modelli, quali gruppi, layer e scene
* Strumenti di analisi, tra cui:
   * Convalida delle superfici a tenuta ermetica e posteriori per la diagnostica e la riparazione di modelli di solidi
   * Sole e ombre
   * Analisi solare
   * Analisi energetica
* Integrazioni di prodotti Autodesk:
   * Autodesk Docs
   * Insight \(Analisi energetica\)
   * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
   * [Revit](https://formit.autodesk.com/page/formit-revit)
* Supporto di formati di file:
   * Apertura/Importazione
      * AXM, DWG, FBX, SAT, STL, OBJ, WSM, SketchUp, immagine
   * Esportazione
      * AXM, FBX, OBJ, STL, SAT, DAE, DXF

FormIt è disponibile gratuitamente in [iOS](https://itunes.apple.com/us/app/autodesk-formit-360/id575282599?mt=8) e [nel browser in uso](https://app.formit.autodesk.com/). Per utilizzare [FormIt per Windows](https://formit.autodesk.com/page/download), la versione più potente e ricca di funzionalità di FormIt, è necessario un abbonamento a **FormIt Pro**. L'abbonamento a **FormIt Pro** consente inoltre di aggiungere funzionalità in iOS e sul Web, ad esempio Analisi solare e Analisi energetica. **FormIt Pro** è incluso in [Autodesk AEC Collection](https://www.autodesk.it/collections/architecture-engineering-construction/overview).

**Che ne è stato di FormIt per Android?**

Per semplificare l'offerta di prodotti FormIt, abbiamo dovuto prendere la difficile decisione di interrompere l'app per Android. Se è stato installato, continuerà ad essere eseguito, ma non sarà più disponibile nel Play Store.

**Come ottenere FormIt?**

Per eseguire la versione per Windows, è necessario disporre dell'accesso a **FormIt Pro**, che fa parte dell'abbonamento ad [AEC Industry Collection](https://www.autodesk.it/collections/architecture-engineering-construction/overview). Quindi, se l'ufficio dispone di Revit, c'è una buona probabilità di avere già accesso a FormIt. È possibile [scaricare FormIt per Windows direttamente dal nostro sito Web](https://formit.autodesk.com/page/download) o dall'app desktop Autodesk.

Inoltre, la versione per il Web può essere eseguita gratuitamente dal nostro sito Web all'indirizzo: [http://formit.autodesk.com](http://formit.autodesk.com)

La versione per iOS può essere scaricata gratuitamente dall'App Store di Apple \(solo iPad\).

**Gli studenti o i docenti possono accedere a FormIt Pro senza costi?**

Sì. È possibile accedere all'abbonamento a FormIt Pro tramite il [portale Autodesk Education](https://www.autodesk.it/education/edu-software/overview?sorting=featured&page=1).

**Come imparare ad utilizzare FormIt?**

Il punto migliore da cui iniziare è l'[esercitazione nella Guida introduttiva di FormIt](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html).

Esistono diverse sezioni della Guida introduttiva, che vanno per principianti \(creazione di un'intera casa moderna\) a quelle per utenti più avanzati \(utilizzo di Revit e Dynamo in modi più avanzati\).

Abbiamo anche più di 20 video nella serie di webinar FormIt Friday. Questi sono disponibili sul [canale YouTube](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH).

## Utilizzo di Revit

**Come funziona FormIt con Revit?**

FormIt è un'applicazione di disegno e progettazione 3D separata, ma crea dati facilmente convertibili in Revit [utilizzando il modulo aggiuntivo FormIt per Revit](https://formit.autodesk.com/page/formit-revit).

**Cosa succede quando si esegue l'importazione in Revit?**

A partire dalla versione 2016, Revit viene fornito con un modulo aggiuntivo per l'utilizzo dei dati di FormIt. Quando si importa un file AXM di FormIt in Revit, questo modulo aggiuntivo esamina ogni oggetto del file e lo ricrea in Revit utilizzando l'API. Per default, ogni elemento di FormIt viene classificato come Massa.

FormIt Converter acquisisce ogni oggetto Massa e crea una famiglia di masse in Revit utilizzando l'[API Direct Shape](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/ITA/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html).

Direct Shape è un oggetto non modificabile utilizzato nei workflow di file IFC. Sebbene non sia modificabile, ha il vantaggio evidente di trasferire trame complete di materiali tra FormIt e Revit. [Di seguito è disponibile un'esercitazione](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html) che illustra in maggiore dettaglio il workflow da FormIt a Revit.

**FormIt è in grado di creare muri, pavimenti e altre famiglie di sistema di Revit?**

Non direttamente. Come indicato in precedenza, per default ogni oggetto è impostato sulla categoria Massa. Per creare muri, pavimenti e così via, è necessario importare il modello in Revit con il modulo aggiuntivo di conversione e utilizzare gli strumenti nativi di Revit per creare famiglie di sistema dal modello di massa sottostante.

**Revit è in grado di inviare nuovamente i dati a FormIt?**

Sì. Per reimportare i dati in FormIt, esportare tutto il file di Revit o, preferibilmente, _una parte_, nel formato di file SAT. In genere non è necessario inviare TUTTI i dati di Revit a FormIt. In Revit, invece, creare una vista filtrata che includa solo i dati minimi \(ad esempio, pavimenti e muri\) prima di eseguire il salvataggio in formato SAT.

## Utilizzo di altre app

**Perché "AXM" è il formato di file di default?**

Il nome in codice interno prima del nome ufficiale di FormIt era XModeler, quindi il formato di file creato era Autodesk X Modeler o AXM in breve.

**Che tipo di formati 3D è possibile importare in FormIt?**

* Windows: AXM, DWG, FBX, OBJ, SAT, SKP, STL
* Web: OBJ, STL
* iOS: OBJ, STL, SAT

**Quali tipi di formati è possibile esportare in FormIt?**

* Windows: FBX, OBJ, SAT, STL, DAE, DXF
* Web: OBJ, SAT, STL
* iOS: OBJ

**Come funziona FormIt con Dynamo?**

[Scoprire come FormIt e Dynamo si integrano](https://formit.autodesk.com/page/formit-dynamo) per creare workflow di progettazione computazionale.

**In che modo FormIt è paragonabile a SketchUp?**

* Migliore [**interoperabilità con Revit**](../tool-library/revit.md) ****
* [**Integrazione di Dynamo**](../tool-library/dynamo.md) per la progettazione computazionale
* Strumenti nativi per l'[**analisi solare**](../tool-library/solar-analysis.md) e l'[**analisi energetica con tecnologia**](../tool-library/energy-analysis.md) Autodesk Insight
* Un kernel di modellazione di solidi più affidabile che consente operazioni di modellazione avanzata
* Strumenti di modellazione avanzati nativi come[**Estrusione su percorso, Copertura, Loft**](../tool-library/cover-sweep-loft.md), Offset/Involucro solidi, Unione/Raccordo (3D) e [**Livella superfici**](../tool-library/flatten-face.md)
* Più [**piani di sezione** ](../tool-library/section-planes.md)visibili
* Strumenti di diagnostica come [**Visualizza: Problemi delle superfici a tenuta ermetica e Visualizza: Superfici posteriori**](../tool-library/visual-styles.md)
* [**Esportazione di parti del modello**](../tool-library/export-data.md) in base a ciò che è selezionato e/o visibile
* Esportazione di file nativi OBJ, SAT e STL

**È possibile utilizzare i tasti di scelta rapida di SketchUp?**

Sì. FormIt per Windows ha una mappa della tastiera completamente modificabile. Per default, sono già presenti molti tasti di scelta rapida di SketchUp comuni, ma è possibile modificarli nel menu Modifica &gt; Preferenze.

**È possibile utilizzare i file DWG?**

Sì. FormIt importa file DWG 2D e 3D.

## Domande comuni per il supporto

**Come accedere al supporto?**

È possibile iniziare con il rivenditore Autodesk o visitare il [forum di FormIt](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=en). È consigliabile prima cercare la domanda che si desidera porre e, se non è stata fornita una risposta, pubblicare un nuovo argomento così il team di FormIt risponderà.

**Come procedere se non è possibile eseguire l'accesso?**

* Questo [post del forum](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572?profile.language=en) illustra i problemi comuni relativi all'accesso.
* Se si dispone di un PC con un processore grafico \(GPU\) commutabile, è importante assicurarsi che FormIt utilizzi sempre la GPU con prestazioni superiori. Di seguito sono riportate le istruzioni per [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) e [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1).

**Come procedere se Analisi energetica di Insight non riesce?**

Se Analisi energetica di Insight segnala un errore o non restituisce alcun risultato, [consultare la pagina FormIt + Insight - Energy Analysis in FormIt](https://formit.autodesk.com/page/formit-insight) per suggerimenti comuni sulla risoluzione dei problemi.

