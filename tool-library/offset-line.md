# Nástroj Odsadit čáru

Pomocí nástroje Odsadit čáru můžete kreslit rovnoběžné neboli odsazené čáry. To je užitečné při vytváření 2D tvarů, které lze později vysunout tak, aby vypadaly jako 3D stěny.

![](../.gitbook/assets/image%20%283%29.png)

Nástroj **Odsadit čáru** funguje podobně jako nástroj [**Čára**](https://windows.help.formit.autodesk.com/tool-library/line-tool):

* Kliknutím nastavte první bod a poté přesuňte kurzor a umístěte následující body, přičemž se čára přichytí k existující geometrii nebo odvozeným osám.
* Zobrazí se náhled výsledného tvaru. Druhý a třetí bod určují rovinu, kterou budou ostatní body sledovat, takže výsledek je rovinný.
* Pokračujte v přidávání bodů. Až budete hotovi, ukončete nástroj kliknutím na tlačítko **Esc** nebo dvojitým kliknutím.
* Všechny průsečíky budou začištěny a sloučeny, takže zůstane jedna vysunutelná plocha.

![Po umístění 2 bodů a tažení 3. bodu](../.gitbook/assets/walls1.png)

Vstupní čára je nakreslena červeně a ve výchozím nastavení je umístěna ve středu odsazených čar.

Zarovnání odsazených čar a jejich tloušťku můžete změnit stisknutím klávesy **Tab**. Tím vyvoláte dialog **Možnosti nástroje**:

![Možnosti nástroje Odsadit čáru](../.gitbook/assets/walls2.png)

Pokud například změníte hodnotu položky **Zarovnání** na **Vlevo** a pro položku **Tloušťka** zadáte hodnotu 6", budou odsazené čáry nakresleny vlevo od vstupních čar, 6 palců od sebe.

![](../.gitbook/assets/walls3.png)

## Užitečné tipy

Uzavřený tvar nakreslíte přichycením k prvnímu umístěnému bodu. Výsledný roh bude automaticky začištěn:

![](../.gitbook/assets/walls4.png)

Vstupní čáry můžete libovolně kreslit přes sebe. Po ukončení nástroje se výsledné průsečíky začistí.

![](../.gitbook/assets/walls5.png)

![](../.gitbook/assets/walls6.png)

Nástroj Odsadit čáru musí ze své podstaty vytvořit geometrii v rovině, takže prvních několik bodů určuje rovinu, kterou budou sledovat ostatní body.

Začněte například kreslit na stěnu krychle, abyste použili rovinu této plochy. Po umístění tří nekolineárních bodů je vstupní rovina pevná pro zbytek bodů. Všimněte si, že při kreslení na plochu je výsledný tvar vložen do plochy, kterou rozdělí na více ploch. Aby se zabránilo vložení, musí být plocha, na které kreslíte, součástí [skupiny](https://windows.help.formit.autodesk.com/tool-library/groups).

![Kreslení na vertikální ploše](../.gitbook/assets/walls7.png)

![Po ukončení nástroje se vloží čáry a s rozdělenými plochami lze dále manipulovat](../.gitbook/assets/walls8.png).

Nástroj Odsadit čáru můžete použít také k trasování z půdorysného výkresu. Importujte půdorys jako obrázek.

* Změňte velikost obrázku tak, aby půdorys měl správné měřítko. Podrobný postup je popsán [zde](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/work-with-images-and-the-ground-plane).
* Pomocí [ortografické kamery](orthographic-camera.md) můžete trasovat v ortografickém [horním pohledu](orthographic-views.md).

![](../.gitbook/assets/walls9.png)

![](../.gitbook/assets/walls10.png)



