# Analiza oświetlenia naturalnego i analiza energetyczna

Po utworzeniu modelu można go wykorzystać do zbadania **wpływu oświetlenia naturalnego i energii** w projekcie. Te funkcje są wbudowane w programie FormIt, dzięki czemu już najwcześniejsze badania można rozpatrywać w kontekście wydajności budynku. Te funkcje są dostępne tylko w programie **FormIt Pro**. Jeśli korzystasz z aplikacji internetowej, możesz nie mieć do nich dostępu.

Jeśli ostatnia sekcja nie została ukończona, kliknij opcje Plik &gt; Otwórz i wybierz plik **farnsworth08.axm** z folderu FormIt Primer.

## Cienie

Przed użyciem tych narzędzi analizy należy [ustawić położenie](). Zapewnia to programowi FormIt dostęp do dokładnych danych dotyczących słońca, cieni i klimatu.

1. Kliknij ikonę słońca na [**pasku narzędzi operacji**](../../formit-introduction/tool-bars.md) i sprawdź opcję **Cienie \(DS\)**.

   ![](../../.gitbook/assets/3bdf0e2a-0ad4-4aac-b6fc-5e789643b0d6.png)

2. Dostosuj suwaki **Dzień** i **Czas**, aby zaobserwować, jak zmieniają się cienie.

   ![](../../.gitbook/assets/upperterracesketch_32.png)

3. Zwróć uwagę, że kryty taras jest zacieniony w najgorętszych godzinach letnich — z pewnością nie jest to przypadek, ale kwestia projektu.

**Uwaga**: Cienie mogą powodować spadek wydajności aplikacji. Dwie sugestie dotyczące łagodzenia tego problemu: wyłącz cienie, jeśli spowalniają nawigację, lub wyłącz warstwy, na przykład warstwę **furniture**, jeśli nie są one potrzebne do badania cieni.

## Analiza oświetlenia naturalnego

Projektanci, którzy są osobami polegającymi na reprezentacjach wizualnych, mogą poznawać i prezentować niesamowitą ilość informacji za pomocą wykresów ciepła, takich jak ten, który zamierzamy utworzyć.

1. W dolnej części [**menu Słońce**](../../formit-introduction/tool-bars.md) kliknij przycisk **Analiza oświetlenia naturalnego**.
2. Tryb specjalny umożliwia włączenie opcji **cieni**, **skrótów klawiaturowych** i innych **pasków narzędzi**.
3. Zachowanie wyboru jest zmodyfikowane w trybie **Analiza oświetlenia naturalnego**. Można wybierać **z grup** (nie trzeba przytrzymywać klawisza **Ctrl** ani **Shift**), aby dodawać elementy do zestawu wyboru, i można usuwać zaznaczenie elementów, klikając je ponownie. Można **klikać pojedynczo**, **klikać dwukrotnie** lub **wybierać geometrię za pomocą okna**.
4. Wybierz powierzchnie, które chcesz zbadać. **Kliknij pojedynczo** górę **dachu** i górę **stropów**. Unikaj wybierania małych elementów, takich jak meble.

   ![](../../.gitbook/assets/upperterracesketch_33.png)

5. W lewym górnym rogu obszaru roboczego znajduje się pasek narzędzi **Analiza oświetlenia naturalnego**. Kliknij przycisk **Analiza**. Program FormIt obliczy i wyrenderuje powierzchnie. Ustawienia w tym miejscu można dostosować przed analizą **oraz** po jej zakończeniu.

   ![](../../.gitbook/assets/solaranalysis.png)

6. Ustawienie **Szczyt miesiąca** zawiera wartości **szczytowe** \(w BTU/stopy kwadratowe\) dla określonego miesiąca. Jest to przeznaczone do **analiz cieniowania**. Można zmienić ustawienie miesiąca, a grafika zostanie natychmiast zaktualizowana. **Umieść kursor** na analizowanej powierzchni, aby uzyskać **określoną** wartość.

   ![](../../.gitbook/assets/460060a0-ea3b-4095-af45-40045811be22.png)

7. Ustawienie **Rok łącznie** pokazuje **skumulowaną** energię dla całego roku \(w kWH/metry kwadratowe\). Jest to przeznaczone do **badań potencjału fotowoltaicznego**.

   ![](../../.gitbook/assets/a9f61dfb-dfc9-4751-b145-b131a69c53cf.png)

8. Te badania **analizy oświetlenia naturalnego** można wyeksportować, klikając opcję **Plik &gt; Eksportuj \(Ctrl + E\)** i wybierając opcję **Obraz** z listy po lewej stronie.

## Analiza energetyczna w usłudze Insight

W programie FormIt zintegrowano te same narzędzia do analizy wydajności budynku, które są używane w programie Revit. Program **Insight** udostępnia pulpit nawigacyjny parametrów systemu budynku, które można dostosować, aby odzwierciedlały potencjalne scenariusze bez konieczności **ponownego analizowania** geometrii modelu. Usługa Insight działa najlepiej z geometrią **massing** programu FormIt.

1. Upewnij się, że zalogowano się na koncie Autodesk. Wyłącz **wszystkie** warstwy **z wyjątkiem** warstwy **massing**. Geometria musi mieć zastosowany co najmniej jeden **poziom**.
2. Program FormIt wyśle tylko **widoczną** geometrię do usługi Insight. Należy pamiętać, że nawet prosta **bryła** spowoduje zwrócenie mnóstwa danych z usługi **Insight**.

   ![](../../.gitbook/assets/energymassing.png)

3. Kliknij przycisk **Insight &gt; Generuj Insight**. Analiza zostanie uruchomiona w chmurze, dzięki czemu można kontynuować modelowanie podczas obliczeń.

   ![](../../.gitbook/assets/energymenu.png)

4. Po zakończeniu analizy kliknij przycisk **Wyświetl Insight**, aby wyświetlić **model energetyczny** i **współczynniki wydajności** \(opcjonalnie można odwiedzić witrynę internetową bezpośrednio pod adresem [**http://insight.autodesk.com**](http://insight.autodesk.com/)\).

   ![](../../.gitbook/assets/energydashboard.png)

5. Na pulpicie nawigacyjnym usługi Insight można ustawić wartość \(lub zakres wartości\) dla każdego widżetu **Współczynnik wydajności**, klikając współczynnik i przeciągając niebieskie kropki. Zakres jest pomocny, jeśli nie wiesz, jaki konkretnie system będzie używany w budynku.
6. Po każdej zmianie **współczynnika** aktualizowany jest całkowity **zakres kosztów energii** \(mierzony w USD/metr kwadratowy/rok\). Możesz sprawdzić wydajność projektu na tle testów porównawczych, takimi jak **Ashrae 90.1** i **Architecture 2030**.
7. Jeśli projekt ulegnie drastycznym zmianom, można ponownie wysłać zaktualizowaną bryłę do tego samego pulpitu nawigacyjnego. Aby utworzyć **nowy** pulpit nawigacyjny dla zaktualizowanego projektu, najpierw należy użyć polecenia **Zapisz jako** w programie FormIt.
8. Jeśli analiza energetyczna nie powiodła się, być może występują związane z geometrią **problemy z uszczelnieniem \(DW\)**, które można przejrzeć i rozwiązać w programie FormIt.
9. Wyłącz warstwę **massing** i ponownie włącz wszystkie pozostałe warstwy.

