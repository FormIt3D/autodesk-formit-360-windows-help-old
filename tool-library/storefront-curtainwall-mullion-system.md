# Systém příčlí výloh/obvodových plášťů

![](../.gitbook/assets/dynamo-storefront-system-options.gif)

## Používá technologii aplikace Dynamo

Možnost rychle vytvořit systémy příčlí výloh/obvodových plášťů v aplikaci FormIt je založena na technologii aplikace Dynamo. Skript Storefront Curtainwall najdete v adresáři Dynamo Samples na panelu Dynamo:

![](../.gitbook/assets/storefront-curtainwall-button%20%281%29.png)

## Výběr „skla“ pro systém příčlí

Počínaje verzí FormIt 2021.2 používá skript Storefront Curtainwall nový uzel [SelectFromFormIt](https://formit.autodesk.com/page/formit-dynamo#dynamo-formit-nodes), který umožňuje vybrat část „skla“ \(jednu plochu nebo vysunuté těleso\), kolem kterého se vytvoří systém příčlí.

![Jednoduchá rovina „skla“ s otvorem pro dveře v dolní části.](../.gitbook/assets/storefron-system-1_glass-only.png)

Když kliknete na miniaturu Storefront Curtainwall \(všimněte si ikony označující, že je vyžadován výběr\), aplikace FormIt zobrazí výzvu k výběru geometrie skla, abyste mohli pokračovat:

![](../.gitbook/assets/storefront-curtainwall-prompt.png)

Několik poznámek a upozornění týkají se výběru skla:

* Aktuálně jsou podporovány pouze rovinné plochy. Pokud vyberete řadu ploch \(například „zakřivenou“ plochu složenou z menších rovinných ploch\), skript najde největší rovinnou plochu a použije ji.
* Pokud je sklo plné, tj. jedna plocha je velmi mírně vysunuta, aby se vyjádřila její tloušťka, skript najde největší plochu, takže výsledné příčle budou vygenerovány na jedné straně skleněného tělesa.
* Můžete nakreslit otvory pro dveře a odstranit výsledný povrch z hranice skla. Výsledné příčle budou respektovat otvor dveří a ponechají otvor prázdný pro přidání dveří.
* Kvůli omezením aplikace Dynamo tento skript nefunguje, pokud má geometrie skla otvory uprostřed.

## Tipy a triky

Při výběru geometrie grafu aplikace Dynamo v aplikaci FormIt vám mohou určité organizační triky zjednodušit práci a umožnit snadné vytváření instancí výsledků:

* Vložte sklo do skupiny a použijte tuto skupinu jako výběr pro skript Storefront/Curtainwall. Tento způsob umožňuje snazší úpravy profilu skla po vygenerování příčlí a pokud je sklo výrazně upraveno mezi jednotlivými spuštěními a ID ploch se změní, skupina zajistí, že skript sklo vždy najde, protože používá ID skupiny, nikoli ID plochy.
* Pokud plánujete kopírovat a vkládat výsledky systému příčlí do jiných míst v modelu, doporučujeme, aby sklo a výsledné příčle byly obsaženy ve skupině. Tím se také předejde problémům s tím, že by uzel výběru nevěděl, kterou instanci skla použít, když je zkopírována a vložena pouze výsledná skupina příčlí.
   * Nejprve vložte sklo do skupiny. Dvojitým kliknutím vyberte sklo a stiskněte klávesu G nebo použijte příkaz Skupina v místní nabídce nebo na panelu nástrojů.
   * Vyberte výslednou skupinu a umístěte ji do jiné skupiny.
   * Dvojitým kliknutím přejděte do první skupiny. Toto je „kontejner“ pro sklo i výsledné příčle.
   * Klikněte na miniaturu Storefront Curtainwall a jako výběr použijte skupinu skla.
   * Po spuštění skriptu můžete skupinu ukončit a podle potřeby kontejner zkopírovat nebo vložit. Můžete bez problémů upravovat libovolnou instanci \(upravit tvar skla nebo parametry\).

## Možnosti systému příčlí

Po výběru skla a spuštění skriptu se na kreslicí ploše aplikace FormIt zobrazí výsledek v podobě skupiny aplikace FormIt. Tato skupina bude automaticky vybrána a na panelu Vlastnosti se zobrazí dostupné možnosti.

![](../.gitbook/assets/storefront-curtainwall-parameters.png)

* **Run**: Na toto tlačítko klikněte, pokud změníte tvar skla a chcete znovu spustit graf, aby se aktualizovaly výsledné příčle.
* **Edit Embedded Graph**: Umožňuje upravit skript aplikace Dynamo, který vytváří geometrii. Tento skript je vložen do souboru aplikace FormIt a je specifický pro tuto skupinu.
* **Select Glass \(Surface or Solid\)**: Kliknutím na toto tlačítko můžete vybrat jiné sklo, kolem kterého chcete vytvořit příčle.

Při prvním spuštění skript použije výchozí hodnoty, takže je vhodné je upravit pro váš jedinečný případ použití. Všechny hodnoty budou používat aktuální jednotky aplikace FormIt.

* **Mullion Width + Depth**: Šířka a hloubka všech prvků příčlí.
* **Vertical Mullion Spacing**: Středová vzdálenost mezi jednotlivými svislými příčlemi.
* **Flip Vertical Mullion Layout**: Skript zahájí rozteč svislých příčlí z jedné libovolně zvolené strany. Pokud pro vaše potřeby ve výsledku začíná rozteč příčlí na nesprávné straně, nastavte tuto možnost na hodnotu True, aby se rozvržení obrátilo a začínalo na opačné straně.
* **Center Vertical mullion Layout**: Místo toho, abyste výpočet rozteče svislých příčlí zahájili na jednom konci skla, zahajte výpočet uprostřed a vytvořte tak symetrické rozvržení svislých příčlí.
* **First Horizontal Mullion Spacing**: Nastaví první rozteč vodorovných příčlí od dolního okraje. Tato možnost je užitečná, pokud potřebujete řadu kratších modulů zasklení v dolní části, odděleně od rozteče zbývajících svislých příčlí.
* **Horizontal Mullion Spacing**: Typická středová rozteč horizontálních příčlí, počínaje první příčlí, jak je uvedeno výše.
* **Flip Horizontal Mullion Layout**: Pokud chcete, aby rozvržení horizontálních příčlí začínalo nahoře místo dole, nastavte tuto možnost na hodnotu True.
* **Center Horizontal Mullion Layout**: Místo zahájení výpočtu rozteče horizontálních příčlí v dolní nebo horní části skla zahajte výpočet uprostřed a vytvořte tak symetrické rozvržení horizontálních příčlí.

## Skryté možnosti

Hledáte další možnosti přizpůsobení? Některé pokročilé možnosti jsou na panelu vlastností aplikace FormIt skryté, ale jsou přístupné po kliknutí na tlačítko Edit Embedded Graph, kterým zobrazíte úplný obsah grafu v aplikaci Dynamo:

![](../.gitbook/assets/dynamo-edit-embedded-graph.png)

### Náhodně rozdělené příčle

![](../.gitbook/assets/storefront-curtainwall-random-verticals.png)

* **Randomize Vertical and Horizontal Mullion Layout**: Tuto možnost nastavte na hodnotu True, pokud chcete pro vertikální nebo horizontální příčle použít náhodnou rozteč.
* **Min/Max Mullion Spacing \(if random\)**: Úpravou těchto hodnot nastavíte rozsah minimálních a maximálních náhodných hodnot rozteče.

### Hraniční příčle

![](../.gitbook/assets/storefront-curtainwall-border-mullion-options.png)

* **Flip Offset Direction of Border Mullions**: Ve výchozím nastavení použije systém příčlí hranici skla a odsadí ji dovnitř, aby se vytvořily hraniční příčle. Chcete-li provést odsazení ven, nastavte tuto možnost na hodnotu True. Tím se zvýší celková velikost systému příčlí vně hranice skla o hodnotu nastavenou pro parametr Mullion Width.
* **Tolerance Between Selection and Border Mullions**: Ve výchozím nastavení se systém příčlí vytvoří přesně na hranici skla, což může způsobit chybu z-fight v místě, kde se střetává hrana skla a vnější povrchy hraničních příčlí. Ve většině případů to nebude viditelné, ale pokud váš případ použití vyžaduje, aby byly hrany systému viditelné, a chcete se vyhnout chybě z-fight, povolte tuto možnost a podle potřeby upravte hodnotu tolerance.

