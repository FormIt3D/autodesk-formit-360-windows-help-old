# Pokročilé modelování

V našich cvičeních s domem Farnsworth House jsme se zaměřili na základní nástroje modelování, jako jsou náčrty, přetažení plochy, posun, pole a odsazení plochy. Také jsme se zabývali základními pracovními postupy zahrnujícími skupiny, hladiny, materiály a úrovně. V této části vám představíme pokročilé nástroje modelování **Tažení** a **Zaoblení**.

Pokud jste nedokončili poslední část, stáhněte a otevřete soubor **farnsworth05.axm** ze složky [FormIt Primer](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).

## Tažení

Pomocí nástroje Tažení vytvořte římsu podél střechy.

1. Nástrojem **Obdélník \(R\)** vytvořte v libovolném rohu střechy profil **6" x 4 5/8"**.

   ![](../../.gitbook/assets/a7297208-cefe-42e7-95ca-1e8ea122ac38.png)

2. Vytvořte další **obdélníkový \(R\)** profil **2" x 2"**

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54.png)

3. **Kliknutím** vyberte čáru mezi profily. Stisknutím klávesy **Delete** odstraňte čáru, čímž vytvoříte jeden obrys.

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_2.png)

4. V [**nabídce Pokročilé modelování**](../../formit-introduction/tool-bars.md) vyberte [**nástroj Tažení \(SW\)**](../../tool-library/cover-sweep-loft.md)**.**

   ![](../../.gitbook/assets/8a17017b-b824-48ac-ba24-064a24e7a6ad.png)

5. V levém horním rohu kreslicí plochy se zobrazí panel nástrojů **Pokročilá geometrie** s pomocnými pokyny.

   ![](../../.gitbook/assets/e8badff2-acd9-4393-af5f-adae2424ad47.png)

6. **Kliknutím** vyberte plochu, kterou jste právě nakreslili. Bude to **profil**, který chcete táhnout.

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_3.png)

7. Panel nástrojů **Pokročilá geometrie** se po výběru plochy změní. Zobrazí se výzva k výběru **trajektorie** pro tažení.

   ![](../../.gitbook/assets/df9fc338-15c0-4953-9ec1-c977117efc4d.png)

8. **Kliknutím** vyberte **horní plochu střechy**. Nástroj odvodí hrany plochy jako trajektorii. Po výběru střechy se vytvoří tažení. 

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_4.png)

9. Dvojitým kliknutím vyberete celý prvek římsy. **Seskupte \(G\)** římsu. Upravte skupinu a nazvěte ji **Římsa.**

   ![](../../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_5.png)

10. Pomalujte skupinu římsy materiálem **Concrete &gt; White**, aby odpovídala střeše. Přidejte **skupinu římsy** do hladiny **střechy**.

Je třeba upravit **výšku sloupů**, aby končily v římse. Upravte jednu ze skupin vysokých sloupů, vyberte horní plochu a snižte ji na správnou výšku. Také může být nutné upravit umístění sloupů tak, aby byly zarovnány s deskami. Nyní je vhodná doba k provedení těchto menších úprav.

## Zaoblení

Nyní se naučíte nástrojem Zaoblení vytvářet zaoblenou hranu, který zjemní vzhled nábytku.

1. **Vypněte** hladinu **střechy**, abyste viděli dovnitř domu.
2. V severovýchodním rohu domu vytvořte **obdélník \(R\)** o rozměrech **4' x 7'**. Vyberte plochu a vysuňte ji do výšky **1'-6"**

   ![](../../.gitbook/assets/upperterracesketch_20.png)

3. V části **Pokročilé nástroje modelování** na [**panelu nástrojů Akce**](../../formit-introduction/tool-bars.md) vyberte [**nástroj Zaoblení \(FI\)**](../../tool-library/cover-sweep-loft.md)**.**

   ![](../../.gitbook/assets/f7e388e3-4ad0-4fef-a701-0d3176adc2c5.png)

4. V zobrazeném dialogu změňte výchozí hodnotu **zaoblení** na 1".
5. **Klikněte** na horní plochu postele. Po výběru plochy se automaticky vytvoří zaoblení.

   ![](../../.gitbook/assets/upperterracesketch_21.png)

## Strom skupin

Místo úpravy skupiny kvůli jejímu pojmenování a kategorizaci použijte strom **skupin**, který umožňuje rychle provádět více úloh správy modelu.

1. **Dvojitým kliknutím** vyberte celou postel. Přidejte postel do **skupiny \(G\)**
2. V pravé části palety klikněte na ikonu **Strom skupin**.

   ![](../../.gitbook/assets/groupstree.png)

3. Pokud vyberete na kreslicí ploše skupinu postele, zvýrazní se v seznamu **Strom skupin** \(platí to i naopak, pokud vyberete skupinu v seznamu, zvýrazní se na kreslicí ploše\).
4. Můžete **dvakrát kliknout** na název v seznamu a změnit jej na **Postel**. Aktualizují se všechny instance skupiny, v našem případě existuje pouze jedna.
5. S vybranou **skupinou Postel** v seznamu můžete v rozevíracím seznamu v horní části palety Strom skupin nastavit kategorii **Nábytek**.

   ![](../../.gitbook/assets/groupstree_palette.png)

## Sloučení hran, vyhlazení hran a filtrování výběru

Nyní na nábytku skryjeme nežádoucí hrany, abychom mu dodali hladší a jemnější vzhled.

1. **Dvojitým kliknutím** upravte skupinu. **Dvojitým kliknutím** vyberte celou postel. **Klikněte pravým tlačítkem** a v místní nabídce vyberte **Sloučit \(MG\)**.

   ![](../../.gitbook/assets/upperterracesketch_215.png)

2. Pomocí **filtru výběru** omezte výběr okna pouze na **hrany.**

   ![](../../.gitbook/assets/25b2428d-bc93-4ae4-9b8a-d8f3749ddb43.png)

3. **Přetažením myši** z levého horního do pravého dolního rohu proveďte **výběr okna**. Pomocí okna vyberte oblouk a hranu v každém rohu postele. Podržením klávesy **Ctrl** nebo **Shift** je přidáte do sady výběru.
4. **Klikněte pravým tlačítkem myši** a vyberte položku **Vyhladit hrany \(SE\)**.

   ![](../../.gitbook/assets/upperterracesketch_216.png)

5. Chcete-li tyto hrany znovu zviditelnit, vyberte **kliknutím** horní plochu postele, poté **klikněte pravým tlačítkem myši** a vyberte položku **Oploškovat hladké plochy** \(UE\).

   ![](../../.gitbook/assets/upperterracesketch_217.png)

6. Změňte **filtr výběru** zpět tak, aby opět zahrnoval plochy a skupiny. Znovu zapněte hladinu **střechy**. Váš model domu Farnsworth House pěkně pokročil!

   ![](../../.gitbook/assets/upperterracesketch_22.png)

