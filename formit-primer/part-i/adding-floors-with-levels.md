# 1.4 — Dodawanie kondygnacji z poziomami

_Poziomy umożliwiają tworzenie płatów brył z odniesieniami do poszczególnych kondygnacji i obliczanie powierzchni całkowitej na bryłę budynku. Poziomy programu FormIt i ich nazwy niestandardowe zostaną przekształcone w poziomy programu Revit po przekonwertowaniu pliku na format programu Revit._

_Jeśli nie ukończono poprzedniej sekcji, pobierz i otwórz plik**1.4 — Add Floors with Levels.axm** z folderu **FormIt Primer Part 1 Datasets**._

## **Tworzenie i dostosowywanie poziomów**

1 — Aby utworzyć poziomy:

1. Przejdź do **palety Poziomy** na **pasku palet**.
2. Kliknij przycisk **+** \(**Dodaj poziom**\) cztery razy, aby utworzyć cztery poziomy.
3. Kliknij dwukrotnie bieżącą rzędną każdego poziomu, aby zmienić je na: **0’-0", 2'-2", 4’-6"** i **17’-8"**.
4. Kliknij dwukrotnie bieżącą nazwę każdego poziomu i zmień je na: **Ground, Terrace, Main Building** i **Top of Roof.**

![](../../.gitbook/assets/0%20%2816%29.png)

_**Uwaga**: Możesz kliknąć ikonę_ _**++**_ _w celu utworzenia wielu poziomów z określonymi i jednakowymi odstępami między nimi. Jest to przydatne w przypadku budynków wielokondygnacyjnych_.

## **Stosowanie poziomów do geometrii**

_W poprzednich krokach tylko utworzyliśmy poziomy. Teraz możemy zastosować te poziomy do utworzonej geometrii._

1 — Aby zastosować poziomy do istniejącej geometrii:

1. Wybierz całą bryłę górnego tarasu, klikając ją dwukrotnie.
2. Na **palecie Właściwości** kliknij opcję **Użyj poziomów**. W tym kroku zostaną wstępnie wybrane wszystkie poziomy, które aktualnie przecinają wybraną geometrię.
3. Obecnie wybrana geometria ma zastosowane trzy poziomy \(**Main Building, Terrace** i **Ground**\), ale w tym ćwiczeniu chcemy zastosować tylko poziom **Ground**. Anuluj zaznaczenie pól wyboru **Main Building** i **Terrace**.
4. Ten proces zapewnia uwzględnienie w obliczeniach powierzchni całkowitej tylko powierzchni przeciętej przez poziom **Ground**, co widać w polu **Powierzchnia wg poziomu**.

![](../../.gitbook/assets/1%20%284%29.png)

_**Uwaga**: Jeśli na bryle nie widać niebieskich linii poziomu, wpisz_ _**DL**_ _w polu_ _**Wyświetl poziomy**._

![](../../.gitbook/assets/2%20%283%29.png)

