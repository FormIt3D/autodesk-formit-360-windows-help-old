# 1.9 – Přidání detailů

_FormIt je skvělý objemový nástroj a také skvělý nástroj pro modelování. Do domu Farnsworth House začneme přidávat detaily v podobě dveří a příčlí pro obvodové zasklení. Poté se zaměříme na některé další nástroje a procvičíme si přidávání nové geometrie, hladin, materiálů a správu skupin._

_Pokud jste nedokončili poslední část, stáhněte a otevřete soubor_ _**1.9 – Adding Details.axm**_ _z_ _**datových sad k příručce Základy aplikace FormIt, Část 1**._

## **Vytvoření okenních rámů**

_Kolem skleněné kóje vytvoříme 2" kovový rám a příčle. Všimněte si, že tyto příčle se záměrně překrývají se skleněnou kójí._

1 – Vytvořte novou hladinu s názvem **Skleněné stěny** a přesuňte do ní skupinu **Skleněná stěna**.

2 – Kvůli usnadnění vizualizace vypněte hladinu **Střecha**, abychom viděli celou skleněnou kóji.

3 – Začněte vytvářet první okenní rám:

1. Na západní straně budovy nakreslete pomocí nástroje **Obdélník \(R\)** novou plochu přímo nad vnější skleněnou plochou. Ujistěte se, že jste plochu vytvořili mimo skupinu **Skleněné stěny**.
2. Vyberte nově vytvořenou plochu a přetáhněte ji o **2"** směrem dovnitř. Stisknutím klávesy **Esc** výběr zrušte. Konečný výsledek by měl vypadat jako na obrázku níže.
3. Klikněte na plochu, kterou jste právě vytvořili. Kliknutím pravým tlačítkem myši zobrazte **místní nabídku**, ve které zvolte nástroj **Odsadit plochu \(OF\).**

_**Poznámka:**_ _Pokud máte potíže s výběrem nové plochy, můžete stisknutím_ _**mezerníku**_ _střídavě vybírat různé objekty nebo dočasně vypněte hladinu_ _**Skleněné stěny**_ _._

![](../../.gitbook/assets/0.jpeg)

4 – Nastavte kótu odsazení tak, že přesunete ukazatel myši směrem dovnitř plochy a zadáním hodnoty **2"** vytvořte nový menší obdélník.

![](../../.gitbook/assets/1%20%289%29.png)

5 – Kliknutím vyberte vnitřní obdélník, který jste právě vytvořili. Znovu klikněte a přetáhněte plochu směrem dovnitř budovy, dokud nezmizí. Dalším kliknutím dokončete odstranění středového objemu z geometrie rámu.

![](../../.gitbook/assets/2%20%2821%29.png)

6 – Dvojitým kliknutím vyberte právě vytvořenou geometrii a vytvořte pro ni **skupinu \(G\)**. Pojmenujte tuto skupinu **Rám příčle – VZ**.​

7 – Vytvořte hladinu s názvem **Příčel** a umístěte do ní novou skupinu.

8 – Nastavte materiál rámu:

1. Na **paletě Materiály** duplikujte materiál **Kov – kartáčovaný – zbarvený** tak, že na něj kliknete pravým tlačítkem a vyberete možnost **Duplikovat materiál**.
2. Dvakrát klikněte na náhled nového materiálu, který chcete upravit.
3. Přejmenujte jej na **Kov – kartáčovaný – šedý**.
4. Upravte barvu materiálu kliknutím na dlaždici **Barva** v části **Mapy** a ztmavte šedou barvu tak, že položku **Val:** nastavíte na hodnotu **150**.

![](../../.gitbook/assets/3%20%284%29.png)

9 – Kliknutím na tlačítko **OK** uložte změny do nového materiálu a poté jím pomalujte skupinu **Rám příčle – VZ**. Poté by **paleta Vlastnosti** skupiny měla odpovídat tomu, co je znázorněno na následujícím obrázku:

![](../../.gitbook/assets/4.jpeg)

10 – Vytvořte novou instanci rámu na východní straně pomocí některého z následujících nástrojů: **Rychlé kopírování**, **Pole** nebo **Zrcadlit**.

11 – Opakujte výše uvedené kroky pro severní a jižní stranu skleněné kóje. Novou skupinu pojmenujte **Rám příčle – SJ**. Nezapomeňte plochy pomalovat a umístit do hladiny **Příčel**.

![](../../.gitbook/assets/5%20%2816%29.png)

_**Poznámka:**_ _Rámy příčlí se v rozích navzájem překrývají, což je záměrné. Výše uvedený výsledek zobrazuje výslednou geometrii rámů příčlí s vypnutými hladinami_ _**Skleněná stěna**_ _a_ _**Sloup**_ _._

**Vytvoření příčlí**

1 – V rovině s vnější skleněnou plochou na jižní nebo severní straně budovy nakreslete **obdélník \(R\) o rozměrech 2" x 10’-10"**, který se nachází mezi spodní a horní částí rámu příčle. Nedělejte si starosti s přesnou polohou obdélníku podél rámu, v následujících krocích jej přesuneme na místo.

![](../../.gitbook/assets/6%20%2811%29.png)

2 – Vysuňte obdélník zpět o **2"**, poté z něj vytvořte **skupinu \(G\)** a pojmenujte ji **Příčel – vertikální**. Umístěte skupinu do hladiny **Příčel** a pomalujte ji materiálem **Kov – kartáčovaný – šedý**.

**Umístění příčlí**

_Nyní nastavíme umístění první příčle tak, aby byla vystředěna na_ _**střed**_ _sloupu._

