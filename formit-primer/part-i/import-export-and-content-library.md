# 1.11 — Importowanie modeli przy użyciu Biblioteki elementów

_W tym rozdziale zaimportujemy istniejące modele programu SketchUp i użyjemy Biblioteki elementów programu FormIt do umieszczenia rodzin OOTB, które zostały przekształcone z formatu programu Revit. Pamiętaj, że pliki SKP otwierane w programie FormIt mają niezmienione materiały, grupy i komponenty, warstwy \(tagi\) oraz sceny. Dla utrzymania porządku w projektach może być konieczne ich oczyszczenie._

_W tym rozdziale będziemy używać plików z folderu_ **Farnsworth House Data Set &gt; Supporting Files**. Jeśli jeszcze tego nie zrobiono, pobierz wymagane foldery lub cały zestaw danych z folderu _**FormIt Primer Part 1 Datasets**._

## **Importowanie i edycja plików SKP**

_Najpierw przejdziemy przez proces dodawania jednego z pobranych elementów do osobistej Biblioteki elementów_. Pamiętaj, że w tym ćwiczeniu będziemy używać tylko plików SKP. Aby dowiedzieć się więcej na temat otwierania/importowania innych formatów plików, zapoznaj się z [**tym wpisem na blogu zawierającym informacje o funkcjach programu FormIt 2021.2**](https://formit.autodesk.com/blog/post/formit-2021-2-and-new-revit-add-in-now-available) i **tym rozdziałem na temat** **rozszerzonego zakresu formatów plików podczas importu i eksportu**.

1 — Pamiętaj o **zapisaniu \(Ctrl + S\)** całej otwartej pracy, a następnie rozpocznij nowy szkic programu FormIt. W tym celu wykonaj jedną z następujących czynności:

1. Otwórz kolejną sesję w nowym oknie programu FormIt, klikając prawym przyciskiem myszy ikonę programu FormIt na **pasku zadań systemu Windows** i klikając ikonę **FormIt**. Spowoduje to otwarcie nowego okna programu FormIt, dzięki czemu możesz mieć uruchomione dwie równoległe sesje programu FormIt.
2. LUB po zapisaniu pliku wybierz polecenie **Nowy szkic \(Ctrl + N\)** z listy rozwijanej **Plik** na pasku **Menu główne**.

![](../../.gitbook/assets/0%20%2819%29.png)

2 — Utwórz nowy folder o nazwie **Custom FormIt Content** w folderze **Farnsworth House Data Set &gt; Supporting Files &gt; FormIt** w zestawie danych _**Farnsworth House Data Set**._

3 — **Zapisz \(Ctrl + S\)** nowy szkic w tym folderze. Zalecamy nadanie mu nazwy **Ottoman — Barcelona\_Mies.axm**

4 — W nowym pustym pliku programu FormIt:

1. **Zaimportuj plik lokalny \(Ctrl + I\)**, wybierając opcję **Importuj &gt; Lokalnie** z listy rozwijanej **Plik** na pasku **Menu główne**.
2. Wybierz plik **Ottoman — Barcelona\_Mies.skp** z folderu **Farnsworth House Data Set &gt; Supporting Files &gt; SketchUp** i kliknij przycisk **Otwórz**.

_**Uwaga:**_ _jeśli nie widzisz_ _**pliku Ottoman — Barcelona\_Mies.skp**, upewnij się, że na liście rozwijanej Format pliku w prawym dolnym rogu wybrano_ _**Wszystkie obsługiwane formaty**._

![](../../.gitbook/assets/1%20%287%29.png)

5 — Zmień nazwę zaimportowanej grupy na **Ottoman — Barcelona\_Mies**.

6 — Po zaimportowaniu tego modelu do pliku zawierającego projekt domu pani Farnsworth zostanie on umieszczony zgodnie z punktem **Początek** tego pliku. Aby sterować punktem umieszczenia, przesuniemy grupę **Ottoman — Barcelona\_Mies** w taki sposób, aby jeden z jej narożników znajdował się w punkcie **Początek**. Aby to wykonać:

1. Upewnij się, że opcja **Przyciągaj do siatki \(SG\)** jest włączona. Narysuj **linię \(L\)** odniesienia, rozpoczynającą się w punkcie **Początek** \(tam, gdzie przecinają się osie X, Y i Z\). Kliknij w dowolnym miejscu, aby umieścić drugi punkt.
2. Wybierz grupę stołka i uruchom polecenie Przesuń, klikając jeden raz lewy dolny narożnik nogi mebla, jak pokazano na ilustracji. _Aby dowiedzieć się więcej na temat przesuwania obiektów, zapoznaj się z poprzednimi rozdziałami._
3. Przesuń grupę do punktu **Początek**, przyciągając ją do punktu początkowego narysowanej poprzednio linii odniesienia.
4. Usuń linię odniesienia.

![](../../.gitbook/assets/2%20%2817%29.png)

7 — Zalecamy usunięcie wszelkich niepożądanych warstw zaimportowanych wraz z plikiem SKP, ponieważ wszystkie warstwy tego modelu zostaną ostatecznie zaimportowane do modelu domu pani Farnsworth. W tym celu przejdź do **palety Warstwy**, wybierz **Warstwę 0** i kliknij przycisk **–**. Spowoduje to usunięcie warstwy, ale bez usuwania leżącej na niej geometrii.

![](../../.gitbook/assets/3%20%2816%29.png)

_**Uwaga:**_ _po usunięciu warstwy geometria lub grupy, które znajdowały się na tej warstwie, otrzymują wartość_ _**Brak warstwy**, czyli wartość domyślną dla każdego obiektu, który nie został jeszcze przypisany do żadnej warstwy._

## **Tworzenie miniatury elementu**

_W tym kroku zostanie skonfigurowana scena, która będzie używana jako miniatura_ _**elementu**_ _wyświetlana na_ _**palecie Biblioteka elementów**._

1 — Zdefiniuj ustawienia widoku dla sceny używanej jako miniatura:

1. Na karcie **Środowisko** na **palecie Style wizualne** usuń zaznaczenie wszystkich pól wyboru i ustaw kolor **Dolny/Tło** na biały.
2. Upewnij się, że ustawiono tryb widoku **Perspektywa** **\(VP\)**.
3. Użyj **narzędzi nawigacji w widoku**, aby powiększyć widok i wybrać położenie kamery, w którym obiekt jest dobrze widoczny, podobnie jak na poniższej ilustracji.

![](../../.gitbook/assets/4%20%2813%29.png)

2 — Aby zapisać powyższe ustawienia, utwórz scenę:

1. Przejdź do **palety Scena**.
2. Kliknij przycisk **+**. Spowoduje to utworzenie nowej sceny na podstawie bieżących ustawień.
3. Zmień nazwę na **Miniatura** i upewnij się, że zaznaczone są co najmniej cztery \(4\)pierwsze pola wyboru: **Kamera**, **Warstwy**, **Słońce i cienie** i **Style wizualne**. Pozostałe ustawienia sceny nie są istotne przy tworzeniu obrazu miniatury.
4. Użyj przycisku **Aktualizuj scenę** zawsze, gdy chcesz odświeżyć **Scenę** zgodnie z bieżącym widokiem kamery i ustawieniami wizualnymi.

![](../../.gitbook/assets/5%20%2811%29.png)

3 — **Zapisz \(Ctrl + S\)** ponownie ukończony model stołka. Pamiętaj, że **miniatura zawartości** jest tworzona na podstawie bieżącego widoku przy ostatnim zapisaniu modelu, dlatego przed zapisaniem należy się upewnić, że jest widoczna **scena miniatury**.

_Jeśli chcesz, możesz porównać swój plik z naszym, otwierając plik_ _**Ottoman — Barcelona\_Mies.axm**_ _zapisany w folderze_ _**Farnsworth House Data Set &gt; Supporting Files &gt; FormIt &gt; Furniture**_ _w zestawie danych_ _**Farnsworth House Data Set**.‌_

_Możesz wykonać powyższe czynności również z plikami SKP ławki i fotela, znajdującymi się w tym samym folderze co plik stołka._

_**Wskazówka:**_ _aby przyspieszyć ten proces, zalecamy użycie utworzonego właśnie pliku_ _**Ottoman — Barcelona\_Mies.axm**_ _jako szablonu. Podczas modelowania można ponownie włączyć_ _**Siatkę**_ _i_ _**Osie**_ _przy użyciu_ _**palety Style wizualne**. Dopasowując tylko położenie kamery __**sceny miniatury**__ dla każdego mebla, możesz mieć pewność, że_ _**miniatury elementów**_ _pozostaną spójne dla modeli wszystkich elementów._

## **Łączenie biblioteki elementów**

_Wróćmy teraz do projektu domu pani Farnsworth. Zobaczymy, jak połączyć folder **FormIt** w zestawie danych **Farnsworth House Data Set**, aby móc łatwo uzyskać dostęp do wszystkich zawartych w nim plików — w tym do utworzonego właśnie folderu_ **Custom FormIt Content** _— z poziomu projektu._

1 — Wróć do modelu domu pani Farnsworth lub otwórz go ponownie. _Jeśli nie ukończono poprzedniego rozdziału, pobierz i otwórz plik_ _**1.11 — Import Models with Content Library.axm**_ _z zestawu danych_ _**Farnsworth House Data Set**._

1. Otwórz **paletę Biblioteka elementów** i kliknij ikonę **Połącz katalog biblioteki elementów**. Zostanie wyświetlone okno **Preferencje** z otwartą kartą **Biblioteka elementów**.
2. Kliknij ikonę **+**, aby **dodać nowe położenie biblioteki elementów**. Zostanie wyświetlone trzecie okno, w którym można przeglądać katalog komputera i wybrać folder.
3. W zestawie danych _**Farnsworth House Data Set** przejdź kolejno do folderów_ _**Supporting Files &gt; FormIt**. Znajdują się tam_ foldery zawierające pliki **.axm** utworzone wcześniej w tym rozdziale. Kliknij dwukrotnie folder **FormIt**, aby go wybrać.
4. Kliknij przycisk **Wybierz folder**, a ścieżka do folderu zostanie wyświetlona w panelu **Położenia biblioteki — lokalne**.
5. W oknie **Preferencje** kliknij przycisk **OK**, aby dodać połączony folder do **Biblioteki elementów**.
6. Aby uzyskać dostęp do nowej biblioteki, otwórz menu rozwijane u góry **palety Biblioteka elementów** i wybierz bibliotekę **FormIt**.
7. Zwróć uwagę, że na **palecie Biblioteka elementów** będzie widoczna struktura folderów i wszystkie pliki **axm** w połączonym folderze. Kliknij dwukrotnie dowolny podfolder, aby uzyskać dostęp do zawartych w nim plików.

![](../../.gitbook/assets/link-library-content.png)

**Uwaga:** jeśli masz dostęp do usługi **Autodesk Docs** \(wcześniej Autodesk 360\), również możesz uzyskać dostęp do zapisanych tam plików za pomocą menu rozwijanego **Biblioteka elementów**.

## **Wstawianie elementu z biblioteki**

_‌Teraz umieścimy utworzone elementy w modelu domu pani Farnsworth._

1 — Aby można było zobaczyć wnętrze domu i umieścić meble, wyłącz warstwę **Dach** i **obróć \(O\)** widok perspektywiczny do momentu, gdy będzie widać całą podłogę budynku głównego.

2 — Wróć do **palety Biblioteka elementów** i upewnij się, że na liście rozwijanej nadal wybrana jest biblioteka **FormIt**. Przed umieszczeniem utworzonych mebli trzeba jeszcze umieścić „rdzeń” domu:

1. Kliknij folder o nazwie **Other**, aby go otworzyć, a następnie kliknij miniaturę **Farnsworth House — Core**, aby ją wybrać.
2. Umieść wskaźnik myszy na **podłodze budynku głównego**, a następnie kliknij **Centroidę** podłogi w celu umieszczenia elementu **Core**.
3. Aby wrócić do folderu FormIt, użyj przycisku **Przejdź w górę**.

![](../../.gitbook/assets/7%20%282%29.jpeg)

3 — Ustaw kamerę na tryb **Ortogonalny \(VO\)** i **Widok z góry \(VT\)**, a następnie wyłącz **podłogę głównego budynku**, aby pokazać **obraz rzutu**. Więcej informacji na temat ustawień **widoków** i **warstw** można znaleźć w poprzednich rozdziałach.

4 — Wybierz element **Farnsworth House — Core** i przesuwaj go, aż będzie on dobrze dopasowany do obrazu rzutu.

![](../../.gitbook/assets/8%20%281%29.png)

_**Uwaga:**_ _podczas przesuwania elementu_ _**Core** należy uważać, aby nie zmienić jego rzędnej. Można użyć klawisza_ _**Shift**_ _, aby ograniczyć ruch tylko do jednej z osi, lub ustawić początkowy i końcowy punkt odniesienia polecenia_ _**Przesuń \(M\)**_ _na tej samej wysokości, klikając tylko_ _**Obraz planu**, a nie sam element_ _**Core**_ _. Zapoznaj się z poprzednimi rozdziałami, aby dowiedzieć się więcej na temat narzędzia_ _**Przesuń \(M\)**_ _.‌_

## **Umieszczanie mebli z biblioteki**

1 — W podobny sposób możesz teraz umieścić meble z folderu **Custom FormIt Content** utworzone we wcześniejszej części rozdziału. Jeśli nie przekształcono wszystkich trzech \(3\) plików SKP, możesz użyć zamiast tego gotowych wersji, które znajdują się w folderze **Meble**.

_**Uwagi:**_

* _Ponownie włącz warstwę_ _**Podłoga budynku głównego**_ _, aby umieścić meble bezpośrednio na powierzchni_ _**podłogi budynku głównego**._
* _Podczas umieszczania nowego obiektu użyj klawisza_ _**Tab**_ _, aby przełączać się między płaszczyznami umieszczania._
* _Podczas umieszczania nowego obiektu użyj klawisza_ _**Spacja**_ _, aby przed umieszczeniem obrócić obiekt o 90 stopni za jednym razem._

![](../../.gitbook/assets/9%20%283%29.png)

2 — Analogicznie, jeśli chcesz umieścić elementy OOTB, zobacz **Przykłady biblioteki zawartości**. Pamiętaj, że w przypadku wielu z nich można wybrać jeden z kilku różnych rozmiarów, podobnie jak w przypadku typów rodzin w programie Revit.

![](../../.gitbook/assets/10%20%286%29.png)

## **Korzystanie z narzędzia Skala**

1 — Korzystając z poznanych technik, umieść jedno wystąpienie elementu **tree\_pine** z folderu **Farnsworth House Data Set &gt; FormIt &gt; Planting**.

1. Po umieszczeniu wybierz grupę i zmień jej nazwę na **Drzewo**. Kliknij prawym przyciskiem myszy, aby otworzyć **menu kontekstowe** i wybierz opcję **Skala niejednorodna \(NU\)**.
2. Kliknij jeden z **przycisków skali niejednorodnej**, aby zmienić rozmiar i proporcje grupy **Drzewo** odpowiednio do potrzeb.

![](../../.gitbook/assets/11%20%283%29.png)

![](../../.gitbook/assets/12%20%282%29.png)

_**Uwaga:**_ _w podobny sposób można użyć narzędzia_ _**Skala \(SC\)**_ _, aby zmienić skalę całego modelu lub grupy w jednorodny sposób._

2 — Skopiuj tę grupę i umieść wiele drzew wokół domu, używając **narzędzi skali**, aby utworzyć drzewa o różnych rozmiarach i proporcjach.

![](../../.gitbook/assets/13%20%286%29.png)

_**Uwaga:**_ _mimo że wszystkie drzewa są wystąpieniami tej samej grupy, można_ _**skalować**_ _je do różnych rozmiarów. Użycie narzędzi_ _**Skala \(SC\)**_ _i_ _**Skala niejednorodna \(NU\)**_ _poza trybem edycji grupy umożliwia modyfikowanie poszczególnych wystąpień tej samej grupy. Gdybyśmy edytowali jedną z grup_ _**Drzewo**_ _i zmodyfikowali jego geometrię lub materiał, wszystkie wystąpienia grupy zostałyby zaktualizowane, ale każde z nich zachowałoby swoją bieżącą skalę niestandardową. Spróbuj._

### **Porządkowanie modelu**

_Pamiętaj, aby zawsze sortować dodane elementy na warstwach. W tym przykładzie zalecamy umieszczenie rdzenia i wszystkich mebli na warstwie_ _**Podłoga głównego budynku**_ _, a drzew na nowej warstwie o nazwie_ _**Zieleń**._

