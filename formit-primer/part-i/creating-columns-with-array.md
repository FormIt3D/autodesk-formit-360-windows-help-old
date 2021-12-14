# 1.8 – Vytvoření sloupů nástrojem Pole

_V tomto cvičení načrtneme prvek detailu – sloup nosníku ve tvaru I. Poté pomocí nástroje Pole rychle vytvoříme několik rovnoměrně rozmístěných kopií._

_Pokud jste nedokončili poslední část, stáhněte a otevřete soubor_ _**1.8 – Create Columns with Array.axm**_ _z_ _**datových sad k příručce Základy aplikace FormIt, Část 1**._

## **Načrtnutí profilu sloupu**

1 – Postup usnadnění procesu kreslení:

1. Přejděte do **horního pohledu \(VT\)**.
2. Přepněte režim pohledu na možnost **Ortografické \(VO\)**.
3. Vypněte hladiny **Podlaží** **hlavní budovy** a **Střecha**. Tento krok zabrání přichycení nové geometrie ke stávající geometrii v těchto hladinách.
4. Přibližte si levý horní roh **importovaného obrázku půdorysu**, abyste si mohli podrobně prohlédnout sloup.
5. Vypněte funkci **Přichytit k osnově \(SG\)** \(pokud je zapnutá\). Pomůže vám to při kreslení čar detailu.

![](../../.gitbook/assets/0%20%2813%29.png)

_Při kreslení sloupu nejprve nakreslíme jednu polovinu a poté ji zrcadlově otočíme, abychom rychle vytvořili druhou symetrickou polovinu._

2 – K vytvoření první poloviny I-nosníku použijte nástroj **Čára (L)** a nakreslete následující náčrt se zadanými kótami. Zatím si nedělejte starosti s přesnou polohou sloupu na půdorysném obrázku.

![](../../.gitbook/assets/1%20%2818%29.png)

3 – Zrcadlení tvaru, který jste právě nakreslili, proveďte takto:

1. Dvojitým kliknutím vyberte všechny plochy a hrany nakreslené geometrie.
2. Klikněte pravým tlačítkem a vyberte **nástroj Zrcadlit \(MI\)**.
3. Klikněte na středový oranžový úchyt **pomůcky Zrcadlit** a umístěte jej do levého dolního rohu geometrie.
4. Pomocí šipky dolů na oboustranném tlačítku šipky v pomůcce otočte osu zrcadlení o -90 stupňů \(ve směru hodinových ručiček\).
5. Kliknutím na volné místo nebo stisknutím klávesy **Esc** dokončete proces zrcadlení. Výsledek by měl vypadat jako profil I-nosníku s čarou uprostřed. Dalším stisknutím klávesy **Esc** zrušte výběr.

![](../../.gitbook/assets/2%20%285%29.png)

![](../../.gitbook/assets/3%20%287%29.png)

_**Poznámka:** Při úpravě pomůcky zrcadlení se zobrazí náhled umístění a orientace konečné geometrie jako stínovaný modrý tvar. Tento náhled můžete použít jako referenci k zrcadlení geometrie do požadovaného umístění._

4 – Spojte obě strany do jediné geometrie: odstraňte čáru, která je rozděluje, tak že na ni kliknete a poté stisknete klávesu **Delete**. Nyní jsou tyto dva povrchy spojeny do jednoho povrchu.

5 – Přesuňte geometrii do jejího konečného umístění:

1. Pokud jsou vypnuty, zapněte hladiny **Obrázek půdorysu** a **Střecha**, aby je bylo možné použít jako vodítko.
2. Dvojitým kliknutím na profil sloupu vyberte jeho plochu a všechny jeho čáry. Začněte výběr přesouvat podél zelené osy \(**osa Y**\). Podržte klávesu **Shift** a přesuňte profil tak, aby byl zarovnán se střechou. Poté jej kliknutím umístěte.
3. Podobně jako v předchozím kroku znovu přesuňte geometrii a tentokrát ji uzamkněte k červené ose \(**osa X**\).
4. Kliknutím profil umístěte na horní část I-nosníku nakresleného v hladině **Obrázek půdorysu** \(horizontální poloha nemusí být dokonalá\).

