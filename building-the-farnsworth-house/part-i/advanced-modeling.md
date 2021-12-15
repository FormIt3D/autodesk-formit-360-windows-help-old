# Zaawansowane modelowanie

W naszych ćwiczeniach z modelem domu pani Farnsworth skupiliśmy się na podstawowych narzędziach modelowania, takich jak Szkicowanie, Przeciągnij powierzchnię, Przenieś, Szyk i Odsuń powierzchnię. Omówiliśmy również najważniejsze procesy robocze dotyczące grup, warstw, materiałów i poziomów. W tej sekcji przedstawimy zaawansowane narzędzia modelowania **Przeciągnięcie** i **Zaokrąglenie**

Jeśli ostatnia sekcja nie została ukończona, pobierz i otwórz plik **farnsworth05.axm** z [folderu FormIt Primer](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).

## Przeciągnięcie

Użyj narzędzia Przeciągnięcie, aby utworzyć gzyms wzdłuż dachu.

1. Za pomocą narzędzia **Prostokąt \(R\)** utwórz profil o **wysokości 6" na 4 5/8"** w dowolnym narożniku dachu.

   ![](../../.gitbook/assets/a7297208-cefe-42e7-95ca-1e8ea122ac38.png)

2. Utwórz kolejny profil **Prostokąt \(R\)** o wymiarach **2" x 2".**

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54.png)

3. **Kliknij raz**, aby wybrać linię między profilami. Za pomocą klawisza **Delete** usuń linię — spowoduje to utworzenie pojedynczego konturu.

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_2.png)

4. Wybierz [**narzędzie Przeciągnięcie \(SW\)**](../../tool-library/cover-sweep-loft.md) z [**menu Zaawansowane modelowanie**](../../formit-introduction/tool-bars.md)**.**

   ![](../../.gitbook/assets/8a17017b-b824-48ac-ba24-064a24e7a6ad.png)

5. W lewym górnym rogu obszaru rysunku zostanie wyświetlony pasek narzędzi **Zaawansowane narzędzia geometrii** wraz z pomocniczymi instrukcjami tekstowymi.

   ![](../../.gitbook/assets/e8badff2-acd9-4393-af5f-adae2424ad47.png)

6. **Kliknij raz**, aby wybrać właśnie narysowaną powierzchnię. Będzie to **profil**, który ma zostać przeciągnięty.

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_3.png)

7. Po wybraniu powierzchni pasek narzędzi **Zaawansowane narzędzia geometrii** ulegnie zmianie. Teraz zostanie wyświetlony monit o wybranie **ścieżki** do przeciągnięcia.

   ![](../../.gitbook/assets/df9fc338-15c0-4953-9ec1-c977117efc4d.png)

8. **Kliknij raz**, aby wybrać **górną powierzchnię dachu**. Narzędzie traktuje krawędzie powierzchni jako ścieżkę. Po wybraniu dachu zostanie utworzone przeciągnięcie.

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_4.png)

9. Kliknij dwukrotnie, aby wybrać cały element gzymsu. **Zgrupuj \(G\)** gzyms. Przeprowadź edycję grupy i nadaj jej nazwę **gzyms.**

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_5.png)

10. Pomaluj grupę gzymsu materiałem **Concrete &gt; White**, aby dopasować ją do dachu. Dodaj **grupę gzymsu** do warstwy **dachu**.

Musisz dostosować **wysokość słupów** tak, aby kończyły się w gzymsie. Przeprowadź edycję jednej z grup wysokich słupów, wybierz górną powierzchnię i przesuń ją w dół na odpowiednią wysokość. Może być również konieczne dopasowanie położenia słupów tak, aby były równoległe do połaci. To dobry moment na wprowadzenie drobnych zmian

## Zaokrąglenie

Teraz poznasz narzędzie Zaokrąglenie, aby utworzyć zaokrągloną krawędź w celu uzyskania bardziej miękkiego wyglądu mebli

