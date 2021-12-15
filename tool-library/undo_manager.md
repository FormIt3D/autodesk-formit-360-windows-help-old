# Menedżer cofania

Program FormIt zawiera wyjątkowy system poleceń Cofnij/Wykonaj ponownie, którego można używać na dwa różne sposoby: do cofania według grupy lub chronologicznie i globalnie:

* Wybranie polecenia Cofnij/Wykonaj ponownie podczas edycji grupy zagnieżdżonej wpłynie tylko na zmiany wewnątrz tej grupy.
   * Oznacza to, że można wprowadzić zmiany w tej grupie, a następnie wprowadzić wiele zmian w innych grupach i po powrocie do tej pierwszej grupy cofać ostatnie zmiany wprowadzone w tej grupie bez wpływu na zmiany wprowadzone później w innych miejscach.
* Polecenie Cofnij/Wykonaj ponownie użyte w szkicu głównym \(a nie podczas edycji grupy\) działa podobnie jak tradycyjne systemy Cofnij/Wykonaj ponownie: cofnięta zostanie ostatnia zmiana wprowadzona w **dowolnej** grupie na podstawie kolejności chronologicznej.

Menedżer cofania rejestruje wszystkie zmiany w każdej grupie w modelu programu FormIt, w tym zmiany wprowadzone w szkicu głównym. Ułatwia to wizualne zrozumienie tego, które operacje zostały cofnięte w dowolnej grupie w modelu.

![](../.gitbook/assets/undo-manager.png)

Menedżer cofania wyróżnia **pogrubieniem czcionki** stan bieżący, jak również wszystkie operacje poprzedzające ten stan oraz wszystkie operacje, które wykonano, ale cofnięto.

Można kliknąć stan prawym przyciskiem myszy i wybrać opcję „Przełącz do”, aby odpowiednio cofnąć lub wykonać ponownie w celu powrócenia do tego stanu modelu.

Grupy, które jawnie usunięto lub już nie istnieją z powodu cofnięcia lub ponownego wykonania operacji, są wyświetlane jako \*Nieaktywne\*. Można je przywrócić przez cofanie lub ponowne wykonywanie operacji w odpowiedniej grupie nadrzędnej do momentu ich ponownego pojawienia się.

