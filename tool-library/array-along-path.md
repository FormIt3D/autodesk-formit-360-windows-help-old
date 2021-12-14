# Skript Array Along Path

## Používá technologii aplikace Dynamo

V aplikaci FormIt 2021 a novějších verzích můžete uspořádat objekty podél trajektorie a rychle přizpůsobovat výsledky na místě. Skript Array Along Path používá technologii aplikace Dynamo, což znamená, že pole lze snadno konfigurovat tak, abyste dosáhli požadovaných výsledků, a novým spuštěním logiky dojde k aktualizaci geometrie na místě.

![](../.gitbook/assets/array-along-path.gif)

## Spuštění skriptu Array Along Path

* V aplikaci FormIt pro systém Windows přejděte na panel aplikace Dynamo a ujistěte se, že se nacházíte v adresáři Dynamo Samples.
* Klikněte na ukázku Array Along Path.
* Na levé straně obrazovky se zobrazí výzva k výběru objektů pro pole.
   * Pro tento krok můžete vybrat libovolnou kombinaci objektů aplikace FormIt.
   * Jakmile něco vyberete, můžete stisknout šipku „Další“ na levé straně obrazovky nebo stisknout klávesu Enter.
* Nyní se zobrazí výzva k výběru trajektorie pro pole.
   * Zde byste měli vybrat pouze řadu přilehlých hran nebo skupinu obsahující řadu přilehlých hran.
   * Po výběru trajektorie klikněte na tlačítko „Dokončit“ nebo stiskněte klávesu Enter.
* Na panelu Dynamo se zobrazí zpráva o zpracování změn. Po dokončení této operace budete mít ve skupině aplikace FormIt pole vytvořené aplikací Dynamo, které bude připraveno k úpravám \(viz níže\).

## Iterace na místě

Po spuštění skriptu Array Along Path uvidíte, že jeho výsledky jsou nastaveny na výchozí hodnoty, takže je vhodné je upravit tak, aby vyhovovaly vašim potřebám.

Při spuštění skriptu Array Along Path se vytvoří nová skupina obsahující výsledky a aplikace FormIt automaticky vybere skupinu a zobrazí dostupné možnosti pro danou instanci skriptu Array Along Path.

K vlastnostem skriptu Array Along Path se můžete kdykoli vrátit výběrem skupiny a přepnutím na panel vlastností nebo úpravou skupiny, která automaticky zobrazí vlastnosti.

![](../.gitbook/assets/array-along-path-options.png)

### Select Object\(s\) to Array <a id="run"></a>

Kliknutím na toto tlačítko se vrátíte do průvodce výběrem a můžete změnit, které objekty budou přidány do pole.

### Select Array Path

Kliknutím na toto tlačítko se vrátíte do průvodce výběrem a změníte trajektorii, která se použije k výpočtu pole.

### Array Type <a id="run"></a>

Přepíná typ pole, které se má vypočítat: podle vzdálenosti nebo podle počtu.

**Pokud je hodnota True**, bude použit výpočet „By Distance“, takže níže uvedené číslo se vztahuje ke vzdálenosti mezi kopiemi.

**Pokud je hodnota False**, bude použit výpočet „By Number of Copies“, takže číslo pod tímto polem označuje počet kopií, které se mají vejít podél trajektorie.

### Include Original Selection In Results

Hodnota **True**:

* Vybrané objekty budou započítány jako jedna z nových kopií.
* Výsledná skupina aplikace Dynamo zahrne do svých výsledků původní výběr, takže nové kopie mohou s původním výběrem trpět chybou z-fight. Původní výběr můžete umístit do [hladiny](layers.md) a jejím vypnutím jej skrýt.

Hodnota **False**:

* Výsledné pole **nebude** obsahovat původní výběr, takže **kromě** původního výběru získáte také počet kopií, které jste zadali, a výsledky nebudou trpět chybou z-fight.

### Rotate Copies Along Path

Pokud je vybrána hodnota **True**, kopie se otočí, aby byla zachována orientace původního objektu vzhledem k trajektorii.

Pokud je vybrána hodnota **False**, kopie nejsou otočeny, pouze přesunuty.

### Use Relative Positioning Along Path

Hodnota **True**:

* Každá kopie zachová vzdálenost mezi trajektorií a původním objektem.
* Pokud původní objekt **není** umístěn v jednom z koncových bodů trajektorie, použije se pro výpočet pole největší zbývající segment trajektorie.

Hodnota **False**:

* K výpočtu pole se použije celá délka trajektorie bez ohledu na to, kde se původní objekt vzhledem k trajektorii nachází.
* Tím se oddělí umístění trajektorie vzhledem k objektu a jednoduše se použije celá trajektorie. Tato možnost je užitečná, pokud se trajektorie a objekt nenacházejí blízko sebe.

### Reverse Path Direction

Pouze pro uzavřené trajektorie. Při použití skriptu Array Along Path s uzavřenou trajektorií může směr křivky neočekávaně převrátit očekávané výsledky pole. Pokud jsou výsledky převráceny, přepnutím této možnosti na hodnotu **True** obrátíte směr pole.

### Run <a id="run"></a>

Po úpravě možností kliknutím na tlačítko Run spusťte základní graf aplikace Dynamo a vygenerujte nové výsledky. Toto tlačítko se po změně parametrů zbarví modře, abyste věděli, že je třeba na tlačítko kliknout, aby se aktualizace zobrazily ve výsledné geometrii.‌

### Edit Embedded Graph <a id="edit-embedded-graph"></a>

Kliknutím na toto tlačítko spustíte prostředí editoru grafu aplikace Dynamo, ve kterém můžete prohlížet a upravovat základní graf Dynamo a rychle měnit parametry a zobrazovat živé aktualizace nebo kontrolovat či upravovat logiku.



## Výběr geometrie

Při výběru objektů pro skript Array Along Path a další grafy aplikace Dynamo založené na výběru platí následující skutečnosti:

* Můžete vybrat libovolnou kombinaci objektů aplikace FormIt – vrcholy, hrany, plochy, tělesa, skupiny a sítě.
   * V závislosti na prováděném kroku by některé z těchto objektů neměly být vybrány.
   * Například při výběru trajektorie byste měli vybrat řadu přilehlých hran nebo skupinu obsahující řadu přilehlých hran. Cokoli jiného způsobí selhání grafu.
* Dvojitým kliknutím na objekt vyberete vše, co je k němu připojeno.
* Pomocí okna pro výběr oblasti můžete uchopit řadu objektů.
* Můžete vybrat objekty, které již byly vybrány, a zrušit jejich výběr.
* Abyste mohli pokračovat v kroku založeném na výběru, je nutné vybrat alespoň jeden objekt.



