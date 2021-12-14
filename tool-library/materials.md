# Materiály

Vylepšete své modely aplikace FormIt pomocí materiálů, které podporují odrazy, lesk a mapy nerovností.

## Panel Materiály

![](<../.gitbook/assets/materials-sample-category (2).png>)

Na panelu materiálů můžete vybírat ze široké škály ukázek materiálů, procházet připojené knihovny materiálů a od verze aplikace FormIt 2021 také přistupovat k obsahu materiálů jiných souborů FormIt (.AXM) a používat je.

### Zdroje knihovny materiálů

V aplikaci FormIt 2021 a novějších verzích obsahuje panel Materiály rozevírací seznam, ve kterém si můžete vybrat z dostupných zdrojů knihovny materiálů: V náčrtu, Ukázky materiálů a [připojené knihovny](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

![](<../.gitbook/assets/materials-directory-picker (1).png>)

#### V náčrtu

Zobrazí materiály uložené v aktuálním náčrtu aplikace FormIt.

#### Ukázky materiálů

Zobrazí seznam dostupných vzorových materiálů. Tyto nabídky jsou uloženy na cloudovém serveru, proto mějte na paměti:

* Při prvním přístupu do kategorií seznamu Ukázky materiálů je nutné připojení k internetu.
* Při prvním přístupu ke kategorii bude daná kategorie stažena a poté uložena do vyrovnávací paměti v počítači, aby budoucí relace nevyžadovaly stažení.
* Tým aplikace FormIt může čas od času aktualizovat nabídku v seznamu Ukázky materiálů. Pokud k tomu dojde, aplikace FormIt automaticky odstraní a znovu stáhne kategorie, abyste měli k dispozici nejnovější verzi.

![](../.gitbook/assets/materials-samples\_original.png)

**Připojené knihovny**

Další adresáře a umístění se zobrazí po [připojení knihoven materiálů](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

### Vytváření, odstraňování a kapátko

![](../.gitbook/assets/materials\_add.PNG)**Vytvořte nový materiál** definováním jeho barvy, textury, mapy nerovností, mapy výřezů, průhlednosti a nastavení odlesku/lesku.

![](<../.gitbook/assets/materials\_delete (1) (1).PNG>) **Odstranit** vybrané materiály.

![](../.gitbook/assets/materials\_eyedropper.PNG)**Kapátko** – Zkopírujte materiál ve scéně a ihned s ním začněte malovat.

* Klikněte na nástroj Kapátko a pak klikněte na plochu pomalovanou požadovaným materiálem.
* Materiál, který se nachází na ploše, se v panelu zvýrazní a aktivuje se nástroj Štětec s načteným materiálem.

### Obnovení, připojení knihoven a čištění nepoužívaných materiálů

\*\*\*\*![](../.gitbook/assets/materials-link.png) **Připojte knihovny materiálů** z místních adresářů. Zobrazí se obsah v adresářích se soubory JPG, PNG nebo AXM (FormIt). Další informace naleznete v části [Připojení knihoven materiálů](https://windows.help.formit.autodesk.com/tool-library/materials#linking-material-libraries).

![](../.gitbook/assets/materials-refresh.png)**Obnovte** aktuální adresář. Tato možnost je povolena pouze při zobrazení místně připojeného adresáře (není k dispozici v seznamu V náčrtu nebo Ukázky materiálu).

![](../.gitbook/assets/materials-purge.png)**Vyčistěte nepoužívané** materiály z aktuálního náčrtu aplikace FormIt.

Nepoužívané materiály se mohou během iterace přirozeně hromadit, ale mohou výrazně zvýšit velikost souboru, pokud používají vysoce kvalitní textury.

Nepoužívané materiály se v seznamu V náčrtu zobrazí s šedě zbarveným názvem.

Kliknutím na nástroj Vyčistit nepoužívané odstraníte všechny nepoužívané materiály. Nejprve se zobrazí výzva, takže pokud si čištění rozmyslíte, můžete akci zrušit. Toto tlačítko je aktivní pouze v seznamu V náčrtu.

### Připojení knihoven materiálů

Aplikace FormIt 2021 a novější nabízí možnost propojit panel Materiály s místními adresáři (knihovnami) obsahujícími materiály včetně složek se soubory JPG, PNG nebo soubory aplikace FormIt:

![](../.gitbook/assets/materials-axms.png)

![Zobrazení jednotlivých materiálů ze souboru FormIt nebo souborů JPG/PNG v adresáři](../.gitbook/assets/materials-axm-content.png)

* **Soubory JPG/PNG** se zobrazí jako materiály, kterými lze malovat přímo v aktuální náčrtu aplikace FormIt.
   * Kliknutím na miniaturu se soubor obrázku za běhu převede na materiál aplikace FormIt a zkopíruje se do aktuálního náčrtu.
   * Aplikace FormIt vás vrátí do adresáře „V náčrtu“, kde uvidíte materiál, který jste právě zkopírovali do náčrtu.
* **Soubory aplikace FormIt (*.axm)** se zobrazí jako složky s ikonou aplikace FormIt.
   * Kliknutím na složky souborů aplikace FormIt zobrazíte všechny materiály aplikace FormIt uložené v daném souboru.
   * Aby bylo možné získat obsah materiálu, musí aplikace FormIt načíst část souboru, takže u větších souborů může zobrazení materiálů na panelu trvat déle.

### Interakce s materiály

**Malujte s materiálem** jedním kliknutím na miniaturu. Aktivuje se nástroj Štětec, který můžete umístit nad geometrii na kreslicí ploše aplikace FormIt a kliknutím na plochy nebo skupiny je vyplnit daným materiálem.

Jakmile se aktivuje nástroj Štětec:

* Můžete jedním kliknutím pomalovat plochy a skupiny.
   * Při malování skupin se materiál promítne do vnořené geometrie a pokryje všechny plochy nebo skupiny vybarvené výchozím materiálem.
* Můžete vybarvit celá tělesa tak, že dvakrát kliknete na některou plochu, čímž vyberete vše, co je k ní připojeno.

Můžete také nejprve vybrat plochy a skupiny a poté jedním kliknutím na miniaturu materiálu pomalovat výběr tímto materiálem.

**Upravte materiál** dvojitým kliknutím na miniaturu, čímž zobrazíte Editor materiálů (viz níže).

**Přejmenujte materiál** dvojitým kliknutím na jeho název.

**Identifikujte materiál** namalovaný na geometrii tak, že jej vyberete a vyhledáte zvýraznění a ikonu označující, které materiály jsou namalovány na vybrané geometrii.

![](../.gitbook/assets/material\_selected.png)

**Výchozí materiál** lze použít k efektivnímu „vyčištěn“ plochy nebo skupiny od jakýchkoli materiálů. Veškerá geometrie, která není vyplněna materiálem, je implicitně omalována výchozím materiálem.

### Správa seznamu

Upravte velikost miniatur nastavením šířky sloupce (klikněte a přetáhněte svislou čáru vpravo od položky „Materiál“).

Konkrétní materiály můžete filtrovat zadáním požadovaného názvu do řádku „Filtr…“.

Názvy materiálů, které se zobrazují šedě, označují materiály, které nejsou v aktuálním náčrtu použity.

## Tvorba a úpravy materiálů

![](<../.gitbook/assets/materials-editor (1).png>)

Při vytváření nebo úpravě materiálu se zobrazí dialog Editor materiálu, ve kterém můžete upravit řadu položek:

* **Barva**
* **Obrázkové mapy**
   * Kliknutím na miniaturu vyberte novou mapu.
   * Kliknutím na ikonu Uložit uložte mapu pro úpravy v jiné aplikaci.
   * Kliknutím na ikonu Odstranit odstraníte mapu z tohoto materiálu.
      * **Textura ze souboru obrázku**
         * JPG nebo PNG
      * **Mapa nerovností ze souboru obrázku**
         * Doporučený formát JPG
         * Ideální pro přidání efektů hloubky k materiálům
         * Pomocí freewaru, jako je například ShaderMap, můžete generovat mapy nerovností s danou texturou.
      * **Mapa výřezů ze souboru obrázku**
         * PNG
         * Ideální pro materiály se selektivní průhledností, jako jsou ploty z drátěného pletiva nebo děrované panely.
* **Název**
* **Horizontální a vertikální měřítko**
   * Pokud je tato možnost povolena, tlačítko Uzamknout poměr stran zajistí, že horizontální a vertikální měřítko bude respektovat poměr stran textury.
   * Roztáhněte materiál nastavením horizontálního měřítka nezávisle na vertikálním měřítku.
   * Horizontální a vertikální měřítko pro plochu můžete přepsat pomocí nástroje Upravit umístění materiálu (viz níže).
* **Průhlednost**, **Odraz** a **Lesk**

## Úprava umístění materiálu

Při malování materiálu na plochu se aplikace FormIt snaží odhadnout nejlepší orientaci:

* Svislé plochy budou orientovány tak, že vrchol textury bude orientován podél osy Z.
* U horizontálních ploch bude textura orientována podélně podél nejdelší strany plochy.

Pomocí nástroje **Upravit umístění materiálu** můžete změnit výchozí umístění materiálu a měřítko materiálu na konkrétních plochách:

* Vyberte plochu nebo plochy pomalované materiálem.
   * Pokud plocha dědí svůj materiál ze své nadřazené skupiny, bude nutné nejprve pomalovat plochu přímo.
* Nástroj Upravit umístění materiálu můžete spustit pomocí klávesové zkratky MP nebo z místní nabídky, která se zobrazí po kliknutí pravým tlačítkem myši:

![](../.gitbook/assets/adjust-material-placement.PNG)

Pomocí ovládacích prvků na obrazovce můžete interaktivně přesouvat a otáčet textury materiálů a měnit jejich měřítko přímo na ploše:

![](../.gitbook/assets/materialplacement.gif)

![](../.gitbook/assets/adjust-material-placement.gif)

Chcete-li zrušit všechny změny umístění materiálu, jednoduše znovu vymalujte plochu původním materiálem z panelu Materiály.

## Převod materiálů do aplikace Revit

Materiály můžete převést do aplikace Revit pomocí [doplňku FormIt](https://formit.autodesk.com/page/formit-revit) pro aplikaci Revit 2018 a novější.
