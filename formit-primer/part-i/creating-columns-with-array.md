# 1.8 — Tworzenie słupów przy użyciu narzędzia Szyk

_W tym ćwiczeniu naszkicujemy element szczegółowy — słup o kształcie dwuteownika. Następnie za pomocą narzędzia Szyk szybko utworzymy wiele kopii w równych odstępach._

_Jeśli nie ukończono poprzedniej sekcji, pobierz i otwórz plik_ _**1.8 — Create Columns with Array.axm**_ _z folderu_ _**FormIt Primer Part 1 Datasets**._

## **Szkicowanie profilu słupa**

1 — Dla ułatwienia procesu kreślenia:

1. Przejdź do **Widoku z góry \(VT\)**.
2. Przełącz tryb widoku na **Prostopadły \(VO\)**.
3. Wyłącz warstwy **Budynek główny**, **Podłoga** i **Dach**. Dzięki temu nowa geometria nie będzie przyciągana do istniejącej geometrii na tych warstwach.
4. Powiększ lewy górny narożnik **zaimportowanego obrazu rzutu podłogi**, aby widzieć szczegóły słupa.
5. Wyłącz **Przyciąganie do siatki \(SG\)** \(jeśli jest włączone\). To pomoże w rysowaniu linii szczegółów.

![](../../.gitbook/assets/0%20%2813%29.png)

_Aby narysować słup, najpierw narysujemy połowę, a następnie wykonamy odbicie lustrzane, aby szybko utworzyć drugą, symetryczną połowę._

2 — Aby utworzyć pierwszą połowę dwuteownika, użyj **narzędzia Linia \(L\)** i wykonaj następujący szkic o podanych wymiarach. Na tym etapie nie musisz się martwić dokładnym położeniem słupa na rzucie.

![](../../.gitbook/assets/1%20%2818%29.png)

3 — Utwórz odbicie lustrzane narysowanego kształtu:

1. Kliknij dwukrotnie, aby wybrać wszystkie powierzchnie i krawędzie narysowanej geometrii.
2. Kliknij prawym przyciskiem myszy i wybierz **narzędzie Odbicie lustrzane \(MI\)**.
3. Kliknij środkowy pomarańczowy uchwyt **narzędzia odbicia lustrzanego** i umieść go w lewym dolnym rogu geometrii.
4. Użyj strzałki w dół na przycisku strzałki dwustronnej w narzędziu, aby obrócić oś odbicia lustrzanego o –90 stopni \(zgodnie z ruchem wskazówek zegara\).
5. Kliknij jeden raz w pustym obszarze lub naciśnij klawisz **Esc**, aby zakończyć proces tworzenia odbicia lustrzanego. Rezultat powinien wyglądać jak profil dwuteownika z linią biegnącą pionowo przez środek. Naciśnij ponownie klawisz **Esc**, aby anulować wybór.

![](../../.gitbook/assets/2%20%285%29.png)

![](../../.gitbook/assets/3%20%287%29.png)

_**Uwaga**: podczas dopasowywania narzędzia odbicia lustrzanego położenie i orientacja tworzonej geometrii są widoczne na podglądzie jako półprzezroczysty niebieski kształt. Można skorzystać z tego podglądu jako odniesienia, aby utworzyć odbicie lustrzane geometrii w zamierzonym położeniu._

4 — Aby połączyć połowy w jedną geometrię, usuń dzielącą je linię, wybierając ją kliknięciem, a następnie naciskając klawisz **Delete**. Teraz obie powierzchnie zostały połączone w jedną.

5 — Przesuń geometrię w jej ostateczne położenie:

1. Jeśli są wyłączone, włącz warstwy **Obraz rzutu** i **Dach**, aby używać ich jako odniesienia.
2. Kliknij dwukrotnie profil słupa, aby wybrać jego powierzchnię i wszystkie linie. Rozpocznij przesuwanie wybranych elementów wzdłuż zielonej osi \(**osi Y**\). Przytrzymaj klawisz **Shift** i przesuwaj profil do momentu wyrównania z dachem, a następnie kliknij, aby go umieścić.
3. Podobnie jak w poprzednim kroku przesuń ponownie geometrię, tym razem blokując ją na czerwonej osi \(**osi X**\).
4. Kliknij, aby umieścić element na belce dwuteowej narysowanej na **obrazie rzutu**. Wystarczy umieścić go blisko, jak na poniższej ilustracji — położenie w poziomie nie musi być idealne.

