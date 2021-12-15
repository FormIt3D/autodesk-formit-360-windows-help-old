# 1.10 — Grupy obliczeniowe w dodatku Dynamo

_W tym rozdziale wykorzystamy moc obliczeniową dodatku_ [_**Dynamo**_](http://dynamobim.org/)_, aby umieścić i zmodyfikować elastyczne grupy powiązane z przykładami wykresów OOTB Dynamo._

_Jeśli ostatnia sekcja nie została ukończona, pobierz i otwórz plik_ _**1.10 – Computational Groups with Dynamo.axm**_ _z zestawów danych_ _**FormIt Primer Part 1 Datasets**._

_Więcej informacji na temat sposobu współpracy programu FormIt z dodatkiem Dynamo w procesach roboczych projektowania obliczeniowego_ [_**można znaleźć tutaj**_](http://formit.autodesk.com/page/formit-dynamo)_._

## **Tworzenie schodów dolnego tarasu**

1 — Upewnij się, że warstwy **Lower Terrace, Main Building Floor** i **Plan Image** są włączone, ponieważ właśnie tam zostaną dodane schody.

2 — Aby umieścić grupę schodów powiązaną z jednym z przykładów OOTB Dynamo Samples:

1. Otwórz **paletę Dynamo** na pasku palet. W katalogu **Dynamo Samples** powinno być widocznych kilka wbudowanych obiektów dodatku Dynamo.
2. Kliknij raz przykład dodatku Dynamo **Stairs**, aby przenieść go do obszaru modelu. Program FormIt uruchomi wykres w tle i na podstawie tego wykresu wygeneruje geometrię schodów.
3. Przesuń kursor na obszar rysunku. Po wczytaniu schodów półprzezroczysty podgląd ich geometrii będzie przesuwał się wraz ze wskaźnikiem myszy. Przesuń kursor na obszar rysunku w pobliżu tarasu i kliknij, aby umieścić tam schody. Naciśnij klawisz **Esc**, aby usunąć zaznaczenie. Zwróć uwagę, że po umieszczeniu schodów automatycznie zostanie otwarta **paleta Właściwości**.

![](../../.gitbook/assets/0%20%2815%29.png)

_**Uwaga:**_ [_**Możesz również dołączać katalogi lokalne**_](https://formit.autodesk.com/page/formit-dynamo#dynamo-getting-started) _zawierające wykresy Dynamo i uruchamiać własne lokalne wykresy Dynamo, podobnie jak w tych przykładach._

3 — Aby zaktualizować wymiary schodów:

1. Po wybraniu grupy schodów zmodyfikuj dane wejściowe dostępne w sekcji **INPUTS** dodatku Dynamo u dołu **palety Właściwości**, aby były zgodne z poniższą ilustracją. Po wybraniu większości grup utworzonych za pomocą skryptów Dynamo w ich właściwościach znajduje się sekcja dodatku Dynamo.
   * Add Top Landing = False
   * Add Middle Landing = False
   * Add Bottom Landing = False
   * Floor-to-Floor Height = 2,6
   * Stair Width = 12
   * Riser Height = 0,6
   * Tread Length = 1,25
   * Tread Overlap = 0,25
   * Tread Thickness = 0,25
   * Height Between Middle Landings = \(nie dotyczy, ponieważ nie jest tworzony środkowy podest\)
   * Middle Landing Length = \(nie dotyczy, ponieważ nie jest tworzony środkowy podest\)
   * Top/Bottom Landing Length = \(nie dotyczy, ponieważ nie jest tworzony żaden podest\)
2. Kliknij przycisk **Run**, aby uruchomić ponownie skrypt Dynamo przy użyciu zaktualizowanych wartości danych wejściowych.
3. Przesuń grupę odpowiednio do potrzeb, aby umieścić schody we właściwym położeniu zgodnie z warstwą **Plan Image**. Uważaj, aby podczas przesuwania nie zmienić rzędnej grupy schodów. Więcej na temat sztuczek i technik stosowanych podczas przesuwania elementów modelu można dowiedzieć się z poprzednich rozdziałów.

![](../../.gitbook/assets/1%20%2811%29.png)

_**Uwaga ‌:**_ _Dane wejściowe_ _**Floor-to-Floor Height**_ _to przybliżona wartość całkowitej wysokości schodów. Parametr_ _**Riser Height**_ _faktycznie definiuje wysokość schodów. W tym przykładzie ustawiamy wartość parametru_ _**Floor-to-Floor Height**_ _na 2,6’, ale ostateczna wysokość schodów wynosi 3,0’ \(0,6’ \(**Riser Height**\) x 5 \(liczba podstopnic\)\). Ponieważ rozpiętość między podłożem a górną powierzchnią stropu tarasu wynosi 3’-2”, pozostałe 2” znajdują się w górnej podstopnicy._

## **Tworzenie schodów budynku głównego**

_W poprzednich krokach utworzyliśmy schody bez podestów. Teraz utworzymy schody korzystające z górnego podestu dopasowanego do warstwy_ _**Main Building Floor**._

1 — Zacznij od utworzenia kopii właśnie utworzonych schodów:

1. Wybierz istniejące schody, a następnie kliknij w dowolnym miejscu na warstwie **Plan Image**, aby uruchomić polecenie przesuwania. Spowoduje to, że program FormIt użyje rzędnej warstwy **Plan Image** jako początkowej wysokości odniesienia do umieszczenia nowej kopii. Naciśnij klawisz **Ctrl**, aby utworzyć **szybką kopię**.
2. Przesuń kursor bliżej głównego budynku powyżej tarasu. Zwróć uwagę, że teraz górna powierzchnia tarasu jest nową płaszczyzną odniesienia. Kliknij, aby umieścić grupę.

![](../../.gitbook/assets/2%20%289%29.png)

_**Uwaga:**_ _Ponieważ warstwa_ _**Plan Image**_ _znajduje się na płaszczyźnie_ _**Ground Level**_ ___**narzędzie Przesuń**_ _będzie używało tej płaszczyzny jako odniesienia dla punktu początkowego. Na powyższej ilustracji zwróć uwagę na etykietkę narzędzia_ _**On Face**_ _wskazującą, że jako odniesienie początkowe została wybrana powierzchnia warstwy Plan Image, a jako odniesienie końcowe — górna powierzchnia warstwy_ _**Lower Terrace Floor**__._

2 — Użyj narzędzia **Ustaw jako niepowtarzalny \(MU\)**, aby zmiana danych wejściowych tych schodów w dodatku Dynamo nie wpłynęła na dolne schody. Zmień położenie grupy odpowiednio do potrzeb, aby znajdowała się ona blisko położenia końcowego — dostosujemy to później. Możesz przełączyć widoczność warstwy **Lower Terrace**, aby wyświetlić poniższy rzut, co ułatwi jego umieszczenie, ale uważaj, aby nie zmienić rzędnej nowych schodów podczas ich przesuwania.

3 — Na **palecie Właściwości** zaktualizuj dane **Dynamo Inputs**, jak pokazano poniżej, i jeszcze raz uruchom skrypt.

* Add Top Landing = True
* Floor-to-Floor Height = 2,333
* Riser Height = 0,466
* Tread Length = 1,5
* Top/Bottom Landing Length = 2,5

![](../../.gitbook/assets/3%20%281%29.jpeg)

_**Uwaga:**_ _Jeśli ustawisz dla parametru_ _**Add Bottom Landing**_ _wartość_ _**True**_ _i uruchomisz ponownie skrypt, górna powierzchnia dolnego podestu powinna pasować do górnej powierzchni warstwy_ _**Lower Terrace Floor**. Dzieje się tak, ponieważ — w odróżnieniu od poprzednich schodów — dopasowaliśmy parametr_ _**Riser Height**_ _do rzeczywistej wysokości parametru_ _**Floor-to-Floor Height**__, jaką chcemy uzyskać \(2’-4” lub 2,333’\)._

2 — Ponownie zmień położenie grupy na końcowe. Górny podest powinien być równoległy do warstwy **Main Building Floor**.

3 — Aby zakończyć tworzenie schodów, dodaj do nich materiał **Stone — Travertine**, aby dopasować go do kondygnacji. Więcej informacji na temat sposobu stosowania materiałów można znaleźć w poprzednich rozdziałach.

