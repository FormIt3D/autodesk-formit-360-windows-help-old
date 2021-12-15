# Płaszczyzny krzywej i powierzchni

Program FormIt jest wielościennym systemem modelowania, w którym obiekty, takie jak okręgi, łuki i splajny, są reprezentowane przez serię prostych krawędzi. Podobnie zakrzywiona powierzchnia, na przykład ściana walca lub kopuła, składa się z szeregu płaskich powierzchni z ukrytymi krawędziami obramowania.

Domyślnie w programie FormIt używanych jest 40 krawędzi lub płaszczyzn do reprezentacji okręgu i 24 płaszczyzny do reprezentacji zakrzywionego obiektu 3D, na przykład walca. W przypadku bardziej złożonych powierzchni, takich jak kopuła, wartość 24 określa liczbę płaszczyzn tworzących obwód, a także wpływa na gęstość płaszczyzn pozostałej części kształtu.

W programie FormIt dla systemu Windows w wersji 18 i nowszych wartości płaszczyzn powierzchni i krzywej można dostosowywać:

![](../.gitbook/assets/faceting\_planter.gif)

![](<../.gitbook/assets/faceting (1).png>)

**Curve Faceting Quality**

Zmiana parametru Curve Faceting Quality wpłynie na liczbę płaszczyzn używanych podczas rysowania nowych okręgów i łuków w programie FormIt oraz podczas umieszczania kształtów prymitywów. Na przykład ustawienie wartości 64 spowoduje utworzenie 64-stronnego pełnego okręgu lub ćwierćokręgu z 16 płaszczyznami.

Ta wartość wpłynie również na jakość okręgów i łuków importowanych z plików SAT, jak również podczas nanoszenia geometrii z dodatku Dynamo. Tę wartość można ustawić dla nowych szkiców lub tylko dla bieżącego szkicu.

W przypadku istniejących krzywych można również użyć wtyczki Rebuild Curve, aby przebudować **istniejący** łuk lub okrąg za pomocą nowej liczby płaszczyzn:

![](../.gitbook/assets/screen-shot-2020-01-10-at-1.20.53-pm.png)

![](../.gitbook/assets/faceting\_rebuild-curve.gif)

**Surface Faceting Quality**

Zmiana tego ustawienia globalnego wpłynie na jakość zakrzywionych powierzchni 3D importowanych z plików SAT, jak również nanoszonych z dodatku Dynamo.

Na przykład ustawienie wartości 64 spowoduje, że po naniesieniu sfery z dodatku Dynamo będą używane 64 płaszczyzny wokół równika sfery i 64 płaszczyzny w każdym z pierścieni biegnących do biegunów sfery, co szybko się sumuje. Wyższe wartości należy stosować ostrożnie, ponieważ w niektórych przypadkach mogą one mieć wpływ na wydajność programu FormIt. Po uzyskaniu wysokiej jakości rezultatu można [przekształcić go w siatkę](meshes.md), aby poprawić wydajność.

Podczas pracy z dodatkiem Dynamo można zmienić jakość płaszczyzn i kliknąć przycisk „Run Graph” w panelu Właściwości, nie zmieniając żadnych parametrów, aby skorzystać z nowej liczby płaszczyzn:

![](../.gitbook/assets/faceting\_column.gif)

Podobnie jak w przypadku krzywych, jakość płaszczyzn powierzchni można ustawić dla nowych szkiców lub tylko dla bieżącego szkicu.

Pamiętaj, że wartości liczby płaszczyzn są obecnie ograniczone do wielokrotności liczby 4, dlatego podczas ręcznego wprowadzania liczb program FormIt będzie zaokrąglał je do najbliższej wielokrotności. Do przełączania akceptowanych wartości służą również suwaki i strzałki.

![](../.gitbook/assets/units-+-precision.png)
