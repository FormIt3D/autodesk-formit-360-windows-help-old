# 1.6 — Sterowanie widocznością za pomocą warstw

_Podobnie jak w programach AutoCAD i Photoshop, warstwy w programie FormIt umożliwiają zarządzanie widocznością obiektów w modelu. W tym rozdziale utworzymy warstwę, aby zapisać i ukryć bryłę budynku na potrzeby przyszłej analizy._

_Jeśli nie ukończono poprzedniej sekcji, pobierz i otwórz plik_ _**1.6 — Control Visibility with Layers.axm**_ _z folderu_ _**FormIt Primer Part 1 Datasets**._

## **Tworzenie warstw**

1 — Aby utworzyć nowe warstwy:

1. Przejdź do **palety Warstwy** i kliknij znak **+** trzy razy, aby utworzyć trzy warstwy.
2. Kliknij dwukrotnie nazwy warstw, aby zmienić ich nazwy na **Massing**, **Main Building Floor** oraz **Plan Image.**

![](../../.gitbook/assets/0%20%2820%29.png)

_**Uwaga:**_ _Możesz kliknąć nazwę warstwy i przeciągnąć ją w górę lub w dół, aby zmienić kolejność warstw._

2 — Aby przypisać grupę **Massing - Main Building** do warstwy **Massing**:

1. W obszarze rysunku wybierz grupę **Massing - Main Building**.
2. Na **palecie Warstwy** wybierz warstwę **Massing** z menu rozwijanego „**Wybór włączony:”**. Podobnie przypisz grupę **Plan Image** do warstwy **Plan Image**.

![](../../.gitbook/assets/1%20%2813%29.png)

## **Powielanie grup**

_Teraz zaczniemy bardziej szczegółowo modelować budynek. Pierwszym krokiem jest utworzenie geometrii kondygnacji na podstawie już gotowego modelu bryłowego budynku._

1 — Ponownie wybierz grupę **Massing - Main Building**. Naciśnij kombinację klawiszy **Ctrl+C \(Kopiuj\)**, aby skopiować bryłę, a następnie **Ctrl+Shift+V \(Wklej lokalnie\)**, aby wkleić bryłę w tym samym miejscu.

2 — Aby odłączyć nową geometrię grupy od oryginalnej grupy: kliknij prawym przyciskiem myszy, aby uzyskać dostęp do **menu kontekstowego**, i wybierz opcję **Ustaw jako niepowtarzalne \(MU\)**.

![](../../.gitbook/assets/2%20%2818%29.png)

_**Uwaga**: Nowa grupa nie jest już skojarzona z oryginalną. Zmiany w nowej grupie nie spowodują zmian oryginalnej grupy._

## **Tworzenie geometrii kondygnacji**

1 — Ponownie przypisz warstwę grupy:

1. Kliknij jednokrotnie, aby wybrać jedną z grup **Massing – Main Building**.
2. Umieść grupę w warstwie **Main Building Floor**, korzystając z listy rozwijanej **Wybór włączony:** na **palecie Warstwy**.
3. Usuń zaznaczenie warstwy **Massing**, aby ukryć jej geometrię i zabezpieczyć ją przed przypadkowymi zmianami.

![](../../.gitbook/assets/3%20%2818%29.png)

2 — Kliknij dwukrotnie widoczną grupę **Massing – Main Building**, aby ją edytować. Zmień nazwę grupy na **Floor** na **palecie Właściwości**.

![](../../.gitbook/assets/4%20%2812%29.png)

3 — **Kliknij jednokrotnie** **górną powierzchnię** geometrii, aby ją wybrać. Kliknij ponownie i rozpocznij przeciąganie powierzchni w dół. Podczas przeciągania powierzchni w dół wpisz **11’-2"**, a zostanie wyświetlone **okno dialogowe Wymiar**. Po wprowadzeniu wartości kliknij przycisk **OK**. Wynikowa podłoga powinna mieć grubość 1'. Kliknij dwukrotnie poza tym obszarem, aby opuścić tę grupę.

![](../../.gitbook/assets/5%20%2810%29.png)

