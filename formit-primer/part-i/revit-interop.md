# 1.15 – Práce s aplikací Revit

_Jednou z nejzajímavějších funkcí aplikace FormIt je možnost přesunout model z flexibilního prostředí modelování, jako je aplikace FormIt, do výkonného parametrického prostředí, jako je aplikace Revit. V této kapitole projdeme několik cvičení, ve kterých přesuneme různé prvky z aplikace FormIt do aplikace Revit a z aplikace Revit do aplikace FormIt._

_V této kapitole budeme používat vzorové rodiny aplikace Revit. Pokud jste to ještě neudělali, můžete si je stáhnout z **datové sady domu Farnsworth House.**Pokud jste až do tohoto bodu neabsolvovali celý výukový program, můžete si také stáhnout a otevřít soubor **1.15 – Working With Revit.axm** z **datových sad k příručce Základy aplikace FormIt, Část 1**._

_V těchto cvičeních budeme používat aplikaci Revit 2022, která má vylepšené možnosti interoperability s aplikací FormIt. Předchozí verze aplikace Revit neobsahují některé nebo žádné funkce zobrazené v tomto výukovém programu a mají jiné uživatelské rozhraní._

## Z aplikace Revit do aplikace FormIt

### Převod rodin aplikace Revit pro použití v aplikaci FormIt

Pokud máte hodně souborů rodin aplikace Revit, které chcete použít v aplikaci FormIt, prostudujte si tuto část, která pojednává o tom, jak dávkově exportovat soubory RFA do aplikace FormIt.

_**Poznámka:**_ _Následující kroky zahrnují rozhraní a postupy prováděné v aplikaci Revit 2022, ale nástroje doplňku_ _**Převést soubor RFA do formátu FormIt**_ _jsou k dispozici od verze aplikace Revit 2016._

1 – Otevřete nový projekt nebo rodinu aplikace Revit. Poté postupujte následovně:

1. Na pásu karet **Doplňky** vyhledejte panel **FormIt Converter** a klikněte na tlačítko **Převést soubor RFA do formátu FormIt**. Zobrazí se dialog **Převést rodiny aplikace Revit**.
2. V poli **Cesta k souboru rodiny aplikace Revit** přejděte do umístění, kam jste uložili následující složku v počítači: **Farnsworth House Data Set &gt; Supporting Files &gt; Revit**.
3. V poli **Cesta k obsahu aplikace FormIt** přejděte do složky **Farnsworth House Data Set &gt; Supporting Files &gt; FormIt &gt; Vlastní obsah FormIt**. Pokud jste nedokončili kapitolu **1.11 – Import modelů pomocí knihovny obsahu**, budete si možná muset vytvořit složku **Vlastní obsah FormIt** nebo vybrat jiný cíl.
4. Zahajte proces převodu kliknutím na tlačítko **OK**.

![](../../.gitbook/assets/0%20%2823%29.png)

_**Poznámky:**_

* _Tento proces bude chvíli trvat, protože aplikace Revit otevře soubor_ _**RFA**_ _zadaný v první cestě, poté jej převede a uloží ve formátu_ _**AXMF**_ _pro aplikaci FormIt._
* _V tomto cvičení převádíme pouze jeden soubor, ale tento postup můžete použít k dávkovému převodu všech souborů_ _**RFA**_ _ve vybrané složce \(včetně všech souborů_ _**RFA**_ _ve vnořených složkách\)._

2 – Po dokončení procesu přejděte zpět do aplikace FormIt. Zde se nový obsah zobrazí na paletě **Knihovna obsahu** ve složce **FormIt &gt;** **Vlastní obsah FormIt**, kterou jsme připojili v předchozích krocích. Pokud jste převedené soubory **AXMF** uložili do jiného umístění nebo jste nedokončili kapitolu **1.11 – Import modelů pomocí knihovny obsahu**, bude pravděpodobně nutné tuto složku přidat do knihovny obsahu, aby se zobrazil její obsah. Pokyny k přidávání složek do knihovny obsahu naleznete v kapitole 1.11.

