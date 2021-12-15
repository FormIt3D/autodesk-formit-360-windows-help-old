# Poziomy i powierzchnia

Po utworzeniu geometrii w programie FormIt można zastosować poziomy, aby wskazać, gdzie znajdują się rzędne kondygnacji, i wygenerować obliczenia powierzchni.

Zobacz poziomy w działaniu, korzystając z podręcznika [FormIt Primer](../formit-primer/part-i/adding-floors-with-levels.md).

## Tworzenie i konfigurowanie poziomów

Panel Poziomy znajduje się po prawej stronie programu FormIt dla systemu Windows:

![](../.gitbook/assets/20191217-levels-panel-1.png)

#### Tworzenie i usuwanie poziomów

* Utwórz nowy poziom, klikając przycisk „+”.
* Utwórz serię poziomów, klikając przycisk „++”.
   * Pozwoli to na określenie liczby tworzonych poziomów i odległości pionowej między nimi.
* Wybierz co najmniej jeden poziom i kliknij przycisk „-”, aby go usunąć.

#### Zmiana nazw, ustawianie rzędnych i ponowne numerowanie poziomów

* Zmień nazwę poziomu, klikając dwukrotnie jego nazwę lub klikając prawym przyciskiem myszy i wybierając opcję „Edytuj nazwę”.
* Dopasuj rzędną poziomu, klikając dwukrotnie tę liczbę lub klikając prawym przyciskiem myszy i wybierając opcję „Edytuj rzędną”.
* Kliknij ikonę Odśwież u góry, aby ponownie ponumerować poziomy.
   * Jest to przydatne, jeśli dodano lub usunięto poziomy i domyślny schemat nazewnictwa jest nieuporządkowany \(np. Poziom 1, Poziom 2, Poziom 5\).
   * Ten przycisk ignoruje wszystkie poziomy o nazwach niestandardowych, ale ponownie numeruje wszystkie poziomy o nazwach zgodnych ze składnią „Poziom 1”.

## Stosowanie poziomów

Aby zastosować poziomy do obiektu, należy wybrać obiekt i przejść do panelu Właściwości.

Należy pamiętać, że aby można było zastosować poziomy do obiektu, musi on być bryłą, bez problemów z powierzchnią tylną ani ze szczelnością. [Dowiedz się, jak sprawdzić model pod kątem problemów z powierzchnią tylną i szczelnością](https://formit.autodesk.com/blog/post/repairing-solid-models).

Po wybraniu obiektu bryłowego w obszarze rysunku \(w tym przykładzie prostej powłoki budynku\) w panelu Właściwości zostanie wyświetlone pole wyboru „Użyj poziomów”.

* Jeśli w szkicu programu FormIt już zdefiniowano poziomy \(zobacz powyżej\), zaznaczenie tego pola spowoduje użycie wszystkich poziomów, które przecinałyby ten kształt \(ze zignorowaniem tych, które wypadłyby zbyt wysoko lub zbyt nisko\).
* Jeśli szkic programu FormIt nie zawiera jeszcze poziomów, zaznaczenie tego pola spowoduje utworzenie wystarczającej liczby poziomów domyślnych\(o wysokości między kondygnacjami równej 12' \), aby przeciąć cały kształt, i automatycznie zastosuje te poziomy do obiektu.

![](../.gitbook/assets/20191217-properties-panel.png)

## Poziomy + program Revit

W przypadku zastosowania poziomów do geometrii programu FormIt zostaną one wysłane do programu Revit podczas korzystania z [dodatku FormIt](https://formit.autodesk.com/page/formit-revit).

W programie Revit można używać poziomów programu FormIt do tworzenia skojarzonych z nimi zakresów kondygnacji, kondygnacji według powierzchni i rzutów kondygnacji.



