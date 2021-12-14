# 1.12 – Vizuální styly

_Modelování koncepčních objemů je jen polovinou toho, co aplikace FormIt nabízí. Druhá polovina je krásná grafika, která usnadňuje komunikaci s klienty nebo členy týmu. V této kapitole se budeme zabývat způsoby nastavení_ _**grafických vizuálních stylů**_ _a vytváření animací._

_Pokud jste nedokončili poslední část, stáhněte a otevřete soubor_ _**1.12 – Visual Styles.axm**_ _z_ _**datových sad k příručce Základy aplikace FormIt, Část 1**._

## **Tvorba animace**

_V následujících krocích se naučíme používat_ _**scény**_ _k vytvoření animace._

1 – Vytvoření první **scény**:

1. Zapněte všechny hladiny kromě **terénu**, **obrázku půdorysu** a **objemů**.
2. Ujistěte se, že je režim kamery nastaven na možnost **Perspektivní \(VP\)**, a umístěte kameru tak, aby se dívala na celý dům mírně shora, podobně jako na obrázku níže.
3. Otevřete **paletu Scény**.
4. Kliknutím na ikonu **+** vytvořte novou scénu z aktuálního pohledu.
5. Přejmenujte ji na **Letecký pohled 1** a ostatní **vlastnosti scény** nastavte způsobem zobrazeným na obrázku níže.

![](../../.gitbook/assets/0%20%2817%29.png)

2 – Vytvoření druhé **scény** a následné animace mezi nimi:

1. Nastavte kameru do nové polohy, abyste se na dům dívali z jiného úhlu. Vytvořte novou **scénu** s názvem **Letecký pohled 2** stejným postupem jako v předchozím kroku.
2. Klikněte na tlačítko **Přehrát**. Po uplynutí **doby pozastavení** nastavené na **2 sekundy** se animace začne pomalu přesouvat mezi dvěma scénami tam a zpět. Přehrávání bude pokračovat, dokud animaci nezastavíte kliknutím na tlačítko **Zastavit**.

![](../../.gitbook/assets/1%20%2812%29.png)

_**Poznámka:**_ _Pomocí nastavení v dolní části okna_ _**Vlastnosti scény** můžete upravit_ _**dobu pozastavení**,_ _**dobu přechodu**_ _a_ _**rychlost kamery**. Zkuste přidat další scény a pohrát si s těmito nastaveními, abyste si animaci přizpůsobili._

## **Přizpůsobení vizuálních stylů**

_Nyní vytvoříme další scénu s několika přizpůsobenými nastaveními **vizuálních stylů**._

1 – Nejprve otevřete **paletu Vizuální styly**. V horní části jsou čtyři \(4\) karty, z nichž každá obsahuje různá vizuální nastavení: **Povrchy**, **Hrany**, **Prostředí** a **Diagnostika modelu**. Další informace o jednotlivých kartách naleznete v kapitole **Vizuální styly** v části **Knihovna nástrojů**.

2 – Přizpůsobte si některá nastavení na kartě **Povrchy**:

1. Zapněte možnost **Stíny \(DS\)**.
2. Zapněte možnost **Okolní stíny \(DA\)**.
3. Zapněte možnost **Monotonní povrchy \(DM\)**. Tím se vytvoří abstraktní černobílý obraz bez jakýchkoli materiálů.

![](../../.gitbook/assets/2%20%2820%29.png)

3 – Přizpůsobte si některá nastavení na kartě **Hrany**:

* 
   1. Zesvětlete **hrany** tím, že pomocí posuvníku nastavíte kontrast přibližně na hodnotu **30%**.
   2. Zapněte možnost **Prodloužit hrany \(DX\).**
   3. Zesvětlete **siluety** tím, že pomocí posuvníku nastavíte kontrast přibližně na hodnotu **30%**.

![](../../.gitbook/assets/3%20%2811%29.png)

4 – Přizpůsobte si některá nastavení na kartě **Prostředí**:

1. Vypněte možnost **Osy**.
2. Pokud je zapnuta, vypněte možnost **Podlaží**.

![](../../.gitbook/assets/4%20%288%29.png)

5 – Vytvořte novou scénu s názvem **Přizpůsobená scéna** a uložte tato nastavení. Nyní můžete přepínat mezi **scénami** tam a zpět a obnovit tak nastavení grafiky.

![](../../.gitbook/assets/5%20%286%29.png)

_**Poznámka:** Pokud u nové scény zrušíte zaškrtnutí vlastnosti_ _**Kamera**_ _, můžete pomocí ní pouze přepnout na vizuální nastavení, které jsme právě vytvořili, bez přesunutí polohy kamery. Vyzkoušejte to tak, že přejdete do jedné z předchozích leteckých scén a dvakrát kliknete na_ _**přizpůsobenou scénu**_ _. Sledujte, co se stane!_

_**Poznámka:**_ _Informace o_ _**diagnostice vizuálních stylů**_ _a pokročilých možnostech použití_ _**scén** získáte v_ _**části II této příručky**._