![](../../.gitbook/assets/1%20%2824%29.png)‌

**Poznámka**: _Export některých kategorií z aplikace Revit není podporován. Rodiny „volně stojící“ nebo „založené na podlaží“ jsou podporovány, ale rodiny „založené na hostiteli“, jako jsou dveře a okna, nikoli. Podporovány jsou kategorie Objem, Truhlářské výrobky, Stafáž, Nábytek, Nábytkový systém, Obecný model, Parkoviště, Pozemek a Speciální vybavení. Všechny nepodporované rodiny ve vybrané složce budou jednoduše přeskočeny._

## Z aplikace FormIt do aplikace Revit

_Existují dva různé způsoby přenesení geometrie z aplikace FormIt do aplikace Revit. Existující soubor__ **.axm** můžete importovat do projektu aplikace Revit nebo souboru rodiny aplikace Revit, který se bude chovat podobně jako importovaný model nebo soubor CAD. Případně můžete aplikaci FormIt spustit z aplikace Revit a přenést každou skupinu aplikace FormIt do aplikace Revit jako samostatný prvek obecného modelu. Druhá metoda je popsána v **části II** v kapitole_ _**2.8**_ – _**Pokročilé pracovní postupy aplikace Revit**._

### Import domu Farnsworth House do aplikace Revit

1 – Chcete-li do aplikace Revit importovat soubor aplikace FormIt \(**.axm**\), vytvořte nový projekt aplikace Revit a otevřete výchozí 3D pohled. Poté postupujte následovně:

1. Přejděte na kartu **Vložit** a klikněte na tlačítko **Importovat CAD**. Otevře se okno **Importovat formáty CAD**.
2. Ujistěte se, že v rozevíracím seznamu **Soubory typu** je vybrána možnost **Soubory aplikace FormIt \(\*.axm\)**.
3. Vyhledejte a vyberte soubor **.axm** domu Farnsworth House, se kterým pracujete. Pokud jste nepostupovali podle části I této příručky, můžete také otevřít soubor **1.15 – Working With Revit.axm** ve složce **Farnsworth House Data Set &gt; Chapter Files**.
4. Ujistěte se, že je zaškrtnuta možnost **Importovat podlaží aplikace FormIt**.
5. Po zadání nastavení klikněte na tlačítko **Otevřít** a geometrie aplikace FormIt se přenese do aplikace Revit jako jeden prvek.

![](../../.gitbook/assets/2%20%2824%29.png)

Import souboru aplikace FormIt pomocí tlačítka Importovat CAD.

![](../../.gitbook/assets/3%20%2821%29.png)  
Importovaný prvek .axm. Všimněte si, že podlaží z modelu aplikace FormIt jsou také importována do aplikace Revit.

_Podobně jako u jiných formátů CAD jsou hladiny v původním souboru importovány do aplikace Revit. Tato funkce umožňuje definovat různá nastavení viditelnosti pro každou hladinu a snadno tak upravovat grafický vzhled souboru FormIt v libovolném pohledu aplikace Revit._

2 – Úprava viditelnosti hladin importovaného souboru .axm:

1. Přejděte do okna **Přepsání viditelnosti/zobrazení \(VG nebo VV\)**, poté na kartu **Importované kategorie**, rozbalte importovaný soubor aplikace FormIt a zrušte zaškrtnutí hladiny **Výsadba**, čímž vypnete tuto hladinu v aktuálním pohledu. Poté klikněte na tlačítko **OK**.
2. Změňte **vizuální styl** na **Realistický** a uvidíte, že všechny materiály aplikace FormIt byly importovány do aplikace Revit.

![](../../.gitbook/assets/4%20%2820%29.png)

3 – Importované materiály aplikace FormIt budou nyní k dispozici v tomto projektu aplikace Revit s přiřazenou třídou **FormIt**. Stačí otevřít **Prohlížeč materiálů** a vyhledat „FormIt“ a uvidíte je všechny. Nyní je můžete použít ve svém projektu Revit stejně jako jakýkoli jiný materiál.

![](../../.gitbook/assets/5%20%2819%29.png)

