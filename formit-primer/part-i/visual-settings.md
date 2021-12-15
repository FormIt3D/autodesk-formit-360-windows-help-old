# 1.12 — Style wizualne

_Modelowanie brył koncepcyjnych to tylko połowa możliwości oferowanych przez program FormIt. Druga połowa to piękne grafiki, które pomagają przedstawić opowieść klientowi lub członkowi zespołu. W tym rozdziale omówiono sposoby konfigurowania_ _**graficznych stylów wizualnych**_ _i tworzenia animacji._

_Jeśli ostatnia sekcja nie została ukończona, pobierz i otwórz plik_ _**1.12 – Visual Styles.axm**_ _z zestawów danych_ _**FormIt Primer Part 1 Datasets**._

## **Tworzenie animacji**

_W ramach następnych kroków dowiemy się, jak tworzyć animacje za pomocą_ _**Scen**_ _._

1 — Aby utworzyć pierwszą **scenę**:

1. Włącz wszystkie warstwy z wyjątkiem warstw **Terrain**, **Plan Image** i **Massing**.
2. Upewnij się, że jako tryb kamery ustawiono opcję **Perspektywa \(VP\)**, i skieruj kamerę tak, aby jej pole widzenia obejmowało cały dom z nieznacznie podwyższonej pozycji, podobnie jak na poniższym rysunku.
3. Otwórz **paletę Sceny**.
4. Kliknij ikonę **+**, aby utworzyć nową scenę z bieżącego widoku.
5. Zmień jego nazwę na **Aerial View 1** i dopasuj pozostałe **Właściwości sceny** do tego, co pokazano na poniższym rysunku.

![](../../.gitbook/assets/0%20%2817%29.png)

2 — Aby utworzyć drugą **scenę**, a następnie dodać animację między nimi:

1. Dostosuj kamerę do nowego położenia, tak aby oglądać dom pod innym kątem. Utwórz nową **scenę** o nazwie **Aerial View 2**, stosując ten sam proces, który przeprowadzono w poprzednim kroku.
2. Kliknij przycisk **Odtwórz**. Po ustawieniu opcji **Czas wstrzymania** na **2 sekundy** animacja zacznie powoli poruszać się w jednym i drugim kierunku między dwoma scenami. Operacja będzie kontynuowana do momentu kliknięcia przycisku **Zatrzymaj** w celu zatrzymania animacji.

![](../../.gitbook/assets/1%20%2812%29.png)

_**Uwaga:**_ _Można dostosować_ _**Czas wstrzymania**,_ _**Czas przejścia** i_ _**Prędkość kamery**_ _za pomocą ustawień na dole okna dialogowego_ _**Właściwości sceny**. Spróbuj dodać więcej scen i dostosować animację, eksperymentując z wartościami tych ustawień._

## **Dostosowywanie stylów wizualnych**

_Teraz utworzymy kolejną scenę z pewnymi dostosowanymi ustawieniami **stylów wizualnych**._

1 — Najpierw otwórz **paletę Style wizualne**. Należy pamiętać, że u góry znajdują się cztery \(4\) karty, z których każda zawiera różne ustawienia wizualne: **Powierzchnie**, **Krawędzie**, **Środowisko** i **Diagnostyka modelu**. Aby dowiedzieć się więcej na temat każdej karty, zapoznaj się z rozdziałem **Style wizualne** w sekcji **Biblioteka narzędzi**.

2 —— Aby dostosować niektóre ustawienia na **karcie Powierzchnia**:

1. Włącz opcję **Cienie \(DS\)**.
2. Włącz opcję **Cienie otoczenia \(DA\)**.
3. Włącz opcję **Powierzchnie monotone \(DM\)**. Spowoduje to utworzenie abstrakcyjnego czarno-białego obrazu bez użycia żadnych materiałów.

![](../../.gitbook/assets/2%20%2820%29.png)

3 — Aby dostosować niektóre ustawienia na **karcie Krawędź**:

* 
   1. Dostosuj suwaki, aby rozjaśnić kontrast dla opcji **Krawędzie** do wartości około **30%**.
   2. Włącz opcję **Wydłuż krawędzie \(DX\).**
   3. Dostosuj suwaki, aby rozjaśnić kontrast dla opcji **Sylwetki** do wartości **30%**.

![](../../.gitbook/assets/3%20%2811%29.png)

4 — Aby dostosować niektóre ustawienia na **karcie Środowisko**:

1. Wyłącz opcję **Osie**.
2. Wyłącz opcję **Poziomy**, jeśli jest włączona.

![](../../.gitbook/assets/4%20%288%29.png)

5 — Utwórz nową scenę o nazwie **Customized Scene**, aby zapisać te ustawienia. Teraz można przełączać się między **scenami**, aby resetować ustawienia grafiki.

![](../../.gitbook/assets/5%20%286%29.png)

_**Uwaga**: Po wyczyszczeniu właściwości_ _**Kamera**_ _nowej sceny możesz za jej pomocą jedynie przełączać ustawienia wizualne utworzone przed chwilą bez przesuwania położenia kamery. Spróbuj przejść do jednej z poprzednich scen widocznych z lotu ptaka („Aerial...”), a następnie kliknij dwukrotnie pozycję_ _**Customized Scene**_ _i obserwuj, co się stanie._

_**Uwaga:**_ _Aby dowiedzieć się więcej na temat_ _**diagnostyki stylów wizualnych**_ _i zaawansowanych zastosowań_ _**scen**, zapoznaj się z częścią_ _**Primer Part II**._