1 – Zobrazte znovu sloupy zapnutím hladiny **Sloup** \(pokud byla vypnutá\). Na **paletě Hladiny** můžete také vypnout hladiny **Dolní terasa** a **Obrázek půdorysu**, aby byly další kroky jednodušší.

2 – Přesunutí příčle do nového umístění:

1. Kliknutím vyberte skupinu vertikálních příčlí, kterou jste právě vytvořili. **Přibližte \(Z\)** pohled a klikněte na **střed** dolní vnější hrany příčle, znázorněnou červeným trojúhelníkem**.**
2. Začněte přesouvat geometrii horizontálně směrem ke sloupu. Stisknutím klávesy **Shift** uzamkněte pohyb v červené ose \(**osa X**\). Všimněte si, že jakmile je pohyb uzamknut, červená osa se zvýrazní.
3. Oddalujte pohled, dokud se nezobrazí základna sloupu. Se stisknutou klávesou **Shift** klikněte na **střed** základny vnější plochy sloupu. Příčel se bude nadále pohybovat pouze podél červené osy (**osa X**\), ale bude zarovnána ke **středu**, na který jste právě kliknuli.

![](../../.gitbook/assets/7%20%281%29.jpeg)

_**Poznámka:**_ _Příčel je nyní přímo za sloupem. Vypněte hladinu_ _**Sloup**_ _nebo_ pomocí nástroje _**Orbit \(O\)**_ _otáčejte pohled, abyste zobrazili příčel._

3 – Stisknutím klávesy **Esc** zrušte výběr nástroje **Přesunout**.

4 – Pomocí nástroje **Pole \(AR\)** nebo **Rychlé kopírování** vytvořte další čtyři \(4\) vertikální příčle podél stejné strany rozmístěné **11’** od sebe. Informace o používání **nástroje Pole** naleznete v předchozích kapitolách.

5 – Pomocí klávesy Tab vyberte všechny skupiny **vertikálních** příčlí a zkopírujte je na opačnou stranu budovy tak, aby **severní** i **jižní** rám měly stejná rozvržení příčlí, jak je znázorněno na následujícím obrázku:

![](../../.gitbook/assets/8%20%286%29.png)

## **Vytvoření dveřních příčlí**

1 – Nástrojem **Orbit \(O\)** otáčejte perspektivní pohled, dokud se nebudete dívat na střed západního rámu příčle.

2 – Podobně jako při vytváření rámů příčlí nakreslete **3’-6"** široký dveřní panel s rámem **2" x 2"**. Vytvořte z něj **skupinu \(G\)** s těmito vlastnostmi: Název skupiny: **Dveře obvodového pláště**; hladina: **Příčel**; materiál: **Kov – kartáčovaný – šedý**.

3 – Zkopírováním této skupiny vytvořte druhý rám dveří a přesuňte oba rámy tak, aby byly vystředěny ve skupině **Rám příčle – VZ**, jak je znázorněno níže.

![](../../.gitbook/assets/9.jpeg)

## **Vytvoření střešní římsy tažením**

_Nyní vytvoříme římsu domu Farnsworth House pomocí jednoho z pokročilých modelovacích nástrojů aplikace FormIt –_ _**Tažení**. Další informace o pokročilém modelování naleznete v kapitole_ **2.2 –** _**Pokročilé nástroje modelování** _v _příručce_ _**Základy aplikace FormIt, Část II**._

_Prvním krokem k vytvoření_ _**tažení**_ _je nakreslení profilu kolmého k „vysunutí“ tažení. K tomu použijeme jako vodítko geometrii střechy._

1 – Zapněte hladinu **Střecha** a přibližte jeden z rohů.

2 – Použijte jako referenci jednu z vertikálních stran střechy a nakreslete dva sousedící obdélníky. První je **6"** vysoký a **4 5/8"** široký a druhý má rozměry **2" x 2"**. Odstraněním čáry, která rozděluje dva obdélníky, vytvořte jednu plochu. Výsledek by měl vypadat, jak je zobrazeno níže.

![](../../.gitbook/assets/10.jpeg)

3 – Vytvořte tažení:

1. Bez vybrané geometrie klikněte na **panelu nástrojů Standard** na tlačítko **Pokročilé nástroje modelování** a vyberte možnost **Tažení \(SW\)**.
2. Spustí se **Průvodce výběrem tažení** a zobrazí se výzva **Vyberte plochu \(nebo hrany\) pro profil tažení**. Vyberte plochu profilu, kterou jste právě vytvořili.
3. Po výběru profilu se zobrazí výzva **Vyberte plochu \(nebo hrany\) pro trajektorii tažení a poté klikněte na tlačítko Dokončit**. Vyberte horní plochu střechy. Aplikace FormIt automaticky použije hranice vybrané plochy jako trajektorii tažení a kolem celé střechy bude vytvořeno tažení.

_**Poznámka:**_ _Pokud máte potíže s výběrem některé z ploch, zobrazte si pomocí nástroje_ _**Orbit \(O\)**_ _plochu trochu lépe a zkuste to znovu. Případně můžete tažení dokončit výběrem všech okrajů střechy místo horní plochy střechy._

![](../../.gitbook/assets/11%20%282%29.png)

4 – Nyní si model uspořádejte: vytvořte skupinu **Střecha – římsa**, přidejte ji do hladiny **Střecha** a přiřaďte k ní materiál **Kov – kartáčovaný – zbarvený**.

![](../../.gitbook/assets/12%20%281%29.png)

5 – Na závěr zapněte hladinu **Sloup**. Jak vidíte, nově vytvořené tažení protíná horní části sloupů. Tento problém vyřešíte tak, že upravíte některou ze skupin **Vysoký sloup** a přetáhnete horní plochu dolů, dokud nebude zarovnána s dolní částí římsy.

![](../../.gitbook/assets/13%20%285%29.png)

