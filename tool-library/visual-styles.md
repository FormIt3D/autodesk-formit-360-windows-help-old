# Style wizualne

Dostosuj wygląd modelu, w tym ogólne oświetlenie, style krawędzi i efekty środowiskowe. Panel Style wizualne można znaleźć, klikając ikonę okularów przeciwsłonecznych na pasku palety:

![](../.gitbook/assets/20200307-visual-styles-icon.png)

Style wizualne [można ustawiać dla poszczególnych scen](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/visual-settings). Można więc zapisać ustawienia ulubionych stylów i zastosować je do innych scen.

## Powierzchnie

Zarządzaj sposobem wyświetlania i cieniowania powierzchni.

![](../.gitbook/assets/visual_styles%20%281%29.png)

**Jasność otoczenia** — ta opcja steruje całkowitą jasnością wszystkich materiałów w scenie. Wartość 100 oznacza, że materiały wystawione na światło będą wyświetlane z pełną jasnością określoną w kolorze lub teksturze materiału. Wartości powyżej 100 powodują nadmierną ekspozycję materiałów, ale mogą być przydatne w przypadku modeli programu SketchUp, których wygląd jest nadal ciemny w programie FormIt. Domyślną wartością jest 100.

**Kontrast otoczenia** — ta opcja steruje tym, jak wyglądają ciemniejsze powierzchnie w cieniu w porównaniu z powierzchniami wystawionymi na bezpośrednie światło słoneczne. Wartość 0 oznacza, że oświetlenie nie ma wpływu \(wszystkie materiały będą wyświetlane z pełną jasnością niezależnie od orientacji\), natomiast wartości wyższe powodują, że powierzchnie znajdujące się w cieniu są coraz ciemniejsze. Domyślną wartością jest 25.

Przełącz opcję **Cienie**, aby zobaczyć, w jaki sposób projekt będzie [cieniowany o bieżącej porze dnia](https://windows.help.formit.autodesk.com/tool-library/shadows).

**Intensywność cienia** — ta opcja określa sposób rysowania ciemnych cieni na płaszczyźnie terenu i innych powierzchniach. Wartość 0 spowoduje, że cienie staną się w zasadzie niewidoczne, a wartość 100 — że staną się czarne. Domyślną wartością jest 20.

**Cienie otoczenia** — ta opcja dodaje cieniowanie do narożników, aby model programu FormIt był bardziej realistyczny.

**Powierzchnie monotone** — ta opcja wyłącza kolor i teksturę wszystkich materiałów oraz powoduje, że środowisko otoczenia staje się białe. Jest to przydatne w przypadku badań cieni i cieniowania.

Sekcja Kolory powierzchni definiuje domyślne kolory powierzchni, gdy nie zastosowano materiału.

**Powierzchnie** — to domyślny kolor wszystkich powierzchni programu FormIt skierowanych przodem \(lub po obu stronach, jeśli nie jest zaznaczona opcja Tylne powierzchnie\), gdy nie zastosowano żadnego materiału.

**Tylne powierzchnie** — ta opcja służy do wyświetlania różnych materiałów po obu stronach pojedynczej powierzchni dla modeli programu SketchUp importowanych do programu FormIt, które tego wymagają. Ta opcja jest domyślnie niezaznaczona, ale jest zaznaczona podczas otwierania lub importowania modeli programu SketchUp. W geometrii innej niż programu SketchUp określony kolor tylnej powierzchni będzie wyświetlany na tylnych stronach powierzchni.

W obszarach Efekty przekroju i Efekty wypełnienia sekcji można zarządzać domyślnymi kolorami powierzchni, linii i efektu wypełnienia, gdy używane jest narzędzie [Płaszczyzna przekroju](section-planes.md).

## Płaszczyzny terenu

Gdy płaszczyzna terenu jest wyłączona w trybie edycji grupy, niebieska siatka płaszczyzny roboczej także jest wyłączona.

Kolor płaszczyzny roboczej można również dostosować z poziomu panelu Style wizualne.

![](../.gitbook/assets/screen-shot-2020-03-30-at-1.30.16-pm.png)

## Krawędzie

Zarządzaj stylem wyświetlania wszystkich krawędzi w modelu.

![](../.gitbook/assets/edges.PNG)

**Kontrast** — ta opcja wpływa na to, jak bardzo widoczne są wszystkie krawędzie. Wartość 0 spowoduje, że krawędzie staną się niewidoczne. Domyślną wartością jest 60.

**Kolor** — ta opcja wpływa na kolor wszystkich krawędzi w modelu. Domyślną wartością jest czarny.

**Grube krawędzie** — ta opcja powoduje, że wszystkie krawędzie stają się grubsze, w tym krawędzie sylwetki.

**Krawędzie szkicu** — ta opcja dodaje efekt szkicu do wszystkich krawędzi, symulując efekt rysowania odręcznego.

**Ukryte krawędzie** — ta opcja wyświetla krawędzie przesłonięte przez powierzchnie.

**Wydłużone krawędzie** — ta opcja dodaje przedłużenie do niektórych krawędzi, symulując efekt rysowania odręcznego.

## Środowisko

Przełącz wyświetlanie efektów środowiskowych i obiektów pomocniczych.

![](../.gitbook/assets/environment.PNG)

**Siatka** — ta opcja steruje wyświetlaniem siatki na płaszczyźnie terenu, jak również siatką wyświetlaną podczas edycji grupy. Opcja „Przyciągaj do siatki” jest wyłączona, gdy siatka jest wyłączona.

**Osie** — ta opcja steruje wyświetlaniem osi XYZ wyświetlanych w początku globalnym lub w początku grupy podczas edycji grupy.

**Poziomy** — ta opcja steruje wyświetlaniem [**poziomów**](levels-and-area.md) **** ustawionych w panelu Poziomy.

**Mgła** — ta opcja steruje wyświetlaniem mgły, która jest rysowana, aby przejście między płaszczyzną terenu a niebem było płynniejsze. Wyłączenie mgły spowoduje utworzenie wyraźnej linii horyzontu, na której płaszczyzna terenu \(jeśli jest włączona) styka się z niebem.

**Strzałka północy** — ta opcja steruje wyświetlaniem małego widżetu graficznego wskazującego kierunek północy projektu \(zgodnie z określeniem położenia i obrazami satelitarnymi\).

Można również dostosować kolory środowiskowe, takie jak nieba, tła i płaszczyzny terenu.

Niebo składa się z gradientu kolorów **Dolne/tło**, **Środek** i **Górne**.

Jeśli opcja **Niebo** nie jest zaznaczona, widoczny będzie tylko kolor **Dolne/tło**.

## Diagnostyka

Przełącz wyświetlanie narzędzi diagnostycznych.

![](../.gitbook/assets/diagnostics.PNG)

**Problemy z uszczelnieniem** — ta opcja powoduje wyróżnienie na czerwono wszystkich krawędzi, które nie są częścią szczelnego obiektu bryłowego.

**Tylne powierzchnie** — ta opcja powoduje wyróżnienie na czerwono wszystkich powierzchni skierowanych w złą stronę \(wszystkie obiekty bryłowe powinny mieć tylne powierzchnie skierowane w stronę wewnętrznej strony kształtu bryły\).

[Dowiedz się więcej na temat korzystania z diagnostyki uszczelnienia i tylnych powierzchni w celu identyfikowania i rozwiązywania problemów z modelami brył](https://formit.autodesk.com/blog/post/repairing-solid-models).

