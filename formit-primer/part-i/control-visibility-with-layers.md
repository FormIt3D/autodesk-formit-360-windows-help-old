# 1.6 – Řízení viditelnosti pomocí hladin

_Hladiny v aplikaci FormIt umožňují spravovat viditelnost objektů v modelu, podobně jako v aplikaci AutoCAD nebo Photoshop. V této kapitole vytvoříme hladinu k uložení a skrytí objemu budovy pro budoucí analýzu._

_Pokud jste nedokončili poslední část, stáhněte a otevřete soubor_ _**1.6 – Computational Groups with Dynamo.axm**_ _z_ _**datových sad k příručce Základy aplikace FormIt, Část 1**._

## **Vytvoření hladin**

1 – Vytvoření nových hladin:

1. Přejděte na **paletu Hladiny** a třikrát klikněte na ikonu **+**, čímž vytvoříte tři hladiny.
2. Dvakrát klikněte na názvy hladin a přejmenujte je na **Objemy**, **Podlaží hlavní budovy** a **Obrázek půdorysu**

![](../../.gitbook/assets/0%20%2820%29.png)

_**Poznámka:**_ _Kliknutím na název hladiny a jejím přetažením nahoru nebo dolů můžete změnit pořadí hladin._

2 – Přiřazení skupiny **Objemy – hlavní budova** k hladině **Objemy**:

1. Na kreslicí ploše vyberte skupinu **Objemy – hlavní budova**.
2. Na **paletě Hladiny** vyberte v rozevírací nabídce **Výběr na** hladinu **Objemy**. Podobně přiřaďte skupinu **Obrázek půdorysu** k hladině **Obrázek půdorysu**.

![](../../.gitbook/assets/1%20%2813%29.png)

## **Duplikování skupiny**

_Nyní zahájíme proces podrobnějšího modelování budovy. Prvním krokem je vytvoření geometrie podlaží na základě objemů budovy, které již máme k dispozici._

1 – Znovu vyberte skupinu **Objemy – hlavní budova**. Stisknutím kláves **Ctrl+C \(Kopírovat\)** zkopírujte a poté stisknutím kláves **Ctrl+Shift+V \(Vložit na místo\)** vložte objem na stejné místo.

2 – Chcete-li geometrii nové skupiny oddělit od původní skupiny, klikněte pravým tlačítkem myši a v **místní nabídce** vyberte možnost **Vytvořit jedinečné \(MU\)**.

![](../../.gitbook/assets/2%20%2818%29.png)

_**Poznámka**: Nová skupina již není spojena s původní skupinou. Změny nové skupiny nezmění původní skupinu._

## **Vytvoření geometrie podlaží**

1 – Změňte přiřazení hladiny skupiny:

1. Kliknutím vyberte některou ze skupin **Objemy – hlavní budova**.
2. Umístěte skupinu na hladinu **Podlaží hlavní budovy** pomocí rozevíracího seznamu **Výběr na** na **paletě Hladiny**.
3. Zrušte zaškrtnutí políčka u hladiny **Objemy**, abyste skryli její geometrii a ochránili ji před náhodnými úpravami. 

![](../../.gitbook/assets/3%20%2818%29.png)

2 – Dvakrát klikněte na viditelnou skupinu **Objemy – hlavní budova**, kterou chcete upravit. Na **paletě Vlastnosti** přejmenujte skupinu na **Podlaží**.

![](../../.gitbook/assets/4%20%2812%29.png)

3 – **Klikněte** na **horní plochu** geometrie a vyberte ji. Klikněte znovu a začněte táhnout plochu dolů. Při tažení plochy dolů zadejte **11’-2"**. Zobrazí se **dialog Kóta**. Po zadání hodnoty klikněte na tlačítko **OK**. Výsledné podlaží by mělo mít tloušťku 1'. Dvojitým kliknutím na volné místo skupinu ukončete.

![](../../.gitbook/assets/5%20%2810%29.png)

