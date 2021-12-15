# 1.15 — Praca z programem Revit

_Jedną z najbardziej ekscytujących funkcji programu FormIt jest możliwość przenoszenia modelu z elastycznego środowiska modelowania, takiego jak program FormIt, do zaawansowanego środowiska parametrycznego, takiego jak program Revit. W tym rozdziale omówimy kilka ćwiczeń, które obejmują przenoszenie różnych elementów z programu FormIt do programu Revit i odwrotnie._

_W tym rozdziale zostaną użyte przykładowe rodziny programu Revit. Jeśli jeszcze nie zostało to zrobione, można je pobrać z zestawu danych **Farnsworth House Data Set.** Jeśli nie wykonano wszystkich czynności opisanych do tej pory w tym samouczku, można również pobrać i otworzyć plik **1.15 – Praca z plikiem Revit.axm** z **zestawów danych FormIt Primer Part 1 Datasets**._

_W tych ćwiczeniach będziemy używać programu Revit 2022, który zapewnia ulepszone możliwości współdziałania z programem FormIt. Poprzednie wersje programu Revit nie będą zawierać niektórych lub żadnych z elementów przedstawionych w tym samouczku i będą miały inny interfejs użytkownika._

## Z programu Revit do programu FormIt

### Konwertowanie rodzin programu Revit do użycia w programie FormIt

Jeśli użytkownik \(lub jego firma\) ma serię rodzin programu Revit, które mają być używane w programie FormIt, przydatne okaże się zapoznanie się z tą sekcją, w której opisano sposób zbiorczego eksportowania plików RFA do programu FormIt.

_**Uwaga:**_ _Poniżej przedstawiono interfejs i czynności niezbędne podczas korzystania z programu Revit 2022, ale narzędzia_ _**Konwertuj RFA na format programu FormIt**_ _są dostępne od wersji Revit 2016._

1 — Otwórz nowy projekt lub rodzinę programu Revit. Następnie:

1. Na wstążce **Dodatki** znajdź panel **Konwerter formatu FormIt** i kliknij przycisk **Konwertuj RFA na format programu FormIt**. Zostanie wyświetlone okno dialogowe **Konwertuj rodziny programu Revit**.
2. W polu **Ścieżka do pliku rodziny programu Revit** przejdź do dowolnego miejsca, w którym zapisano na komputerze następujący folder: **Farnsworth House Data Set &gt; Supporting Files &gt; Revit**.
3. W polu **Ścieżka do zawartości FormIt** przejdź do zestawu danych **Farnsworth House Data Set &gt; Supporting Files &gt; FormIt &gt; Custom FormIt Content**. Jeśli rozdział **1.11 — Importowanie modeli przy użyciu Biblioteki elementów** nie został jeszcze ukończony, może być konieczne utworzenie folderu **Custom FormIt Content** lub wybranie innego miejsca docelowego.
4. Kliknij przycisk **OK**, aby rozpocząć proces konwersji.

![](../../.gitbook/assets/0%20%2823%29.png)

_**Uwagi:**_

* _Ten proces zajmie trochę czasu, ponieważ program Revit otworzy plik_ _**RFA**_ _w pierwszej ścieżce, a następnie przekonwertuje go i zapisze w formacie_ _**AXMF**_ _dla programu FormIt._
* _W tym ćwiczeniu konwertujemy tylko jeden plik, ale w ramach tego procesu można zbiorczo przekonwertować wszystkie pliki_ _**RFA**_ _w wybranym folderze \(w tym wszystkie pliki_ _**RFA**_ _w folderach zagnieżdżonych\)._

2 — Po ukończeniu procesu wróć do programu FormIt. Na **Palecie Biblioteki elementów** pojawi się nowa zawartość wewnątrz folderu **FormIt &gt;** **Custom FormIt Content**, który wcześniej połączyliśmy. Jeśli przekonwertowane pliki **AXMF** zapisano w innym położeniu lub nie ukończono rozdziału **1.11 — Importowanie modeli przy użyciu Biblioteki elementów**, może być konieczne dodanie tego folderu do Biblioteki elementów, aby wyświetlić jego zawartość. Instrukcje dotyczące dodawania folderów do Biblioteki elementów znajdują się w rozdziale 1.11.

