# Często zadawane pytania

## Informacje o dodatku FormIt

**Co to jest program FormIt i subskrypcja FormIt Pro?**

FormIt to środowisko do modelowania 3D, wizualizacji, analizy i obliczeń używane w projektowaniu architektonicznym.

Funkcje programu FormIt:

* Solidny mechanizm modelowania brył z rozbudowanymi narzędziami i procesami zoptymalizowanymi pod kątem projektowania budynków.
* Ulepszona wizualizacja środowiska umożliwiająca ilustrowanie wariantów projektu, w tym zapisanych stanów modelu, przy użyciu scen.
* Położenie, obrazy satelitarne i teren 3D z użyciem Map Bing.
* Materiały z Biblioteki materiałów Autodesk.
* Narzędzia do porządkowania modelu i określania widoczności, w tym grupy, warstwy i sceny.
* Narzędzia do analizy, w tym:
   * Sprawdzanie uszczelnienia i tylnych powierzchni w celu diagnostyki i naprawy modelu bryłowego.
   * Słońce i cienie.
   * Analiza oświetlenia naturalnego
   * Analiza energetyczna
* Integracja z produktami Autodesk:
   * BIM 360 Docs
   * Insight \(Analiza energetyczna\)
   * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
   * [Revit](https://formit.autodesk.com/page/formit-revit)
* Obsługa formatów plików:
   * Otwieranie/importowanie
      * AXM, DWG, FBX, SAT, STL, OBJ, WSM, SketchUp, obraz
   * Eksportuj
      * AXM, FBX, OBJ, STL, SAT, DAE, DXF

Program FormIt jest dostępny bezpłatnie w systemie [iOS](https://itunes.apple.com/us/app/autodesk-formit-360/id575282599?mt=8) i [w przeglądarce](https://app.formit.autodesk.com/). Do korzystania z programu [FormIt dla systemu Windows](https://formit.autodesk.com/page/download), najwydajniejszej i najbardziej funkcjonalnej wersji programu FormIt, wymagana jest subskrypcja **FormIt Pro**. Subskrypcja **FormIt Pro** udostępnia również dodatkowe funkcje, takie jak analiza oświetlenia naturalnego i analiza energetyczna, w wersji dla systemu iOS i w przeglądarce. Subskrypcja **FormIt Pro** jest zawarta w kolekcji [Autodesk AEC Collection](https://www.autodesk.pl/collections/architecture-engineering-construction/overview).

**Co się stało z aplikacją FormIt dla systemu Android?**

Aby zoptymalizować ofertę produktu FormIt, musieliśmy podjąć trudną decyzję o wycofaniu aplikacji dla systemu Android. Jeśli jest zainstalowana, będzie nadal działać, ale nie będzie już dostępna w Sklepie Play.

**Jak można uzyskać program FormIt?**

Aby uruchomić wersję dla systemu Windows, wymagany jest dostęp do subskrypcji **FormIt Pro**, która jest częścią subskrypcji [kolekcji branżowej AEC](https://www.autodesk.pl/collections/architecture-engineering-construction/overview). Jeśli więc w Twoim biurze używany jest program Revit, być może masz już dostęp do programu FormIt. Można [pobrać program FormIt dla systemu Windows bezpośrednio z naszej strony internetowej](https://formit.autodesk.com/page/download) lub z aplikacji Autodesk Desktop.

Ponadto wersję internetową można uruchomić bezpłatnie na naszej stronie internetowej: [http://formit.autodesk.com](http://formit.autodesk.com)

Wersję dla systemu iOS można pobrać bezpłatnie ze sklepu Apple App Store \(tylko iPad\).

**Czy uczniowie i nauczyciele mogą bezpłatnie uzyskać dostęp do subskrypcji FormIt Pro?**

Tak! Dostęp do subskrypcji FormIt Pro można uzyskać za pośrednictwem [portalu Autodesk Education](https://www.autodesk.com/education/free-software/formit-pro).

**Jak można nauczyć się korzystania z programu FormIt?**

Najlepiej zacząć od [przewodnika FormIt Primer](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html).

Przewodnik Primer zawiera wiele sekcji, obejmujących zagadnienia dla początkujących \(tworzenie całego nowoczesnego domu\) i zaawansowanych użytkowników \(bardziej zaawansowane metody pracy z programami Revit i Dynamo\).

Mamy również ponad 20 filmów w serii webinariów FormIt Friday. Można je znaleźć na naszym [kanale w serwisie YouTube](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH).

## Praca z programem Revit

**W jaki sposób program FormIt współdziała z programem Revit?**

FormIt to osobna aplikacja do szkicowania i projektowania 3D, ale tworzone w niej dane można łatwo przekształcić w dane programu Revit [za pomocą dodatku FormIt dla programu Revit](https://formit.autodesk.com/page/formit-revit).

**Co się stanie po zaimportowaniu danych do programu Revit?**

Począwszy od wersji 2016, program Revit jest dostarczany z dodatkiem umożliwiającym korzystanie z danych programu FormIt. Podczas importowania pliku AXM z programu FormIt do programu Revit ten dodatek analizuje poszczególne obiekty w pliku i odtwarza je w programie Revit za pomocą interfejsu API. Domyślnie wszystkie elementy z programu FormIt są klasyfikowane jako Bryła.

Konwerter FormIt pobiera wszystkie obiekty brył i tworzy rodzinę brył w programie Revit za pomocą [interfejsu API kształtu bezpośredniego](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/PLK/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html).

Kształt bezpośredni jest obiektem nieedytowalnym używanym w procesach roboczych IFC. Mimo że nie jest dostępny do edycji, jego zdecydowaną zaletą jest przenoszenie całych tekstur materiałów między programami FormIt i Revit. [Tu znajduje się przewodnik](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html), w którym szczegółowo wyjaśniono proces roboczy importu z programu FormIt do programu Revit.

**Czy w programie FormIt można tworzyć ściany, stropy i inne rodziny systemowe programu Revit?**

Nie bezpośrednio. Jak wspomniano powyżej, każdy obiekt domyślnie przypisywany jest do kategorii Bryła. Aby utworzyć ściany, stropy itp., należy zaimportować model do programu Revit za pomocą dodatku konwertera i użyć własnych narzędzi programu Revit, aby utworzyć rodziny systemowe na podstawie oryginalnego modelu bryłowego.

**Czy z programu Revit można wysłać dane z powrotem do programu FormIt?**

Tak. Aby zaimportować dane z powrotem do programu FormIt, należy wyeksportować cały plik programu Revit lub jego _część_ (ta druga opcja jest preferowana) do formatu pliku SAT. Zazwyczaj nie ma potrzeby wysyłania WSZYSTKICH danych programu Revit do programu FormIt. Zamiast tego należy utworzyć w programie Revit przefiltrowany widok zawierający tylko minimalną niezbędną ilość danych \(na przykład stropy i ściany\) przed zapisaniem pliku w formacie SAT.

## Praca z innymi aplikacjami

**Dlaczego domyślnie używany format pliku nosi nazwę AXM?**

Przed nadaniem oficjalnej nazwy FormIt program ten nosił nazwę wewnętrzną XModeler, a więc opracowany przez nas format pliku otrzymał nazwę Autodesk X Modeler, w skrócie AXM.

**Jakie formaty 3D można importować do programu FormIt?**

* Wersja dla systemu Windows: AXM, DWG, FBX, OBJ, SAT, SKP, STL
* Wersja internetowa: OBJ, STL
* Wersja dla systemu iOS: OBJ, STL, SAT

**Jakie formaty można eksportować z programu FormIt?**

* Wersja dla systemu Windows: FBX, OBJ, SAT, STL, DAE, DXF
* Wersja internetowa: OBJ, SAT, STL
* Wersja dla systemu iOS: OBJ

**W jaki sposób program FormIt współdziała z dodatkiem Dynamo?**

[Dowiedz się, jak program FormIt i dodatek Dynamo współdziałają ze sobą](https://formit.autodesk.com/page/formit-dynamo) w procesach roboczych projektowania obliczeniowego.

**Jak program FormIt wypada na tle programu SketchUp?**

* Lepsze [**współdziałanie z programem Revit**](../tool-library/revit.md).****
* [**Integracja z dodatkiem Dynamo**](../tool-library/dynamo.md) na potrzeby projektowania obliczeniowego.
* Własne narzędzia do [**analizy oświetlenia naturalnego**](../tool-library/solar-analysis.md) i [**analizy energetycznej**](../tool-library/energy-analysis.md) obsługiwane przez oprogramowanie Autodesk Insight.
* Bardziej niezawodne jądro modelowania brył umożliwiające wykonywanie zaawansowanych operacji modelowania.
* Własne zaawansowane narzędzia modelowania, takie jak [**Przeciągnięcie, Zakrycie, Wyciągnięcie złożone**](../tool-library/cover-sweep-loft.md), Odsunięcie/tworzenie skorupy bryły, Połączenie/zaokrąglenie 3D i [**Spłaszczenie powierzchni**](../tool-library/flatten-face.md).
* Wiele widocznych [**płaszczyzn przekroju**](../tool-library/section-planes.md).
* Narzędzia diagnostyczne, takie jak [**wyświetlanie problemów ze uszczelnieniem i wyświetlanie tylnych powierzchni**](../tool-library/visual-styles.md).
* [**Eksportowanie elementów modelu**](../tool-library/export-data.md) na podstawie wyboru i/lub widoku.
* Własna funkcja eksportowania plików OBJ, SAT i STL.

**Czy można używać skrótów klawiaturowych z programu SketchUp?**

Tak! Program FormIt dla systemu Windows zawiera w pełni edytowalną mapę klawiatury. Wiele często używanych skrótów z programu SketchUp jest już dostępnych domyślnie, ale można je edytować w menu Edycja &gt; Preferencje.

**Czy można używać plików DWG?**

Tak! Program FormIt obsługuje importowanie plików DWG 2D i 3D.

## Typowe pytania dotyczące pomocy technicznej

**Jak uzyskać pomoc techniczną?**

Możesz zacząć od kontaktu ze sprzedawcą Autodesk lub odwiedzić nasze [forum programu FormIt](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=en). Najlepiej najpierw wyszukać pytanie, na które potrzebujesz odpowiedzi — jeśli nie znajdziesz odpowiedzi, opublikuj nowy temat i zaczekaj na odpowiedź od zespołu programu FormIt.

**Co zrobić, jeśli nie mogę się zalogować?**

* Ten [wpis na forum](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572?profile.language=en) zawiera informacje o typowych problemach z logowaniem.
* Jeśli masz komputer z możliwością przełączania między kartami graficznymi \(GPU\), ważne jest, aby na potrzeby programu FormIt zawsze była używana karta GPU o wyższej wydajności. Tu znajdziesz instrukcje dotyczące kart [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) i [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1).

**Co zrobić w przypadku niepowodzenia analizy energetycznej programu Insight?**

Jeśli funkcja analizy energetycznej programu Insight zgłosi błąd lub nie zwróci żadnych wyników, [zapoznaj się z naszą stroną dotyczącą analizy energetycznej programu Insight](https://formit.autodesk.com/page/formit-insight), aby uzyskać wskazówki dotyczące rozwiązywania typowych problemów.

