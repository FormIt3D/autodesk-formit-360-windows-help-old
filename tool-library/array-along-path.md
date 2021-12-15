# Array Along Path

## Obsługiwane przez dodatek Dynamo

W programie FormIt 2021 i nowszych wersjach można ustawiać obiekty w szyku wzdłuż ścieżki i szybko dostosowywać wyniki lokalnie. Szyk wzdłuż ścieżki jest obsługiwany przez dodatek Dynamo, co oznacza, że można go łatwo skonfigurować, aby uzyskać żądane wyniki, a ponowne uruchomienie logiki spowoduje zaktualizowanie geometrii lokalnie.

![](../.gitbook/assets/array-along-path.gif)

## Uruchamianie przykładu Array Along Path

* Przejdź do panelu Dynamo w programie FormIt dla systemu Windows i upewnij się, że znajdujesz się w katalogu Dynamo Samples.
* Kliknij przykład Array Along Path.
* Po lewej stronie ekranu zostanie wyświetlony monit „Select object\(s\) to array”.
   * W tym kroku możesz wybrać dowolne połączenie obiektów programu FormIt.
   * Po wybraniu elementu możesz kliknąć strzałkę „next” po lewej stronie ekranu lub po prostu nacisnąć klawisz Enter.
* Teraz zostanie wyświetlony monit „Select path for array”.
   * W tym miejscu należy wybrać tylko serię przylegających krawędzi lub grupę zawierającą serię przylegających krawędzi.
   * Po wybraniu ścieżki kliknij przycisk „finish” lub naciśnij klawisz Enter.
* W panelu Dynamo będzie wyświetlana informacja o przetwarzaniu zmian. Po zakończeniu szyk wygenerowany przez dodatek Dynamo będzie dostępny w grupie FormIt i będzie można go modyfikować \(patrz poniżej\).

## Iteracja lokalna

Po uruchomieniu narzędzia Array Along Path wyniki jego działania będą miały wartości domyślne, dlatego należy zmodyfikować je odpowiednio do potrzeb.

Gdy narzędzie Array Along Path jest uruchomione, tworzona jest nowa grupa zawierająca wyniki, a polecenie FormIt automatycznie wybiera grupę i wyświetla dostępne opcje dla wystąpienia tego narzędzia.

W każdej chwili można wrócić do właściwości narzędzia Array Along Path, wybierając grupę i przełączając się na panel Właściwości lub edytując grupę, co spowoduje automatyczne wyświetlenie właściwości.

![](../.gitbook/assets/array-along-path-options.png)

### Select Object\(s\) to Array <a id="run"></a>

Kliknij tę opcję, aby wrócić do kreatora wyboru i zmienić obiekty ustawiane w szyku.

### Select Array Path

Kliknij tę opcję, aby wrócić do kreatora wyboru i zmienić ścieżkę służącą do obliczenia szyku.

### Array Type <a id="run"></a>

Ta opcja służy do przełączania typu szyku do obliczenia: By Distance lub By Number.

**W przypadku wybrania wartości True** obliczenia będą wykonywane według odległości \(„By Distance”\), dlatego liczba poniżej odnosi się do odległości między kopiami.

**W przypadku wybrania wartości False** obliczenia będą wykonywane według liczby kopii \(„By Number of Copies”\), dlatego liczba poniżej tego pola odnosi się do liczby kopii, które mają zostać dopasowane wzdłuż ścieżki.

### Include Original Selection In Results

W przypadku wartości **True**:

* Wybrane obiekty będą liczone jako jedna z nowych kopii
* Powstała grupa Dynamo będzie uwzględniała w wynikach oryginalny wybór, dlatego w przypadku nowych kopii i oryginalnego wyboru będzie występował efekt Z-fight. Oryginalny wybór można umieścić na [warstwie](layers.md) i wyłączyć, aby go ukryć.

W przypadku wartości **False**:

* Powstały szyk **nie** będzie zawierał oryginalnego wyboru, dlatego otrzymasz określoną liczbę kopii **oprócz** oryginalnego wyboru, a w wynikach nie będzie występował efekt Z-fight

### Rotate Copies Along Path

Gdy jest ustawiona wartość **True**, kopie są obracane w celu zachowania orientacji oryginalnego obiektu względem ścieżki.

Gdy jest ustawiona wartość **False**, kopie nie są obracane, a tylko przesuwane.

### Use Relative Positioning Along Path

W przypadku wartości **True**:

* Każda kopia zachowuje odległość między ścieżką a oryginalnym obiektem.
* Jeśli oryginalny obiekt **nie** znajduje się w jednym z punktów końcowych ścieżki, do obliczenia szyku zostanie użyty największy pozostały segment ścieżki.

W przypadku wartości **False**:

* Do obliczenia szyku zostanie użyta cała długość ścieżki, niezależnie od tego, gdzie znajduje się oryginalny obiekt względem ścieżki.
* Powoduje to odłączenie położenia ścieżki względem obiektu i pozwala na użycie całej ścieżki. Jest to przydatne, gdy ścieżka i obiekt nie znajdują się blisko siebie.

### Reverse Path Direction

Dotyczy tylko zamkniętych ścieżek. W przypadku użycia narzędzia Array Along Path z zamkniętą ścieżką kierunek krzywej może spowodować nieoczekiwane odwrócenie spodziewanych wyników szyku. Jeśli wyniki są odwrócone, przełącz tę opcję na **True**, aby odwrócić kierunek szyku.

### Uruchom <a id="run"></a>

Po zakończeniu edycji opcji kliknij przycisk „Run”, aby uruchomić podstawowy wykres dodatku Dynamo i wygenerować nowe wyniki. Po zmianie parametrów przycisk zmienia kolor na niebieski, dzięki czemu wiesz, że należy go kliknąć, aby zobaczyć aktualizacje w końcowej geometrii.‌

### Edit Embedded Graph <a id="edit-embedded-graph"></a>

Kliknięcie tego przycisku spowoduje uruchomienie środowiska edytora wykresów Dynamo, aby można było wyświetlić i edytować podstawowy wykres Dynamo w celu szybszej zmiany parametrów i wyświetlenia aktualizacji na żywo bądź sprawdzenia/dopasowania logiki.



## Wybieranie geometrii

Podczas wybierania obiektów dla narzędzia Array Along Path i innych wykresów Dynamo opartych na wyborze:

* Możesz wybrać dowolne połączenie obiektów FormIt — wierzchołków, krawędzi, powierzchni, brył, grup i siatek.
   * Pamiętaj, że w zależności od kroku niektórych z tych obiektów nie należy wybierać.
   * Na przykład podczas wybierania ścieżki należy wybrać tylko przylegającą serię krawędzi lub grupę zawierającą przylegającą serię krawędzi. Wszystkie pozostałe opcje spowodują błąd wykresu.
* Klikając dwukrotnie obiekt, możesz wybrać wszystkie dołączone elementy.
* Aby pobrać serię obiektów, możesz użyć okna wyboru obszaru.
* Wybierając już wybrane obiekty, możesz usunąć ich zaznaczenie.
* Do wykonania kroku opartego na wyborze wymagany jest co najmniej jeden obiekt.