_**Uwaga:**_ _klawisz_ _**Shift**_ _umożliwia zablokowanie geometrii w celu przesuwania jej tylko wzdłuż jednej osi, w tym przypadku — zielonej \(**osi Y**\). To zapobiega przypadkowemu przesunięciu profilu słupa w górę i wyrównaniu go do górnej części płaszczyzny dachu._

![](../../.gitbook/assets/4%20%289%29.png)

## **Wyciąganie słupa i tworzenie szyku**

1 — Dla ułatwienia kolejnego procesu kreślenia przełącz widok z powrotem na tryb **Perspektywa \(VP\)** i **obróć \(O\)** kamerę w taki sposób, aby widzieć profil belki dwuteowej z północnego zachodu. Użyj strzałki wskazującej północ w lewym dolnym rogu, aby łatwiej ustawić widok.

![](../../.gitbook/assets/5%20%281%29.jpeg)

_**Uwaga:**_ _aby dowiedzieć się, jak poruszać się po szkicu, zapoznaj się z rozdziałem_ _**Nawigacja po scenie**_ _._

2. Wybierz powierzchnię profilu słupa i wyciągnij powierzchnię w górę o **17 stóp i 8 cali**.

_**Uwaga:**_ _jeśli podczas przesuwania profil słupa został wyrównany względem dachu, wyciągnij powierzchnię o_ _**17 stóp i 8 cali**   w dół, a nie w górę._

3 — Pomniejsz widok i włącz warstwę **Dach** \(jeśli jest wyłączona\). Górna powierzchnia słupa powinna być wyrównana do górnej powierzchni dachu.

![](../../.gitbook/assets/6%20%289%29.png)

4 — Uporządkuj model, ponownie wybierając geometrię słupa i wykonując następujące czynności:

1. Dodaj słup do **grupy \(G\)** i nazwij ją **Słup — wysoki**.
2. Utwórz nową **Warstwę** o nazwie **Słup** i dodaj do niej tę grupę.
3. Zaimportuj materiał **Metal — matowy — kolorowy** i pomaluj nim grupę.

![](../../.gitbook/assets/7%20%284%29.png)

_**Uwaga:**_ _więcej informacji na temat_ _**grup**,_ _**warstw** i_ _**materiałów** zawierają poprzednie rozdziały._

4 — Naciśnij klawisz **Esc**, aby wyczyścić narzędzie pędzla.

## **Tworzenie szyku słupów**

1 — Przejdź do **widoku z góry \(VT\)** i ponownie przełącz tryb kamery na **Prostopadły \(VO\)**.

2 — Wyłącz warstwę **Dach**.

3 — Rozpocznij tworzenie szyku:

1. Kliknij grupę słupa jeden raz, aby ją wybrać. Kliknij prawym przyciskiem myszy, aby wyświetlić **menu kontekstowe**, i wybierz narzędzie **Szyk \(AR\)**.
2. W oknie dialogowym **Właściwości szyku** użyj następujących ustawień:
   * **Długość pomiędzy kopiami**
   * **Liniowa** \(ustawienie domyślne\)
   * **Pogrupuj każdą bryłę, a następnie utwórz szyk** \(ustawienie domyślne\)
   * **Liczba kopii: 3**
   * Kliknij przycisk **OK**, aby zamknąć okno dialogowe.

![](../../.gitbook/assets/8%20%283%29.png)

4 — Umieść nowe elementy:

1. Kliknij słup jeden raz, aby rozpocząć tworzenie **szyku**. Przesuń kursor wzdłuż czerwonej osi \(**osi X**\).
2. Ustaw wymiar na **22 stopy**. Masz teraz **cztery** słupy w odległości **22 stóp**.
3. Naciśnij klawisz **Esc**, aby anulować wybór.

![](../../.gitbook/assets/9%20%286%29.png)

5 — Aby wybrać wszystkie grupy **Słup — wysoki** jednocześnie, umieść wskaźnik myszy na jednej z nich i naciśnij klawisz **Tab** jeden raz. Zobaczysz, że wszystkie 4 ramki ograniczające słupów zostały wyróżnione. Kliknij jeden raz słup, na którym znajduje się kursor myszy, aby wybrać wszystkie z nich. To szybki sposób na wybranie wszystkich wystąpień tej samej grupy jednocześnie.

