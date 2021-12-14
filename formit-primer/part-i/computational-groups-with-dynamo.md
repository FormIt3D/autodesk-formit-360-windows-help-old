# 1.10 – Výpočetní skupiny v aplikaci Dynamo

_V této kapitole využijeme výpočetní výkon aplikace_ [_**Dynamo**_](http://dynamobim.org/) _k umístění a úpravám flexibilních skupin, které jsou vázány na ukázky grafů aplikace Dynamo._

_Pokud jste nedokončili poslední část, stáhněte a otevřete soubor_ _**1.10 – Computational Groups with Dynamo.axm**_ _z_ _**datových sad k příručce Základy aplikace FormIt, Část 1**._

_Další informace o tom, jak aplikace FormIt a Dynamo spolupracují při pracovních postupech výpočetních návrhů_ [_**naleznete zde**_](http://formit.autodesk.com/page/formit-dynamo)_._

## **Vytvoření schodiště dolní terasy**

1 – Ujistěte se, že jsou zapnuty hladiny **Dolní terasa, Podlaží hlavní budovy** a **Obrázek půdorysu**, protože to je místo, kam se chystáte přidat schodiště.

2 – Umístění skupiny schodiště vázané na jednu z ukázek ze složky Dynamo Samples:

1. Na panelu palet otevřete **paletu Dynamo**. V adresáři **Dynamo Samples** byste měli vidět několik předpřipravených objektů aplikace Dynamo.
2. Kliknutím na ukázku aplikace Dynamo **Stairs** ji přeneste do modelového prostoru. Aplikace FormIt spustí graf na pozadí a vygeneruje z něj geometrii schodiště.
3. Přesuňte kurzor nad kreslicí plochu a po načtení schodiště se nyní vedle kurzoru bude pohybovat stínovaný náhled geometrie schodiště. Přesuňte kurzor nad kreslicí plochu poblíž terasy a kliknutím schodiště umístěte. Stisknutím klávesy **Esc** zrušte výběr. Všimněte si, že po umístění schodiště se automaticky otevře **paleta vlastností**.

![](../../.gitbook/assets/0%20%2815%29.png)

_**Poznámka:**_ [_**Můžete také připojit místní adresáře**_](https://formit.autodesk.com/page/formit-dynamo#dynamo-getting-started) _obsahující grafy Dynamo a spouštět vlastní místní grafy Dynamo stejně jako tyto ukázky._

3 – Aktualizace kót schodiště:

1. Vyberte skupinu schodiště a upravte vstupy dostupné v části **INPUTS** aplikace Dynamo v dolní části **palety vlastností** tak, jak je uvedeno níže. Většina skupin vytvořených pomocí skriptů aplikace Dynamo bude mít ve svých vlastnostech po výběru zahrnutou část Dynamo.
   * Add Top Landing = False
   * Add Middle Landing = False
   * Add Bottom Landing = False
   * Floor-to-Floor Height = 2.6
   * Stair Width = 12
   * Riser Height = 0.6
   * Tread Length = 1.25
   * Tread Overlap = 0.25
   * Tread Thickness = 0.25
   * Height Between Middle Landings = \(není relevantní, protože se nevytváří žádná střední podesta\)
   * Middle Landing Length = \(není relevantní, protože se nevytváří žádná střední podesta\)
   * Top/Bottom Landing Length = \(není relevantní, protože se nevytváří žádná střední podesta\)
2. Kliknutím na tlačítko **Run** znovu spusťte skript aplikace Dynamo s aktualizovanými vstupními hodnotami.
3. Podle potřeby přesuňte skupinu tak, aby se schodiště nacházelo na správném místě podle **obrázku půdorysu**. Dbejte na to, abyste při přesouvání skupiny schodiště vůbec neměnili její výšku. Další tipy a informace o technikách při přesouvání prvků modelu najdete v předchozích kapitolách.

![](../../.gitbook/assets/1%20%2811%29.png)

_**Poznámka:**_ _Vstup_ _**Floor-to-Floor Height**_ _je přibližná hodnota celkové výšky schodiště. Skutečnou výšku schodiště definuje parametr_ _**Riser Height**_ _. V tomto příkladu nastavíme parametr_ _**Floor-to-Floor Height**_ _na hodnotu 2.6’, ale konečná výška schodiště je 3.0’ \(0.6’ \(parametr **Riser Height**\) x 5 \(počet podstupnic\)\). Protože rozpětí mezi zemí a horní stranou terasy činí 3’-2", jsou zbývající 2" obsaženy v horní podstupnici._

## **Vytvoření schodiště hlavní budovy**

_V předchozích krocích jsme vytvořili schodiště bez podest. Nyní vytvoříme schodiště s horní podestou, která se zarovná s_ _**podlažím hlavní budovy**._

1 – Začněte vytvořením kopie schodiště, které jsme právě vytvořili:

1. Vyberte existující schodiště a poté kliknutím kamkoli na **obrázek půdorysu** spusťte příkaz k přesunu. To způsobí, že aplikace FormIt použije výšku **obrázku půdorysu** jako počáteční referenční výšku k umístění nové kopie. Stisknutím klávesy **Ctrl** vytvořte **rychlou kopii**.
2. Přesuňte kurzor blíže k hlavní budově nad terasou. Všimněte si, že nyní je horní plocha terasy novou referenční rovinou. Kliknutím skupinu umístěte.

![](../../.gitbook/assets/2%20%289%29.png)

_**Poznámka:**_ _Protože se_ _**obrázek půdorysu**_ _nachází v rovině_ _**Úroveň terénu**_ _,použije nástroj_ _**Přesunout**_ _tuto rovinu jako referenci pro svůj počáteční bod. V obrázku výše si všimněte popisku_ _**Na ploše**_ _, který označuje, že plocha obrázku půdorysu je vybrána jako počáteční reference a horní plocha_ _**podlaží dolní terasy**_ _je vybrána jako koncová reference._

2 – Použijte nástroj **Vytvořit jedinečné \(MU\)**, abyste zajistili, že když změníte vstupy aplikace Dynamo tohoto schodiště, nebude to mít vliv na dolní schodiště. Podle potřeby skupinu přemístěte tak, aby se blížila svému konečnému umístění – později to doladíme. Viditelnost hladiny **Dolní terasa** můžete přepnout, aby se lépe zobrazil půdorys, který vám pomůže s umístěním, ale opět dávejte pozor, abyste při přesouvání nezměnili výšku nového schodiště.

3 – Na **paletě vlastností** aktualizujte **vstupy aplikace Dynamo**, jak je znázorněno níže, a spusťte skript znovu.

* Add Top Landing = True
* Floor-to-Floor Height = 2.333
* Riser Height = 0.466
* Tread Length = 1.5
* Top/Bottom Landing Length = 2.5

![](../../.gitbook/assets/3%20%281%29.jpeg)

_**Poznámka:**_ _Pokud nastavíte parametr_ _**Add Bottom Landing**_ _na hodnotu_ _**True**_ _a znovu spustíte skript, horní plocha dolní podesty by se měla zarovnat s horní plochou_ _**podlaží dolní terasy**. Děje se tak proto, že (na rozdíl od předchozího schodiště) jsme upravili parametr_ _**Riser Height**_ _tak, aby parametr_ _**Floor-to-Floor Height**_ _odpovídal skutečné požadované výšce \(2’-4” neboli 2.333’\)._

2 – Znovu přemístěte skupinu do konečné polohy. Horní podesta by měla být zarovnána s **podlažím hlavní budovy**.

3 – Chcete-li schodiště dokončit, přidejte k němu materiál **Stone – Travertine**, aby se shodoval s materiálem podlaží. Další informace o použití materiálů naleznete v předchozích kapitolách.