_**Poznámka:**_ _Klávesa_ _**Shift**_ _uzamkne geometrii, aby se pohybovala pouze podél jedné osy, v tomto případě zelené \(**osa Y**\). Tím se zajistí, že se profil sloupu náhodně neposune nahoru a nezarovná se k horní části roviny střechy._

![](../../.gitbook/assets/4%20%289%29.png)

## **Vysunutí a uspořádání sloupu**

1 – Abyste si usnadnili další proces kreslení, přepněte režim pohledu zpět na **Perspektivní \(VP\)** a pomocí nástroje **Orbit \(O\)** umístěte kameru tak, aby zobrazovala profil I-nosníku od severozápadu. Šipka severu v levém dolním rohu vám pomůže s umístěním pohledu.

![](../../.gitbook/assets/5%20%281%29.jpeg)

_**Poznámka:**_ _Informace o tom, jak se pohybovat v náčrtu, získáte v kapitole_ _**Navigace ve scéně**_ _._

2 – Vyberte plochu profilu sloupu a vysuňte ji nahoru do vzdálenosti **17’-8"**.

_**Poznámka:**_ _Pokud se při přesouvání profil sloupu zarovnal ke střeše, vysuňte plochu dolů o_ _**17’-8"**  , nikoli nahoru._

3 – Oddalte pohled a zapněte hladinu **Střecha** \(pokud je vypnutá\). Vrchol sloupu by měl být zarovnán s horní částí střechy.

![](../../.gitbook/assets/6%20%289%29.png)

4 – Aby byl model uspořádaný a přehledný, vyberte znovu geometrii sloupů a proveďte následující kroky:

1. Vytvořte **skupinu \(G\)** a pojmenujte ji **Vysoký sloup**.
2. Vytvořte novou **hladinu** s názvem **Sloup** a přidejte do ní vytvořenou skupinu.
3. Importujte materiál **Kov – kartáčovaný – zbarvený** a pomalujte jím skupinu.

![](../../.gitbook/assets/7%20%284%29.png)

_**Poznámka:**_ _Další informace o_ _**skupinách**,_ _**hladinách** a_ _**materiálech** získáte v předchozích kapitolách._

4 – Stisknutím klávesy **Esc** ukončete nástroj Štětec.

## **Vytvoření pole sloupů**

1 – Přejděte do **horního pohled \(VT\)** a znovu přepněte režim kamery na možnost **Ortografické \(VO\)**.

2 – Vypněte hladinu **Střecha**.

3 – Zahajte proces tvorby pole:

1. Kliknutím vyberte skupinu sloupů. Kliknutím pravým tlačítkem myši zobrazte **místní nabídku** a vyberte položku **Pole \(AR\)**.
2. V dialogu **Vlastnosti pole** použijte následující nastavení:
   * **Délka mezi kopiemi**
   * **Lineární** \(výchozí\)
   * **Seskupit každé těleso a poté vytvořit pole** \(výchozí\)
   * **Počet kopií: 3**
   * Kliknutím na tlačítko **OK** zavřete dialog.

![](../../.gitbook/assets/8%20%283%29.png)

4 – Umístěte nové prvky:

1. Kliknutím na sloup spusťte nástroj **Pole**. Přesuňte kurzor podél červené osy \(**osa X**\).
2. Nastavte kótu na **22'**. Nyní máte **čtyři** sloupy vzdálené od sebe **22'**.
3. Stisknutím klávesy **Esc** zrušte výběr.

![](../../.gitbook/assets/9%20%286%29.png)