6 — Ponownie użyj narzędzia **Szyk \(AR\)**, aby utworzyć słupy po drugiej stronie budynku. Tym razem utwórz 1 kopię wzdłuż zielonej osi biegnącej w poprzek budynku. Ustaw wymiar na **29 stóp i 4 i 5/8 cala.**

_**Uwaga:**_ _29 stóp i 4 i 5/8 cala = 8 i 5/8 cala \(głębokość słupa\) + 28 stóp i 8 cali \(szerokość budynku głównego\)._

7 — Aby wyświetlić cały budynek, przejdź do **widoku 3D \(V3\)** i ustaw tryb **Perspektywa \(VP\)**. Jeśli są wyłączone, włącz warstwy **Podłoga budynku głównego**, **Dach**, **Taras dolny** i **Słup**.

![](../../.gitbook/assets/10%20%287%29.png)

## **Tworzenie słupów tarasu**

_Teraz powielimy słupy budynku głównego, aby utworzyć podobne, ale krótsze słupy tarasu._

1 — Dla ułatwienia kreślenia zalecamy powrót do ustawień **Ortogonalny \(OV\)** i **Widok z góry \(VT\)**.

2 — Utwórz nowe słupy:

1. Przytrzymaj wciśnięty klawisz **Ctrl** lub **Shift** i kliknij 3 słupy znajdujące się najbliżej **podłogi dolnego tarasu**, aby je wybrać.
2. Kliknij jeden raz dowolny ze słupów, aby rozpocząć przesuwanie wszystkich 3 wybranych słupów jednocześnie. Naciśnij jeden raz klawisz **Ctrl**, aby utworzyć **szybką kopię**. Zostanie wyświetlony półprzezroczysty podgląd kopii.
3. Przesuń kopie w dół zielonej osi \(**osi Y**\) o **23 stopy i 4 i 3/8 cala**. Naciśnij klawisz **Esc**.
4. Nie anulując wyboru, przesuń skopiowane słupy wzdłuż czerwonej osi \(**osi X**\) o **22 stopy**, aby umieścić je w docelowym położeniu.
5. Nadal nie anulując wyboru 3 nowych słupów, kliknij prawym przyciskiem myszy jeden ze skopiowanych słupów i wybierz opcję **Ustaw jako unikatowe \(MU\)**. Słupy są teraz skojarzone ze sobą, ale unikatowe względem oryginałów.

_**Uwaga:**_ _przytrzymanie naciśniętego klawisza_ _**Shift**_ _lub_ _**Ctrl**_ _pozwala wybrać wiele elementów jednocześnie lub usunąć elementy z bieżącego wyboru._

![](../../.gitbook/assets/11%20%287%29.png)

3 — Zmodyfikuj nową grupę słupów:

1. Kliknij dwukrotnie, aby edytować jedną z nowych grup i zmień jej nazwę na **Słup — krótki.**
2. Dopasuj wysokość nowej kolumny, aby wyrównać ją względem górnej krawędzi **Podłogi** **dolnego tarasu** \(3 stopy i 2 cale\). W tym celu wybierz powierzchnię słupa i przeciągnij ją w dół wzdłuż niebieskiej osi \(**osi Z**\), przytrzymując naciśnięty klawisz **Shift**. Umieść kursor w dowolnym miejscu na górnej powierzchni **Podłogi dolnego tarasu**, a wysokość słupa zostanie automatycznie wyrównana do dolnego tarasu. Po ustawieniu wysokości kliknij, aby zakończyć.

![](../../.gitbook/assets/12%20%284%29.png)

_**Uwaga:**_ _wysokość krótkich słupów można sprawdzić za pomocą narzędzia_ _**Zmierz \(ME\)**_ _. Można również wybrać jedną z pionowych krawędzi słupa i wyświetlić jej długość na_ _**palecie Właściwości**._

4. Korzystając z poznanych tu technik, skopiuj najbardziej oddalony krótki słup na przeciwległą stronę **Podłogi dolnego tarasu**, aby utworzyć ostatni słup.

![](../../.gitbook/assets/13%20%284%29.png)

