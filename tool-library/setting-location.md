# Ustawianie położenia

Ustawienie położenia projektu na świecie ma znaczenie dla dokładności modelu i analiz następczych. Dotyczy to między innymi następujących kwestii:

* Położenie jest używane przy importowaniu obrazu satelitarnego, który może być używany do śledzenia istniejącego terenu lub budynku.
* Położenie jest używane przy importowaniu terenu 3D, który może być używany do tworzenia odniesień do danych topologicznych terenu.
* Położenie jest używane do dokładnego pozycjonowania słońca na niebie, co wpływa na obliczenia cieni.
* Położenie jest używane do analizy oświetlenia naturalnego i analizy energetycznej w celu zapewnienia dokładnych obliczeń analitycznych.

Aby uzyskać dostęp do okna dialogowego Ustaw położenie i jego usług, należy się zalogować przy użyciu konta Autodesk.

### Położenie — pierwsze kroki

* Uruchom okno dialogowe **Ustaw położenie** z narzędzia **Położenie** na pasku narzędzi lub za pomocą skrótu klawiaturowego SL.

![](../.gitbook/assets/location-toolbar.png)

* Najpierw wpisz położenie projektu w polu wyszukiwania w lewym górnym rogu okna _Ustaw położenie_.

![](../.gitbook/assets/location-step-1%20%281%29.png)

* Wybierz jedną z automatycznie wypełnionych opcji położenia lub naciśnij klawisz Enter, aby wybrać pierwszą.
* Widok zostanie powiększony do położenia, które zostało automatycznie wyszukane.

### „Ustaw tylko położenie” a „Importuj obraz satelitarny i teren”

Po wyszukaniu położenia można wybrać jedną z dwóch opcji:

* **Ustaw tylko położenie** spowoduje ustawienie położenia w pliku bez importowania obrazów satelitarnych.
* **Importuj obraz satelitarny i teren** spowoduje ustawienie położenia, a także zaimportowanie obrazów satelitarnych i terenu przy użyciu poziomu powiększenia i zakresu, które można skonfigurować.

### Importowanie obrazów satelitarnych

* Kliknij opcję **Importuj obraz satelitarny i teren** w prawej górnej części okna **Ustaw położenie**.
* W środku okna zostanie wyświetlony podgląd obrazu satelitarnego wraz ze wskazaniem miejsca, w którym pojawi się początek programu FormIt (względem obrazu).

![](../.gitbook/assets/location-step-2.png)

* Przeciągnij obraz satelitarny w kwadracie, aby dopasować jego położenie.
* Po ujęciu w obszarze kwadratowym odpowiedniego obrazu kliknij przycisk **Zakończ importowanie**.
* Obraz zostanie zaimportowany z przeskalowaniem, przy czym północ rzeczywista jest skierowana w górę, wyśrodkowana w początku obszaru rysunku FormIt. Przezroczystość i kolejność względem osi Z zaimportowanego obrazu można zmienić, klikając go dwukrotnie i przechodząc do [**palety Właściwości**](../formit-introduction/tool-bars.md).

![](../.gitbook/assets/location-step-3.png)

### Aktualizowanie obrazów satelitarnych

Po wstępnym zaimportowaniu obrazów satelitarnych można za pomocą okna Ustaw położenie dostosować poziom powiększenia lub zakres obrazu satelitarnego.

* Ponownie uruchom okno **Ustaw położenie**, uzyskując do niego dostęp z paska narzędzi, jak wyjaśniono powyżej.
* Kliknij opcję **Importuj obraz satelitarny i teren.**
* Zostanie wyświetlony bieżący poziom powiększenia obrazu satelitarnego i zakres, jak pokazano w obszarze rysunku FormIt.
* Wystarczy dopasować położenie lub powiększenie, a następnie kliknąć przycisk **Zakończ importowanie**, tak jak poprzednio.
* Po ponownym zaimportowaniu obrazu do obszaru rysunku zostanie on przesunięty do właściwego położenia względem oryginalnego położenia obrazu \(i może nie być już wyśrodkowany w początku\):

![](../.gitbook/assets/location-step-4.png)

### Importowanie terenu

Nowość w programie FormIt 2021.3: w przypadku importowania obrazów satelitarnych przy użyciu okna dialogowego **Ustaw położenie** uzyskuje się również teren.

![](../.gitbook/assets/terrain-button_original.png)

Po zaimportowaniu terenu jest on umieszczany na warstwie, która jest domyślnie wyłączona \(w przypadku rozpoczęcia modelowania model może być przykryty przez teren).

Gdy wszystko będzie gotowe do wyświetlenia terenu, zaznacz pole wyboru w celu przełączenia warstwy terenu:

![](../.gitbook/assets/terrain-layer%20%281%29.png)

![](../.gitbook/assets/terrain_solid.png)

### Praca z terenem

Teren zostanie umieszczony w grupie programu FormIt. Kliknij dwukrotnie grupę, aby ją edytować.

Wewnątrz znajdują się dwie siatki: jedna dla boków i dołu oraz jedna dla góry.

Aby zmodyfikować teren, należy przekonwertować siatki na pojedynczy obiekt bryłowy:

* Wybierz obie siatki.
* Kliknij prawym przyciskiem myszy i wybierz opcję Siatki na obiekty lub użyj skrótu MO.

![](../.gitbook/assets/terrain-mesh-context.png)

W przypadku konwertowania obu siatek na obiekt w tym samym czasie program FormIt może połączyć je w bryłę, obiekt rozgałęziony, którego można używać do operacji bryłowych, takich jak Wycięcie logiczne.

W tym miejscu można użyć połączenia opcji [Widok z góry](orthographic-views.md) i [Kamera prostopadła](orthographic-camera.md), aby śledzić obszar graniczny na płaszczyźnie poziomej, a następnie wyciągnąć tę płaszczyznę w obiekt objętościowy przecinający teren. Zastosowanie przezroczystego [materiału](materials.md) pomaga w obserwowaniu terenu poprzez bryłę tnącą:

![](../.gitbook/assets/terrain-cutter-before.png)

Użyj narzędzia Dotnij geometrię i wybierz teren jako bryłę, w której ma zostać wycięty element, oraz tnący obiekt objętościowy jako bryłę do usunięcia.

![](../.gitbook/assets/terrain-cut-menu.png)

W wyniku tego powstanie teren z usuniętą bryłą tnącą, co spowoduje odsłonięcie miejsca, w którym można narysować nowy teren i fundament.

![](../.gitbook/assets/terrain-cutter-after.png)

Za pomocą [warstw](layers.md) można ukryć bryłę tnącą lub nawet utworzyć kopie terenu z wycięciem i bez niego na wypadek, gdyby trzeba było utworzyć odniesienie do pierwotnego terenu lub zmienić kształt wycięcia przed wykonaniem operacji wycięcia bryły.