![](../../.gitbook/assets/1%20%2824%29.png)‌

**Uwaga**: _Nie wszystkie kategorie z programu Revit są obsługiwane podczas eksportowania. Rodziny „wolnostojące” i „poziom bazowy” są obsługiwane, ale rodziny „oparte na obiekcie nadrzędnym”, takie jak drzwi i okna, nie są obsługiwane. Obsługiwane są wszystkie następujące kategorie: bryła, zabudowa, otoczenie, meble, system mebli, model ogólny, parking, teren oraz wyposażenie specjalistyczne. Wszystkie nieobsługiwane rodziny w wybranym zawinięciu zostaną po prostu pominięte._

## Z programu FormIt do programu Revit

_Istnieją dwa różne sposoby przenoszenia geometrii z programu FormIt do programu Revit. Istniejący plik_ _**.axm** można zaimportować do projektu programu Revit lub pliku rodziny programu Revit i będzie on się zachowywać podobnie jak zaimportowany model lub plik CAD. Można również uruchomić program FormIt z poziomu programu Revit i przenieść poszczególne grupy programu FormIt do programu Revit jako pojedyncze elementy modelu ogólnego. Druga metoda jest opisana w rozdziale **Part II** __**2.8** __**Zaawansowane procesy robocze programu Revit**._

### Importowanie domu pani Farnsworth do programu Revit

1 — Aby zaimportować plik programu FormIt \(**.axm**\) do programu Revit, uruchom nowy projekt programu Revit i otwórz domyślny widok 3D. Następnie:

1. Przejdź do **karty Wstaw** i kliknij przycisk **Importuj CAD**. Zostanie otwarte okno **Importuj formaty CAD**.
2. Upewnij się, że lista rozwijana **Pliki typu** jest ustawiona na **Pliki FormIt \(\*.axm\)**.
3. Przejdź do pliku Farnsworth **.axm**, nad którym pracujesz, i wybierz go. W przypadku nieprześledzenia materiałów w części Primer Part I możesz również otworzyć plik **1.15 – Working With Revit.axm**, folder **Farnsworth House Data Set &gt; Chapter Files**.
4. Upewnij się, że zaznaczona jest opcja **Importuj poziomy FormIt**.
5. Po zdefiniowaniu ustawień kliknij przycisk **Otwórz**, a geometria programu FormIt zostanie przeniesiona do programu Revit jako pojedynczy element.

![](../../.gitbook/assets/2%20%2824%29.png)

Importowanie pliku programu FormIt za pomocą przycisku Importuj CAD.

![](../../.gitbook/assets/3%20%2821%29.png)  
Zaimportowany element .axm. Warto zauważyć, że poziomy z modelu programu FormIt są również importowane do programu Revit.

_Podobnie jak w przypadku innych formatów CAD, warstwy w oryginalnym pliku są importowane do programu Revit. Ta funkcja umożliwia zdefiniowanie różnych ustawień widoczności dla każdej warstwy, co ułatwia manipulowanie wyglądem graficznym pliku programu FormIt w dowolnym widoku programu Revit._

2 — Aby dostosować widoczność warstwy zaimportowanego pliku .axm:

1. Przejdź do okna **Nadpisania widoczności/grafiki \(VG lub VV\)**, na karcie **Kategorie importowane** rozwiń zaimportowany plik programu FormIt i wyczyść zaznaczenie warstwy **Planting**, aby wyłączyć warstwę w bieżącym widoku, a następnie kliknij przycisk **OK**.
2. Zmień ustawienie **Styl wizualny** na **Realistyczny**. Zobaczysz, że wszystkie materiały programu FormIt zostały zaimportowane do programu Revit.

![](../../.gitbook/assets/4%20%2820%29.png)

3 — W rzeczywistości zaimportowane materiały programu FormIt będą teraz dostępne w tym projekcie programu Revit oznaczonym klasą **FormIt**. Wystarczy otworzyć **Przeglądarkę materiałów** i wyszukać „FormIt”, aby zobaczyć je wszystkie. Można ich teraz używać w projekcie programu Revit tak samo jak innych materiałów.

![](../../.gitbook/assets/5%20%2819%29.png)

