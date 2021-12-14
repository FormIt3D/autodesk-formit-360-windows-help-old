# Analýza slunečního záření a energetická analýza

Vytvořený model můžeme využít k vytvoření studie **slunečního záření a energetické analýzy** pro náš návrh. Tyto funkce jsou součástí aplikace FormIt, takže můžete zkoumat i ty nejranější studie návrhu z hlediska výkonnosti budovy. Tyto funkce jsou k dispozici pouze v aplikaci **FormIt Pro**, takže pokud používáte webovou verzi aplikace, pravděpodobně k nim nebudete mít přístup.

Pokud jste nedokončili poslední část, klikněte na Soubor &gt; Otevřít a vyberte soubor **farnsworth08.axm** ze složky FormIt Primer.

## Stíny

Před použitím libovolného nástroje analýzy je nutné [nastavit umístění](). To aplikaci FormIt umožní přístup k přesným údajům o slunci, stínech a klimatu.

1. Na [**panelu nástrojů Akce**](../../formit-introduction/tool-bars.md) klikněte na ikonu slunce a zaškrtněte políčko **Stíny \(DS\)**.

   ![](../../.gitbook/assets/3bdf0e2a-0ad4-4aac-b6fc-5e789643b0d6.png)

2. Nastavte posuvníky **Den** a **Čas**, abyste viděli, jak se mění stíny.

   ![](../../.gitbook/assets/upperterracesketch_32.png)

3. Všimněte si, že krytá terasa je v nejteplejších hodinách letních měsíců zastíněná – to určitě není náhoda, ale záměr.

**Poznámka**: Stíny mohou způsobit snížení výkonu aplikace. Dva návrhy na zmírnění tohoto problému: vypněte stíny, pokud zaznamenáte snížení výkonu, nebo vypněte hladiny jako **nábytek**, pokud nejsou ke studiu stínů nezbytné. 

## Analýza slunečního záření

Designéři dokáží pracovat s vizuálními informacemi, díky čemuž mohou získat a využívat neuvěřitelné množství informací z diagramů tepelných map, jako je ten, který se chystáme vytvořit.

1. V dolní části [**nabídky Slunce**](../../formit-introduction/tool-bars.md) klikněte na tlačítko **Analýza slunečního záření**. 
2. Přejdete do speciálního režimu, ve kterém jsou vypnuty **stíny**, **klávesové zkratky** a další **panely nástrojů**.
3. Chování výběru je v režimu **analýzy slunečního záření** upraveno. Můžete vybírat **ve skupinách**, nemusíte držet klávesu **Ctrl** nebo **Shift** pro přidání do sady výběru a můžete zrušit výběr položek tak, že na ně znovu kliknete. Výběr geometrie můžete provádět **kliknutím**, **dvojitým kliknutím** nebo pomocí **okna výběru**.
4. Vyberte plochy, které chcete studovat. **Klikněte** na horní část **střechy** a horní část **podlaží**. Nevybírejte malé prvky, například nábytek.

   ![](../../.gitbook/assets/upperterracesketch_33.png)

5. V levém horním rohu kreslicí plochy vyhledejte panel nástrojů **Analýza slunečního záření**. Klikněte na tlačítko **Analyzovat**. Aplikace FormIt vypočítá a vyrenderuje povrchy. Zde uvedená nastavení lze upravit před **a** po dokončení analýzy.

   ![](../../.gitbook/assets/solaranalysis.png)

6. Nastavení **Měsíční špička** zobrazuje **špičkové** hodnoty \(v BTU/čtv. stopu\) pro zadaný měsíc. Tato možnost je určena pro **studie stínování**. Nastavení měsíce lze změnit a grafika se okamžitě aktualizuje. **Přesunutím kurzoru** nad analyzovaný povrch získáte **konkrétní** hodnotu.

   ![](../../.gitbook/assets/460060a0-ea3b-4095-af45-40045811be22.png)

7. Nastavení **Roční kumulativní** zobrazuje **kumulativní** energii za celý rok \(v kWh/čtv. m\). Tato možnost je určena pro **studie potenciální energetických zisků z instalace fotovoltaických panelů**.

   ![](../../.gitbook/assets/a9f61dfb-dfc9-4751-b145-b131a69c53cf.png)

8. Tyto studie **analýzy slunečního záření** lze exportovat kliknutím na možnost **Soubor &gt; Exportovat \(Ctrl+E\)** a výběrem možnosti **Obrázek** v seznamu vlevo.

## Energetická analýza s aplikací Insight

V aplikaci FormIt jsou integrovány stejné nástroje pro analýzu výkonnosti budovy, jaké používá aplikace Revit. Aplikace **Insight** obsahuje řídicí panel se systémovými parametry budovy, které lze upravit tak, aby odrážely potenciální scénáře, aniž by bylo nutné **znovu analyzovat** geometrii modelu. Aplikace Insight nejlépe funguje s geometrií**objemů** aplikace FormIt.

1. Ujistěte se, že jste přihlášeni k účtu Autodesk. Vypněte **všechny** hladiny **kromě** hladiny **objemů**. Geometrie musí mít alespoň jedno **podlaží**.
2. Aplikace FormIt odešle do aplikace Insight pouze **viditelnou** geometrii. Všimněte si, že i pro jednoduchý **objem** získáte z aplikace **Insight** spoustu dat.

   ![](../../.gitbook/assets/energymassing.png)

3. Klikněte na tlačítko **Insight &gt; Generovat přehled**. Analýza bude probíhat v cloudu, takže během výpočtu můžete pokračovat v modelování.

   ![](../../.gitbook/assets/energymenu.png)

4. Po dokončení analýzy klikněte na tlačítko **Zobrazit přehled**, čímž zobrazíte **energetický model** a **faktory výkonu** \(případně můžete přejít přímo na web na adrese [**http://insight.autodesk.com**](http://insight.autodesk.com/)\).

   ![](../../.gitbook/assets/energydashboard.png)

5. Na řídicím panelu aplikace Insight můžete nastavit hodnotu \(nebo rozsah hodnot\) pro jednotlivé **faktory výkonu** tak, že kliknete na požadovaný faktor a přetáhnete modré body. Rozsah je užitečný, pokud ještě neznáte konkrétní systém, který bude budova používat.
6. Při každé změně **faktoru** se aktualizuje celkový **rozsah nákladů na energie** \(měřeno v USD/čtv. m za rok\). Výkon svého návrhu můžete porovnat s referenčními hodnotami, jako je například standard **Ashrae 90.1** nebo výzva **Architecture 2030**.
7. Pokud se podoba vašeho návrhu zásadně změní, můžete znovu odeslat aktualizovaný objem na stejný řídicí panel. Jestliže chcete pro aktualizovaný návrh vytvořit **nový** řídicí panel, nezapomeňte návrh nejprve uložit pomocí příkazu **Uložit jako** v aplikaci FormIt.
8. Pokud se energetická analýza nezdaří, můžete geometrii zkontrolovat a opravit v aplikaci FormIt pomocí nástroje **Problémy s vodotěsností \(DW\)**.
9. Vypněte hladinu **objemů** a znovu zapněte všechny ostatní hladiny.