5 – Chcete-li vybrat všechny skupiny **Vysoký sloup** najednou, přesuňte ukazatel myši nad jednu z nich a stiskněte klávesu **Tab**. Všimněte si, že byly zvýrazněny ohraničující kvádry všech 4 sloupů. Kliknutím na sloup, nad kterým je umístěn ukazatel myši, nyní vyberete všechny sloupy. Tímto způsobem můžete rychle vybrat všechny instance stejné skupiny najednou.

6 – Pomocí dalšího **pole \(AR\)** vytvořte sloupy na druhé straně budovy. Tentokrát vytvořte jednu kopii podél zelené osy napříč budovou. Nastavte kótu na hodnotu **29'-4 5/8"**

_**Poznámka:**_ _29’ 4 5/8" = 8 5/8" \(hloubka sloupů\) + 28’-8" \(šířka hlavní budovy\)._

7 – Chcete-li vizualizovat celou budovu, přejděte do **3D pohledu \(V3\)** a nastavte možnost **Perspektivní \(VP\)**. Pokud jsou vypnuty, zapněte hladiny **Podlaží hlavní budovy**, **Střecha**, **Dolní terasa** a **Sloup**.

![](../../.gitbook/assets/10%20%287%29.png)

## **Vytvoření sloupů terasy**

_Nyní zkopírujeme sloupy hlavní budovy a vytvoříme podobné, ale kratší, verze pro terasu._

1 – Kvůli usnadnění kreslení doporučujeme vrátit se k nastavení **Ortografické \(OV\)** a **Horní pohled \(VT\)**.

2 – Vytvořte nové sloupy:

1. Podržte klávesu **Ctrl** nebo **Shift** a kliknutím vyberte 3 sloupy, které jsou nejblíže **podlaží dolní terasy**.
2. Kliknutím na kterýkoli ze sloupů začněte přesouvat všechny 3 vybrané sloupy najednou. Chcete-li vytvořit **rychlou kopii**, stiskněte jednou klávesu **Ctrl**. Zobrazí se obrys kopie.
3. Posuňte kopie dolů podél zelené osy \(**osa Y**\) o **23’-4 3/8"**. Stiskněte klávesu **Esc**.
4. Aniž byste zrušili výběr, přesuňte zkopírované sloupy podél červené osy \(**osa X**\) o **22’** a umístěte je do konečné polohy.
5. Se stále vybranými 3 novými sloupy klikněte pravým tlačítkem myši na jeden z kopírovaných sloupů a vyberte možnost **Vytvořit jedinečné \(MU\)**. Tyto sloupy jsou nyní navzájem propojeny, ale jsou jedinečné oproti originálům.

_**Poznámka:**_ _Podržením klávesy_ _**Shift**_ _nebo_ _**Ctrl**_ _můžete vybrat více prvků najednou nebo odebrat prvky z aktuálního výběru._

![](../../.gitbook/assets/11%20%287%29.png)

3 – Upravte novou skupinu sloupů:

1. Dvojitým kliknutím upravte jednu z nových skupin a přejmenujte ji na **Krátký sloup**
2. Upravte výšku nového sloupu tak, aby byl zarovnán s horní částí **podlaží** **dolní terasy** \(3’-2"\). To provedete tak, že vyberete a přetáhnete plochu sloupu dolů podél modré osy \(**osa Z**\) a podržíte klávesu **Shift**. Umístěte ukazatel myši na libovolné místo na horní ploše **podlaží dolní terasy** a výška sloupu se automaticky zarovná k dolní terase. Jakmile je výška nastavena, kliknutím ukončete akci.

![](../../.gitbook/assets/12%20%284%29.png)

_**Poznámka:**_ _Výšku krátkých sloupů můžete zkontrolovat pomocí nástroje_ _**Měřit \(ME\)**_ _. Případně můžete vybrat jednu ze svislých hran sloupu a zobrazit jeho délku na_ _**paletě Vlastnosti**._

4 – Pomocí technik, které jste se právě naučili, vytvořte poslední zbývající sloup zkopírováním nejkratšího sloupu na opačnou stranu **podlaží dolní terasy**.

![](../../.gitbook/assets/13%20%284%29.png)

