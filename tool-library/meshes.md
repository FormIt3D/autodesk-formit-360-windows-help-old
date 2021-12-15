# Siatki

Począwszy od wersji 17.0, program FormIt oferuje nowy typ geometrii: Siatki.

Siatki to lekkie reprezentacje standardowych obiektów programu FormIt, które doskonale zwiększają wydajność geometrii wieloboków, takich jak meble lub elementy otoczenia 3D, na przykład ludzie, drzewa, samochody i oznakowanie. Siatki są również przydatne w przypadku złożonej geometrii DWG, która bez nich mogłaby mieć wpływ na wydajność programu FormIt.

Obiekty można przekształcać w siatki, a siatki można przekształcać z powrotem w obiekty bez utraty danych. Niektóre typy plików są automatycznie importowane jako siatki, na przykład OBJ, STL i DWG. Poniżej znajdziesz więcej informacji na temat przekształcania typów oraz innych korzyści i ograniczeń dotyczących siatek.

### Przekształcanie obiektów w siatki

Dowolną kombinację wierzchołków, krawędzi, powierzchni lub brył można przekształcić w siatkę.

Wystarczy wybrać obiekty i użyć skrótu OM \(Obiekty na siatki\) lub kliknąć prawym przyciskiem myszy i wybrać opcję Obiekty na siatki w menu kontekstowym:

![](../.gitbook/assets/context-menu_object-to-mesh.PNG)

Po przekształceniu obiektów w siatki na górze ekranu zostanie wyświetlony komunikat potwierdzający:

![](../.gitbook/assets/success_object-to-mesh.PNG)

**Podczas przekształcania obiektów w siatki**

* Krawędzie, które zostały wygładzone na obiektach, pozostaną wygładzone w powstałych siatkach.
* Orientacje materiałów na obiektach pozostaną niezmienione w powstałych siatkach.
* Dla każdego zastosowanego materiału jest tworzona siatka. Na przykład w przypadku przekształcania pojedynczego sześcianu pomalowanego 6 różnymi kolorami otrzymamy 6 różnych siatek.
   * Przekształcenie z powrotem w obiekt spowoduje ponowną zamianę poszczególnych siatek w bryłę.
* Wybranie bryły spowoduje przekształcenie i zastąpienie całej bryły siatką, ale wybranie pojedynczych krawędzi lub wierzchołków należących do bryły spowoduje utworzenie nowej siatki na istniejącej geometrii bez wpływu na oryginalną bryłę.
* Przekształcenie zestawu krawędzi lub wierzchołków spowoduje utworzenie pojedynczej siatki liniowej \(siatki złożonej z krawędzi\) lub pojedynczej siatki punktów \(siatki złożonej z punktów\), co oznacza, że nie będzie można wybrać poszczególnych krawędzi lub wierzchołków po ich połączeniu w jedną siatkę. Aby dopasować położenie pojedynczego elementu, należy przekształcić je z powrotem w obiekty.

**Przekształcanie zgrupowanej geometrii w siatki:**

* Siatki dają jeszcze więcej możliwości po przekształceniu całej grupy i wszystkich jej zagnieżdżonych grup.
* Grupy i ich zagnieżdżone elementy można przekształcić w siatki za pomocą wtyczki:
   * Znajdź ikonę narzędzia Plugin Manager po prawej stronie aplikacji:
      * ![](../.gitbook/assets/plugin-manager_icon.PNG)
   * Znajdź wtyczkę „Mesh + Unmesh All” i kliknij pole wyboru, aby ją zainstalować:
      * ![](../.gitbook/assets/plugin-manager_mesh-unmesh-all.PNG)
   * Zostanie wczytana wtyczka Mesh + Unmesh All. Wystarczy wybrać grupę zawierającą obiekty, które mają zostać przekształcone w siatki, a następnie kliknąć opcję Mesh All.
      * ![](../.gitbook/assets/mesh-unmesh-all-plugin.PNG)
   * Podczas przekształcania obiektów zagnieżdżonych lub siatek za pomocą tej wtyczki na górze ekranu będzie wyświetlany komunikat dotyczący aktualizacji z informacjami o liczbie grup i wystąpień grup, na które miała wpływ operacja:

