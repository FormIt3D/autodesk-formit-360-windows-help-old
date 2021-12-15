# Salvataggio automatico

A partire dalla versione v17.3, FormIt per Windows include il comando Salvataggio automatico che crea una copia di backup del modello di FormIt mentre si lavora. Questo file di backup può essere utilizzato per recuperare i dati se FormIt si chiude con modifiche non salvate.

### Attivazione/Disattivazione di Salvataggio automatico

Le opzioni di configurazione per Salvataggio automatico sono presenti in Modifica &gt; Preferenze &gt; Salvataggio automatico.

![](../.gitbook/assets/20190613-autosave.png)

Il comando Salvataggio automatico è attivato di default, ma può essere disattivato completamente deselezionando semplicemente la casella.

Impostare l'intervallo \(in minuti\) in cui Salvataggio automatico eseguirà una copia di backup immettendo un valore nella casella del numero Intervallo di Salvataggio automatico.

Tenere presente che queste preferenze sono a livello di applicazione e non verranno modificate quando si aprono file diversi.

### Funzionamento di Salvataggio automatico

Quando l'opzione Salvataggio automatico è attivata, determina se il file di FormIt corrente contiene modifiche non salvate. Se sono presenti modifiche non salvate, Salvataggio automatico crea una copia di backup del file all'intervallo specificato.

I file di backup vengono memorizzati accanto al file originale e hanno un'estensione `.axmb`.

Ad esempio, se il file di FormIt originale è memorizzato in `C:/Users/<user>/FormIt/MyProject.axm`, il file di backup è disponibile in `C:/Users/<user>/FormIt/MyProject.axmb`.

Se si avvia una nuova sessione di FormIt senza aprire un file esistente, le modifiche non salvate sono disponibili in `C:/Users/<user>/Documents/Untitled.axmb`. Dopo aver salvato il nuovo modello in un'altra posizione, con il backup si inizieranno ad aggiungere le modifiche non salvate nella nuova posizione, come indicato in precedenza.

Quando si salvano le modifiche apportate al file originale, Salvataggio automatico elimina automaticamente il file di backup poiché il backup è ora meno recente del file originale. Tuttavia, se si apportano modifiche successive al file salvato, verrà richiesto di avviare nuovamente il backup di Salvataggio automatico all'intervallo specificato.

Se il file di lavoro contiene modifiche non salvate e si sceglie di chiudere FormIt e ignorare le modifiche, il backup di Salvataggio automatico verrà eliminato. Tuttavia, se si forza la chiusura di FormIt, tramite un arresto del computer o un arresto anomalo di un'applicazione, il file di backup di Salvataggio automatico rimarrà e potrà essere utilizzato in un secondo momento per recuperare i dati.

### Utilizzo di Salvataggio automatico attivato

FormIt riduce al minimo l'impatto potenziale di Salvataggio automatico sulle prestazioni eseguendo il backup in un processo separato. Con i file di piccole e medie dimensioni, non si dovrebbe notare quando si esegue il backup di AutoSave. Con file molto grandi \(oltre 400 MB\), si potrebbe notare una pausa momentanea mentre in FormIt viene copiato l'intero modello e si inizia il backup in un processo separato.

Se si desidera sapere se Salvataggio automatico è attualmente in fase di backup, è possibile controllare la barra di stato nella parte inferiore sinistra dell'applicazione per ricercare il breve messaggio Salvataggio automatico in corso...:

![](../.gitbook/assets/20190613-autosave-status-bar.png)

Se la barra di stato è disattivata, è possibile attivarla in Finestra &gt; Barra di stato o tramite il collegamento HS.

### Recupero di dati con Salvataggio automatico

Quando si apre un file di FormIt con un backup disponibile, l'utente viene avvisato che esiste il file di backup. Come già detto, questo problema potrebbe essere semplicemente dovuto alla chiusura di FormIt senza scegliere di salvare le modifiche apportate al progetto l'ultima volta che è stato modificato o a causa della chiusura imprevista di FormIt.

![](../.gitbook/assets/20190613-autosave-notification.png)

Facendo clic sul collegamento ipertestuale Aprirlo? si consente di caricare il file di backup `.axmb`.

Analogamente, è possibile utilizzare File &gt; Apri e selezionare manualmente il file `.axmb` da Esplora file per aprire un backup.

Una volta aperto il file di backup, al successivo salvataggio, in FormIt verrà richiesto di selezionare un file di FormIt diverso \(`.axm`\) da sovrascrivere. Non è possibile sovrascrivere i file di backup di FormIt \(`.axmb`\).



