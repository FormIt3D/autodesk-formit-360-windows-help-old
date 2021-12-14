# 3D text

## Používá technologii aplikace Dynamo

V aplikaci FormIt 2021 a novějších verzích lze generovat a upravovat 3D textové objekty, které používají technologii aplikace Dynamo. Aplikace Dynamo umožňuje upravovat písmo, velikost a další vlastnosti textu na místě, aniž by bylo nutné text v případě potřeby znovu generovat a měnit jeho umístění.

![](../.gitbook/assets/3d-text.gif)

## Umístění 3D textu

![](../.gitbook/assets/3d-text-placement.gif)

* V aplikaci FormIt pro systém Windows přejděte na panel aplikace Dynamo a ujistěte se, že se nacházíte v adresáři Dynamo Samples.
* Klikněte na ukázku 3D Text.
* Přesuňte kurzor na kreslicí plochu a na kurzoru se zobrazí 3D text.
   * Před umístěním můžete přesunout ukazatel myši na geometrii a změnit orientaci 3D textu, například na vertikální povrch, aby se text zarovnal na výšku. Mezi orientacemi můžete také přepínat stisknutím klávesy Tab.
* Kliknutím umístěte 3D text, který bude vygenerován uvnitř skupiny aplikace FormIt.
* Po umístění se zobrazí panel vlastností, ve kterém se zobrazí dostupné možnosti pro 3D text.

## Iterace na místě

Výhoda použití aplikace Dynamo ke generování 3D textu spočívá v tom, že lze snadno provádět jeho úpravy, a je zachována aktuální pozice textu, což umožňuje rychlou iteraci.

Volby 3D textu jsou dostupné v panelu vlastností při výběru skupiny 3D textu nebo při úpravách skupiny.

Po počátečním umístění 3D textu se automaticky zobrazí panel vlastností. Můžete také vybrat skupinu a přepnout na vlastnosti sami nebo dvojitým kliknutím na skupinu automaticky přepnout na panel vlastností.

![](../.gitbook/assets/3d-text-options.png)

### Text

Zadejte text, který chcete zobrazit v geometrii 3D textu. V tomto poli se také zobrazí náhled vybraného písma a zarovnání. Stisknutím klávesy Enter/Return můžete zadat více řádků textu.

### Font

Vyberte písmo 3D textu. V tomto seznamu se zobrazí písma dostupná v počítači a výběrem nového písma se aktualizuje obsah v poli Text. 

Všimněte si, že některá písma mají složitější geometrii a jejich generování pomocí aplikace Dynamo může trvat delší dobu.

### Justification

Tímto nastavením se text zarovná vzhledem k počátku místního souřadnicového systému skupiny.

* Možnost Left zajistí, že text bude začínat na počátku skupiny a rozbalí se doprava.
* Možnost Center zajistí, že text bude vždy vystředěn kolem počátku skupiny.
* Možnost Right zajistí, že text bude končit na počátku skupiny.

![](../.gitbook/assets/3d-text-justification-combined.png)

### Text Size

![](../.gitbook/assets/3d-text-text-size.png)

Výška textu v aktuálních jednotkách aplikace FormIt.

### Extrusion Depth

Velikost 3D vysunutí textu v aktuálních jednotkách aplikace FormIt. 3D text je navržen tak, aby tvořil těleso, takže tato hodnota nemůže být nulová, ale můžete ji nastavit velmi blízko 0, aby nebylo tak patrné, že je vysunutý.

### Tracking

![](../.gitbook/assets/3d-text-tracking.png)

Tato možnost umožňuje nastavit výchozí mezery mezi písmeny určitého písma. Použijí se aktuální jednotky aplikace FormIt a hodnota může být kladná nebo záporná. Pokud jsou jednotky například stopy, hodnota 0.25 přidá mezi jednotlivá písmena 3" mezeru. Naopak hodnota -0.25 přiblíží všechna písmena o 3".

### Multi-Line Spacing

![](../.gitbook/assets/3d-text-multi-line.png)

Pokud je v poli Text více řádků, tato hodnota určuje, jak velká mezera bude mezi jednotlivými řádky textu. Použijí se aktuální jednotky aplikace FormIt.

### Invert Text

![](../.gitbook/assets/3d-text-inverted.png)

Pokud je vybrána hodnota True, vytvoří tato možnost kolem textu těleso a odstraní z něj text, čímž vznikne „převrácený“ text – jako by byl text vyříznut v materiálu.

### Inverted Text Border

![](../.gitbook/assets/3d-text-inverted-border.png)

Platí pouze v případě, že je možnost Invert Text nastavena na hodnotu True. Určuje velikost ohraničení okolo textu, které se použije pro těleso, z něhož je text odstraněn. Použijí se aktuální jednotky aplikace FormIt.

### Curve Faceting Quality

Křivky z písem jsou pomocí 3D textu převedeny na úsečkové segmenty, takže tato hodnota určuje, jak jemně jsou křivky složeny z plošek.

Nižší čísla budou mít za následek hrubší plošky \(delší úsečky\) a vyšší čísla budou mít za následek jemnější plošky \(kratší úsečky\). Tato hodnota přepíše nastavení tvorby plošek křivek a ploch v předvolbách aplikace FormIt.

### Run

Po úpravě možností kliknutím na tlačítko Run spusťte základní graf aplikace Dynamo a vygenerujte nové výsledky. Toto tlačítko se po změně parametrů zbarví modře, abyste věděli, že je třeba na tlačítko kliknout, aby se aktualizace zobrazily ve výsledné geometrii.‌

### Edit Embedded Graph

Kliknutím na toto tlačítko spustíte prostředí editoru grafu aplikace Dynamo, ve kterém můžete prohlížet a upravovat základní graf Dynamo a rychle měnit parametry a zobrazovat živé aktualizace nebo kontrolovat či upravovat logiku. Není to nutné, ale může to být užitečné při řešení potíží nebo pro rychlejší úpravy. Viz podrobnosti níže.

## Rychlejší iterace v aplikaci Dynamo

Pokud iterujete možnosti 3D textu, může být rychlejší spustit editor grafu aplikace Dynamo, ve kterém můžete upravovat parametry a zobrazovat změny v reálném čase. Také vám to umožní zkontrolovat logiku grafu v případě, že se vyskytnou problémy.

![](../.gitbook/assets/3d-text-edit-embedded.png)

Editor grafu aplikace Dynamo můžete spustit kliknutím na tlačítko Edit Embedded Graph na panelu vlastností.

![](../.gitbook/assets/3d-text-edit-embedded-windows.png)

## Řešení potíží

3D text využívá na pozadí aplikaci Dynamo, jež používá modelovací jádro ASM ke generování geometrie, která je předávána zpět do aplikace FormIt.

Některá písma mohou vytvářet „křivky, které protínají samy sebe“, nebo jinou problematickou geometrii způsobující chyby v ASM.

Pokud při pokusu o spuštění 3D textu dojde k chybě nebo pokud písmena zmizí, můžete kliknout na tlačítko Edit Embedded Graph, abyste zjistili, co je s grafem špatně a kde může docházet k chybě.

Některá písma mají také známé problémy, které brání jejich převedení do správné geometrie. Příkladem je písmo Bahnschrift. Pokud narazíte na jiné problematické písmo, [dejte nám vědět na fórech](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=en). Uděláme, co bude v našich silách, abychom problémy s konkrétními písmy vyřešili.





