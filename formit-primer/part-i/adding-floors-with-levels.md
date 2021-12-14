# 1.4 – Přidání podlaží

_Podlaží umožňují „odříznout“ objemy pomocí jednotlivých základen podlaží a vypočítat hrubou plochu na objem budovy. Při převodu souboru do aplikace Revit budou podlaží aplikace FormIt a jejich uživatelské názvy převedeny na úrovně aplikace Revit._

_Pokud jste nedokončili poslední část, stáhněte a otevřete soubor **1.4 – Add Floors with Levels.axm** z **datových sad k příručce Základy aplikace FormIt, Část 1**._

## **Vytváření a přizpůsobení podlaží**

1 – Vytvoření podlaží:

1. Na **panelu palet** přejděte na **paletu Podlaží**.
2. Čtyřikrát klikněte na tlačítko **+** \(**Přidat podlaží**\), čímž vytvoříte čtyři podlaží.
3. Dvakrát klikněte na aktuální výšku jednotlivých podlaží a zadejte následující hodnoty: **0’-0", 2'-2", 4’-6"** a **17’-8"**.
4. Dvakrát klikněte na aktuální název jednotlivých podlaží a přejmenujte je na: **Přízemí, Terasa, Hlavní budova** a **Vrchol střechy**

![](../../.gitbook/assets/0%20%2816%29.png)

_**Poznámka**: Kliknutím na ikonu_ _**++**_ _můžete vytvořit více podlaží se zadanou a jednotnou vzdáleností od sebe. To je užitečné u vícepodlažních budov_.

## **Použít podlaží na geometrii**

_V předchozích krocích jsme pouze vytvořili podlaží. Nyní jsme připraveni použít tato podlaží na geometrii, kterou jsme vytvořili._

1 – Použití podlaží na existující geometrii:

1. Dvojitým kliknutím vyberte celý objem horní terasy.
2. Na **paletě Vlastnosti** zaškrtněte políčko **Použít podlaží**. Tímto krokem vyberete všechna podlaží, která aktuálně protínají vybranou geometrii.
3. Nyní jsou u aktuálně vybrané geometrie použita tři podlaží \(**Hlavní budova, Terasa** a **Přízemí**\), ale v tomto cvičení chceme použít pouze možnost **Přízemí**. Zrušte zaškrtnutí políček **Hlavní budova** a **Terasa**.
4. Tento postup zajišťuje, že při výpočtu hrubé plochy se bere v úvahu pouze plocha, kterou protíná **Přízemí**. Tato plocha je zobrazena v poli **Plocha podle podlaží**.

![](../../.gitbook/assets/1%20%284%29.png)

_**Poznámka**: Pokud na objemu nejsou zobrazeny modré čáry podlaží, zadejte_ _**DL**_ _, čímž aktivujete příkaz_ _**Zobrazit podlaží**._

![](../../.gitbook/assets/2%20%283%29.png)