1. **Wyłącz** warstwę **dachu**, aby zobaczyć wnętrze domu.
2. Utwórz **Prostokąt \(R\)** o wymiarach **4' x 7'** w północno-wschodnim rogu domu. Wybierz powierzchnię i wyciągnij ją na wysokość **1'-6".**

   ![](../../.gitbook/assets/upperterracesketch_20.png)

3. Wybierz [**narzędzie Zaokrąglenie \(FI\)**](../../tool-library/cover-sweep-loft.md) z **narzędzi Zaawansowane modelowanie** na [**pasku narzędzi operacji**](../../formit-introduction/tool-bars.md)**.**

   ![](../../.gitbook/assets/f7e388e3-4ad0-4fef-a701-0d3176adc2c5.png)

4. W wyświetlonym oknie dialogowym zmień domyślną wartość **zaokrąglenia** na 1".
5. **Kliknij raz** górną powierzchnię łóżka. Po wybraniu powierzchni automatycznie zostanie utworzone zaokrąglenie.

   ![](../../.gitbook/assets/upperterracesketch_21.png)

## Drzewo grup

Zamiast edytować grupę w celu nadania jej nazwy i kategorii, użyjmy **drzewa grup**, które umożliwia szybkie wykonywanie wielu zadań związanych z zarządzaniem modelem.

1. **Kliknij dwukrotnie**, aby wybrać całe łóżko. Dodaj łóżko do **grupy \(G\).**
2. Kliknij ikonę **Drzewo grup** z palet po prawej stronie.

   ![](../../.gitbook/assets/groupstree.png)

3. Jeśli wybierzesz grupę łóżka w obszarze rysunku, zostanie ona wyróżniona na liście **Drzewo grup** \(działa to również w drugą stronę — jeśli wybierzesz grupę na liście, zostanie ona wyróżniona w obszarze rysunku\).
4. Możesz **kliknąć dwukrotnie** nazwę na liście i zmienić ją na **Bed** — wszystkie wystąpienia grupy zostaną zaktualizowane — w naszym przypadku jest tylko jedna.
5. Gdy na liście jest wybrana **grupa Bed**, z listy rozwijanej u góry palety Drzewo grup możesz wybrać kategorię **Meble**.

   ![](../../.gitbook/assets/groupstree_palette.png)

## Scalanie krawędzi, wygładzanie krawędzi i filtrowanie wyboru

Teraz ukryjemy niepotrzebne krawędzie mebli, aby uzyskać gładszy i bardziej miękki wygląd.

1. **Kliknij dwukrotnie**, aby edytować grupę. Wybierz całe łóżko **dwukrotnym kliknięciem**. **Kliknij prawym przyciskiem myszy** i z menu kontekstowego wybierz polecenie **Scal \(MG\)**.

   ![](../../.gitbook/assets/upperterracesketch_215.png)

2. Użyj opcji **Filtr wyboru**, aby ograniczyć wybór okna tylko do **krawędzi.**

   ![](../../.gitbook/assets/25b2428d-bc93-4ae4-9b8a-d8f3749ddb43.png)

3. **Przeciągnij wskaźnik myszy** od lewego górnego do prawego dolnego narożnika, aby dokonać **wyboru okna**. Wybierz w oknie łuk i krawędź w każdym narożniku łóżka. Przytrzymaj naciśnięty klawisz **Ctrl** lub **Shift**, aby dodać je do ustawionego wyboru.
4. **Kliknij prawym przyciskiem myszy** i wybierz opcję **Wygładź krawędzie \(SE\)**

   ![](../../.gitbook/assets/upperterracesketch_216.png)

5. Aby ponownie wyświetlić te krawędzie, **kliknij raz** w celu wybrania górnej powierzchni łóżka, **kliknij prawym przyciskiem myszy** i wybierz opcję **Powierzchnie wygładzone płaszczyzną** \(UE\).

   ![](../../.gitbook/assets/upperterracesketch_217.png)

6. Zmień jeszcze raz **Filtr wyboru**, aby znowu uwzględnić powierzchnie i grupy. Włącz z powrotem warstwę **dachu**. Twój model domu pani Farnsworth jest coraz ładniejszy.

   ![](../../.gitbook/assets/upperterracesketch_22.png)

