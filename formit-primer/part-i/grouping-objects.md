# 1.5 – Seskupování objektů

_Skupiny v aplikaci FormIt fungují podobně jako rodiny v aplikaci Revit a komponenty v aplikaci SketchUp. Seskupení různých objektů zabraňuje spojení jejich geometrie. Kopie skupiny se chovají jako instance původní geometrie, což znamená, že změny jedné kopie ovlivní všechny kopie._

_Pokud jste nedokončili poslední část, stáhněte a otevřete soubor_ _**1.5 – Group Objects.axm**_ _z_ _**datových sad k příručce Základy aplikace FormIt, Část 1**._

## **Vytvoření skupiny**

1 – Dvakrát klikněte na objem horní terasy, abyste ji vybrali.

2 – Klikněte pravým tlačítkem myši a vyberte položku **Skupina \(G\)** nebo jednoduše stiskněte klávesu **G**.

![](../../.gitbook/assets/0%20%281%29.jpeg)

3 – Všimněte si, že po vytvoření skupiny se automaticky aktivuje nástroj Přesunout.

## **Přesunutí skupiny**

1 – Pro usnadnění procesu modelování zapněte funkci **Přichytit k osnově \(SG\)**, pokud byla vypnuta.

![](../../.gitbook/assets/1%20%2814%29.png)

2 – Chcete-li začít přesouvat vybraný objekt, stále v nástroji **Přesunout \(M\)** klikněte na libovolný dolní roh objemu. Poté přesuňte kurzor nahoru. Měla by se objevit modrá čára osy \(Z\). Tato čára vám pomůže přesunout objekt rovně nahoru.

3 – S viditelnou modrou osou zadejte **4'-6"**. Zobrazí se dialog Kóta. Po zadání kóty klikněte na tlačítko **OK** nebo stiskněte klávesu **Enter**. Tím se celý objem přesune nahoru ze základní roviny podél **osy Z**.

_**Poznámka:**_ _Podobně jako v aplikaci Revit můžete také zadat_ _**4'6**,_ _**4'6"**_ _nebo_ _**4.5** a aplikace bude hodnotu interpretovat jako 4 \(stopy\) 6 \(palců\) (při použití britských jednotek)._

![](../../.gitbook/assets/2%20%282%29.png)

## **Úpravy skupiny**

1 – Dvakrát klikněte na objem, čímž přejdete do **režimu úprav skupiny**. 

1. Na **paletě Vlastnosti** přejmenujte skupinu na **Objemy – hlavní budova**.
2. Chcete-li uložit změny a ukončit režim **úprav skupiny**, klikněte na ikonu zaškrtnutí **Dokončit úpravy skupiny** v levém horním rohu kreslicí plochy nebo dvakrát klikněte na volné místo.

![](../../.gitbook/assets/3%20%2812%29.png)

_**Poznámky**:_

* _Další informace o možnostech_ _**kategorie**_ _naleznete v kapitole_ _**Práce s aplikací Revit**_ _._‌
* _Každá skupina má vlastní historii vrácení/opakovaného provedení akcí, která se liší od celkového projektu. Můžete kliknout na šipky_ _**Zpět**_ _a_ _**Znovu**_ _v_ _**Průvodci úpravami skupiny**_ _v levém horním rohu kreslicí plochy._

## **Použití podlaží na skupinu**

_**Poznámka:**_ _Seskupení geometrie přepíše předchozí nastavení, která jste na geometrii použili. Proto bude nutné znovu použít podlaží z předchozího cvičení._

1 – Použití úrovní na skupinu:

1. Vyberte skupinu **Objemy** **– hlavní budova** tak, že na ni kliknete.
2. Přejděte na **paletu Vlastnosti** a zaškrtněte políčko **Použít podlaží**
3. Zrušte zaškrtnutí všech ostatních položek a zachovejte pouze podlaží **Hlavní budova**.
4. V poli **Plocha podle podlaží** se zobrazí hrubá plocha aktuálně vybraných objektů. Plocha každého **podlaží** je zobrazena před názvem každého **podlaží**.
5. Pokud se nezobrazí modrá čára horizontálně protínající objekt, zapněte zobrazení podlaží v nabídce **Nastavení &gt; Vizuální styly &gt; Zobrazit podlaží \(DL\)**

_**Poznámka:** Pokud není uvedena žádná plocha pro podlaží_ _**hlavní budovy**_ _, je možné, že geometrie neprotíná podlaží, která by měla být ve výšce 4'-6". Problém vyřešte změnou polohy geometrie nebo výšky_ _**podlaží**_ _tak, aby se protínaly._

![](../../.gitbook/assets/levels-to-groups.png)

2 – Zrušte výběr skupiny stisknutím klávesy **Esc** nebo kliknutím na volné místo. Pokud není vybrán žádný objekt, na **paletě Vlastnosti** se zobrazí celková hrubá plocha náčrtu, nikoli plocha konkrétního objektu.

![](../../.gitbook/assets/5%20%2815%29.png)

## **Správa skupin**

1 – Zobrazení a správa všech skupin v náčrtu:

1. Přejděte na **paletu Strom skupin**. Zde uvidíte následující skupiny:
   * **Terén** – skupina automaticky vytvořená při importu **satelitního snímku**.
   * **Objemy – hlavní budova** – skupina geometrie objemu budovy, kterou jsme právě vytvořili.
   * **skupina 2** – nepojmenovaná skupina obsahující obrázek půdorysu podlaží.
2. Chcete-li přejmenovat **skupinu 2** na paletě Strom skupin, dvakrát klikněte na **skupinu 2** a poté zadejte text **Obrázek půdorysu**.

![](../../.gitbook/assets/6%20%284%29.png)

_**Poznámky:**_

* _Aby byl model přehledný, doporučujeme zadávat popisné názvy skupin._
* _Toto je praktický způsob správy a úpravy všech skupin v modelu z jednoho místa._

2 – Se stále vybranou skupinou **Obrázek půdorysu** přejděte na **paletu Vlastnosti**. Všimněte si, že název skupiny byl aktualizován také v poli **Skupina**.

![](../../.gitbook/assets/7.png)

## **Nástroj Skrýt kontext skupiny**

_Tento nástroj představuje rychlý způsob, jak skrýt veškerou geometrii mimo skupinu, kterou právě upravujete. To je velmi užitečné, pokud pracujete s velkým a složitým modelem a ostatní geometrie vám překážejí._

1 – Izolování skupiny:

1. Chcete-li skupinu upravit, dvakrát klikněte na její geometrii.
2. V **hlavní nabídce** přejděte k položce **Nastavení** a zaškrtněte políčko **Skrýt kontext skupiny** nebo stiskněte klávesu **H**. Všimněte si, že **obrázek půdorysu** zmizel.
3. Dokončete úpravy skupiny. Režim **Skrýt kontext skupiny \(H\)** je aktivní pouze v **Průvodci úpravami skupiny**.
4. Chcete-li tento režim opět vypnout, stačí stisknout klávesu **H**. Tuto možnost lze kdykoli přepnout, uvnitř skupiny i mimo ni.

![](../../.gitbook/assets/8%20%285%29.png)