![](../.gitbook/assets/success_mesh-all.PNG)

### Interakcja z siatkami

**Ze względu na ich lekką naturę siatki mają określone ograniczenia i zachowania:**

* Nie można edytować poszczególnych powierzchni, krawędzi ani wierzchołków siatki.
   * Można jednak ponownie malować siatki i przesuwać poszczególne siatki utworzone w wyniku zastosowania do powierzchni innych materiałów \(patrz wyżej\).
* Przyciąganie do siatek jest ograniczone do ich powierzchni i wierzchołków. Ze względu na wydajność przyciąganie i wnioskowanie nie działa z krawędziami siatek.
   * Jednak pliki DWG przekształcone w siatki \(inny typ siatki zwany siatką liniową\) zachowują możliwość przyciągania i wnioskowania w przypadku krawędzi siatki.
* Do siatek nie można stosować poziomów.
* Siatki nie zgłaszają problemów ze szczelnością ani tylnymi powierzchniami. Aby sprawdzić, czy siatki są szczelne, należy przekształcić je z powrotem w obiekty.
   * Obiekty, które były szczelne przed przekształceniem w siatkę, po przekształceniu z powrotem w obiekt pozostają szczelne.
* Siatek nie można używać w zaawansowanych operacjach modelowania, takich jak łączenie/docinanie brył, skorupa 3D, odsunięcie 3D, zaokrąglenie, wyciągnięcie złożone, przeciągnięcie lub zakrywanie.

W przeciwnym razie siatki są wyświetlane i zachowują się tak samo jak wszystkie pozostałe obiekty programu FormIt: umieszczone w grupach, przypisane do warstw, wizualizowane w scenach, używane do analizy itp.

**Jeśli na etykietce narzędzia jest wyświetlana informacja „Na siatce” lub w panelu Właściwości jest wyświetlana informacja o siatce, wiesz, że masz do czynienia z siatką:**

![](../.gitbook/assets/snap_on-mesh.PNG)

![](../.gitbook/assets/properties-panel_mesh.PNG)

**Niektóre typy plików są automatycznie importowane jako siatki w celu zwiększenia wydajności:**

* Pliki STL i OBJ, które mogą zawierać gęstą geometrię, na przykład chmury punktów z innych aplikacji, są automatycznie importowane jako siatki.
* Pliki DWG, które mogą zawierać miliony małych segmentów krawędzi na krzywych o wysokiej jakości, są automatycznie importowane jako siatki.

### Przekształcanie siatek z powrotem w obiekty

Wystarczy wybrać siatki, a następnie użyć skrótu MO \(Siatki na obiekty\) lub kliknąć prawym przyciskiem myszy i wybrać z menu kontekstowego opcję Siatki na obiekty:

![](../.gitbook/assets/context-menu_mesh-to-object.PNG)

Po przekształceniu obiektów w siatki na górze ekranu zostanie wyświetlony komunikat potwierdzający:

![](../.gitbook/assets/success_mesh-to-object.PNG)

**Podczas przekształcania siatek z powrotem w obiekty:**

* Wszystkie obiekty, które przed przekształceniem w siatkę były szczelne lub miały postać bryły, podczas przekształcania z powrotem w obiekt zostaną ponownie połączone w szczelną bryłę.
* Przekształcenie serii krawędzi \(na przykład z pliku DWG\) lub serii wierzchołków \(na przykład z chmury punktów\) w siatkę i z powrotem spowoduje automatyczne umieszczenie obiektów bez siatki w grupie.
   * Zapobiega to scalaniu nowych krawędzi lub wierzchołków z inną geometrią, co mogłoby mieć negatywny wpływ na wydajność.
   * Aby zwolnić krawędzie i/lub wierzchołki, można po prostu usunąć grupowanie powstałej grupy.

**Przekształcanie zgrupowanych siatek z powrotem w obiekty:**

* Aby użyć wtyczki Mesh + Unmesh All w celu przekształcenia grup i ich zagnieżdżonych siatek z powrotem w obiekty, zapoznaj się z powyższymi instrukcjami.

