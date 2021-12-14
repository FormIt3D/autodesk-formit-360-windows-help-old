# 1.11 – Import modelů pomocí knihovny obsahu

_V této kapitole naimportujete existující modely aplikace SketchUp a pomocí knihovny obsahu aplikace FormIt umístíte rodiny, které byly převedeny z aplikace Revit. Všimněte si, že soubory SKP otevírané v aplikaci FormIt obsahují nedotčené materiály, skupiny, komponenty, hladiny a scény. Aby byly vaše projekty přehledné a uspořádané, může být nutné provést určité vyčištění._

_V této kapitole budeme používat soubory ze složky_ **Datová sada Farnsworth House &GT; Podpůrné soubory**. Pokud jste tak dosud neučinili, stáhněte si požadované složky nebo celou datovou sadu z _**datových sad k příručce Základy aplikace FormIt, Část 1**._

## **Import a úprava souborů SKP**

_Nejprve si projdeme postup přidání části staženého obsahu do vaší vlastní osobní knihovny obsahu_. V tomto cvičení budeme používat pouze soubory SKP. Další informace o otevírání a importu jiných formátů souborů naleznete v [**tomto blogovém příspěvku o funkcích aplikace FormIt 2021.2**](https://formit.autodesk.com/blog/post/formit-2021-2-and-new-revit-add-in-now-available) a v **této kapitole pojednávající o** **pokročilém importu a exportu formátu souborů**.

1 – Nezapomeňte **uložit (Ctrl+S)** jakoukoli otevřenou práci a poté vytvořte nový náčrt FormIt. Postupujte následovně:

1. Otevřete další relaci aplikace FormIt v novém okně tak, že kliknete pravým tlačítkem myši na ikonu aplikace FormIt na **hlavním panelu systému Windows** a pak kliknete na ikonu aplikace **FormIt**. Tím se otevře nové okno aplikace FormIt, ve kterém můžete souběžně spouštět dvě relace aplikace FormIt.
2. Případně můžete po uložení práce kliknout na příkaz **Nový náčrt \(Ctrl+N\)** v rozevíracím seznamu **Soubor** na panelu **Hlavní nabídka**.

![](../../.gitbook/assets/0%20%2819%29.png)

2 – Ve složce **Datová sada Farnsworth House &gt; Podpůrné soubory &gt; FormIt** v **datové sadě Farnsworth House** vytvořte novou složku s názvem _**Vlastní obsah FormIt**._

3 – **Uložte \(Ctrl+S\)** nový náčrt do této složky. Doporučujeme jej pojmenovat: **Ottoman – Barcelona\_Mies.axm**

4 – V novém prázdném souboru aplikace FormIt:

1. **Importujte místní soubor \(Ctrl+I\)** výběrem možnosti **Importovat &gt; Místně…** v rozevíracím seznamu **Soubor** na panelu **Hlavní nabídka**.
2. Ve složce **Datová sada Farnsworth House &gt; Podpůrné soubory &gt; SketchUp** vyberte soubor **Ottoman – Barcelona\_Mies.skp** a klikněte na tlačítko **Otevřít**.

_**Poznámka:**_ _Pokud nevidíte soubor_ _**Ottoman – Barcelona\_Mise.skp**, zkontrolujte, zda je v rozevíracím seznamu formátu souborů v pravém dolním rohu nastavena možnost_ _**Všechny podporované formáty**._

![](../../.gitbook/assets/1%20%287%29.png)

5 – Přejmenujte importovanou skupinu na **Ottoman – Barcelona\_Mies**.

6 – Když tento model nakonec naimportujete do souboru Farnsworth House, bude umístěn pomocí bodu **počátku** tohoto souboru. Chcete-li řídit bod umístění, je třeba přesunout skupinu **Ottoman - Barcelona\_Mies** tak, aby se jeden z jejích rohů nacházel v bodu **počátku**. Postupujte následovně:

1. Ujistěte se, že je zapnuta možnost **Přichytit k osnově \(SG\)**. Nakreslete referenční **čáru \(L\)** začínající v bodu **počátku** \(zde se protínají osy X, Y a Z). Kliknutím na libovolné místo umístěte druhý bod.
2. Vyberte skupinu sedačky a spusťte příkaz pro přesun kliknutím na levý dolní roh nohy, jak je znázorněno níže. _Další informace o přesouvání objektů naleznete v předchozích kapitolách._
3. Přesuňte skupinu do bodu **počátku** přichycením k počátečnímu bodu referenční čáry, kterou jste právě nakreslili.
4. Odstraňte referenční čáru.

![](../../.gitbook/assets/2%20%2817%29.png)

7 – Doporučujeme odstranit všechny nežádoucí hladiny, které byly importovány se souborem SKP, protože všechny hladiny tohoto modelu budou nakonec importovány do našeho modelu domu Farnsworth House. Provedete to tak, že přejdete na **paletu Hladiny**, vyberete položku **Hladina 0** a kliknete na tlačítko **-**. Tím dojde k odstranění hladiny při zachování její geometrie.

![](../../.gitbook/assets/3%20%2816%29.png)

_**Poznámka:**_ _Kdykoli odstraníte hladinu, všechny geometrie nebo skupiny, které byly v této hladině, budou přiřazeny k hodnotě_ _**Žádná hladina**, což je výchozí hodnota pro všechny objekty, které dosud nebyly přiřazeny k nějaké hladině._

## **Vytvoření miniatury obsahu**

_V tomto kroku nastavíte scénu, která bude použita jako miniatura_ _**obsahu**_ _, a která se zobrazí na paletě_ _**Knihovna obsahu**._

1 – Definujte nastavení zobrazení pro scénu miniatury:

1. Na kartě **Prostředí** na **paletě Vizuální styl** zrušte zaškrtnutí všech políček a nastavte barvu **Dolní/Pozadí** na bílou.
2. Ujistěte se, že je režim pohledu nastaven na možnost **Perspektivní** **\(VP\)**.
3. Pomocí **nástrojů navigace v pohledech** přibližte pohled a vyberte umístění kamery, které dobře zobrazuje objekt, podobně jako na obrázku níže.

![](../../.gitbook/assets/4%20%2813%29.png)

2 – Chcete-li uložit nastavení, které jste právě nastavili, vytvořte scénu:

1. Přejděte na **paletu scén**.
2. Klikněte na tlačítko **+**. Tím se vytvoří nová scéna na základě aktuálních nastavení.
3. Přejmenujte ji na **Miniatura** a zkontrolujte, že jsou zaškrtnuta alespoň první čtyři políčka: **Kamera**, **Hladiny**, **Slunce a stíny** a **Vizuální styly**. Ostatní nastavení scény nejsou pro vytvoření miniatury obrázku důležitá.
4. Tlačítkem **Aktualizovat scénu** můžete kdykoli aktualizovat **scénu**, aby odpovídala aktuálnímu pohledu kamery a vizuálnímu nastavení.

![](../../.gitbook/assets/5%20%2811%29.png)

3 – Znovu **uložte \(Ctrl+S\)** dokončený model sedačky. Všimněte si, že **miniatura obsahu** je vytvořena z aktuálního pohledu při posledním uložení modelu, proto se před uložením ujistěte, že se nacházíte ve **scéně Miniatura**.

_Pokud si přejete, můžete svůj soubor porovnat s naším, a to tak, že otevřete soubor_ _**Ottoman - Barcelona\_Mies.axm**_ _uložený ve složce_ _**Datová sada Farnsworth House &GT; Podpůrné soubory &gt; FormIt &gt; Nábytek**_ _v_ _**datové sadě Farnsworth House**.‌_

_Stejným postupem jako výše můžete postupovat u souborů SKP lavice a židle umístěných ve stejné složce jako sedačka._

_**Tip:**_ _Pro urychlení postupu doporučujeme použít právě vytvořený soubor_ _**Ottoman - Barcelona\_Mies.axm**_ _jako šablonu. Při modelování můžete zapnout_ _**rastr**_ _a_ _**osy**_ _z_ _**palety Vizuální styly**. Tím, že pro každý kus nábytku upravíte pouze polohu kamery_ _**scény Miniatura**_ _, zajistíte, že_ _**miniatury obsahu**_ _budou konzistentní pro všechny modely obsahu._

## **Připojení knihovny obsahu**

_Nyní se vraťme k projektu domu Farnsworth House. Naučíme se, jak propojit složku **FormIt** v **datové sadě Farnsworth House**, abychom měli z našeho projektu snadný přístup ke všem jejím souborům – včetně_ **vlastního obsahu FormIt**_, který jsme právě vytvořili._

1 – Po přepnutí zpět na model domu Farnsworth House nebo novém otevření modelu domu: _Pokud jste nedokončili poslední kapitolu, stáhněte a otevřete soubor_ _**1.11 – Import Models with Content Library.axm**_ _z_ _**datové sady Farnsworth House**._

1. Otevřete **paletu Knihovna obsahu** a klikněte na ikonu **Připojit adresář knihovny obsahu**. Zobrazí se okno **Předvolby** s otevřenou kartou **Knihovna obsahu**.
2. Kliknutím na ikonu **+** **přidejte nové umístění knihovny obsahu**. Zobrazí se třetí okno, ve kterém můžete procházet počítač a vybrat požadovanou složku.
3. V _**datové sadě Farnsworth House** přejděte do následujících složek:_ _**Podpůrné soubory &GT; FormIt**. Zde naleznete složky_ obsahující soubory **.axm**, které jsme vytvořili dříve v této kapitole. Dvojitým kliknutím vyberte složku **FormIt**.
4. Klikněte na tlačítko **Vybrat složku** a cesta k této složce se zobrazí na panelu **Umístění knihovny – místní**.
5. V okně **Předvolby** klikněte na tlačítko **OK** a připojená složka bude přidána do **knihovny obsahu**.
6. Chcete-li získat přístup k této nové knihovně, otevřete rozevírací nabídku v horní části **palety Knihovna obsahu** a vyberte možnost **FormIt**.
7. Struktura složek a všechny soubory **.axm** v připojené složce se zobrazí na **paletě Knihovna obsahu**. Dvojitým kliknutím na jakoukoli podsložku získáte přístup k souborům v ní. 

![](../../.gitbook/assets/link-library-content.png)

**Poznámka:** Pokud máte přístup ke službě **Autodesk Docs** \(dříve známé jako Autodesk 360\), můžete prostřednictvím rozevírací nabídky **Knihovna obsahu** přistupovat také k souborům, které jste si uložili v této službě.

## **Umístění obsahu z knihovny**

_‌Nyní umístíme položky obsahu, které jsme vytvořili, do modelu domu Farnsworth House._

1 – Abychom viděli dovnitř domu a mohli umístit nábytek, vypněte hladinu **Střecha** a nástrojem **Orbit \(O\)** otáčejte perspektivní pohled, dokud se nezobrazí celé podlaží hlavní budovy.

2 – Na **paletě Knihovna obsahu** zkontrolujte, zda je rozevírací seznam stále nastaven na možnost **FormIt**. Před umístěním nábytku, který jsme právě vyrobili, musíme umístit „jádro“ domu:

1. Kliknutím na složku s názvem **Další** ji otevřete a poté klikněte na miniaturu **Farnsworth House – jádro**, abyste ji vybrali.
2. Přesuňte ukazatel myši nad **podlaží hlavní budovy** a kliknutím na **těžiště** podlaží umístěte **jádro**.
3. Pro návrat zpět do složky FormIt klikněte na tlačítko **Přejít nahoru**.

![](../../.gitbook/assets/7%20%282%29.jpeg)

3 – Nastavte kameru na možnost **Ortografické \(VO\)**, **Horní pohled \(VT\)** a poté kliknutím na **podlaží hlavní budovy** zobrazte **obrázek půdorysu**. Další informace o nastavení **pohledů** a **hladin** naleznete v předchozích kapitolách.

4 – Vyberte objekt **Farnsworth House – jádro** a přesuňte jej tak, aby byl co nejvíce zarovnán s obrázkem půdorysu.

![](../../.gitbook/assets/8%20%281%29.png)

_**Poznámka:**_ _Při přesouvání_ _**jádra** neměňte jeho výšku. Buď můžete pomocí klávesy_ _**Shift**_ _omezit pohyb vždy podél jedné z os, nebo můžete zajistit, aby počáteční i koncový referenční bod příkazu_ _**Přesunout \(M\)**_ _byly ve stejné výšce, a to kliknutím pouze na_ _**obrázek plánu**, nikoli na samotné_ _**jádro**__. Další informace o nástroji_ _**Přesunout \(M\)**_ _naleznete v předchozích kapitolách.‌_

## **Umístění nábytku z knihovny**

1 – Pomocí podobného postupu nyní můžete umístit nábytek, který jste vytvořili dříve v této kapitole, ze složky **Vlastní obsah FormIt**. Pokud jste nepřevedli všechny tři \(3\) soubory SKP, můžete místo nich použít předpřipravené verze ve složce **Nábytek**.

_**Poznámky:**_

* _Znovu zapněte hladinu_ _**Podlaží hlavní budovy**__, abyste mohli umístit nábytek přímo na povrch_ _**podlaží hlavní budovy**._
* _Při umísťování nového objektu můžete pomocí klávesy_ _**Tab**_ _přepínat mezi rovinami umístění._
* _Při umísťování nového objektu jej před umístěním můžete pomocí_ _**mezerníku**_ _otáčet v 90°°intervalech._

![](../../.gitbook/assets/9%20%283%29.png)

2 – Podobně můžete prozkoumat **ukázky knihovny obsahu** a umístit obsah dodávaný s aplikací FormIt. Všimněte si, že řada objektů má na výběr několik různých velikostí, podobně jako je tomu u typů rodin v aplikaci Revit.

![](../../.gitbook/assets/10%20%286%29.png)

## **Použití nástroje Měřítko**

1 – Pomocí technik, které jste se právě naučili, umístěte jednu instanci komponenty **tree\_pine** ze složky **Datová sada Farnsworth House &gt; FormIt &gt; Výsadba**.

1. Po umístění vyberte skupinu a přejmenujte ji na **Strom**. Kliknutím pravým tlačítkem myši zobrazte **místní nabídku** a vyberte položku **Nejednotná změna měřítka \(NU\)**.
2. Kliknutím na některé z tlačítek nástroje **Nejednotná změna měřítka** změňte velikost a proporce skupiny **Strom** podle potřeby.

![](../../.gitbook/assets/11%20%283%29.png)

![](../../.gitbook/assets/12%20%282%29.png)

_**Poznámka:**_ _Podobně lze pomocí nástroje_ _**Měřítko (SC)**_ _jednotně změnit měřítko celého modelu nebo skupiny._

2 – Tuto skupinu zkopírujte a umístěte kolem domu více stromů, přičemž pomocí **nástrojů Měřítko** vytvořte různé velikosti a proporce.

![](../../.gitbook/assets/13%20%286%29.png)

_**Poznámka:**_ _Přestože jsou všechny stromy instancemi stejné skupiny, mohli jsme je_ _**škálovat**_ _na různé velikosti. Pomocí nástrojů_ _**Měřítko \(SC\)**_ _a_ _**Nejednotná změna měřítka \(NU\)**_ _mimo režim úprav skupin můžete upravit jednotlivé instance stejné skupiny. Pokud bychom upravili některou ze skupin_ _**Strom**_ _a upravili její geometrii nebo materiál, všechny instance skupin by byly stále aktualizovány, ale každá z nich by si zachovala své aktuální přizpůsobené měřítko. Vyzkoušejte to!_

### **Udržujte model v uspořádaný**

_Nezapomeňte přidaný obsah vždy roztřídit do hladin. V tomto příkladu doporučujeme umístit jádro a veškerý nábytek do hladiny_ _**Podlaží hlavní budovy**_ _a stromy do nové hladiny s názvem_ _**Výsadba**._

