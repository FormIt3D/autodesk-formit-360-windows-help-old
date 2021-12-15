# Linea di offset

È possibile disegnare linee parallele, o di offset, utilizzando lo strumento Linea di offset. Questa opzione è utile per creare forme 2D che possono essere successivamente estruse per assomigliare a muri 3D.

![](../.gitbook/assets/image%20%283%29.png)

Lo strumento **Linea di offset** funziona come lo strumento [**Linea** ](https://windows.help.formit.autodesk.com/tool-library/line-tool):

* Fare clic per impostare il primo punto, quindi spostare il cursore e posizionare i punti successivi, eseguendo lo snap alla geometria esistente o agli assi di deduzione.
* Viene mostrata un'anteprima della forma risultante. Il secondo e il terzo punto determinano il piano per il resto dei punti da seguire, pertanto il risultato è piano.
* Continuare ad aggiungere punti e premere **ESC** oppure fare doppio clic per terminare lo strumento.
* Eventuali autointersezioni verranno corrette e unite, lasciando un'unica superficie estrudibile.

![Dopo aver posizionato 2 punti e aver trascinato il terzo punto](../.gitbook/assets/walls1.png)

La linea di input viene disegnata in rosso e, per default, viene posizionata al centro delle linee di offset.

È possibile modificare l'allineamento delle linee di offset e il relativo spessore premendo il tasto **TAB**. Verrà aperta la finestra di dialogo **Opzioni strumento**:

![Opzioni per lo strumento Linea di offset](../.gitbook/assets/walls2.png)

Modificare **Allineamento** in **Sinistra** e **Spessore** in 6", ad esempio, e le linee di offset verranno disegnate a sinistra delle linee di input, a 6 pollici di distanza.

![](../.gitbook/assets/walls3.png)

## Suggerimenti utili

È possibile disegnare una forma chiusa eseguendo lo snap al primo punto posizionato. L'angolo risultante verrà corretto automaticamente:

![](../.gitbook/assets/walls4.png)

È possibile disegnare liberamente le linee di input l'una sopra l'altra. Al termine dello strumento, le intersezioni risultanti vengono corrette.

![](../.gitbook/assets/walls5.png)

![](../.gitbook/assets/walls6.png)

Di per sé, lo strumento Linea di offset deve generare la geometria su un piano, in modo che i primi punti determinino il piano che seguiranno i punti rimanenti.

Iniziare a disegnare sul lato di un cubo, ad esempio, per utilizzare il piano di tale superficie. Dopo aver posizionato tre punti non collineari, il piano di input è fisso per il resto dell'input. Notare che quando si disegna su una superficie, la forma risultante viene inserita nella superficie, dividendola in più superfici. Per evitare l'inserimento, la superficie disegnata deve far parte di un [gruppo](https://windows.help.formit.autodesk.com/tool-library/groups).

![Disegno su una superficie verticale](../.gitbook/assets/walls7.png)

![Una volta chiuso lo strumento, le linee vengono inserite e le superfici di divisione possono essere ulteriormente modificate](../.gitbook/assets/walls8.png).

È inoltre possibile utilizzare lo strumento Linea di offset per eseguire il tracciamento da un disegno di pianta. Importare la pianta come immagine.

* Ridimensionare l'immagine in modo che la pianta abbia la scala corretta. Questa procedura è descritta in maggior dettaglio [qui](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/work-with-images-and-the-ground-plane).
* È possibile utilizzare la vista della [cinepresa Ortogonale](orthographic-camera.md) per eseguire il tracciamento in una [vista dall'alto](orthographic-views.md) ortogonale.

![](../.gitbook/assets/walls9.png)

![](../.gitbook/assets/walls10.png)



