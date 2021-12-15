# Railing Along Path

## Obsługiwane przez dodatek Dynamo

W programie FormIt 2021 i w nowszych wersjach można generować poręcz wzdłuż ścieżki i szybko dostosowywać wyniki lokalnie. Poręcz wzdłuż ścieżki jest obsługiwana przez dodatek Dynamo, co oznacza, że wynikową poręcz można łatwo skonfigurować, aby uzyskać żądane wyniki, a ponowne uruchomienie logiki spowoduje zaktualizowanie geometrii lokalnie.

![](../.gitbook/assets/railing-along-path.gif)

## Uruchamianie przykładu Railing Along Path

* Przejdź do panelu Dynamo w programie FormIt dla systemu Windows i upewnij się, że znajdujesz się w katalogu Dynamo Samples.
* Kliknij przykład Railing Along Path.
* Po lewej stronie ekranu zostanie wyświetlony monit „Select path for railing”.
   * W tym miejscu należy wybrać tylko serię przylegających krawędzi lub grupę zawierającą serię krawędzi.
   * Po wybraniu ścieżki kliknij przycisk „finish” lub naciśnij klawisz Enter/Return.
* W panelu Dynamo będzie wyświetlana informacja o przetwarzaniu zmian. Po zakończeniu poręcz wygenerowana przez dodatek Dynamo będzie dostępna w grupie FormIt i będzie można ją modyfikować \(patrz poniżej\).

## Iteracja lokalna

Po uruchomieniu narzędzia Railing Along Path wyniki jego działania będą miały wartości domyślne. Być może będą w danym przypadku odpowiednie, ale poręcz można w znacznym stopniu dostosować do własnych potrzeb.

Gdy narzędzie Railing Along Path jest uruchomione, tworzona jest nowa grupa zawierająca wyniki, a polecenie FormIt automatycznie wybiera grupę i wyświetla dostępne opcje dla wystąpienia tego narzędzia.

W każdej chwili można wrócić do właściwości narzędzia Railing Along Path, wybierając grupę i przełączając się na panel Właściwości lub edytując grupę, co spowoduje automatyczne wyświetlenie właściwości.

![](../.gitbook/assets/railing-along-path-options.png)

### Wysokość poręczy

Całkowita wysokość poręczy. Używane są bieżące jednostki programu FormIt.

### Post Spacing

Odstępy między głównymi słupkami pionowymi. Używane są bieżące jednostki programu FormIt.

### Add Posts at Path Vertices

Gdy jest ustawiona wartość **true**, słupki zostaną dodane w poszczególnych wierzchołkach wybranej ścieżki, a obliczenia dla następnego położenia słupka zostaną zresetowane w tych punktach.

Na przykład jeśli wybrano serię 3 krawędzi, w każdym z dwóch punktów wewnętrznych pojawi się słupek. Jest to przydatne, jeśli wierzchołki wskazują zmianę kierunku \(np. kierunek schodów w górę lub zakręty\) w miejscach, w których słupki w naturalny sposób występują.

Gdy jest ustawiona wartość **false**, słupki zostaną dodane tylko wzdłuż ścieżki rozpoczynającej się na jednym końcu i z pomiarem odległości wzdłuż ścieżki oraz ignorowaniem występujących wzdłuż ścieżki wierzchołków. Jest to przydatne, jeśli wybrano łuk, splajn lub okrąg, w których wierzchołki nie są ważne i powinny być ignorowane w odstępach między słupkami.

### Reverse Path Direction

Podczas obliczania położenia słupków kierunek wybranej ścieżki określa, od którego końca ścieżki rozpocznie się pomiar odstępów między słupkami.

W przypadkach gdy odstępy między słupkami powodują powstanie pustej przestrzeni na nieodpowiednim końcu ścieżki, można zmienić tę wartość na **true**, aby odwrócić krzywą i rozpocząć pomiar odstępów między słupkami na przeciwległym końcu.

### Post Width + Depth

Rozmiar \(w rzucie\) profili pionowych słupków prostokątnych. Używane są bieżące jednostki programu FormIt.

### Handrail Width + Height

Rozmiar \(w przekroju\) profilu poręczy prostokątnej. Używane są bieżące jednostki programu FormIt.

### Baluster Orientation

Gdy jest ustawiona wartość „true”, tralki będą zorientowane poziomo, podobnie jak kable. W przypadku wartości „false” tralki będą zorientowane pionowo, zapewniając bardziej tradycyjną estetykę.

### Baluster width + Depth

Rozmiar profilu prostokątnego tralki. Używane są bieżące jednostki programu FormIt.

### Baluster Spacing

Ilość miejsca między poszczególnymi tralkami. Używane są bieżące jednostki programu FormIt.

### Bottom Rail Start Height

Odległość między dołem poręczy a dolną szyną, która podpiera tralki. Używane są bieżące jednostki programu FormIt.

### Uruchom

Po zakończeniu edycji opcji kliknij przycisk „Run”, aby uruchomić podstawowy wykres dodatku Dynamo i wygenerować nowe wyniki. Po zmianie parametrów przycisk zmienia kolor na niebieski, dzięki czemu wiesz, że należy go kliknąć, aby zobaczyć aktualizacje w końcowej geometrii.‌

### Edit Embedded Graph

Kliknięcie tego przycisku spowoduje uruchomienie środowiska edytora wykresów Dynamo, aby można było wyświetlić i edytować podstawowy wykres Dynamo w celu szybszej zmiany parametrów i wyświetlenia aktualizacji na żywo bądź sprawdzenia/dopasowania logiki.

